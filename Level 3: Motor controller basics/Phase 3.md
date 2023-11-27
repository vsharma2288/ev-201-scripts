https://do7js0tdxrds1.cloudfront.net/ntqrh78f9jabtnxjyovwnasjcju0?response-content-disposition=inline%3B+filename%3D%22phase+3+presentation-2.png%22%3B&response-content-type=image%2Fpng&Expires=1701085064&Signature=qycUjOprPK7Fl3KkSqyKIKrppvazO0I73t6BlaV7egPHRp0mT8knybu8ZY0YW4vECNW6Y-Ofdw-XSCmCpWsEnwaBo5MflIxehubJE~3-t-sOdIK-nAeLLvxIzGURw2Ia~Ps0cxADhTEnAhEQE96nQws95oAaTEc0g8ChEsVSvEM-wWsME5cMjnUwGkyAHntm1oKEX3xRyZLriOwe5X5397FtnYQK6NXp1RHES0hV2efWcV9pEMbC65sW5oOUAgMWYslZXLRxB2RT4ZokUJcGFXblsZaHsMjFUBM09YsiG3Hd4~7pX2WHXRSx5AayzQSDYYqj3z7B7O7XhKVrKbO5Fg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption : Microcontroller Overview (Q1, Q2, Q3, Q4, Q5, Q6 are MOSFETs shown as switches for simplification)

Now that we have understood how a basic motor rotates visually in the previous example where we energized individual coils to attract the motor towards it. 

Let's now look into motors that use attraction and repulsion of the rotor magnets to produce rotation and torque. 

Have a look below to get a basic idea on how our microcontroller will activate switches to produce the required motions.

### Step 1 :

In step 1, MOSFETs Q1 and Q6 are activated, which in turn energizes Coil U and Coil W.

In this configuration, Coil U is repelling the magnet, while coil W is attracting it to produce a push and pull motion.

https://do7js0tdxrds1.cloudfront.net/8gyi8ly2xly2vh8fbnjqm9xgfi3j?response-content-disposition=inline%3B+filename%3D%22phase+3+presentation-4.png%22%3B&response-content-type=image%2Fpng&Expires=1701085064&Signature=OEylXppKtCXCzIZV81BC8hNLNHjCvMi63sIYimauHH7raABey9kBT3tFlTitpDtv4B3KEip~aBR4vduJQy0~Eg0RH2FlCZBq66tZJFjPwYOAY~mOsdlErkXLzKJfh37ZV68BfU3RWimTpG-BUvVH-XZ9Vc88PEN2I3x-HMH36txvXburXj-0KQ~tae80R2TAM1jwwKTlb~gsAcK9iiSKAiXmmL35CBH9n50iHm1-nhVoYrC7UDQRO~9cUOWJuBErrjSI4BbTf5~2srusFM7uPW7ap8lztcZaFxx7DeN24aYPkWGoVbCKVSIlAU-9GvCzLbt6PH7nWE~DYfGF9yxtVg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Step 1

### Step 2 :

In step 2, MOSFETs Q2 and Q4 are activated, which in turn energizes Coil U and Coil V.

In this configuration, Coil V is repelling the magnet, while coil U is attracting it to produce a push and pull motion.

https://do7js0tdxrds1.cloudfront.net/dz5wt8bawjlc8czlkocfemkgynrl?response-content-disposition=inline%3B+filename%3D%22phase+3+presentation-6.png%22%3B&response-content-type=image%2Fpng&Expires=1701085064&Signature=V6-zMdwZRVSy0xSSQmdGghiTAz5qI43V9Oa9erXi4cyU27LIQcoO9Cs9gLFhBq9mLpdQG0-ZQC-GQ~~sbAgYI9-869HdBQEQPM3agh~go4io6KLVHeXvNZ3uR1o-WIpWZtlvEYOvX5rKh3GG1P4Hue0~xUstxpZboYFJmbFRuPqgJiIWBEJHUigAjieYlHPNZNO4BM-cZH5Slu5~ayWNT0G6gy5fOar2-NYKBquzO7vKlWIcudHMT5pbybBN93S2Xdix2MysvB73n5M-OFytfxnYWLMajyoLmzS6qSeMB0au-TPNFzHObUQb6-VAZRaRZAHvm-UouOFrroa2EAYJcA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption:Step 2

### Step 3 :

In step 3, MOSFETs Q3 and Q5 are activated, which in turn energizes Coil V and Coil W.

In this configuration, Coil U is repelling the magnet, while coil V is attracting it to produce a push and pull motion.

https://do7js0tdxrds1.cloudfront.net/2io6hqk1nujno7btgjaygyvmlema?response-content-disposition=inline%3B+filename%3D%22phase+3+presentation-8.png%22%3B&response-content-type=image%2Fpng&Expires=1701085064&Signature=sBB8TGf8tlH3xbq1zMhlo6JpXq1fg1nykkDeRuQxHVaTloT2tXF-3LA1ysamIV1qw6lApdtVw~jCXEpgeCJeDwsJn1EFUeWVF8XbT-7yLYMGbEPuKq-l0HMvcF7Rj5yqujWPpOZhqC3v0cbl3opLCgjtSj1FD9PHFxF6mwg4KEiQ3Rc7WF3zjeqOF1wZMKPEJ9pyEX-k3t0DQStSxTMg4PgFw5PK6tp6bQWza8f~AVCK7Zy4XI7p6JfbxYJkNQ9xiO3aEXDl838WjONBAqm603orM1eLcO5aerK0oLWay94-hvGNmAeqhyeg77cC8RhkqlL1Y5DxpHLDZ71t-azLaA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption:Step3 

