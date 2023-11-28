### 1. Transmission Modes in Serial Communication

Serial communication is the most widely used approach to transfer information between data processing peripherals. Every electronics device whether it is Personal Computer (PC) or Mobile runs on serial communication. The protocol is the secure and reliable form of communication 

#### Simplex Method:

In the simplex method, either of the mediums, i.e. sender or receiver, can be active at a time. So if the sender is transmitting the data, then the receiver can only accept and vice versa. Therefore, the simplex method is a one-way communication technique.

https://do7js0tdxrds1.cloudfront.net/in3tqvn2k0kfcu78bmq4ogi7hjez?response-content-disposition=inline%3B+filename%3D%22Simplex.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701171315&Signature=E54XsHxqAB9QnkUBewFePY9s5SooPDlTcnAg1RT0b-W5BoO74KPhAgyHny-r6SqPaiz7teEoRAtHCGhC7irTB2P2Vgvk3otoKZmEowejtfuldrYmthrHNgt0UCcMuKlSskES39xMDG-ViLzGr4uk-qpLO9IGlhntGmZr9nY9cOlt3bcs~XCzZqIf3Ma6~xxK1vYdXslXlcsoGZxgGFhJs~eYerTzqRogoPn8C2b3kuolf~GQFfUH37zBUA821M0VKPLCyg1awGVSMK2lt~0MVSgzpACsZOXxxM0gcffoU8GWmzSEvXUB9PzdBDMFpyfja1WOllMONfJudyFCsOKpjg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Caption: Simplex Method

-=- Source: [SlmedioP](https://commons.wikimedia.org/wiki/File:Simplex.jpg) | License: [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)

#### Half Duplex Method:

In the half-duplex method, both sender and receiver can be active but not at the same time. So, if the sender is transmitting then the receiver can accept but cannot send and similarly vice versa. The well-known example of the half-duplex is the internet, where the user sends a request for data and gets it from the server.

https://do7js0tdxrds1.cloudfront.net/hvxa7v2zpy2ztgii6hdlol3hiipt?response-content-disposition=inline%3B+filename%3D%22HalfDuplex.jpeg%22%3B&response-content-type=image%2Fjpeg&Expires=1701171315&Signature=e2sOgqPP8DJEQVGltRyFg0YxXyM0lG-rQZI-57Dc1IE0tBa~OQEcG7ZVmVMrCOdnnZDWPB6cpshj8PHCt38di1R3rU7m7YAkJJzvsEF1VEq5E4aCerYi7G2~EcrbJVI7Xw29rBJQoP29t7ZxkKcXkPk6M0mIb0-B2Pq93k~9lTw4rzmvFI1J~5x2M8fbixuno6mH--9MHB7UNFTWYxv~RsO1DQw33evW34uyXv1-YmhW75OrMKvMhXYMBnoaNDzlI~~crwQ9awVX779l6nP3tvMOPgoV0iSAvEycn7Agza8ItmrSwB77lVSkqWXqSbE-v7Nbc60TkgJvW1RlsWq1xA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Caption: Half Duplex Method

-=- Source: [Greggreggreg](https://en.wikipedia.org/wiki/File:HalfDuplex.JPG) | License: [Public Domain](https://creativecommons.org/publicdomain/mark/1.0/)

#### Full Duplex Method:

In full-duplex method, both receiver and transmitter can send data to each other at the same time. A well-known example is a mobile phone.

https://do7js0tdxrds1.cloudfront.net/dw3mcrhayc1mpp6xazpgs9gswjfn?response-content-disposition=inline%3B+filename%3D%22FullDuplex.jpeg%22%3B&response-content-type=image%2Fjpeg&Expires=1701171315&Signature=fdCWn9ZpGLCu7RYwFQAhWlznHmB6CUvaRYoPY6Ai3VUyJ43~cDO85xk1ajIgkDlAq0~hrKw1cc7Fx2jQ3HSJZpW5B7nqPLByjqM3C6p8pc4cRE5dxCirAM-BxZ3m2bmS9KdmdpVUCk8lNgTD3GZPVUmGhtrMCrHLSTaFoswypEL5KwJqiEwCrkROSjAUnvPvqTL5K-MpQIupWlgXYnbSnbGT42wstnb5GVRlyVk0J5sfzjTzl1pmLN9v42jj-3jXG3nV4JnHhyl3XNhoxcbIg6l5--gjogsZg-P5Wp7Z9NKk5BmCCMyx1d1A6M-tawbnJogUaAgRzlz2VWwBPxjN9Q__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Caption: Full Duplex Method

-=- Source: [Greggreggreg](https://en.wikipedia.org/wiki/File:FullDuplex.JPG) | License: [Public Domain](https://creativecommons.org/publicdomain/mark/1.0/)


### 2. Clock Synchronization


![Synchronous-Serial-Communication.png](https://www.pupilfirst.school/markdown_attachments/4478/UdMXXPIh1vwEGlHicfeqSw)

-=- Source [Sparkfun](https://learn.sparkfun.com/tutorials/serial-peripheral-interface-spi/all) | License: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)



#### Synchronous Serial Interface:

It is a point-to-point connection from a master to a slave. In this type of interface, all the devices use a single CPU bus to share data and clock. The data transmission becomes faster with the same bus to share clock and data.

#### Asynchronous Serial Interface:

In Asynchronous Serial Interface, the external clock signal is absent. The Asynchronous Serial Interfaces can be seen mostly in long-distance applications and are a perfect fit for stable communication. 

In Asynchronous Serial Interface, the absence of external Clock Source makes it rely on several parameters such as Data Flow Control, Error Control, Baud Rate Control, Transmission Control and Reception Control.

### 3. Other Terms

#### Baud Rate:

Baud rate is the rate at which the data is transferred between the transmitter and receiver in the form of bits per second (bps). The most commonly used baud rate is 9600. 

>You might have seen Baude Rate of 9600 commonly used in Arduinos.

But there are other selections of baud rates such as 1200, 2400, 4800, 57600, 115200. The more the baud rate, faster will be the data will be transfer.

>Also for the data communication, the baud rate has to be the same for both transmitter and receiver.

#### Framing: 

Framing is referred to the number of data bits to be sent from transmitter to receiver. The number of data bits differs in the case of application. Most of the application uses 8 bits as the standard data bits, but it can be selected as 5, 6 or 7 bits as well.

#### Synchronization: 

Synchronization bits tell the start and end of the data bits. The transmitter will set start and stop bits to the data frame, and the receiver will identify it accordingly and do the further processing.

#### Error Control:

Error control plays an important role while serial communication, as there are many factors that affect and adds noise in serial communication. 

To get rid of this error the parity bits are used where parity will check for even and odd parity. 

So if the data frame contains the even number of 1’s, then it is known as even parity and the parity bit in the register is set to 1. Similarly, if the data frame contains an odd number of 1’s, then it is known as odd parity and clears the odd parity bit in the register.