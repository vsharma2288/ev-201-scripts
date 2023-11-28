### Overview of the battery monitoring part in the Battery management system PCB


Before we move on to working with a Battery management system, let's build a simple battery monitoring circuit to learn how we can extract the voltages of the cells in your battery pack.

https://do7js0tdxrds1.cloudfront.net/zefo08mryiu0nddtj8wfq8fbocdd?response-content-disposition=inline%3B+filename%3D%22overview1.png%22%3B&response-content-type=image%2Fpng&Expires=1701168398&Signature=sBK8m~WFHAXAcsiJ~HZnF-BwBIkb4TRZ5NkIqMpw-UOEzDFaCeACTPJkOREdVdS4iyqGqC~fPpOhyGCya3pjwaJ8qskow4FI61Sj26XJQxO860SilWCbkKlMJcWVKqIv02veXU2e5-zveBXa4Gs7ObQEnvE54LAFVXr9IEZlvh5Gg3s5dJVrSXE4Hih9xdu1JGKn8ium0a2ePHVvBg52SwRsZTAZFQd9Oxv~8Xq84uT-zM87UR44Ur9hpql0DSo8j3SV5moLiVXW7jGAS3ocVsqaJcNk2L648xv8imVRAJ2aqbN0bMAm475pjqIfZN~OQSzfAPZNl08ZKky1eewrcQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Fig 1 : Overview of battery monitoring system which we will be working with

>Arduino analog input pins can only tolerate an input voltage of 5 volts. So if you plan to measure voltages over 5 volts, you will need to use a voltage divider to reduce the incoming voltage.

#### 1. Voltage dividers

A voltage divider is a simple circuit that turns a large voltage into a smaller one. Using just two series resistors and an input voltage, we can create an output voltage that is a fraction of the input.

https://do7js0tdxrds1.cloudfront.net/gajxixkniy5qa5gopf3a50zagzz7?response-content-disposition=inline%3B+filename%3D%22Voltage-divider-circuit-formula.png%22%3B&response-content-type=image%2Fpng&Expires=1701168398&Signature=NWWL9NjlJkvy3g-4743CjtH28uXHHFJ5L5356ER9-s0lKFIOcUNNGIPFPfpe9WoePI82WfsORJo8ZEmhaOAfH6yS5F5bHgUP-kKHDJUem93vycAPbWawhzLmqzJDhMhZRujIkKwoyWMeMG~sym-fa6TE~Z5bji5bT-wCX60HnyYlh7yW88aEahDpEZ7ArMWohYQo4tIe8c0s4An3tUnucCD3VxL9BlroEmFAqi3l~uCcMeYtB-jzyeHDYJV8E7sLU~Ul5KcLzcxvNZY-LFC5xk8zWSr4lC6oxc~0vaVeDjuj~4zlbZnMw7lfKh8-0WAe42xm-VTIklOrHqnwoJyJKA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

A voltage divider involves applying a voltage source across a series of two resistors.

We'll call the resistor closest to the input voltage (V~in~) as R1, and the resistor closest to the ground as R2. The voltage drop across R2 is called V~out~, that's the divided voltage our circuit exists to make.

That's all there is to the circuit. V~out~ is our divided voltage. That's what'll end up being a fraction of the input voltage.

#### The Equation

The voltage divider equation assumes that you know three values of the above circuit: the input voltage (V~in~), and both resistor values (R1 and R2). Given those values, we can use this equation to find the output voltage (V~out~).

https://do7js0tdxrds1.cloudfront.net/a9lm0drcnjm2n94040maj1kpis9v?response-content-disposition=inline%3B+filename%3D%2251197073ce395f5d6d000000.png%22%3B&response-content-type=image%2Fpng&Expires=1701168398&Signature=LycKpZ9NVeHsm5BWC9ojk4sEpiFu1Jmlce5gNnzb87Zn1GeUQr62HOSN5ESersEIR3VV0r0vyc~oboggE8oslKEaGb72lA~3Gcr4nM6w6W3x5NEcqYYXm9bWCfI3N~D-LJy38dNjPYFzCCmck4CCbGGP5KLEAt~S1BSIHQLA~Xretds3qGaO-vuBtf-wgWE8VrrruN6Nku1zVyos~Sd~Oj51zBqb3dcWuEeDmGV56gNxIUM9q01~25MPicxfxAWpAZ4OymUUqQiB2NJw4cr7hCIztn3xRzAPnOdpRv-qZ1gpaTM8icz6IvlzoTGjtG4JHXMaAc1hxjaof0EF1WvpHQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

