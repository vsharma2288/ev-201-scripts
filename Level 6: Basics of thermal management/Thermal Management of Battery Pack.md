Batteries generate heat during charging and discharging due to enthalpy changes, electrochemical polarization, and resistive heating within the cells. 

For electric vehicle (EV) batteries, heat is an important consideration as it affects battery performance, lifespan and safety. Electric vehicle batteries generate heat mainly during the charging and discharging process and when power demand is high. There are several factors that contribute to the heating of battery cells in electric vehicles.

#### **Resistance:**

When current flows through a battery cell, internal resistance causes a voltage drop that leads to heat build-up. This resistance is affected by many factors, including cell design, materials, and temperature. 

 Let's do a basic calculation of the heat generation of a cell during charging due to resistive heating.
Consider the Samsung ICR 18650 cell. According to the cell's datasheet, the cell's internal resistance varies between 7 and 16 mOhm. Calculations assume 16mΩ. Now assume a 100kW fast charge and a battery pack containing 10,000 cells. Each cell voltage is 3.7 V.
The current flowing through each cell during charging will be 10W/3.7V=2.7A.

 The resistive heat loss for each cell can be calculated using the formula:

 Resistive heat loss = I^2^*R

 where,

 I is the current (A) flowing through the cell.
R is the internal resistance of the cell in ohms

 Heat loss = 2.7*2.7*0.016=0.11 W

 Total resistive heat loss of the battery = 0.11 * 10000 = 1166 W

#### **Charging and Discharging Efficiency:**

Energy conversion during charging and discharging is not 100% efficient and some energy loss occurs in the form of heat. Inefficiency can result from resistive losses, polarization effects, and chemical reactions within the battery.

#### **High Current Demand:**

Battery cells can have high current demands during acceleration or when high performance is required. As the current increases, resistive losses and heat generation can increase.

#### **Insufficient Cooling:**

If the battery cells are not sufficiently cooled, the heat generated during operation can accumulate and increase their temperature. Elevated temperatures can adversely affect battery performance, capacity, and lifespan.

In Battery it is important to maintain the optimum temperatures, ideal temp is from 20 to 30C. But during the winter, the surrounding temperature can fall below 0C in particular regions of the world. To achieve the optimum performance of the battery during the sub zero temperature heating of the battery pack is required. So the battery thermal management system consists of both cooling and heating systems.


#### **Methods of Battery and Battery pack thermal management (cooling and heating)**

https://www.youtube.com/watch?v=a1K3yT00ELo

To control excess heat and maintain optimal operating conditions of cells, EV manufacturers employ a variety of cooling and heating methods in thermal management systems for battery packs. These systems may include liquid or air cooling, heat sinks, and thermal interface materials to efficiently dissipate heat. Also there are heat pumps, PTC heaters for heating the battery packs. Additionally, the Battery Management System (BMS) monitors and adjusts operating parameters to prevent overheating and ensure cells are operating within safe temperature limits.

Let’s see some of the cooling/heating methods in details

**1) With Cooling Fins:**

The surface area of cooling fins is enhanced to boost the efficiency of heat transfer. Through conduction, heat moves from the battery pack to the fin, and through convection, it is then transferred from the fin to the surrounding air. Fins possess excellent thermal conductivity and can effectively accomplish cooling objectives, but they contribute significantly to the overall weight of the pack. While fins have been widely employed in electronics and as supplementary cooling systems in traditional internal combustion engine vehicles, their utilization for cooling electric car batteries has declined due to the drawback of increased weight outweighing the cooling advantages. Fins made of aluminum alloys are commonly employed in the cooling systems of 2 Wheeler and 3 Wheeler vehicles. In certain cases, aluminum casings and chassis are utilized as substantial heat sinks to effectively dissipate heat from the battery pack. A notable example of this can be observed in the Ather scooter. However, a significant drawback of this approach is that it cannot be utilized for heating the battery during low-temperature operations.

**2) Phase change material cooling**

Phase change materials function by absorbing heat energy through a transition from a solid to a liquid state. During this phase change, the material can absorb significant amounts of heat while experiencing minimal temperature variation. While phase change material cooling systems can fulfill the cooling requirements of a battery pack, their application is limited by the volume change that occurs during the phase transition.

https://www.youtube.com/watch?v=KsnFwAwoMfo&t=31s

**3) Cooling/heating with Air:**

The process of air cooling relies on convection to remove heat from the battery pack. When air flows over the surface, it absorbs and carries away the emitted heat. While air cooling is straightforward and uncomplicated, it is not as efficient or refined as liquid cooling. In earlier iterations of electric cars like the Nissan Leaf, air cooling was commonly utilized. However, as electric cars become more prevalent, concerns regarding safety have emerged regarding battery packs that rely solely on air cooling, particularly in hot climates. In contrast, certain car manufacturers like Tesla advocate for the use of liquid cooling as the safest approach.

In sub-zero applications, by directing hot air flow over the components, heat can be transferred to the battery pack, helping to maintain its temperature in cold conditions. This dual-functionality allows the system to both cool the battery pack in normal operating conditions and provide heating capabilities when necessary in sub-zero environments.

https://www.youtube.com/watch?v=msi0YrX3Mzw

Additional Info: https://www.tycorun.com/blogs/news/what-is-air-cooled-battery-cooling

**4) Liquid (Water+Glycol) cooling and heating:**

Liquid coolants possess superior heat conductivity and heat capacity compared to air, enabling them to function highly efficiently. They offer distinct benefits such as a compact structure and easy arrangement. Among the available options, liquid coolants are the optimal choice for effectively maintaining the appropriate temperature range and uniformity of a battery pack. However, it is important to note that liquid cooling systems come with safety concerns related to potential leaks and proper disposal, as mishandling glycol can pose environmental hazards. Notably, prominent automotive manufacturers like Tesla, Jaguar, and BMW currently employ these systems. There are two ways of cooling with liquid: they are direct and indirect.

Direct cooling systems place the battery cells in direct contact with the coolant liquid. These thermal management schemes are currently in the research and development stage, with no cars on the market using this system. Direct cooling is more difficult to achieve, due to the fact that a new type of coolant is required. Because the battery is in contact with the liquid, the coolant needs to have low to no conductivity.

https://www.youtube.com/watch?v=sD-cyg-z9kc

Indirect cooling systems are similar to ICE cooling systems in that both circulate liquid coolant through a series of metal pipes. However, the construction of the cooling system will look much different in electric vehicles. The structure of the cooling system that achieves maximum temperature uniformity is dependent on the shape of the battery pack and will look different for each car manufacturer.

https://www.youtube.com/watch?v=ri0cZJyuFwo

**5) Refrigerant cooling/heating**

Similar to liquid cooling and heating systems, refrigerant-based cooling utilizes a refrigerant as the working fluid instead of a water and glycol mixture. Refrigerants of  HVAC systems, such as, R1234yf, R134a, R1233zd, and others are employed for cooling and heating purposes. Refrigerant cooling outperforms other methods in terms of cooling and heating performance. For heating the battery pack, a heat pump mode is utilized. Refrigerant cooling allows both direct and indirect cooling methods.

**6) Positive temperature coefficient (PTC) heater**

PTC heaters find frequent application in battery packs due to heating requirements. These heaters are constructed as thin, flexible printed circuits with a wide geometry, which enables efficient thermal transfer. The design of PTC heaters is crucial to optimize efficiency and minimize temperature fluctuations within the cells. Utilizing advanced screen printing processes, PTC heaters are self-regulating heating elements that offer cost-effectiveness and environmental friendliness.

https://www.youtube.com/watch?v=gRlZksTHND8

**7) Heat pump**

https://www.youtube.com/watch?v=DyGgrkeds5U

For more info visit this link: https://www.dober.com/electric-vehicle-cooling-systems