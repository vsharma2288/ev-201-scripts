Now that you have all the hardware gathered, let's start with building our motor controller. 

We will be building our controller in blocks so that you know exactly why each and every component is used and its purpose in the whole circuit.

> Note: If you have not received a pre-soldered Arduino, watch the video below on soldering the board.

https://vimeo.com/633896946

## What is Phase 1?

Phase 1 will be a section of the experiment where we make sure all our parts work by testing our code with an array of LEDs instead of the high current coils present on the motor.

This helps us make mistakes and not damage any of our components. This also makes it easy to explain how everything works and also to visualize our code in action.

#### Let's move forward with building our Circuit.

Build the circuit exactly as shown in the diagram Below.

>If you have access to a 12 volt power supply, connect the power supply instead of the battery to achieve similar result

https://do7js0tdxrds1.cloudfront.net/zm7kifghaeafxbo55vtdp6h0cqqh?response-content-disposition=inline%3B+filename%3D%2210k+OHM.png%22%3B&response-content-type=image%2Fpng&Expires=1701083858&Signature=iki1RI~Iaa2NMpcTeAAyCPjaHhyuDgrenKiAiKq6QXkaMd9uYVRantYrikgUoBzmcLTv21bdZ19Q9Q7VNDj0BKWGNQui9BjF0BZDSvxqbYQjAwVJDsx0xik7K7VXXURydOen1223Ac4xsmlm6gLIdr8fJHP30Vlo1M0WCwh2nN8Qc7t22KeGBfguk7b6MWu9F-yHmUMggKmpSQ7nWzAl8qSfEokhlR30QKyfdPnKyWvzm4VxegzbooLTl1rzbgY63B7SJzJNKGrNrK68zZLCzHZ3evYw8DD3yRb7~yO31hrWM4fE7oCOV0Pk8m35zG3NaQHlwTuxLjLPfVPHE7Qjug__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Once done, it should look something like this.

https://do7js0tdxrds1.cloudfront.net/9pa4hcxwl4zq44rq89t8nig0qh0v?response-content-disposition=inline%3B+filename%3D%22WhatsApp+Image+2021-10-06+at+9.57.37+PM.jpeg%22%3B&response-content-type=image%2Fjpeg&Expires=1701083858&Signature=mLJ7dWw~2hg736w~jKG3YZA7LslaHPJAwlejmb1RcGIQDbHFdXCWrc6yZaEM-B~GH671JkvtrqTUAf6~PkxyHWaRIeMNiLByLZDj36~rL2F24UyGv3vYLZMlmIwHbjwW33egKdnYteKAY~rQZQsZgDCYuXJinlsROHlKXWdj9HXIgAjxuyWasmFUeKtcI82yOW~1ne6UF7qGFj~sFVdRr6jMh7tPCFk-4KDt-qhXhFEHAipWBewwqGAyt1VuHGYuJ5jPr4pVWdz9~of-zZ3KXecC3Vujp-6Q3hmfR5MsRuzuMo3YloT5JWiqnzgVW5YZCajAenaV965cHALLRK5maA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

