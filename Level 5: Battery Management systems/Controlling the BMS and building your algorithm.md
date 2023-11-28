### Now that you were successful in getting valuable data from your battery management system, it's time to build an algorithm to control how your BMS behaves while it is charging or discharging.

There are Four Core functions available for controlling the BMS and there are 

### **BMS Control**

1. **Start/Stop Charging**
2. **Start/Stop Discharging**
3. **Start/Stop Balancing Battery 1**
4. **Start/Stop Balancing Battery 2**

Then, you have 8 other commands to Extract data from the battery management system. these are 


### **Data Extraction**
1. **Get voltage of Battery 1**
2. **Get voltage of Battery 2**
3. **Get Temperature of Battery 1**
4. **Get Temperature of Battery 2**
5. **Get Ambient Temperature**
6. **Get Battery pack Voltage**
7. **Power in milliWatts**
8. **Output current in Amps**
9. **Active Time.**

Now that you know what commands are available and what data you can extract from the BMS, let's look at how to use the commands.

Open the file named `control.py` 

and write the code after the  `# --Add Your Code/Algorithm here ---` line


### Using the Control Commands

Basically, all you have to do is write If/else statements to control the BMS

For example, if you want to start charging of the batteries if the voltage of the battery pack is lower than a set value, all you do is,

```py
# Check if voltage of cell 1 and voltage of cell 2 is less than 3.2, if yes, set the charge state as "undercharged"
if (cell_1_voltage < 3.2 and cell_2_voltage < 3.2 ) :
       charge_state = "undercharged"

# if charge state is "undercharged" start charging.
if charge_state == "undercharged" :
        charge()
```

https://do7js0tdxrds1.cloudfront.net/pe4pnp34v29v0k7somruw43uppvv?response-content-disposition=inline%3B+filename%3D%22Control+Flowcharts.png%22%3B&response-content-type=image%2Fpng&Expires=1701168657&Signature=BkyJeLHe56zF1tTNdY~1BYs2EJFTuqzu8b7IBuCO-oj6OhsxJz9zjWFvv-ezDzizqAh2xq2G-JC7w6zr6hwVgpG5ltYC5xDO8aKXNkRM-lQPbcrOZadzIKOH1yVyr6kpfFdf1KlTNC49kRy7aoooaUQ9yzw-FcJfo3Wgc8QcMF3EsgyeXEYlMQT7xvYGVpflp4tDwx~TB02OPeKOw-5NXTtZiRgR0nOY8ItrW6-Lz254TRG8kJFyV3X-X3CxLC6dzEclcf7I8ezUTi-TNT3mURkq6ovEDZPEJfWIXLhE8nGUac6Mh~Ofz0eCT1y0i-3~rg-sqqaWTwQfEMIIF0wCxQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Similarly, here is an expanded version of the sample code above that also includes balancing of the cells if the voltages of both cells are not similar. 

```py
if (cell_1_voltage >= 3.6 or cell_2_voltage >= 3.6 ):
        charge_state = "charged"
  # if both cells are undercharged, change charge state to undercharged
elif (cell_1_voltage < 3.2 and cell_2_voltage < 3.2 ) :
        charge_state = "undercharged"
  
    
  # if cell 1 voltage is more than cell 2 voltage, change cell state to cell_1_unbalanced
if (cell_1_voltage > (cell_2_voltage + 0.03) ) : 
        cell_state = "cell_1_unbalanced"
  # if cell 2 voltage is more than cell 1 voltage, change cell state to cell_2_unbalanced
elif (cell_2_voltage > (cell_1_voltage + 0.03) ) :
        cell_state = "cell_2_unbalanced"

#Charging and balancing cells
  # if cells are undercharged then charge
if charge_state == "undercharged" :
        charge()
  # if cell 1 is unbalanced then balance cell 1
elif charge_state == "charged" and cell_state == "cell_1_unbalanced" :
        Balance_1()
  # if cell 2 is unbalanced then balance cell 2
elif charge_state == "charged" and cell_state == "cell_2_unbalanced" :
        Balance_2()
  # if cells are charged then stop
elif charge_state == "charged" or charge_state == "fault-temperature" :
        stop()

```

### **In the Above code**

### 1. Check Voltage

```py
if (cell_1_voltage >= 3.6 or cell_2_voltage >= 3.6 ):
        charge_state = "charged"
  # if both cells are undercharged, change charge state to undercharged
elif (cell_1_voltage < 3.2 and cell_2_voltage < 3.2 ) :
        charge_state = "undercharged"
```

The above code, checks voltages and sets the battery state as `Charged` or `Undercharged` depending on the voltages of the batteries/batterypack

### 2. Check Balance state

```py
if (cell_1_voltage > (cell_2_voltage + 0.03) ) : 
        cell_state = "cell_1_unbalanced"
  # if cell 2 voltage is more than cell 1 voltage, change cell state to cell_2_unbalanced
elif (cell_2_voltage > (cell_1_voltage + 0.03) ) :
        cell_state = "cell_2_unbalanced"

```

This code checks the voltages of the cells individually and compares it with each other.

As we have learned before, all the cells in a battery pack needs to be the same voltage for it to be balanced, if the cell voltages in the battery pack are not equal to each other, the battery pack is said to be unbalanced.

Now, in the first step, we check to see if cell 1 voltage is greater than cell 2 voltage, if yes, we mark cell 1 as `Unbalanced` 

Similar steps are followed for the cell 2, and we mark the pack as `balanced` or `unbalanced`

### 3. Start appropriate commands.

```py

if charge_state == "undercharged" :
        charge()
  # if cell 1 is unbalanced then balance cell 1
elif charge_state == "charged" and cell_state == "cell_1_unbalanced" :
        Balance_1()
  # if cell 2 is unbalanced then balance cell 2
elif charge_state == "charged" and cell_state == "cell_2_unbalanced" :
        Balance_2()
  # if cells are charged then stop
elif charge_state == "charged" or charge_state == "fault-temperature" :
        stop()

```

So, after marking the battery pack's state, we start with either charging the battery pack, or we start by balancing the battery pack first so that the voltage difference is not very high, then we start charging.

#### It's time for you to do your own algorithm, start by building a simple control system and then we can move to a much more complex algorithm

>Build an algorithm to Start or stop discharging of the cell depending on the voltage of the battery pack. If the battery pack voltage drops below 6V, stop discharging