## Testing our logic explained above

https://vimeo.com/643317674

## Basic circuit you need to build.

https://do7js0tdxrds1.cloudfront.net/hh02rb0s9l3en7bniu8buwljjj4t?response-content-disposition=inline%3B+filename%3D%222.png%22%3B&response-content-type=image%2Fpng&Expires=1701085064&Signature=t2ea26b3JXnGfuWIGsuGpyZJYznou58K~qzZPtiFsYpo1WOTi7enS-ZluV6V~WkMIzdrU3033n1una0gzaASNw5d29sKsLXQ1M~yQ-uN1-UxANgYS7jRhWfEaruz5AmCkqkrrrzC2NfYu6TClQn5YQQtpR8NOJcOUFzvavlq-KqHiB-Fa1tAjiTCcy8C3IjcbbQPOtMAaLDoORMRrS46RUEmwgFqktN2UxRGoPKQUK6QYGvPrLK1AGsdZy~KnXgi133d5UnBC~W1PJfNzRb9LjuKZp1CMYJ8tOCz8GOT4ZIQV7mYYUFwyXe4xusZsgX9mqH7m8-gDo8EVM9Su5k3~A__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

```
Assign digital pins 2,3,4,5,6 & 7 on the Arduino to respective RELAYS as shown in the image above.

Q1 👉 D4
Q4 👉 D3
Q2 👉 D2
Q5 👉 D5
Q3 👉 D6
Q6 👉 D7

```

## Writing the Arduino program

Paste the below code into the IDE and click on the "Right arrow"

```c
// Assign digital pins 2,3,4,5,6 & 7 to respective RELAYS.

int Q1 = 4;
int Q4 = 3;
int Q2 = 2;
int Q5 = 5;
int Q3 = 6;
int Q6 = 7;


void setup() {
  // initialize digital pins 2,3,4,5,6,7 as an output.
  pinMode(Q1, OUTPUT); //RELAY Q1
  pinMode(Q4, OUTPUT); //RELAY Q4
  pinMode(Q2, OUTPUT); //RELAY Q2
  pinMode(Q5, OUTPUT); //RELAY Q5
  pinMode(Q3, OUTPUT); //RELAY Q3
  pinMode(Q6, OUTPUT); //RELAY Q6
}

// the loop function runs over and over again forever
void loop() {


reset_relays();
phase_1();
delay(500);
reset_relays();
delay(500);
phase_2();
delay(500);
reset_relays();
delay(500);
phase_3();
delay(500);

}

void phase_1() {

  digitalWrite(Q6, LOW);
  digitalWrite(Q1, LOW);
  
}

void phase_2() {

  digitalWrite(Q4, LOW);
  digitalWrite(Q2, LOW);

}

void phase_3() {

  digitalWrite(Q5, LOW);
  digitalWrite(Q3, LOW);
  
}



void reset_relays()
{
    digitalWrite(Q1, HIGH);
    digitalWrite(Q2, HIGH);
    digitalWrite(Q3, HIGH);
    digitalWrite(Q4, HIGH);
    digitalWrite(Q5, HIGH);
    digitalWrite(Q6, HIGH);   
}


```

Once you execute the above program, your motor should be able to run without issues and produce much more power than before.

Submit a video of the running motor once you are done.

### **Student Submission for reference.**

#### 1.Debajyoti Das

#### -=- **At 10 MS Delay**

https://www.youtube.com/watch?v=mdf1p79C4Uk&ab_channel=DebajyotiDas

#### -=- **At 8 MS Delay**

https://www.youtube.com/watch?v=4JTyfVvCA6s&ab_channel=DebajyotiDas

Now that you have made the motor run, lets understand how you have wired it to make it work.

We will be specifically discussing about the coil winding and connections that you have done.

https://do7js0tdxrds1.cloudfront.net/9sdel4l8l2dp9xkfwavggbmw03zh?response-content-disposition=inline%3B+filename%3D%22Wye-vs-Delta-Winding.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701085064&Signature=dypMgP0T89x89-L3AL6~LTviqKrYMaJ4UkN6G-Prw532UyKLyqGHVHVd9ruOHXLx6dCtoRu6FKhzEpwl4XuX-eQojhVla8OUa840PVqEpYPL3sF2-xA2NAXvin5DuhVveUrAGAq7fxMlUyrSDaVflWlOOcgTr~OWWDH~uCKnQalPBKHzEx5eKN2ij2Vu~JNXMowOJ8vmMYYNatey7bBcA1gIU197FQZLvOSKoj3BMlrGojW~LoZoqqrzkd7nS68mqrMGH-CTpSBylMRi0N4gRPz8wcHOdFVzbFee8iV3Xqre6OvAASEUtulN2tjOhKW7d-L9NbNFcYHOpQH2qVJ0eA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

##  Star winding

In a star winding configuration, the stator windings are connected in a "Y" shape, with one end of each winding connected to a common point. This common point is known as the star point, and it is used to provide a reference voltage for the windings.

To control the rotation of the motor, the stator windings are energized in a specific sequence. This is typically done using electronic commutation, in which a controller switches the stator windings on and off at the appropriate times to create the rotating magnetic field.

The advantage of using a star winding configuration in a BLDC motor is that it allows for a more balanced distribution of the magnetic flux, which can result in improved performance and efficiency. It also simplifies the control of the motor, as the star point provides a convenient reference voltage for the windings.

Overall, the use of a star winding configuration in a BLDC motor allows for efficient and precise control of the motor's rotation, making it an important aspect of the motor's design.