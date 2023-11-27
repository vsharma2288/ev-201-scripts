# BMS in Level 6

The custom designed printed circuit board inside the KIT is the Battery Management System (BMS) which we will be using for the EV 201 course. Below are certain dos and don'ts while handling the KIT to avoid safety hazards and malfunction.

## Do’s:


- Remove the cells after every use.
- While inserting the cells in the cell holder, insert the negative side of the cells first and then push the cell from the positive side.
- Similarly, while removing the cells, remove the cells from the negative side first.
- Always charge the cells with supervision.
- Charge the cells as soon as they fall below the range of 3.1V. Do not wait for cells to get fully discharged, i.e.2V. 
- While charging, make sure there is no overheating of any component, stop the charging process if any unusual behavior is noticed.
- While charging the cells in CV mode for the first time, make sure to first remove the batteries and set the voltage of pot to a safe level. Once the voltage is set, there is no need to change it again afterward.
- Always connect the cells and turn the kill switch on before any data collection. Otherwise, the readings might be wrong.
- Discharged cells maybe lead to incorrect readings, make sure to use charged cells for data collection.
- Don’t short/connect the output terminals to each other while discharging.
- Don't use the charging circuit for discharging, i.e. when the 12v adapter is connected make sure the contactor is off.
- While charging the voltage value of the cells might increase slowly between 3.20 V and 3.45 V, wait until the voltage begins to rise.

## Don’ts:


- Avoid exposing the cells to extreme heat or cold, as this can damage the cells and increase the risk of fire or explosion.
- Don't keep cells for charging while going to sleep, overnight charging.
- While checking the voltage of cells, make sure charging is turned off i.e. to get open circuit voltage.
- Try not to mishandle the BMS PCB, bending the heat sinks/transistors multiple times will lead to breakage of transistor leads.
- Never let the cells get over discharged, i.e. cell voltage below 2V.
- Don't exceed the recommended voltage (3.60 V) while charging as this can cause damage to the cells or even result in a fire or explosion.

# Graphical User Interface (GUI) for Analytics in Level 6

- Close the Serial monitor in the Arduino IDE before starting the GUI.
- Start the GUI only after connecting the BMS.
- Always save the plots obtained while performing any operation on BMS. To save the plot 
- Click on Plot Graphs under analytics in the GUI, then 
- Open the PDF in the browser  
- Press “Ctrl + P” 
- Under “More Settings” tick the “Background Graphics” and save the PDF.