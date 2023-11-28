https://do7js0tdxrds1.cloudfront.net/z0r4llt25heuepuqr73uq4187055?response-content-disposition=inline%3B+filename%3D%22New+BMS+pcb+connections.png%22%3B&response-content-type=image%2Fpng&Expires=1701168554&Signature=PuQPlLNEy3FI7VtZV1eoflRhQ16oGbURX8JTAGz60jHja318SORdOrEAiptc-Wla28qeJLTQfrVZXFRKfOKMtDDU-MgXoUzv~lLNaZGtstTrSpG6cfdFOOMz~fBsOhAXiJIut2t6zLqsvYhqaCgjJY6k4qrowWFAy7k0l2N7KikpBbfuRG7EM07kGjst9bqr6MzcTsK-I~Zq-zGD9oBU84SliFuJblg3P4KQMJ3-re1bTEDz-OD-9YGpuOxblK6MZPPUfmB~15I2ARKQq17pujcs1bPRn6HpUSCyE~62rtAFJyLIRevicIv1lVRI3cGS8AM9oACsg1U8fAB~aZ9U8w__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

#### Code

Once you have finished the wiring and assembly, please copy the below code and run the code in an Arduino to check battery voltages.

1. Open the workspace/folder that you created earlier
2. Click on `BMS_main.ino` to open the Arduino Program
3. Connect the arduino on the BMS circuit to your computer.
4. Select the right `COM` port of your BMS arduino..
5. Click on `Upload` or the `Check` mark to upload the code to the PCB.
6. Click on the serial monitor or press `Ctrl` + `shift` + `m` to check if data is being published

The Code consists of 4 components

1. Gathering all data and Presenting and sharing it to our python program (Which we will work with later)
2. Gathering Battery voltages
3. Gathering Battery Temperatures
4. Gathering Current data.

### 1. Gathering all data and Presenting and sharing it to our python program.

```c
#include "BMSvariables.h"
#include <Wire.h>
#include <Adafruit_INA219.h>

Adafruit_INA219 ina219;


const int ledPin = 13; // the pin that the LED is attached to
int incomingByte;      // a variable to read incoming serial data into


void setup() {
  Serial.begin(9600);
  analogReference(EXTERNAL); // use AREF for reference voltage
  pinMode(muxA, OUTPUT);
  pinMode(muxB, OUTPUT);
  pinMode(Bal_1, OUTPUT);
  pinMode(Bal_2, OUTPUT);
  pinMode(Discharge, OUTPUT);
  pinMode(Charge, OUTPUT);

  digitalWrite(Bal_1, LOW);
  digitalWrite(Bal_2, LOW);
  digitalWrite(Discharge, LOW);
  digitalWrite(Charge, LOW);
pinMode(ledPin, OUTPUT);

  if (! ina219.begin()) {
    Serial.println("Failed to find INA219 current sensor chip");
    while (1) {
      delay(10);
    }
  }
  ina219.setCalibration_16V_400mA();
  //analogReference(INTERNAL);
}


void Bbal1() {
  digitalWrite(Bal_1, HIGH);
  cellOne_balaningState = 1;
  //  Serial.println("\t ");
  //  Serial.print("Battery 1 Balance on");
}
void Bbal2() {
  digitalWrite(Bal_2, HIGH);
  cellTwo_balaningState = 1;
  //  Serial.println("\t ");
  //  Serial.print("Battery 2 Balance on");
}
void charge() {
  digitalWrite(Charge, HIGH);
  chargingState = 1;
  //  Serial.println("\t ");
  //  Serial.print("Charging");
}
void discharge() {
  digitalWrite(Discharge, HIGH);
  dischargingState = 1;
  //  Serial.println("\t ");
  //  Serial.print("Discharging");
}

void resetBms() {
  digitalWrite(Bal_1, LOW);
  digitalWrite(Bal_2, LOW);
  digitalWrite(Charge, LOW);
  digitalWrite(Discharge, LOW);
  chargingState = 0;
  dischargingState = 0;
  cellOne_balaningState = 0;
  cellTwo_balaningState = 0;
}


void loop() {
  Loop += 1;

  
  //Data sent via serial UART to python
  //| 1  | Iteration                          |
  //| 2  | LM35                               |
  //| 3  | Environment/ board NTC temperature |
  //| 4  | Cell 1 Temperature                 |
  //| 5  | cell 2 temperature                 |
  //| 6  | cell 1 voltage                     |
  //| 7  | cell 2 voltage                     |
  //| 8  | pack voltage                       |
  //| 9  | charging state                     |
  //| 10 | discharging state                  |
  //| 11 | cell_1 Balancing                   |
  //| 12 | cell_2 Balancing                   |
  //| 13 | power                              |
  //| 14 | current                            |
  //| 15 | bus voltage                        |
  //| 16 |                                    |

  temperature();
  delay(250);
  batt1_voltage();
  delay(250);
  batt2_voltage();
  delay(250);
  pack_Voltage();
  delay(250);
  current_sensor();
  delay(250);
//
if (Serial.available() > 0) {
    // read the oldest byte in the serial buffer:
    incomingByte = Serial.read();
//    Serial.println(incomingByte);
    // if it's a capital H (ASCII 72), turn on the LED:
    if (incomingByte == 'H') {
      digitalWrite(ledPin, HIGH);
   
    }
    // if it's an L (ASCII 76) turn off the LED:
    if (incomingByte == 'L') {
      digitalWrite(ledPin, LOW);
      
    }
  }

// CSV format sent to Python
  // Iteration, LM35,Environment/board NTC temperature,Cell 1 Temperature, cell 2 temperature, cell 1 voltage, cell 2 voltage, pack voltage, charging state,discharging state, cell_1 Balancing, Cell_2 Balancing,power,current,bus voltage

  Serial.println((String) Loop +","+  Temperature_sensor +","+ Te+","+Tb1+","+Tb2+","+voltage1+","+voltage2+","+totVoltage+","+chargingState+","+dischargingState+","+cellOne_balaningState+","+cellTwo_balaningState+","+power_mW+","+current_mA+","+busvoltage);

}


```

