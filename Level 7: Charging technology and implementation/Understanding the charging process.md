https://do7js0tdxrds1.cloudfront.net/qci15q3p9xbw3bvegs4z76uu699e?response-content-disposition=inline%3B+filename%3D%22Operations+began+shortly+after%2C+when+all+business+permits+and+other+essential+documents+were+finally+approved+by+the+government.+During+the+wait%2C+the+brothers+began+establishing+connections+in+the+industry.+%283%29.png%22%3B&response-content-type=image%2Fpng&Expires=1701171051&Signature=iX8QNWDGdOx-iMdPBnZyCwMbAs-b8pVnyk3STlgVax6oiMaqzM98mnFCbEsqtipFEB9h5uPyvqWTxalDinf0-V2JXKRKG8Ku~JN~miTdP1jqlRt82OrUO3YmihiG6vww9L-U0N17YiqYLr7-dnme9a507b2pjMDQNX9cc0D6f6JQTp5j96Mo2d3Ocbh9296kga7CG0e6un4dJlOpKxE73cLyNredKmWaIQnLz7pbQt-pbV9tIZImFCXaem~yJuwtUHlnn8OxhklhGUiP5mFKCks4nA78gOfYc7LEu64~TbB9uxxvQFPCXaIzaO4DM2MvmMcZYs58hmPk~nyl26Sh2Q__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

## Step 1
Once the user presses the ‘start charge’ button, the charger sends a signal to the EV.


## Step 2 & 3
The EV detects this signal from the charger and sends all the parameters of the battery to the charger so that the charger knows how much current can be supplied safely and what voltages need to be set.


## Step 4
The Charger takes that information and checks whether is it compatible to charge that vehicle. Compatibility can be based on the maximum voltage that can be supplied by the charger or the max current capabilities etc. 


## Step 5
Once the compatibility check is complete, the charger sends all the charger parameters to the vehicle. Parameters like the maximum voltage and the maximum current capacity of the charger.


## Step 6
Once the EV is satisfied the charger is compatible, it calculates the max charging time.

## Step 7
Once everything is calculated and set, it gives permission to the charger to initiate charging. 

##Step 8
The charger recognizes the permission and, in turn, sends a signal internally to lock the connector in place and performs insulation and ground tests. This ensures the charger’s connector and cable are in
working order, allowing charging to begin, once tests are completed, it sends a "Ready signal" to the EV to let it know that the charger is ready.

## Step 9
The EV recognizes that the charger is ready and closes the switch or also called a contactor, This allows a direct connection between the charger and EV battery pack for charging. 


## Step 10
Once the charging begins, The EV transmits the required current every 0.1 seconds, and the charger supplies this current through constant current control. The EV constantly monitors the battery pack
parameters (voltage, current, temperature, etc.) and can stop the current flow in four different ways if a problem arises

  1. It will request 0A current from the charger, this will basically shut off the current.
  2. It will send an error message to the charger.
  3. Remove the charging enabled signal to switch off charging internally.
  4. Opening the EV contactor, thus manually disconnecting the charger.

The charger is also monitoring its own voltage, current, and temperature for potential problems.
Should a problem be detected, the charger sends the EV and error signal and stops the charging
process.

## Step 11
Once the charging has been completed, the EV transmits a zero-current request, the charger stops outputting.

## Step 12
Once the EV confirms zero current is flowing, the EV opens the battery contactor.

---------

>This is the basic communication flow between a charger and an EV, and all of these communications are done over a CAN Bus.

We will be learning more about CAN bus in the Next Level

https://youtu.be/RMxB7zA-e4Y
