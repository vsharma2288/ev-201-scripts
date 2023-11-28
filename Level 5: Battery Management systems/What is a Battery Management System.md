Now that you have learnt about the different types of batteries and their applications in the previous chapter. Let's now learn more about controlling the power of those batteries for better stability and safety. 

#### But, let's first understand how battery cells in a battery pack act when they are not controlled or monitored.

Imagine a scenario where you buy completely new cells and gather all the cells with the same voltage and build a battery pack out of those cells. 

### For example

You buy 10 Lithium-ion cells, check their individual voltages, and observe that all the voltages are at 4.1 volts. Let's assume 4.1 volts is the voltage when the battery is 100% charged.

Once you have done that, you take those batteries and go on to build a battery pack by connecting them in series, thus making the total battery pack voltage of 41 Volts.

`4.1 V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` = `41 V`


https://do7js0tdxrds1.cloudfront.net/ymo9cye0iumvq87ppv0baavmju7v?response-content-disposition=inline%3B+filename%3D%22balanced.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701167080&Signature=cEN3figopv~6qDf9dQdh5ReXQ-Oq0rPV9bhcPoM85jFptV2ffbmgUtnrkQWK4ASgVVZE1c5xZQR2T4i10HyAZQm1wXBkB-wcwq3qy1QhPskbRWJ4S~QS92qj0jAMG3-MayZuH0A~JJMZ1Sb90HlLnedySGuT9t3VzKaaTL12q~gik2ANrHAd~wQwMX8P7~FivpxkMeK~YHajggqcVKDqWKakp4sCKF~km5ebIHPbvRZY7r-EbDUSdh0YUYyp-kX5PtFklSFUnnGYxBh7b6bkzlgvH6dPqzyHZiZm60GaeTuXZOli4DEMHK2NpW0L2vwBD8bzONd0os-Q2O9LawWpRQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Cells in a battery pack that have same voltage

Now, once you have a battery pack ready, let's try and use your battery pack for an application, like running a motor for 1 hour.

Now,

After using your newly built battery pack to run a motor for 1 hour, it most likely will have lost some charge, just like your smartphone loses charge after an hour of usage.

Now, to understand how the battery was discharged and how much, let's disconnect the battery and the motor and completely disassemble the battery pack and check the voltages of individual battery cells again. 

Once you check the voltages of each battery, we can find that they are not consistent. Some batteries have discharged more than the others and some have retained some of their charges and it might look somewhat like this:

`3.7 V` + `3.4V` + `3.6V` + `2.9V` + `4.1V` + `3.7V` + `3.5V` + `3V` + `3.6V` + `3.5V` = `35 V`

https://do7js0tdxrds1.cloudfront.net/y0fvhczp1lyj0i5m72bq6ezmpec8?response-content-disposition=inline%3B+filename%3D%22imbalanced.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701167080&Signature=L8qz78mOPM3NYLE4~UWEaJ7WiQJUr-qOozqSugbkp2bEkA~5vrfGURhn-jfDb7R0GuMpsPRXLsWXn-ZA2EOF2Q1-dF8WeGZSu3LKdOQUburEx-CfVNvvBv8I18g-nJ1uFNMWt5kMfBVXL7UbT5XN6AXldenFijOPlZBw7fnGZKDjBDuMeQXaeTpcEhdpvk1T6yvRtN-FCz8cvUEJMaVyeeR9OY~r9ppKeXwsHQ~URkcMlfB3Vv1I0E43QuES2DOTZK7B82AV1~5yP5mogliK02cCKIeLYBB7TUJVWyUrHfLRdrIStvmnEVdeWY6IrZd5fiRf6Qmq4o9RyFxR~JypzA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Cells in a battery pack after use

As you can see, the cells in this battery pack are not "In balance" i.e, the cells in the battery pack have not discharged at the same rate. 

## Why is this a problem?

This becomes a problem when you start to charge the battery pack, i.e when you charge your battery pack, all the cells in the battery receive input current at the same time. Thus the cells that still have higher charge levels than the other cells will get charged faster and the cells that have lost a lot of charge compared to the others will take a lot of time. 

This means, charging will not stop until all cells are fully charged, this, in turn, will be a problem for the cells that began charging at a higher charge level because these cells won't stop charging even after they are fully charged. This will damage the cells as shown in the example below.

## From our previous example. This is how it is going to work. 

#### 1. You build a new battery pack that is 100% charged and balanced.
`4.1 V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` + `4.1V` = `41 V`

#### 2. You use the battery pack for an application and check voltages, the cells are discharged irregularly and are imbalanced.

`3.7 V` + `3.4V` + `3.6V` + `2.9V` + `4.1V` + `3.7V` + `3.5V` + `3V` + `3.6V` + `3.5V` = `35 V`

#### 3. You want to charge the battery pack, so you connect a power supply to the negative and positive terminals of the battery pack.
Assume in half an hour you charge all the cells in the battery pack by **0.2 volts**,
i.e. add 0.2 volts to all the cells in the battery pack.

**Adding 0.2 volts**

`3.9 V` + `3.6V` + `3.8V` + `3.1V` + **`4.3V`** + `3.9V` + `3.7V` + `3.2V` + `3.8V` + `3.7V` = `37 V`

As you can observe above, cell number 5 is currently at **4.3 volts instead of 4.1 volts**. That cell is now overcharged and is damaged. 

>Let's understand what the main functionalities of a BMS are and problems that can occur if a Li-ion cell is overcharged or damaged without a BMS in place.