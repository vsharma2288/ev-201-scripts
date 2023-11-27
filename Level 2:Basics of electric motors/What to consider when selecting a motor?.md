There are several characteristics that you need to pay attention to when selecting a motor, but voltage, current, torque, and velocity (RPM) are the most important.

## 1. Current

Current is what powers the motor, and too much current will damage the motor. For DC motors, operating and stall current is important. Operating current is the average amount of current the motor is expected to draw under typical torque. Stall current applies enough torque for the motor to run at stall speed or 0 RPM. This is the maximum amount of current the motor should be able to draw, as well as the maximum power when multiplied by the rated voltage. Heat sinks are important as they are constantly running the motor or is running it at higher than the rated voltage in order to keep the coils from melting.

## 2. Voltage

Voltage is used to keep the net current flowing in one direction and to overcome the back current. The higher the voltage, the higher the torque. The voltage rating of a DC motor indicates the most efficient voltage while running. Be sure to apply the recommended voltage. If you apply too few volts, the motor will not work, whereas too many volts can short windings, resulting in power loss or complete destruction.

In DC motors, Voltage is directly proportional to No-load speed of the motor. 

## 3. Torque values 
Operating and stall values also need to be considered with torque. Operating torque is the amount of torque the motor was designed to give and stall torque is the amount of torque produced when power is applied from stall speed. You should always look at the required operating torque, but some applications will require you to know how far you can push the motor. 

In the case of DC motors, the torque is directly proportional to armature current, which means, to get higher torque outputs from the motor, you will need to increase the armature current supply to the motor. 



## 4. RPM or required top speed
Velocity, or speed (RPM), can be complex regarding motors. The general rule is that motors run most efficiently at the highest speeds, but it is not always possible if gearing is required. Adding gears will reduce the efficiency of the motor, so take into account speed and torque reduction as well.

In care of DC Motors, speed is inversely proportional to the torque of the motor, which means, at higher speeds, the Torque output of the motor is reduced.


https://do7js0tdxrds1.cloudfront.net/7ft8kkkjpk8piyz7bq0aaiboucx3?response-content-disposition=inline%3B+filename%3D%22motor_individual_2x2.png%22%3B&response-content-type=image%2Fpng&Expires=1701079586&Signature=EDD3ZyUUCxSZBlgFGCC57BBGaG~Hpu7Z2Lla5XiUZzsM5Tq21ezDPxyOeHwMKMBkVoc8pKNMOCKyD2pyhj~V90ZHfVkFWuWLZsk7NAVu2EKCLWLX2bnkuWBKDFRLl4MaWFdNlfwWSNxtVuehpfCH7-IzuEhF8nJ1rYp6VUqy1gR5cr6vL6iVclLm19lkG6FR1muFDSmRHgPuxvnqBYV-ZeHD27tJh37iE1sGrTtO5U9n0RXwY8pakN~DNjrRHV2sq6KcNvPIHkEUFYiWMewaTdpTssYQCorI~~vT23ejEaBNVrNfK8O0KTc6-Htj0MSJXDziIr7okQ4xirNXTxOwIw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

An EV’s motor and electronics efficiency also directly influences the battery weight because the lost power needs to be compensated. Every 1% lower efficiency requires 1% more power from the battery (meaning more batteries). The EV’s performance directly depends on the electrical motor specifications. The performance of the motor is determined by the torque -speed and power-speed characteristics of the traction motor. You will need to take this into account before adding gears or any other mechanical component in order to increase torque.


https://do7js0tdxrds1.cloudfront.net/b3yu47vmroa6opovgdqi2zh8jl37?response-content-disposition=inline%3B+filename%3D%22image002_bezhrr.png%22%3B&response-content-type=image%2Fpng&Expires=1701079586&Signature=o4pvnuBxZecO7oiXz6L7BO9Qa0SJiHPt64twaylwq5lkjt1akbkCDDdS4cqn1LQ7D5-JH-D4XLXd7eLGkbzoEwTjmwDdB413I9dL2RhoCQe7YBwg6djezLMNFinh3IXgoHWPVS6S9ox0LGUkv2uKYrVYsE-2YFCsn6Z4EOLFtBzl-UwQxJodkxoJJ5vc5elYTUAfZf2eagHEqsRJ0OdrtWKEVhd2YzgiwXVZvDNOuVgLLrnbyzsNYngOJK-At9ccU4q-RFcd4j331-Bz5mudsWp6m50rnlf6V~BU1~0fSy5dXHMx0FW6OaA7FVCUghY1UtTUMg76ftdMkXaGdVxAdg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF


The grade ability and maximum speed are important parameters in these curves. The desired motor grade ability requires high torque at low speed, enabling proper starting and acceleration. The EV motor needs to have high power at high speed and a wide speed range in the constant power region, as shown in the plot above. The constant torque operating region is important at low speed to provide a good start and uphill drive. The constant power region determines the maximum EV speed on flat surfaces.

