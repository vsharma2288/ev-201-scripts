In the previous chapters, we have learnt the need for battery management systems and seen what would happen if a BMS is not used while working with Li-ion cells. 

Moving forward, we will learn the different types of battery management systems as well as their working principles. 

But first, let's understand all the terminologies used with respect to batteries and battery management systems.

### State of Charge (SoC) Estimation

The **SOC** is an indicator of the amount of remaining energy or charge available in a battery as a fraction of the nominal value that is the rated value of capacity.

For example, the SOC reading for a battery might read 95% full or 10% full. The **SOC** provides the user with information on how much longer the battery can perform before it needs to be charged or replaced.

We also need to keep in mind that, with time and use, the maximum capacity of the battery constantly and non-linearly degrades, making it very difficult to extract the exact value of **SOC**.

### Coulomb Counting - SoC Estimation.

Coulomb Counting is the most common method used to estimate the state of charge of a battery. 

According to this method, the capacity of a battery can be calculated by integrating the battery current over a period of time. 

This method depends highly on the initial state of charge of the battery and the total capacity of the battery.

To explain this method in simple terms, imagine a battery as a movie theater, and when the battery is full, the movie theater is full. 

Consider, the total capacity of the movie theater is calculated by the number of seats it has. 

Now, after a movie is finished, all the people in the movie theater get up to leave and they move towards the exit door. (The movie theater is now "Discharging" if we assume the theater is similar to a battery.)

When the people start leaving, the doorman at the exit door starts counting people as they leave. i.e he is counting how much the theater has discharged, as he knows the total capacity of the theater and has counted how many people have left over a period of time. He can estimate how much longer he will have to wait to get the theater empty. 

Similarly, regarding batteries, the coulomb counting method counts the number of coulombs that have left the battery and estimates the state of charge and the amount of time left for the battery to keep running. 

### Kalman Filters - SoC Estimation

Kalman Filter is another method to calculate the SOC of a battery, this method is highly sensitive to the accuracy of the model of the battery and its parameters.

https://www.youtube.com/watch?v=rOwcxFErcvQ

### Battery State of Health (SoH)

The Battery state of health is basically the capacity of the battery to hold charge compared to when you first bought it or when it was first manufactured. 

The capacity of a battery degrades over time which leads the battery to hold less and less charge.

https://www.youtube.com/watch?v=imjbyeS1caI

### Battery Depth of Discharge (DoD)
The Depth of Discharge of a battery is basically the reverse of SOC. Depth of discharge (DoD) is the fraction or percentage of the capacity which has been removed from the fully charged battery.

Compared to SOC, which indicates the remaining amount of capacity the battery still has. 

When a battery has discharged its full energy capacity, the depth of discharge, or DoD, is 100%. When it is anything less than that, the depth of discharge, measured in percent (%), is the ratio of the energy that would have been discharged by the battery to reach its present state of discharge from a state of full charge, divided by its energy capacity. When the battery is fully charged, its DoD is 0%.

### Battery Life Span
Why is DoD important? The life span of many types of batteries (for instance lithium-ion batteries, indicated as Li-Ion, lead-acid batteries or nickel-iron batteries) depends heavily upon the number of charge/discharge cycles they undergo. The deeper the DoD per cycle, the shorter the life span.

Now that we have looked at the basic terms and their meanings involved in Battery management systems, lets look at different types of battery management systems.

https://do7js0tdxrds1.cloudfront.net/f9glpkleggwsn3ubty4vk59314h6?response-content-disposition=inline%3B+filename%3D%22nickel_iron_battery_-_depth_of_discharge_life-wikipedia.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701167415&Signature=i~3lNuAHrY~kxcE9ZiRXmH9UZ~czoOWGXuMkJOARbFGgmnfF5HGdw2-By2rOTnm5dQoeJjBB0UmoJb24QYNHotSlMCwFkMPT-5K205FoB85gMgfKuecyI-7WCGkCTgVNzY2SSmRdSIwIgQPpjujRlrL~vlFVfU~Ud37YBBiDNdj~oFcl4xMzkt-PROVbtooi9CPG9AVCWiKH0AeLF97Ng-X4PmWdSBy9hMGnLxiaENYvNhfUhLqxgHNjUoNbRm~2lOf2gRWag0YWECR~-SFGWtfr14nH-jwsWRhW-Zd282a2Q9FDPf3MPthPPonf9nKdFOXo0edQNSPJJixexhyYRw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Nickel-Iron battery life cycle – source Wikipedia

### Cycle Life

One charge cycle is a period of use from fully charged, to fully discharged, and fully recharged again.

https://do7js0tdxrds1.cloudfront.net/rgv8gefd367hpvscckgcmwhqgs0l?response-content-disposition=inline%3B+filename%3D%22wevj-11-00066.pdf%22%3B&response-content-type=application%2Fpdf&Expires=1701167415&Signature=o2igyB0nmNPMaRl74UeoKtIHsoT~OiD1rYxq815byBiSIgmSk1FBbPTczclW2Lq~m44hyg48PeoIOc0xTGVEmGA8jJU1oUSsb4s99m25lDOJR9PEb8sY3WYJw~Ji6C0I03C6Us~aJuSJ8RxO-62FWSiuuZQA5Le5jYL2o9pluYI8sqYjyipCWMd-MpetfrAjP1t6UrlDs97ENOrPGwNQludV2JpCUPfmVMFb~US6MYA5HkcN9e87l0IYsh4kH5UncIbUIxNt-BhYMfjBM5C9l~R64wU3LPSttEjkzApnMnXDYWtW7r1JY0TWHPoLGmOh-0d3U-1GFi96dZfOUhXfcA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF