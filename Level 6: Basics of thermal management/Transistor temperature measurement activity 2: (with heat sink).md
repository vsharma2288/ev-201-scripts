# Transistor 2n5298 temperature measurement 


In the previous thermal simulation results, we observed a temperature drop in the Discharge transistor 2n5298 with external heatsink. Now, let's verify this outcome through a measurement activity. We will replicate the earlier temperature measurement process, but this time, we must first connect the heat sink to the Discharge transistor 2n5298.
After that, connect the NTC to the transistor as shown below. Make sure NTC is in good contact with the transistor.

![image15.jpg](https://www.pupilfirst.school/markdown_attachments/6501/eJ0QvmEDKF4rLeJaSBHopQ)

After following above steps mentioned in the earlier temperature measurement activity, you will obtain similar graph from GUI 

![image22.png](https://www.pupilfirst.school/markdown_attachments/6502/3Z2b7jYgJdqnac1mqwk2nw)

**Observation (with heatsink)**

From the above graph the Initial temperature(Ti) = 30 °C and Final temperature(Tf) =  41 °C. 

Thus,

ΔT = (Tf - Ti) = 41 - 30 = 11 °C.

**Calculations**

The formula for heat dissipation is given by :- 

![image2.png](https://www.pupilfirst.school/markdown_attachments/6503/N3QgNJMeUGBPZr0OdFs4LQ)


Where , 

h = Convective heat transfer coefficient

A = Total surface area

ΔT = Different between initial temperature and final temperature = (Tf - Ti)

Put the temperature change in formula and find heat dissipated in watts

Here , 
h    =  25  W/m2K

A    =  0.002280  m2 (Surface area of heatsink)

Ti    =  30  °c

Tf    =  41  °c

ΔT  =  11  °c 

So , 

**Q = 25 * 0.002280 * 11 = 0.627 W**

**Points to note**

> * When discharging is turned on , the shunt resistor will get heated up so place it away from PCB and 
>* Do not try to touch the shunt resistor with bare hands while discharging is on as its surface temperature might be very hot
> * Monitor the PCB as well as jumper wires connected at output connectors , as while discharging they might get warm.