>Grade ability is the vehicle's ability to climb slopes.

The graph above shows the specifications of what an ideal motor should have. 

Selecting the proper output characteristic of an EV motor is a challenge because it is necessary to find the balance between acceleration performance and wide speed range in the constant power region. When increasing the constant power region, the power requirement for acceleration performance is decreased. The torque requirement is increased which influences the motor size and its final price. These are the features we desire in an EV motor:
* High efficiency
* High instant power
* Fast torque response
* High-power density
* Low cost
* High acceleration

Let's do an overall comparison of the different types of motors and see what can be used:



|             Motor type           | Brushed DC        |AC Induction         | Permanent Magnet        | Switched reluctance       |
|------------------------|-----------|------------|-----------|-----------|
| Power density          | Low       | Medium     | Very high | Medium    |
| Efficiency             | Low       | Medium     | Very high | Medium    |
| Controllability        | Very high | Very high  | High      | Medium    |
| Reliability            | Medium    | Very high  | High      | Very high |
| Technological maturity | Very high | Very high  | High      | High      |
| Cost                   | Low       | Very low   | High      | Low       |


### Brushed DC Motor
The biggest advantages of DC motors in EVs are robust construction and simple control. DC motors have appropriate torque-speed characteristics providing high torque at low speed. Their main disadvantages are size, low efficiency, low reliability and high maintenance, and limited speed because of the friction between brushes and collectors.

### Permanent Magnet Brushless DC Motor (PM BLDC)

PM BLDC motors use permanent magnets instead of the rotor windings. Since they do not include rotor losses their efficiency is higher than Induction motors. PM BLDC motors have a short constant power operation region because of their permanent magnet field weakened by a stator field. Since EVs require a wider constant power region, this can be extended by using conduction angle control where the speed range may reach three to four times the base speed. The permanent magnets also limit the motor torque to be high. The magnets are significantly influenced by the high temperature which reduces the remnant flux density and thus the motor torque capacity. The mechanical forces and magnet prices are the biggest disadvantages of this type of motor. The increased centrifugal forces caused by higher motor rotation speed can cause safety issues due to the possible breaking of the magnets.

### Induction Motor

This motor type is very common in EVs because of its simple construction, high reliability, robustness, simple maintenance, and low cost and operation under different environmental conditions. The disadvantages of Induction Motors are slightly lower efficiency (compared to PM motors), higher power losses (increased because of the cage losses), and a relatively low power factor. 

### Switched Reluctance Motor (SRM)

The benefit of SRMs is their high torque component, enabling their use in many applications such as wind energy, generator starter systems in gas turbine engines, and high-performance aerospace applications. Moreover, their advantages in EVs include their robustness, simple control, high efficiency, wide constant power operation region, fault tolerance, and effective torque-speed characteristics. Since they do not contain brushes, collectors, or magnets, the maintenance of SRMs is very simple and effective and their price is very competitive. The absence of magnets eliminates the problem with mechanical forces, enabling the motor to operate at a high speed. Since the motor's windings are not used, there are no copper losses in the rotor ensuring the rotor temperature is lower than other motor types.

----------------

It is noticeable that the Induction Motor type has all the characteristics suitable for EVs. 

In this application, safety is one of the most important considerations and the SRM and Induction Motor types provide driving safety. 

However, the rated speed of Induction Motors is relatively low. A permanent magnet has a higher power factor and efficiency in the low-speed region. The SRM type does not use brush collectors and magnets and thus has fewer maintenance requirements. This type also has lower power losses than other types. This is because of the short winding ends and their total length. 

The rotor does not contain conductors enabling low rotor temperature and easy cooling, which is one of the main advantages of SRM type motors. 

SRM operates at high speeds in a wide constant power region and allows extremely high-speed operation. Besides this, the motor is lightweight, competitive and has high efficiency. If all characteristics are considered, SRM is the most suitable motor type for EVs. Even with their relatively high power density and efficiency, BLDC motors are not commonly used in EV applications, mostly because of their limited constant power range.

### Motor Types Used by Popular EVs

The Tesla Model S and Model X use conventional Induction Motors. The Model 3 uses an SRM with internal permanent magnets in the stator, called an internal permanent magnet switched reluctance motor (IPM-SRM). Dual-motor versions were also introduced by Tesla—the Model 3 uses an IM in the front and an IPM-SRM in the back. It is the opposite case for the Model S and Model X. The GM Chevrolet Bolt uses a PMSM where the magnets are placed inside the rotor. This motor type is also used by the Toyota Prius, Nissan Leaf, and BMW i3. Every manufacturer utilizes their approaches and technologies to make their propulsion as efficient as possible and produces many varieties of the same motor type.