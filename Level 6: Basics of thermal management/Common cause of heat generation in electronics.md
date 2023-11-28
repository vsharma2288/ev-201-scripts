Now that you know why heat is generated in electronic components, let's simulate it and also estimate the amount of heat that will be dissipated by a simple electronic component.
For this experiment, we will use a resistor. As it is the most basic component that generates heat.

**Why do we need to estimate heat dissipation?**

Heat dissipation is an important factor to consider when designing electronic circuits, as excess heat can cause the components to malfunction or fail.
One way to calculate the heat dissipated by a resistor is to use the equation:

![image4.png](https://www.pupilfirst.school/markdown_attachments/6478/nSDCbv6ffhdRFR1473S74w)

Where:
H is the heat loss in Joules (J)
I is the current in Amperes (A)
R is the resistance in Ohms (Ω)
t is the time in seconds (s)

This equation is known as **Joule's law**, and it is a fundamental principle of electrical engineering. It states that the heat (H) produced in a resistor is directly proportional to the square of the current (I) passing through it and the resistance (R) of the resistor, and is also proportional to the time (t) for which the current flows.

For example, Suppose we have a resistor with a resistance of 100 ohms (R = 100 Ω) through which a current of 2 amperes (I = 2 A) flows for a duration of 10 seconds (t = 10 s).

Using the formula:

H = I^2^ * R * t

Plug in the values:

H = (2 )^2^ * (100 ) * (10 )
H = 4 * 100 * 10
H = 4000 J


Therefore, the heat loss in the resistor is 4000 Joules.

This means that 4000 Joules of energy are converted into heat as the current flows through the resistor over a 10-second period. To calculate the heat generated in Watt, divide the above equation by time.
This equation can be used to calculate the heat dissipated by any resistor, provided that the current, resistance and time values are known. It's worth noting that this equation only applies to resistors that are operating at a constant temperature. If the temperature of the resistor is changing, the heat dissipation will also change, as the resistance of the resistor is temperature-dependent.

In summary, Joule's law is a useful equation for calculating the heat dissipated by a resistor. This is an important consideration when designing electronic circuits, as excess heat can cause the components to malfunction or fail.

https://www.youtube.com/watch?v=LC5o2jC3yaw

## Let’s study the heat loss in IC2n5298 at specified operating condition

### About IC 2n5298 and its usage

2N5298 is a **PNP** (Positive-Negative-Positive) bipolar junction transistor (BJT). It is designed for high-power switching and amplification applications. There are two such IC’s used in BMS boards used in L5 for the charging and dis-charging of the battery.

The transistors are connected in series, back-to-back. The circuit is used for controlling charging and discharging a battery. The circuit comprises a first Transistor for controlling discharging the battery, and a second Transistor coupled in series to the battery. The first and second Transistors have diodes respectively, and the first diode of the first Transistor and the second diode of the second Transistor are coupled in opposite directions. A load is coupled to the battery and a common node between the first and second Transistors such that power in the battery is delivered to said load when the first Transistors is turned on. The circuit further comprises a power source coupled to the second switch in series and power is delivered from the power source to the battery when the first and second Transistors are turned on.

![image9.png](https://www.pupilfirst.school/markdown_attachments/6479/RBs6NFcJsvt3oij_vFDBog)

![image19.png](https://www.pupilfirst.school/markdown_attachments/6480/yeU2Muoauj_qeJxbivdnlw)

2n5298 Heats up because all the current going in and out of the batteries have to pass through the transistor, The resistance applied by the transistor generates heat.

![image23.jpg](https://www.pupilfirst.school/markdown_attachments/6481/TFs3b_NgW-6poWkazNf-Bw)


### Calculating the heat loss of IC 2n5298

Calculating the heat loss in the 2N5298 IC involves understanding the power dissipation and thermal resistance of the device. The heat loss in the IC is primarily due to the power it consumes during operation. The formula to calculate the heat loss is as follows:

Heat Loss (in watts) = Power Dissipation (in watts)

The power dissipation of the 2N5298 IC can be determined by multiplying the voltage drop across the device (Vce) with the current passing through it (Ic). The formula for power dissipation is:

Power Dissipation (in watts) = Vce x Ic

Where:

Vce = Voltage drop across the collector-emitter junction of the transistor (in volts)
Ic = Collector current flowing through the transistor (in amperes)

Once you have the power dissipation, this value represents the heat loss in the IC during its operation.
Keep in mind that the power dissipation may vary depending on the specific operating conditions and application of the IC.

Let’s calculate it in particular operating condition:

When a resistor of 4.7ohm is connected as load , the max current discharge transistor allows is around 0.8-0.9 amps . And at this current the transistor heats up at considerable levels 
So, for the above condition

Vce = 0.75v (considering voltage drop transistor )
Ic = 0.9amp

Therefore , 

Power Dissipation (in watts) = Vce x Ic = 0.75 x 0.9 = 0.67 watts

So , from the above calculation we can state that when **0.85** amps of current flow through the transistor, it dissipates **0.67** watts of power from the transistor circuit.