### 2. Gathering Battery Voltages

```c
float batt1_voltage() {

  digitalWrite(muxA, LOW);
  digitalWrite(muxB, LOW);
  sensorValue = analogRead(muxOut); // Getting analog sensor data from Voltage divider
  float batt1 = sensorValue;
  voltage1 = batt1 * (5.00 / 1023.00); //converting analog 0 -1023 data to readable voltages
}

float batt2_voltage() {

  digitalWrite(muxA, HIGH);
  digitalWrite(muxB, LOW);
  sensorValue = analogRead(muxOut); // Getting sensor data from Voltage divider
  float batt2 = sensorValue;
  voltage2 = batt2 * (5.00 / 1023.00) * 2;  //converting analog 0 -1023 data to readable voltages


}

float pack_Voltage() {
   totVoltage = voltage1 + voltage2; // total battery pack voltage
}
```
### 3. Gathering battery Temperatures

```c
void temperature() { // Temperature readings
  
  // LM35 sensor reading
  float rawTemperature = analogRead(A2);
  float mv = (rawTemperature / 1024.0) * 5000;
  Temperature_sensor = mv / 10;

  
  // PCB environment NTC sensor
  sensorValue = analogRead(A3);
  R2 = R1 * (1023.0 / (float)sensorValue - 1.0);
  logR2 = log(R2);
  T = (1.0 / (c1 + c2*logR2 + c3*logR2*logR2*logR2));
  Te = T - 273.15; 





  // Battery 1 NTC sensor
  digitalWrite(muxA, LOW);
  digitalWrite(muxB, HIGH);
  sensorValue = analogRead(muxOut);
  R2 = R1 * (1023.0 / (float)sensorValue - 1.0);
  logR2 = log(R2);
  T = (1.0 / (c1 + c2*logR2 + c3*logR2*logR2*logR2));
  Tb1 = T - 273.15; 



  
  // Battery 2 NTC sensor
  digitalWrite(muxA, HIGH);
  digitalWrite(muxB, HIGH);
  sensorValue = analogRead(muxOut);
  R2 = R1 * (1023.0 / (float)sensorValue - 1.0);
  logR2 = log(R2);
  T = (1.0 / (c1 + c2*logR2 + c3*logR2*logR2*logR2));
  Tb2 = T - 273.15; 

//  //Calibration
//  if(Loop%10 == 0){
//  if(Te > (Temperature_sensor+1)){
//    Calibration = Te-Temperature_sensor ;
//  }
//  else if(Te < (Temperature_sensor-1)){
//    Calibration = Temperature_sensor-Te ;
//  }
//  }
//  if(Te > (Temperature_sensor+1)){
////    Te = Te-Calibration;
//    Tb1 = Tb1-Calibration;
//    Tb2 = Tb2-Calibration;
//  }
//  else if(Te < (Temperature_sensor-1)){
////    Te = Te+Calibration;
//    Tb1 = Tb1+Calibration;
//    Tb2 = Tb2+Calibration;
//  }


}

```

### 4. Gathering Battery pack Current

```c
void current_sensor() { // Current and output voltage readings.


shuntvoltage = ina219.getShuntVoltage_mV();
busvoltage = ina219.getBusVoltage_V(); // Voltage output
current_mA = ina219.getCurrent_mA();
power_mW = ina219.getPower_mW();
loadvoltage = busvoltage + (shuntvoltage / 1000); // Voltage from the batteries

}


```

>Once you click upload and the code is running, click on tools in the Arduino IDE and select ```Serial monitor``` from the drop-down menu to display all the results.