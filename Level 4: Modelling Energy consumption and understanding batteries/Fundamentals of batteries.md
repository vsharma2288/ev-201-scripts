### Introducing important battery terminology

This topic is basically the fundamental preparation for knowing how to use batteries optimally in an application. 

Here, our objective is to introduce a lot of background terminology that will be absolutely important to understand energy storage systems. It may seem like all we're doing is making a list of definitions and in fact, that's a big part of it. 

But doing so is necessary for us to come to a common language, to be able to describe carefully and specifically everything that we study regarding battery cells and battery packs.


**1. Cells**

We start at the very beginning with a definition of a cell. A cell is the smallest electrochemical unit.
  
   1.  A cell delivers a voltage that can be used to power a load and that voltage depends on the chemistry used to build this cell. 
   2. Some cells are designed to be used only one time and then recycled. Others are designed to be rechargeable. 
   3. The single-use cells are referred to as primary cells and rechargeable cells are referred to as secondary cells. 
   4. If we're being technical and careful and precise with our terminology, it is important to note that a cell is different from a battery. Technically, a battery comprises more than one cell, somehow connected together. 
   5. Oftentimes, in common use though, people use the terms cell and battery interchangeably.
   6. We need to be careful and make sure to refer to the individual unit as a cell or sometimes as a battery cell. And when referring instead to connected cells, you can refer to that as a battery or a battery pack.
   7. The voltage of a cell depends on the combination of active chemicals or active materials that are used inside the cell. 



**2. Battery or Battery Pack**

If we connect individual cells together, we build what is known as a battery or a 
battery pack. 

1. It doesn't matter whether the cells are wired together in series or in parallel. A battery pack comprises cells wired either in series or parallel or even in some combination of series and parallel. 
2. Batteries are sometimes packaged in a single physical unit. For example, the standard automotive 12 V lead-acid battery is built from six 2 V lead-acid cells wired in series inside of a single package. 
3. Sometimes, high capacity lithium-ion cells are in fact, batteries because internal to the packaging, multiple smaller cells happen to be wired together in parallel. So it's not always possible simply to look at the package and know whether it is a cell or whether it is a battery. 
4. In high capacity battery packs, there are often be dozens or even hundreds of individual battery cells that are wired together, and that wiring is usually then external to the cells, and large bus bars or thick wires connect the cells together in order to be able to carry the high electrical currents needed by the application.


**3. Nominal voltage**

The voltage of a battery cell changes depending on whether it's fully charged or whether it's completely discharged or at some point in between. However, we need some kind of a voltage label to put on this cell when we market it and sell it. So we have some kind of an idea of what the voltage range is of this cell that we're working with. So we define something called a nominal voltage, which is a typical voltage or maybe an average voltage of a battery cell, and it's somewhere between the fully charged voltage of a cell and a fully discharged voltage of a cell.
1. For many single-use or primary battery cells, this voltage is around 1.2 V. For example, standard alkaline battery cells or dry cells have a voltage of 1.2 V. Even some rechargeable or secondary cells have a similar voltage. 
2. For secondary battery cells that have nickel-based chemistries, like nickel-cadmium or nickel-metal hydride, the voltage is often around 1.2-1.5 V. 
3. Lithium-based cells have a nominal voltage of over 3 V, and this is true whether it's a single-use primary lithium-based cell or whether it's a rechargeable secondary lithium-based cell.
4. The nominal voltage is an average voltage or a typical voltage. The voltage of the cell at any point in time will be different from this nominal voltage. It could be higher or it could be lower depending on how the battery cell has been used over the past.


**4. Battery Capacity**

The capacity of the battery cell, sometimes also referred to as total capacity or total charge capacity specifies the quantity of charge that the cell is rated to hold. If you want to be precise and technical, the metric unit for the charge is in coulombs. But coulombs are very difficult units to work with when analyzing circuits and they're also very small units of charge, and a small battery cell usually holds many thousands of coulombs of charge. So instead of coulombs, which is the same thing as ampere x seconds, capacity is specified often in terms of Amperes x hours or milliAmperes x hours instead. And we call that Ampere hours and milliAmpere hours or sometimes, 
1. We are a little bit imprecise and we call it Amp-hours and milliAmp hours. 
2. If a battery cell has a capacity of one Ampere hour, then a fully charged cell can deliver one Ampere of current for the period of one hour before it is fully discharged. 
3. At the beginning of life, most battery cells will actually have a slightly higher capacity than what is printed on the package. And over life, for various reasons that you will learn about, the capacity will decrease. And for secondary battery cells, we usually consider them to have reached the end of life when their capacity is only 70% of the original capacity. That is when the cell has lost 30% of its capacity



**5. C Rating**

Electrical current as explained previously is measured in amperes, or simply amps. But the impact of one ampere of current from a small battery cell is quite different from the impact of one ampere of current from a large battery cell. Hence a relative measure of electrical current is used to scale the size of a battery cell, and this relative measure is known as the C rate. 
1. The C rate of a battery cell is the level of constant current charge or discharge that the cell can sustain for one hour of time. 
1. For example, a cell having a capacity of 20-ampere hours should be able to deliver 20 amperes of current for one hour or two amperes of current for 10 hours. This relationship is not a completely linear relationship. It's not quite that simple, but it's a pretty close relationship, it's a good approximation. So when we say that the cell should be able to deliver 20 amperes of current for one hour, we are saying that the C rate of a 20-ampere hour cell is 20 amperes. It's what we call the 1C rate. In this example, two amperes is what we would call the C divided by 10 rates because it is one-tenth of the 1C rate. 
1. To compute the C rate of a battery cell from its nominal capacity, you simply write out the capacity together with its units, which might be 20 Ah where the A is for ampere and the h is for an hour. And then you take your eraser and you erase the h, and we are left with 20 A or 20 amperes. So, ampere-hours become amperes, and milliampere-hours become milliamperes. 
1. If we start with a fully charged battery cell and we discharge the cell at a 10C rate, the cell will be completely discharged in about six minutes. 


**6. Total energy storage capacity**

1. The total energy storage capacity of a cell is approximately its nominal voltage multiplied by its nominal capacity. 
1. The units for energy are either watt-hours or milliwatt hours if we're talking about a small battery cell. It could even be kilowatt-hours if we're talking about a large battery pack.
1. For example, if a cell has a ```nominal voltage of 3.7V``` and a `nominal capacity of 1.9-ampere hours`, the total energy capacity or storage capacity would be 
`3.7 x 1.9 = 7.03 Watt hours`
1. Energy storage and power are different things. Power is the rate at which we release energy from a battery cell. It's the rate at which the energy is used. Power is measured then either in milliwatts or in watts or even sometimes in kilowatts.


**7. Extra**

When battery cells are connected in series, the voltage of the battery pack is the sum of the individual cell voltages. However, the battery capacity is equal to the individual cell capacity. The reason for this is that the cells are connected in series, and the same electrical current must pass through one cell as it passes through all of the other cells. So all of the cells are charged and discharged at the same rate.

https://www.youtube.com/watch?v=86jz_JKblXA
