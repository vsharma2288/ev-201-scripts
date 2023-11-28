Now that we have looked at the basic terminologies involved with battery management systems. 

Let's have a look at different topologies/architectures of battery management systems. 

Many different applications require different types of BMS designs, for example, small vehicles like 2 wheelers mostly use only 1 battery directly connected to the drive train systems, while bigger vehicles might require multiple smaller batteries connected in series or parallel to give out the power needed. 

Such battery modules need to have their own separate battery management systems and selecting the best topology directly influences costs, ease of installation, maintenance, measurement accuracy and above all the reliability of the entire battery system.

Let's understand more about topologies and their applications. BMS topologies are divided into:

1. Centralized
2. Modularized
3. Distributed
4. Decentralized

## 1. Centralized BMS

In centralized BMSs, the entire functionality is integrated into a single module, which is connected to the batteries or battery cells via several wires.

Such BMS modules are usually utilized in small low-power 2 wheelers that use a single battery pack module. Such modules are also used in laptop batteries as shown in the image below.

https://do7js0tdxrds1.cloudfront.net/tdq0w6reh8l2g2am7cwc6efn6odx?response-content-disposition=inline%3B+filename%3D%22centralised+BMS.png%22%3B&response-content-type=image%2Fpng&Expires=1701167544&Signature=NxbEMbEvgBfos2y7NSUgpKSFeVF8JNwikRgNkUZ2UVYzPth0IXnIwyY3iD0yTi84lUmpIXPSialwqkaFEZ1XNSrlRul-JQePLkPwBg6YwVe8K3p5Z965xDLuJe3FCU4BnCMn1j2ORf3~LRMLaC0-MRq2id3T6GAmN6r9xxvLM4g6e2~SE0XxXX-5NbIIQ~y1mJg4LOgiLukWu3p5FIKI44Rhf4AjH~UBR~20mquHlGPr-5cyNjOEJ8k-PTLUz2O7lUOEZsvA8XuGoMhDaOSGvvqGxtcOQ4eRY5mEBo7zFRGwq~20hlw-KX03Jh49leIFpBkIakU7X549eRtGiSfW0g__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Caption: centralised BMS.png

https://do7js0tdxrds1.cloudfront.net/9e63ns2xobstwd7zip0uum326zmj?response-content-disposition=inline%3B+filename%3D%22Lithiumion-laptop-battery-internals.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701167544&Signature=B4ipD8Ed3v~PhOXMMEr632MpWYrWAF2Utt0dw4W29S6OcpPlLFkNIhY25TOF4d4~O3f1mLv4qJoMmEGoKccGvEea0hntAahOz3stuiPsraGsXhEHTj8Bh8rcPtNxHx7mQCEGxTkdSS6kYVSkYZkhvXT-UXL2353lUtWpZoD6wRGAEP22YukDDAZGJzs0XNXwc1yT4HHe0CkZg2YEulYfi-5APy9~2w8YPjRHreB0jhuY-ztF3WaXm~3BT1iAyiV9LD3~dINIUzIE9Us447M7dVY5rl3Qd5KmBwPLfFzum8GBQVaw1GS01KyEeRfLKQUaTRCX~ou~hWt3hWcQeId2AA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

