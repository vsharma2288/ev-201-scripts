https://do7js0tdxrds1.cloudfront.net/a0zznidlvxvdilrhz9hhnyg7qtdy?response-content-disposition=inline%3B+filename%3D%22level+3+Phase+2.3.png%22%3B&response-content-type=image%2Fpng&Expires=1701084468&Signature=o~aSdyYSpj8hK7WynGZOjdqtrnsTSymztENubSM8uF~rLIDbqhE9DpbwBvgtY4z6kG~1gDWE1pDKVXl99GIFwRfCKCvoQ6lspzz8VcpdcMnAN16BUHMp7n0q6DTWwFs0pAACrHoS5DSB0df05s3Tlpb-e44ncqYUqdTYRiZa1qOW6Y53d6q~Eo5psWYxvhkHRidx1XGReHHz0r0QhZHJsoPFZHGcnW7eC3i4aJFzgFvHToUjCQZf-9KczYiJRkZocbI2YtGuo2ZlxCkxOqwoK4Y4JY~Yk5YZLO8FzRbY4dIIFgefvRMVF3N9F7nlcpL2Npb2RqkF5sv9uQURkv7OOQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

https://vimeo.com/721725188/1d46f1e5f1

https://do7js0tdxrds1.cloudfront.net/ikdn1tjzp5gc4elxdkzjr7tdj1ch?response-content-disposition=inline%3B+filename%3D%22IMG_20220618_180538.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084468&Signature=Px4BoQa0KhoKTQfg5KDFlP8k3WY-QYX1GYuhkBDfHIztclbWCJnrAQJYkjtYrLDoF5YCMGGiNltAFjYbtOr0g4OCHZ8~GhRoKSE2WIZiDF6ETMy41kR109A2XU6N6cw~1eGgK6rcMADjA6efV6uyowtWDXMAi635~a2hY3d7-eAVKSeYYGVKglvAUyx4adEtPRvAvx4E6sfZa--h5HN-U0vKv7NRXOldRas4aKueaNlJzCM-WPyAijrrwFHqfKoYdHe0aJp1a8iiK0fuLZuBDI6Dmp~go9LforasnUci056kJcUAMxfi~WVC4QRSrBrX39WPQkf5lW3szNU2NmT5vQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

- Make sure to connect relay GND to Arduino GND
- Do not connect Arduino GND to the GND/negative terminal of the 12 volt supply



Paste the below code into the IDE and click on the "Right arrow" or "upload" button

```C
int Delay = 500;


//Engage coil = HIGH
//Disengage coil = LOW

void setup() {
  // initialize digital pins 2,3,4 as an output.
  pinMode(2, OUTPUT);
  pinMode(3, OUTPUT);
  pinMode(4, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {


  digitalWrite(2, LOW);
  digitalWrite(3, HIGH);
  digitalWrite(4, HIGH);
  delay(Delay); 
  digitalWrite(2, HIGH);
  digitalWrite(3, LOW);
  digitalWrite(4, HIGH);
  delay(Delay); 
  digitalWrite(2, HIGH);
  digitalWrite(3, HIGH);
  digitalWrite(4, LOW);
  delay(Delay); 
 
}

```

### **Student Submission for reference.**

#### 1.Debajyoti Das 
#### -=- **At 200 MS Delay**

https://youtu.be/o1zDvtg-Fh4

#### -=- **At 20 MS Delay**

https://youtu.be/eU4jOa5kETo

#### -=- **At 10 MS Delay**

https://youtu.be/mdf1p79C4Uk

#### -=- **At 8 MS Delay**

https://youtu.be/4JTyfVvCA6s