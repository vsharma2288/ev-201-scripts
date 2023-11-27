>Now that you have learned the basic types of BLDC motors and their topologies, let's find out about motor control algorithms and how they work. You also read about some real-world examples in various areas

An algorithm is a set of instructions designed to perform a specific task. Computer programs are essentially groups of algorithms.

As we have understood previously, in brushless DC (BLDC) motors or permanent magnet synchronous motors (PMSMs), different software algorithms in the motor controller improve efficiency and reduce operating cost by monitoring and controlling motor operations. 

In sensored BLDC motors/PMSMs, some of the primary functions of the main algorithm are as follows:

1. Initialising or starting up the Motor
2. Detecting the position/angle of the rotor using Hall sensors or encoders
3. Checking for increase or decrease in current reference using switch signals
4. Figuring out the rotation direction of the rotor


###  Understanding how the motor controller takes in and processes Sensor data.

A regular BLDC or PMSM motor contains three hall sensors at 120 degrees out of phase from each other, when their digital output is combined, it produces a three-bit number that denotes the motor position.

https://do7js0tdxrds1.cloudfront.net/7x08nyp7m106ky445eqastriqey5?response-content-disposition=inline%3B+filename%3D%22scorpion+stator+120.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084769&Signature=OluUDqpeKr5JN4ysU3IDbuRntocxMRIw9z7hkm6~SIK9hdKSOP~KFxU50EpOnGWRk7PNMaKQCO3t5lxWH8XdrAbzD5S2Y3uAGNFXlQzVNx7nwSGqBmDx0GX9~-Bpce2uZZN8NSiwJTZbSLnjfN7ImR~yzsaxHX1bDiZo0b-~-PZSkIuDQKZxhTTKsg82HL0bz~Om59O7ag87NwAmDkZuqQrutnK6fLueunJXX2bYSvkmNeaKK-KLVawlSTYkD0ggi~om2MDbTBhgJT4QiubA~fjPsIsw~dfg3SwjPX89JyeKhWAPmZsSVlIdWcdtapJrgxrK29KPgASHn6pZlGahzw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Fig 3 : Red Dots represent hall effect sensor placement.

Now that we know the number of hall effect sensors, their positioning and we also understood that they give out a 3-bit number data output (each bit connected to one hall sensor).


To clarify this process more, let us understand what a hall effect sensor is and how it works. 
* A Hall-effect sensor is basically a device that gets activated whenever there is a magnetic field present nearby. 

  1. When a magnet is brought near the sensor, it gets activated and starts to conduct electricity. 
  2. In simple terms, it is a type of switch that goes to an “ON” position whenever there is a magnet nearby.
  3. But in reality, a Hall sensor can be used to calculate the intensity of the magnetic field. But for simple explanation purposes, let us just consider it as a simple ON or OFF switch. 
  4. Now, when the Hall effect sensor is in ON position, let us consider that state as “1”, and when the sensor is in OFF position, let's consider the signal as “0”.
* As there are 3 Hall effect sensors, there will be 3 different “0” or “1”, to let the controller know if any of the 3 sensors are On or OFF,  thus giving out a 3-bit output to the controller.

A three-phase BLDC motor has six states (the six possible current states derived from the three-phase outputs). 

The sensors are placed to provide a three-bit data output using six of the eight opcodes (1 through 6). 

This information is useful because the controller can determine when an illegal opcode (0 and 7) has been issued and act on the legal opcodes (1 through 6).

https://do7js0tdxrds1.cloudfront.net/6mulpk2zrf2sjp0lzbz5x0pamd5o?response-content-disposition=inline%3B+filename%3D%22imageonline-co-piechart+%281%29.png%22%3B&response-content-type=image%2Fpng&Expires=1701084769&Signature=VaLzD4yTHg~60-QwX3~3KXojGIFhD86xv47EI4X9Mrc1crCHSHvRVjLvYBWhhIEYLxkbu56yFb3xlXpvhdvy3gid2GeSiD~Cb~qaogEpPlprSjWUav5R0sG1XhdFXPY14wYX4A4Yu8pYo7dvvx5lwqRznqQ1TnNHbn7WzYnPuD6w0g~wN2MNw8Tg92P7yfU9RrZ-wTp8oUxWyXNRcli2QjCnwW8vpeSD8S3-KArhyV7gcukQaOrrRH4U~Ux-WN7DNShw-PiTWM3-Klxt3~O0OqMV8NiQnPZw2xQwBdxA3sYMcjUmVx-sfzFkPG2yurW8rVEE8~ZojGnP9LkGc3hHHQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption: Commutation motor sectors

https://do7js0tdxrds1.cloudfront.net/v528qe1veoyrqhcfsnemurskzwkd?response-content-disposition=inline%3B+filename%3D%22Untitled+design+%286%29.png%22%3B&response-content-type=image%2Fpng&Expires=1701084769&Signature=Ys0YQ2lD6XMDkMHZOscGammwzyVBnbMcS1topyHnj~9dYCrmhv230XGAcwryS5EoZ60Y1sqtozaB3Y615VzSGh7YtgZ4osnxa~etnMcLtD6cIzyL3p3CPUNzzmgBsE4tFolYi~QM7Wnlwb3QGbQC5sHTW7Ahl-eSpS5eBdc4FD-VE7B~pqcAutFoU6JNQikFpWfsFWMSVVDLttkhTSSwLTFHhA3oIIxWefRWtisRGaJKnmXdDABmxpHAwVYnCpdD284JvvEVaCdiszQy-KsgaQ1ABUAa9ATQL2OX4zSg4MJsbTaP3hwCrQJT0b5OVBftpBeSnvKVcDJV6uYeaC6t6Q__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption: The commutation (Energization) sectors when placed on a motor.

| HSW Hall sensor 1 | HSV Hall sensor 2 | HSU Hall sensor 3 | Hall Sensor Opcode | Sector |
|:-----------------:|:-----------------:|:-----------------:|:------------------:|:------:|
|         1         |         0         |         1         |          5         |    0   |
|         1         |         0         |         0         |          4         |    1   |
|         1         |         1         |         0         |          6         |    2   |
|         0         |         1         |         0         |          2         |    3   |
|         0         |         1         |         1         |          3         |    4   |
|         0         |         0         |         1         |          1         |    5   |


Here’s how to read the lookup table

* When the Hall sensor W, V, U equals opcode 1-0-1, opcode-5,
sector 0 is energized.
* When the Hall sensor W, V, U equals opcode 1-0-0, opcode-4, sector 1 is energized.
And so on, for each of the other possible states. 

Each Hall sensor is positioned on a rotor so that one change state occurs per rotor sector.

The algorithm obtains the Hall sensor opcode and decodes it. 

As soon as the Hall sensor opcode changes in value, the controller must change the energization scheme to achieve commutation. 

The microcontroller uses the opcode to extract energization information from the lookup table. 
After the three-phase inverter/controller is energized with the new sector command, the magnetic field moves to the new position, pushing the rotor along with it. This process repeats endlessly while the motor operates. Similar to a donkey following a carrot as shown in the image below.

>In simple terms, the Hall Sensors detect where the magnets are located and switches on the coils nearby appropriately. just like you did in the motor controller you built.

https://vimeo.com/625836391

https://do7js0tdxrds1.cloudfront.net/6soydy7h6l62ug54d87plzpbrlea?response-content-disposition=inline%3B+filename%3D%22final_6103142662a8fb0099216335_811908.gif%22%3B&response-content-type=image%2Fgif&Expires=1701084769&Signature=HVh2IvGWrvvKyav413JX-hYz4iwwQ5fx-RS4znsAzYjur2wDPt9CBe6lClRNtj6KRHCpALInyYUiYKLJMZtRCEFMjzlTDTBVk6gykuJaqWuqOkNDoU--3kcXilJjRJ4WNyyw-YUsTHUUoEDBreZL0bDkKZVwi9aC4hw9XtRKkG9J36WSYYUolKcHtBWAH7HW3zJoSuj0Gf9Z8TU7VSwSZ7FvGq9oLjVVBKk-QuqNvld754ZIOwBW6nFGferLD8Bfe~jctKl4~ylqRI22~xHO6hJuokzYFOF3egT6bngeyejjm~V16TTAF19MW~yhF~nrm-Xpga8Q9E4I3CXrTbCJWQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Here, with respect to our motors, consider the rotating shaft in the centre also called as a **rotor** in the Figure with a permanent magnet with 2 poles as your **donkey**, and consider the stationary part with the orange coils also called as a **Stator** as your **Carrot**. 

The orange coils on the stator work as an **electromagnet** that attract the poles of the permanent magnets present in the rotor in between the stator - see Figure 1. 

The rotor rotates whenever the electromagnets are switched on, and the magnets in-between move towards the electromagnets. 

Now, once the electromagnets attract the magnets on the rotor they need to change its polarity, in order to push the rotor forward along its rotational path. so that it continues rotating, instead of getting stuck in one position. 

That is basically how a BLDC motor works.

Further Learning:
* https://www.youtube.com/watch?v=bCEiOnuODac
* https://www.youtube.com/watch?v=ZAY5JInyHXY
* https://www.youtube.com/watch?v=WyQInXjpGwU
* https://www.youtube.com/watch?v=fpTvZlnrsP0
* https://www.youtube.com/watch?v=VI7pdKrchM0
* https://www.youtube.com/watch?v=5eQyoVMz1dY
* https://www.youtube.com/watch?v=bZwLFpXhFbI