https://do7js0tdxrds1.cloudfront.net/1zzk7hmmo7bmmcxucwxyhvfowdys?response-content-disposition=inline%3B+filename%3D%22bms+functionalities.png%22%3B&response-content-type=image%2Fpng&Expires=1701167306&Signature=IIZPOPGKz6cBRTHTgXICKH5xnbyVwCV2mWCx8BS0d~iXjarjM3wJX~y8HlrZdJlw0X~icQukDeWa9ckYsSaNd2~ttI304w5aLYmukrjTGgkm7g-0sac2WmnMjHff-aG3uBoyUeV~UQjP3yU7o3~HaWMty-9SrExHprn~9dPDN5kCG~9E3LGARRaxp--~9OtmuKP5LeRt4P5crTbGgj~N-ghKWcSbleUtKn7TxX6z7M4Q4Oxb6SXj9ytngA9oWsLZRoIdrOqB6Xi8GPZd2XSkYq6yBx6AJHUJKIw4cNePTf8h7GTEKALu-MgrqW1CjzYQ2P~i3FLtTuxCmBuR8QDW9Q__&Key-Pair-Id=K2Q3HDJ6ZAQGFF


A battery management system has many other functionalities other than keeping the cells in a battery pack balanced. These functionalities can be subdivided into 

1. Monitoring
2. Protection
3. Charging and Discharging Management
4. Diagnosis

### 1. Monitoring

BMS focuses on monitoring the battery pack voltage, current, cell voltage,
temperature, isolation, and interlocks. 

1. A faulty battery charging system or voltage regulator can cause overvoltage in the battery system. 
2. An overvoltage or overcurrent may cause permanent damage to the battery system, while the overcharge causes cell venting. As vented gases are flammable, it creates a severe safety concern. 

3. Similarly, a low voltage or current significantly affects battery performance. 
4. Isolation of the central battery system is an essential task for BMS, especially for a high voltage system. If a human body comes into contact with a faulty high voltage battery system, the current will flow through the body and cause death. 
5. Temperature control is another crucial task for BMS. High temperatures
create heat and other abnormal issues that negatively impact the battery system 

### 2. Protection

A BMS must ensure protection against any battery system hazards. 

The BMS safeguard includes (among others) 
1. Detecting the operating mode. 
2. Setting fault criteria.
3. Authenticating and identifying the system.
4. Predicting the pack/cell overvoltage and overcurrent.
5. Predicting the isolation fault.
6. Detecting the high/low temperature.

A BMS must protect the battery system from the external event, since the external environment of the battery pack has an effect on the cell/pack parameters.


### 3. Charging and Discharging Management

The state of charge (SOC) has a significant impact on battery life. Each battery has a specific number of charging and discharging cycles, and the battery life reduces with the increased number of charging and discharging phenomena. 

BMS must confirm the efficient way for charging and discharging procedures. Additionally, a BMS must maintain the proper SOC so that the battery lifetime will be maximized. To ensure management in this area, BMS performs the following tasks: 

1) Control the charger current. 
2) Turn on/off active switches between the pack and load/charger.
3) Run the pre-charge sequence. 
4) Set dynamic power limits.
5) Conduct active and passive balancing.


### 4.  Diagnosis

1. BMS estimates and predicts the 
   1. Depth of discharge (DOD). 
   1. State of charge (SOC).
   1. Battery capacity.
   1. Cell temperature. 
   1. State of fitness (SOF). 
   1. Available energy.
   1. Charging time.
   1. Remaining useful life (RUL). 
   1. Remaining runtime.
   1. Inner impedance of cell and current capability to ensure efficient battery performance. 

2. BMS is also responsible for detecting faults, such as 
   1. Fires
   1. Thermal runaways 
   1. Explosions 
   1. Minimizing the consequences of fault effects. 

Therefore, fault diagnosis is an important functionality for BMS.

### Summary of functionalities

1. Protect the battery pack.
2. Monitor the battery pack state.
3. Measure battery cell and pack voltage.
4. Measure battery cell and pack temperature.
5. Measure battery pack current flow.
6. Detect battery system leakage currents.
7. Determine battery pack critical state.
8. Manage operating modes.
9. Receive information from the master control system (EMS, VMS, etc.).
10. Control the battery pack (dis)connection.
11. Control the (dis)connection of the electric line of charge.
12. Control the (dis)connection of the electric line of discharge.
13. Inform master control system (EMS, VMS...) of battery pack (dis)connection status.
14. Inform operator (HMI) of battery pack (dis)connection status.
15. Optimize battery lifetime and energy availability.
16. Monitor and control battery pack state of charge (SOC) and state of health (SOH).
17. Manage cell balancing.
18. Monitor and control non-safety battery support systems (BSS).
19. Diagnostic—record battery life history log.

https://www.youtube.com/watch?v=8eItvOuDRjw