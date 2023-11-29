https://do7js0tdxrds1.cloudfront.net/0bj5zgh6nmyoqipmja8nisjczd24?response-content-disposition=inline%3B+filename%3D%22201+overiview.png%22%3B&response-content-type=image%2Fpng&Expires=1701255409&Signature=sDMWeGBhcqfbr6P5s0kowrO~nHkfp9qZP65r6d8jhH6jt8JU2zzM4Lh6Yo56kxHDMeUWyXZ1XdN8DgN8uOh2P5uSm2jymEV-XWed0hRQgHfqskj4NbMTbCpOYat7rmTZNucRZnI7JAaWhO0f9Ze533r-SxAOHmPGxAtI6qoJira3G1BQfH11ox3Diw4TRLrlcbHYEyVS5p6rRIh1zYpS4L~q-l~2oVvTcGHQq-jOxm~-VewDJCNPFAH57ICRbucxQ~nCoP50ui~b-9aoT1TJkooRt5brd2FL5cPF7Jd0O1U-AdgDDpYJuGWBfG0s8sfp5YWYxKE5FlmYje515zmJPQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF
Caption: Overview of the EV drive train we covered in this course

### What is electronic communication?

Electronic communication is basically the process of transmitting and receiving signals from one electronic machine to another electronic machine. 

This can be done two ways.

1. Serial Communication
2. Parallel Communication

#### 1. Serial communication.

In serial communication, all the data is sent in a queue. 

Imagine you are a packet of data. So now in a serial communication, you are standing in a single queue to get to your location.

https://do7js0tdxrds1.cloudfront.net/scz165qiewrs3pdi6nbaqe3b6df6?response-content-disposition=inline%3B+filename%3D%22serial+gif.gif%22%3B&response-content-type=image%2Fgif&Expires=1701255409&Signature=O92AlGbxDIk20BNvO8jPokPI8mv16zEwNJ5pVX5wr4Aw-IF0B~51ONbi0o0JUupsIAUdUjlgA2SmscJ~4BP8NBHdhTCPhyjmZ9i28zgYKvdg6Iu~gprfR39pmRTf7yd~bbokvV-ozN7Ed0GUW54LnN2hpUuFKw1W4pnvKM6nkgh5IQDQVJ1VxXqw5L58vtWAtQKBz50hMATz0TfDw600XrCXSRMN-PE7IYfQEsllV6rg0V~vn6Hw16F54Pm71Rm7v6yMovnYh54ZeI6uMVQ3av2f9l-eOesUhmEVkXoGu~-N0VVgmtg8pnwXXkoLw67tZtU-soIN3LSnu9jTmsrpDg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Can you imagine all the advantages? And also the disadvantages?

The advantages of using a serial communication are, it's a lot less complicated to handle. But the disadvantages would be it is a bit slower than a parallel communication system.

So, what is a parallel communication system?

#### 2. Parallel communication.

https://do7js0tdxrds1.cloudfront.net/ssw9cw2xk3bqp8b2pdbjrza5ffln?response-content-disposition=inline%3B+filename%3D%22parallel+queue.gif%22%3B&response-content-type=image%2Fgif&Expires=1701255409&Signature=X9TctLkJFUhbwNrHYXekIe485xQM8rf2xuZXXn2EHn9-6IML44x7vZ967uZ19J0HtpVBfgqirNvZgUV0d5j2u-xprsH3x8Pg3uDsf8EmLyWCxamPvDq6wLcuN0kw1guahlOfsPHhD4rjh-bkTrlp0dLaCTwozkPxpZ0MZl3LMor4ks-LGztznQNHKI-I1uR4rYsMU7PrKNc4DXFSiq9cUL6v4or5z7Up0Xd-YWw1zOtut8-35CTliCRx~2WjhGT96PFc7fjTHNLc9SNlxUS49vc4hsyKL-U~Lrp68OcMRNkzKqSPkTcNJOSaTubqhzwpfZvjcprhB7G5GVHrMXprVQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF


Parallel communication is precisely what you guessed! It's two or more than two queues of data transmitting at the same time. 

The advantages to this method are, it's a lot faster. But the disadvantages are, it only works for short distances, and the part of receiving the data gets complicated. 

As one part of the data is in another queue, and another part is in another queue, locating all data packets and combining into a meaningful pack of data gets complicated, and during large data transmissions, there are chances of data losses.

Therefore, for our model, we will only use serial communication. As it is also easy to understand and to implement, and most cars on the road today use serial communication in their electronics, for example. CAN bus.

But for now, we will use i2c as a serial communication protocol as it is easier for beginners to understand and also because it is quite similar to CAN bus.

#### So, let's start with the wiring.

https://do7js0tdxrds1.cloudfront.net/i2pn5tbupyj9kiiyjrbopo92fubc?response-content-disposition=inline%3B+filename%3D%22L7+wiring.png%22%3B&response-content-type=image%2Fpng&Expires=1701255409&Signature=dInrEWrr1xadATbEbqRcMpXjgNjwXevkMJLI1XEqvtcIGuOQdZCDsDTV6O~O9LlwMFvwrDrXDF9oaZ7HadH7EQsOFP~sdFFUMfKb5NMYgc0t71T9RAjK21vSfxnepAS94vmgDjcoCN4krmqQZVSokTxnjfq1rXseWcOrAcE2U-f2CrKbtPM~ECUJwAoe-uwMLp7jaiGaAt4Tgg8u~1eU1kxk5O9aIwsXNPzBmEXfKVhw2hRv6cGu4NL7zulzuKdwv0z-tzyZ7YjxNxTE2oZ~9NyEI3l0HxZHHTcJFFR~NRRSB40Cc2H0Nh0aWxroibK6-czEeGphEmPRbXaeBJrrvg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

There is nothing complicated to add here:

You will need to use the existing models from Level 3 and level 5 and join them together using 2 wires for communication.

```
A4 from Motor controller -> A4 of BMS
A5 from Motor controller -> A5 of BMS
```