-=- Centralized BMS in a Laptop battery
-=- *Source: [Lead holder](https://commons.wikimedia.org/wiki/File:Lithiumion-laptop-battery-internals.jpg) | License [(CC BY-SA 3.0)](https://creativecommons.org/licenses/by-sa/3.0/deed.en)*

## 2. Modularized

Modularized battery management systems are characterized by several identical modules, which are connected to the individual batteries or battery cells via cables, similar to centralized BMS.

The BMS modules provide data like single-cell voltage, current, temperature and communication interfaces to the other BMS modules. Often one of the modules is assigned the role of master, and the master module controls the entire battery pack and communicates with the rest of the system. While the other modules merely record the measured data and transmit it to the master.

Modular BMS units help in scaling up and building big battery packs. 

For example, The Tata Nexon uses around 4000 small li-ion cells that are similar to the ones used in a laptop to build its battery pack.  

In this situation, it would be very difficult to manage or get data effectively from all of those 4000 individual cells. Thus, to solve this problem, we can divide those 4000 cells into small blocks of 300 cells, and build a battery pack module of those 300 cells with its own individual BMS unit. 

Now, you can join as many of these small battery modules as you need to get the required power output. In this way, we can simplify battery management and also make it easier to replace defective batteries as you will only need to change a few batteries from the 300 cell battery module instead of the entire 4000 cell battery pack.

https://do7js0tdxrds1.cloudfront.net/fk9k814zeuxv74vb4y8n2abjzpyj?response-content-disposition=inline%3B+filename%3D%22Modular+BMS.png%22%3B&response-content-type=image%2Fpng&Expires=1701167544&Signature=AFSpJNTOOJ2GWIupcGvDBsYZXeS1~hQDzXZo9iMQvITrzIUUsix88Hm5RdULd7~73-Wr2Ao5izYRImTyul33OVZt8J8A-QCGmuwaMgMXrLOEVySwUE85rwHjH9S6QZKNYo-jk-7HcjmTUFXBW5Qwoichzi4zsWY~zOfB4d~TVlkiPVoBQkJDJppxQtb-OrqS7uHkIcS8pcd6qdwkT~Q66Z~YoHEMqW-k81akSExmCadmjtO1~EAIzxaVoZ0cAboW18wwQXDZgnaQoVDfCTxfknNzRbOuu9a7cB2whXO6vLU~J496xmHOWMrqeEco3e2nBYd3fivfGBYTfY5i07UG1Q__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Modular BMS

## 3. De-Centralized

De-centralised battery management systems are similar to Modular BMS systems, but instead of having a BMS unit for a battery module of 300 cells, we get a BMS unit for every individual cell. 

This helps for easy scaling and replacement of individual cells in a large battery pack. 

Each of the individual BMS units can operate independently of the remaining ones, they do their own calculations and take in measurements without the need of an external controller. Communication lines between the units enable information exchange and task coordination between the units.

https://do7js0tdxrds1.cloudfront.net/46uafz3ye9w6cxzsxgcg4cwgud03?response-content-disposition=inline%3B+filename%3D%22Decentralised+bms.png%22%3B&response-content-type=image%2Fpng&Expires=1701167544&Signature=pt9GSJ1XR0ChfqB7VEQV-PCKVmLLSocEIxPeoJ5xo85jnFx8cZGLzdtbIS6izcBcGh15ZCZIw0bBRsiqbvXYxSG9u9j1SXANd05gl0MZc2yMcq4twc9h5KbfoWMMoeb32ZLeJ7MJ9FFu4lsHJFVoYN6qHZtfE3ZILjvJAbsOHCOKX0bqseoryFVIwYW8lE0nhQ53KanTUhbzlulkGyU3eytZ~QE9ACLoG6s28PeDnsiokOEfPEpjOHuN8L-80nJpzJFKSedTiNb8h5ulJXXh3EdQbri9FmtJ~ze5n3DBiuyTUSh1v2Rnll39RQfxtiyxLHRuzTmdVKb5FSl7VdFPBQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Captions: Decentralised bms


## 4. Distributed BMS systems

In distributed BMSs, each cell string or cell is equipped with its own BMS module, similar to the De-centralised BMS topology. 

But in the Distributed system, The cell BMS modules provide a measurement of operating parameters, balancing, and communication. While a separate BMS controller handles the calculation and communication.

This topology helps reduce costs as we don't have to spend money on getting intelligent BMS modules for each individual cell, instead an inexpensive primitive BMS slave can be installed while a singular intelligent controller connected separately takes care of all the important calculations.

This approach helps in massive scalability as there are no maximum cell limits.

https://do7js0tdxrds1.cloudfront.net/76gjppz177ghyzgcuoyi1yhbu6ld?response-content-disposition=inline%3B+filename%3D%22Distributed+BMS.png%22%3B&response-content-type=image%2Fpng&Expires=1701167544&Signature=BWvxHYRh7MKTTJCSG92aCPsz~TBHswXlX-6rSY7xeQ6p6CbmECS1JZRgcT~XJKfbvPkyl1kpTHm3GLo3OB8R6KAu944UoooHs~5Kk4NlR-H-bA1RJwmI-bP1Tw7b85hBAgPj0mMUPmZGD9vo9a~z4Bf0gyc6pYrCT5fwhdD5zVF-QyMXyZYU3sbWsuvlpppFp7LzkmQEHVGzQv8TPEVu9xr62z0JjjchZG02AZWQ06a5l1ziuwwrdW~gAGNcSSY2p-0OjplinrdajKYXWwPdZ80kMFwAZbDcthSrd0ToXPfhoIznBzhBIup2T0L-jJi5b4iDqI5MIhMon6lzkYetlQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF