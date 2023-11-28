# Transistor 2n5298 temperature measurement 


As mentioned in the earlier chapter, we have gained familiarity with the transistor 2n5298 and its application in the BMS board. Now, our focus shifts to measuring the temperature of this transistor during a specific operation. For this purpose, we will select a Discharge transistor, which is clearly highlighted in the image below for easy identification. The temperature measurement will be conducted while the battery is being discharged. To facilitate the discharge, we will connect a load of a 4.7 ohms resistor between the output terminals of the BMS. Subsequently, we will calculate the total heat loss from transistor 2n5298 by determining the Initial temperature (T1) and the Final temperature (T2) of the transistor. Let us start the measurement process.


![image17.jpg](https://www.pupilfirst.school/markdown_attachments/6482/G_LFyWKRAWL5YAgU4AgnIA)


### Component requirement list

* BMS PCB with NTC sensor
* 4.7 10(or 5) watt resistor 
* 2 Female to Female Jumper wire
* 2 Male to Female Jumper wire
* 2 male to male Jumper wire
* Tape 

> Note: Please remove the heatsink on the discharge transistor carefully. 

**Steps :**

1. Unplug the INA219 sensor from its header pins

![image22.jpg](https://www.pupilfirst.school/markdown_attachments/6483/ntLqULKFvQe_yWXVulZxNg)

2. Locate the top screw on the heatsink and unscrew it

![image7.jpg](https://www.pupilfirst.school/markdown_attachments/6484/dayDSkb_b0xfSzSiw8wb7A)

3. Turn the BMS board upside down and locate the screw placed below heatsink and unscrew the screw placed below heatsink.

![image16.jpg](https://www.pupilfirst.school/markdown_attachments/6485/CRuB8aFRyY_gsJ9B9rT-LQ)

![image10.jpg](https://www.pupilfirst.school/markdown_attachments/6486/Dz63Tp02FtFKb2jI3OGj8g)

4. Remove the heatsink by sliding it upwards

5. Plug INA219 sensor again into header pins 
Align both the labels on INA219 sensor and PCB , and insert the pins of sensor into PCB header pi


![image26.jpg](https://www.pupilfirst.school/markdown_attachments/6489/CIkLBLI_M9Rp1gHCO9CjVw)

### **Activity Procedure**
 

**Step 1** : Stick NTC sensor to backside of transistor

Connect the NTC sensor to the transistor heatsink backplate with help of a tape as shown in the image below. Make sure the NTC sensor is in proper contact with the heat sink surface of the transistor.


![Untitled.png](https://www.pupilfirst.school/markdown_attachments/6492/ENeubOvHk6XC72syKQHNbA)

**Step 2**  : Connecting Resistor
Connect resistor at output terminals of the BMS PCB with help of jumper wires.


![image13.jpg](https://www.pupilfirst.school/markdown_attachments/6493/k0Bz51Tyi-H3LzDNqJVDpQ)

**Step 3**  : Writing code
Turn on the Discharge mode in the BMS by :- 
* Making changes in the control.py file available in the BMS_main folder.

```
if iteration > 30 and iteration <600 : 
Discharge() 
else 
stop()
```

* Once the GUI opens, wait for 30 seconds till the Calibration temperature and the ambient temperature becomes equal and the Discharging starts. 

**Step 4** : Setting up GUI

* For collecting the temperature data while discharging you will need to start the GUI using the steps provided in Level 5. 
* Once the GUI starts, wait for  the calibration to set in i.e. the Calibration temperature and Ambient Temperature becomes equal.
* When the discharging starts(at Time = 30 seconds), note the initial temperature of the NTC sensor that is connected to the discharging transistor.
* Make sure that the Battery pack voltage is above 5.50V and the Current withdrawal is around 900mA. If the voltage is below 5.50V, charge the cells and try again.


![image15.png](https://www.pupilfirst.school/markdown_attachments/6494/nVe91HYd6-LJ7K1geBjX2w)

**Step 5** : Saving plots
* When 600 iterations are completed the GUI will freeze and then click on the Plot Graphs icon at the bottom of the GUI. 
* The temperature plot should look similar to this plot.


![image7.png](https://www.pupilfirst.school/markdown_attachments/6504/QlwF99ZkefKdvSjwkRgY2Q)


Step 6 : Observation 
From the above graph the Initial temperature(Ti) = 31 °C and Final temperature(Tf) =  55 °C. 

Thus ΔT = (Tf - Ti) = 55 - 31 =  24 °C.


**Calculations**

The formula for heat dissipation is given by :- 


![image2.png](https://www.pupilfirst.school/markdown_attachments/6496/3mJwYJp14YJ5GWMvPf49vA)


Where , 
h = Convective heat transfer coefficient 

A = Total surface area of transistor

ΔT = Difference between initial temperature and final temperature = (Tf - Ti)

Put the temperature change in formula and find heat dissipated in watts

Here , 
h    =  25  W/m2K

A    =  0.000242  m2

ΔT  =  24  °c 

So,


![image6.png](https://www.pupilfirst.school/markdown_attachments/6497/DDcjG0-69_ATOW6caN4zkg)


>Cautionary Note :
When discharging is turned on , the shunt resistor will get heated up so place it away from PCB and do not try to touch the shunt resistor with bare hands while discharging is on as its surface temperature might be very hot.Monitor the PCB as well as jumper wires connected at output connectors, as while discharging they might get warm.