![IMG_20211006_220035-res.jpg](https://www.pupilfirst.school/markdown_attachments/4291/jdJHmSX-xIVq0ZZxsqB4kA)


![IMG_20211007_035520.jpg](https://www.pupilfirst.school/markdown_attachments/4292/RpuA_C5T82xCUYWbV--WBQ)


https://do7js0tdxrds1.cloudfront.net/qfdcmlewdg0p99eymtopc0jw9xx0?response-content-disposition=inline%3B+filename%3D%22phase1.png%22%3B&response-content-type=image%2Fpng&Expires=1701083858&Signature=tiHqOneplDR6FzwTpY5PHMNDKkaPZeAfCFaCYqNwwuD-LEf~8bYSwgUtRyfWinRrXyiAPA9ZvbFs-G-pepi3n4Y9pMYUXdbCMIfWi9sfgdsmgcZt0~bQ2-ct25XHMSlkXnTsQ9wIjM5Lh5V12H0PATjnRRN6k~4yqiAX3SH~2~02qE~XVHX3JjyoIKHodlBkdYndw6DI4V~ETWG1Wu0Er4FA3NFP00iz~HGBQD0bgf9KOwdLnWmGTfu5tQeQjN-xdvYiuOekvTM6Jkfv1igsEnJ5jpgfRJa7572x8xbXbxIlIfdEunOjCRLdylN-kZz3f5~oU4usUTyk8nS~hv9ofg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

>If you have access to a 12 volt power supply, connect the power supply instead of the battery to achieve similar result

https://do7js0tdxrds1.cloudfront.net/pudbtk2rpopqy9m5lhh9gfvumzzg?response-content-disposition=inline%3B+filename%3D%22IMG_20211007_040005-res.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701083858&Signature=FCyL9IZHSDtfLRIsLoX0C2pDZM3ImfTVaZUZB6d0~PGFxQ8dEgFKGi7j~WZvtdh18jcibi5RUaTLs0JUmqutDLNMjGsXgEHeDk6QW53lmo9vJHStBNU38cZpziaBz51mOiQm1wgey-~O3tKJ7wexApsUGYJ8-go8O8Qp20UAa7q2p~fMYgsElczvJCCVKgmTRjdTYsYsNeOkAnit26RJKaZlHsFZU0EkGl1dN5peQIk4pu9z3HestjBEXzsfHuHV4mBvPj5l91aYHvMyXzWnQOMg1DU3AidHu9LenRc8kh9F3sqHbXzwPdMyUN-eFBNNJAqwqDp2vAGWWeKlHW6Oww__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

### What are the MOSFETs doing in the circuit?

MOSFETs basically act as a switch or a separate pathway for the power to reach the coils.

As the motor coils need a lot of current to run, this cannot be provided by the Arduino. That's why we are using a MOSFET as a middle-man to supply the required current and voltage to the coils and making the Arduino act as a gatekeeper.

Whenever the Arduino sends a positive signal to the gate of the MOSFET, it starts conducting electricity through it and energizes the coils. 

It basically acts as the push-button from our previous experiment. 

Have a look at the video below for an explanation with an example.

https://do7js0tdxrds1.cloudfront.net/oks4zrjr4z5mubg8m81mc8rqm88p?response-content-disposition=inline%3B+filename%3D%222.png%22%3B&response-content-type=image%2Fpng&Expires=1701083858&Signature=hhhCna9Ls7pcCY3oSchglX3D4ODzgYzC25Wt3gqtE6EbX7-u-r2uJInHXotVH-Cda4OjG80pGnHVsdfHHOEE~JFOdJbePqPVJNXaPglh2WuJTeTXozf3PvS27IzEoea-Qb8ZRVNRkeGIwwLI6KewyHIE1ywT8ovhAYTdJQD1rrX8r3ND9UYlx8GnQ~oNgXWac0vDdTQPE6M9Reg~ljLSpUcSaP6AQjmvz-YRhJ8OO7hOHfX3yeOknnp-wRYau21bS1JHOdFP8KeF5r2kTgDUQGWYz~0L2Z4ufK4u9BRhGfQ7wdDu5uct8ykrei6q3iy3jsygiIGP6t12cNnj4-xlbw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

https://vimeo.com/625842602

## Programming

### Step 1: Install Arduino IDE

1. Go to [Arduino Download](https://www.arduino.cc/en/donate/) and click on **Just download**.
2. Once the download completes. Click on the executable and run the installation.
3. Launch the Arduino IDE.

https://do7js0tdxrds1.cloudfront.net/t52u9dz2xmmxrnodw5z817z2pprx?response-content-disposition=inline%3B+filename%3D%221.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701083858&Signature=tgvexHMjQN0gzyForqVebd7ewU8MpjcbMee2tRRJxU8H-L0LDX6e9Ew63KHbOYgRgnwUWpTZYoprU3uPX~8F-ci6ONc2tKeg44KOEvsfl~8eCnvhJ2lqUuWyhH4evmViQBRv0-haKufnd3YQWO5u34aW45mC9PwUcZDR5GjrRv7OKrgPu9XNclimBaID1LWe5mXeYJ7EAWti3hnmhiiAvJLWZp6BZXKQs2YIwJj17Ji61TIg1F1Tc4xT0dRnjmTNNMjRT8mY52VVWm133uG8~v5vXRYxiXPuoX2MT1yYEiGPxeKMhOLxSy0oEoVPkaacGcrf7FMZOXl0sdkpFBHiJg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF


4. Click on tools and select your Arduino board, as well as assign the port that your Arduino is connected to.

>Tip : if you have only one Arduino connected, there will be only one port visible. select that.

https://do7js0tdxrds1.cloudfront.net/sn1oifaun3aqkgnzxobig36xaxt0?response-content-disposition=inline%3B+filename%3D%22Screenshot+%28103%29.png%22%3B&response-content-type=image%2Fpng&Expires=1701083858&Signature=iqhi19Jt--Ktmqvk27OFLNR9eP8r3iCW~iQKIQTFI3k1kLm8XKiY8mb8zan7uRyUTNtzpRJ09p~B3ouHchO5W77CJNvQ~L05fxKUD2eDIttZ66dW4RId4HW2AOUpSgb0ErtpqrbuuOPkMMAaTK5LrL0KMGCTMp0dtYM33vnVGUzSKXIoByafej8gXqusvWnN9v1RF8nX6DHQonGyBu9gdvp97RI0dq7eiCBobaD3wxOLvkd79ZPGN6ab-VlK3QcIKfbTUhozU~x3djuEFHVPZKLLC2urAvrOfBvK-dl3K888LyAQ~GuljI7Kk2JUS24bYTy-lu8RzvvUw2eRbwk4PQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption: Select processor "ATmega328p"

5. Paste the below code into the IDE and click on the "Right arrow"

```
void setup() {
  // initialize digital pins 2,3,4 as an output.
  pinMode(2, OUTPUT);
  pinMode(3, OUTPUT);
  pinMode(4, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(2, HIGH); 
  digitalWrite(3, HIGH);
  digitalWrite(4, HIGH);
  delay(1000);                       // wait for a second (1000 milliseconds)
  digitalWrite(2, LOW);
  digitalWrite(3, LOW);
  digitalWrite(4, LOW);
  delay(1000);                       // wait for a second (1000 milliseconds)
}
```

Once you run the code, this should be the result.

https://do7js0tdxrds1.cloudfront.net/b8kj6inoknhk7292j0hh19d6jnx4?response-content-disposition=inline%3B+filename%3D%22result+phase1.gif%22%3B&response-content-type=image%2Fgif&Expires=1701083858&Signature=MtqJXEzPirOFsZJA4pz0xvSOOSWPpeCPOHLOZ~J5GtGMeiyxDpcRe1-vVDwBN7TCYwDx~yHBvLqzqslXplebPwp61ir3TP9cKPoxuGF0Mg60NZTshlu7ySGxo1EE4ClGJlCMWartgnpD57Wa4YFZetaIP4YWzrraE8GHhVr6Wk-Vw7~qlaTT85-fPjAiWEPl8VHHXhAeLfYl~KFx~V4mNRo6p10fw5VNKUtJXPoCxO2CyPQJih9gyZ7-Jy6nJKoYbn~lEjmdP1Fjew4zgpfumUfjt5fx~G-Z~v1d1by7kAW0gMop3H3qVGtVpBsfD7FepqlGcpsZ67rBSVt4-qbnOg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Now that we know everything works as it should. Let's move on to building our controller for the motor.