https://vimeo.com/665711765


We will be using our Battery monitoring system as the Master for our i2c communication experiment.

#### Battery Management system code

```C

#include <Wire.h>

int iteration;
int sensitivity = 66;
int offsetVoltage = 2500;



const float energy_consumption = 25; // Enter Energy consumption Wh/Km as calculated in Level 4.

void setup() {
  // initialize serial communication at 9600 bits per second:
  Serial.begin(9600);
  Serial.println("");
  Serial.println("s/n\tBatt 1\t\tBatt 2\t\tBatt 3\t\tBatt 4\t\tTotal Voltage\t\tCurrent(A)\tTemperature\t\tCharge(%)\t\tRange(Km)");
  iteration = 1;
  Wire.begin();
}

// the loop routine runs over and over again forever:
void loop() {

 //   read the voltages on analog pins 0 to 1:
  float batt1 = analogRead(A0);
  float batt2 = analogRead(A1);



  //--------------- measure cell voltage -------------

  float tempVoltage1 = batt1 * (5.67 / 1224.00);      //convert the value to a true voltage.
  float tempVoltage2 = batt2 * (5.67 / 1224.00);      //convert the value to a true voltage.
 
  float voltage1 = tempVoltage1;
  float voltage2 = tempVoltage2 - voltage1;
  float totVoltage = tempVoltage2;

  
  //--------------- Battery percentage -----------------

  const float battery_max_V = 7.2; //maximum voltage of battery
  const float battery_min_V = 5;  //minimum voltage of battery before shutdown


  float Batt_percentage = ((totVoltage - battery_min_V) / (battery_max_V - battery_min_V)) * 100;


  //--------------- Battery percentage END -----------------


  //--------------- Vehicle Range -----------------

  // for this calculation, we are going to assume that the capacity of the battery pack is around 25 Ah to make calculation easier

  const float battery_capacity = 25;

  // Regular cells have a capacity 1.5 AH, as we have connected the cells in series. capacity will not increase, but with a Battery pack capacity of 1.5,
  // the Power output would be around 9 Watt-hours (1.5Ah x 6V) and if the energy consumption of your vehicle is 25 Watt-hour per km, it would not be enough to power your vehicle or calculate range.
  // in order to solve this issue, let's assume the battery capacity is 25Ah

  float battery_power = battery_capacity * totVoltage; // calculate available battery power in Watt hours.

  float range = battery_power / energy_consumption;


  //--------------- Vehicle Range END -----------------


  //--------------- Output -----------------


  Serial.println("\t");
  Serial.print(iteration);
  Serial.print("\t| ");
  Serial.print((String) "Bat 1: " + voltage1 + (String) "v");
  Serial.print("\t| ");
  Serial.print((String) "Bat 2: " + voltage2 + (String) "v");
  Serial.print("\t| ");
  Serial.print((String) "Pack Volt: " + totVoltage + (String) "v");
  Serial.print("\t| ");
  Serial.print((String) "Current: " + currentValue + (String) "A");
  Serial.print("\t| ");
  Serial.print((String) "Pack temp: " + temperature + (String) " C");
  Serial.print("\t| ");
  Serial.print((String) "Charge: " + Batt_percentage + (String) " %");
  Serial.print("\t| ");
  Serial.print((String) "Approx Range " + range + (String) " Km");

  iteration = iteration + 1;

  delay(1000);  // delay in between reads for stability

  

  //--------------- Communication with motor controller -------
  Wire.beginTransmission(4); // transmit to device #4
  
  if(totVoltage < 4.5 || temperature > 35 ) {
  Wire.write(0);     // Send "0" if total battery pack voltage less than 4.5V and temperature is above 35 degrees
  
  }
  else  {
    Wire.write(1); // Send "1" if total battery pack voltage and temperature is normal 
  }

  Wire.endTransmission();   // stop transmitting

  //--------------- Communication with motor controller end

}
```

And our motor controller will be listening to our BMS to see if it can run or whether it should shut down.