As shown in fig 1, all negative terminals are common and the only measured inputs are the positive terminals of each battery. 

Let's assume for a while that the voltage dividers are not connected, 

So now, without the voltage dividers:
```
1. the input voltage to A0 would be 3.2 volts. 
2. the input voltage to A1 would be 6.4 volts.

```

As you can see, the voltage going to A1 is 6.4 volts, it's higher than the 5-volt threshold. 

So now we have 2 options:

1. Add a voltage divider to all the cells and divide the voltages by 2 to the overall system.
2. Or consider the voltage going into Analog pin separately as "Battery pack voltage" and add a voltage divider to only Battery 2 and do all the calculations in the Arduino program to revert the division to get the actual voltage of the battery pack. 

For now, we will stick to option 1.

https://do7js0tdxrds1.cloudfront.net/u8tohx1563p0rsc5ydzujwb3k0tn?response-content-disposition=inline%3B+filename%3D%22overview1.png%22%3B&response-content-type=image%2Fpng&Expires=1701168398&Signature=GpwqI6GGYuCfCaJR191FCTOJ5wt-YoKfeZbF3IHBICVgor-xus7Zi4N-b8XusA-cQ~IRkEfXkSZu~G0j56iXm71dl2EzCh6AAkt8McPRHov3WUp34V2t4E0hJphmVKqxKcDVP-8fVQLFdkGanCHkGoODVPG9AF18naio-yDefNX1-glJqQ8G2AVt2LS9FQ-NusT6OkTtTqzCGWMqtFT3aeDdIWPTlZ0qw3pjy5tOmvauqK8thA1UIQlhx7pjubh2QUt-Cbex2JtBpeLEAz9gPuhAOQ2RHJYqsZQgsTKXH79Cwl2xeO3Jrrv89dyv96Q9mQuN5DJLObOrsLQ37PjD9g__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

The image above shows you how you can get the individual voltages of the cells and how they are connected to the arduino.

The Voltage divider come in between the arduino and the Batteries

### Let's start with building our Battery monitoring system and understand how everything works. 

#### Step 1, Connect all wires as shown.

https://do7js0tdxrds1.cloudfront.net/8bdj0b3phb3i6yiv8qgh1umizp7i?response-content-disposition=inline%3B+filename%3D%22overview2.png%22%3B&response-content-type=image%2Fpng&Expires=1701168398&Signature=fN2Fk53LgGYyG9TMkQIdgOuELuFBEt6xVhghBpgHYy4xvByg2oAObhfibmfgcUNVRnOV1c5dmUQAduhKwoFq70zW84i3Kj6KacjPdZ~j7BzXg6gTpT1~~cUU~kD91GgOWX9JNK5AJdNtmB1Va7Gp2TmOm6hi6qp7zsD5JXCe10OVG~KVRFN5fq5~qfkyJCe~gyIiynmY7HYiThrBo18Fffdve3yB3kvfIuDxpESR7K6I4OsWKZvoH7zWHAdkTOJKSkaDoEimfjP6qZ393kPWyT6w54eNOiQayc-f4A-NYc0T6W8M26t4IjSr2v-cbN1ZJgSFZcsclyoO~HydYPSbAw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Once all connections are done, Copy the code below into the arduino and check the serial monitor to get Voltage data.

```C
int iteration;




void setup() {
  // initialize serial communication at 9600 bits per second:
  
  Serial.begin(9600);
  Serial.println("");
  Serial.println("s/n\tBatt 1\t\tBatt 2\t");
  iteration = 1;
  
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


  //--------------- Output -----------------


  Serial.println("\t");
  Serial.print(iteration);
  Serial.print("\t| ");
  Serial.print((String) "Bat 1: " + voltage1 + (String) "v");
  Serial.print("\t| ");
  Serial.print((String) "Bat 2: " + voltage2 + (String) "v");
  Serial.print("\t| ");
  
  iteration = iteration + 1;

  delay(1000);  // delay in between reads for stability
}
```

As discussed before, the main objective here is to gather data from the batteries

To achieve that, we will need to use the analog pins of the arduino to get the individual voltages of the batteries.

The easiest way to do that is by connecting the batteries directly to the analog pins with a voltage divider in-between.

But, in our BMS we only have 2 batteries, what if we want to calculate more than 3 or 5 batteries? we will need more analog input pins, 

as we have limited Analog input pins, we will need to use a Multiplexer, 

**What is a multiplexer?**

A multiplexer is a simple device which can take in input from multiple channels and send the data through one output pin.