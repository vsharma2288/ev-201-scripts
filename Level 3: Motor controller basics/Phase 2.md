Before Starting on the motor controller, Here are the Do's and Don'ts

### Do's and Don'ts

**Do’s:**

1. Before soldering, make sure all the components are placed correctly in their place with correct orientation because resoldering would be much harder.
2. While doing the connections with Arduino  make sure the in1 and in2 pins are connected properly as per schematics, incorrect connections can cause shorts between MOSFETs. 
3. While soldering the MOSFETs, make sure to keep a good amount of gap between the BMS Printed Circuit Board and MOSFET screw hole, such that the heat sink will fit properly in its place.


**Don’ts:**


1. Do not press the soldering iron continuously at a spot or to a particular component on the Motor controller PCB as this may damage the component due to excessive heat.

Before you start wiring, You need to select the correct MOSFET,

In your kit, there are 2 different MOSFETS, you will need the ones that say **IRFZ44N** on it. (Refer the Image below)  

Make sure you have 3 Pieces of the said MOSFETS

https://do7js0tdxrds1.cloudfront.net/qo17zwy7jk9udtzyp0s6goytlw6x?response-content-disposition=inline%3B+filename%3D%22irfz44-n-channel-power-mosfet-1-800x800.jpeg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084125&Signature=YuUepNLl-YYVzfQ68y-3h0HN9dGF6Uw59Xko1HLRnfLhhfq58fFkNF1Dc7QXz-TsKa6NvQQiFBOcAP6wc7T~eaAYAVlVxBhQ~5PrJ4LnSWo2FxPfd6nRZTjzvE5QfmX9veOn9LWftnGqDCKQ8ll7DExt4weFBn7RKy0VbHTUxqVdUjnxys1FZDovbVhCzL9-~MKX~YoBCODinwZ2kfKQEvXBqKfCp1rB7pinr3DsgF6drW69B0epkEm2Qd8Nl3nyhPIA1pkelgQyzhrtF753ixU4HK1J1-gdYsNknGGeghQRpO6Pk72Be5uHohTU8-XL9w1~mVxSjHa19ucdzN2CWw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Once You have the MOSFETs in hand, Use the image below to note the Pin Naming.

https://do7js0tdxrds1.cloudfront.net/4e1w1z85o8b4g9p33e05hmjpxmdx?response-content-disposition=inline%3B+filename%3D%22IRFZ44_2_RobotechBD.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084125&Signature=s9IaWejtK4PwfN3vSRxK52IcTQEBpGyT5p45wK1vAtcrFmZC7sUe2O1mX8PUAVSP65Me7DYpE~okGf~c5QHjhmkbu6iBAetYMJicztLsZvN8nc69Zaiw5L7RQFLLGMlgoUi-F0W-SvpFy7VNnmVj3EG-sU8X5OBr8KkiDdkExOjx7sBplqCisfzBuUrC~bkfmxel4fjMG~a0EUnkbNphDVQP3BnmTeUpadQhi~IPGBsrzZoaS446nKCgX5GbnT2fTs80TOTYlt78A6qqxpgICXbmEL1GchVQ3PwVajw61aLsnP7yV~JWAb6UlrYGNlxWBvgW2kKu8viYVOWG1dLsww__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

IRFZ44N Pinout

#### Lets move forward with building the Motor controller

https://do7js0tdxrds1.cloudfront.net/hcgsjw3d8fb1r8dnox7n519dj5u0?response-content-disposition=inline%3B+filename%3D%22phase+2+breadboard+%2B+pwr+supply_bb.png%22%3B&response-content-type=image%2Fpng&Expires=1701084125&Signature=MbYPDY~hxKhQLh9xJyLAlheH7ZOtKUrwfH6oP7VbDJgaWPwQp-2IBcJXBHJtEmgtjfXmiDL7eRHCk5QGmJqVA-FGRbYSpM~zcvX2d-cD6pVIU4fLg1cYJPQ6k2P206ljUZw9jC2YtxxnVJNSWVGweqQtgrst3MV6tfn5LOa1GMpJvJ5zyQCw0XUGmQcy9Wg5FgQM-XzDZKz1TU-TI3VGWX-7L6~FQD~nFCwtQsaakufxDRCHf0O7C1-smU5bxZdsQ0mgfvEBG6ghKvJy-z2Tl44RrojMhuhibwzx2PZXp5RhsKHvBQP~E~20C0X-rQ6tq8GgWpVZTtz3W7vtIAbXqA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption: Step 1, wire the controller just as shown in the image above, use the given Jumper wires to do the connections

https://do7js0tdxrds1.cloudfront.net/xlt1gqnp011pgkahyaj470agfvmk?response-content-disposition=inline%3B+filename%3D%22BMS+As+power+supply.png%22%3B&response-content-type=image%2Fpng&Expires=1701084125&Signature=B-SAXN30NBCF4oLh8XR-26DOlaBfL3iaZ-9m0TJiPb0R1ZkfjmNbBsNCW83avocyvWbi0XYoUSdDd0TK5UbwuwHsYBstMGLvV9atiGsKCgyfjnAg6p4BhbfbDD32SQ~5RcUR3fiqE75igxSPjeGdfXBwyYG8XaeSerGB-Q8Y1sU2JYcuW474qJpTyTDt6u~jJZcPgfDGev45CS1T7286epLCLzKmHTY4L6h~okxKyaQzQ2-Iddk9-VhLk21BfagSttDoy0-igog8BTPibpo2DKMGvEYPgYCd8BkWTCxpl-X8ITiwJPgZpn3VXYa3U0Igf5XevhdhHixk5kksOwnQ~w__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption 2: Step 2, Use the BMS as shown to provide power to the Motor controller that you have built

https://do7js0tdxrds1.cloudfront.net/rbuqwtudmde8yhh5kpcnialv26nx?response-content-disposition=inline%3B+filename%3D%22Motor_control.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084125&Signature=UFdUr-juA36uJEvMfivoiLdwlYT2lADamhzI~08dyZgzKCKWmUo9wILaNP8MSbhve-FQGMIezsORGX~65gp9zxlEaNtST~ng6auLKXP8xSWYoSYOGl8zTbE~OH510N-5ODxtsbAkhQ2811GlUufo8-Ut6Qo~YmdbzE5yzf2zzjugdcPxbWMPqtdZZ0sxEw0wFYMCiV0eUtVuz4HllFhl1Nn734JA3US96sJAW0xzCCxC-UgIdiISlHyHOe5eJmTgec-pu4ngs3NmQHLoPsN9eiCzseAqTTBj8Li2kdtw7icu4-OwARTVxjxhvqyxkpc9XpasYUjFPlHNCP2nWMPgfA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Now that you have everything ready, all you need to do is upload the code below into the Arduino to make it run.

Connect the Arduino to your PC using the given USB and Upload the code below.

Paste the below code into the IDE and click on the "Right arrow" or "upload" button

```C
int Delay = 800;


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


  digitalWrite(2, HIGH);
  digitalWrite(3, LOW);
  digitalWrite(4, LOW);
  delay(Delay); 
  digitalWrite(2, LOW);
  digitalWrite(3, HIGH);
  digitalWrite(4, LOW);
  delay(Delay); 
  digitalWrite(2, LOW);
  digitalWrite(3, LOW);
  digitalWrite(4, HIGH);
  delay(Delay); 
 
}

```

Once you run the code, this should be the result.

https://do7js0tdxrds1.cloudfront.net/aly0sluiz8ngte5zde00gzp4bbr7?response-content-disposition=inline%3B+filename%3D%22IMG_20211007_195723.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084125&Signature=Aa9DOKCjBP4s2n~V1nmXNpLe7W58P6dQOyBLl1JC6b1yoOk2TUNzwsKe1Gw84oJWC9u7Dd64kR~Ac8Ry-MMcfxgw8nkK79I-dfVsWE0kC4c~pR7Xg5OdOXggzYz1p3~H0cWTQAUrWXBE6mapzoN39cJqwrglhj2HQ0ZiNIpuz7mo~1ZIcDQnxsVghaVWpBbX9zxisLETCXBc3nQ0DE~sWdFZA4Dx5vIGm8-vhB1hjLsDfna6uu2wlPE2VJh~fpMmZcqSvciiNibX4PS0kARqY5d8uBlFdcDLANoC-R3INA1f9KXSbr2lk245Y~RJUFQdJQiK4g1WNW1evTeGb4mc1w__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption: Make sure to use resistors in series with the LEDs if the power source is greater than 3 volts.

https://do7js0tdxrds1.cloudfront.net/z9rb506svbtknxk5w4f3lxiqmn5u?response-content-disposition=inline%3B+filename%3D%22WhatsApp+Image+2022-07-12+at+2.19.54+AM+%281%29.jpeg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084125&Signature=O8bTWHN6L3DNvZWS0-RRZxrmb4vG0OGtfigO8bssHW3dvFsKNy-OoO7eFzcDDxt2FD3UGjtl3Nj9nAS3wTLan3IoxWPS32Ke2D5fgBU7MgMUzZIwzDdmDcQAKTINacw0QITFll7ur5E9qUyp0tzonw2UA~JcS~vwBsgkYuHoHEIUukVwAdcN23uiClXZ~-vt7Jc8Qg2QrF~00Lg~ZbrUv0cnDWO-1yq70W1DeQxp3232DHw-ROk0FcZRcJWgcsGFnEodegf~2PFQrtA1NzenREi3htjjo0TKpNU1pSx4nuLMlY5xnOfGYCdJXtoZEangNQVDADkrxTLdbAgerZMkuQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

https://do7js0tdxrds1.cloudfront.net/axb5m6hvt95yfy0ccbrco3eiyo0b?response-content-disposition=inline%3B+filename%3D%22WhatsApp+Image+2022-07-12+at+2.19.54+AM.jpeg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084125&Signature=Jg1Xez9zyVV3oS4Qb1aI374~jU6Wnsp-0shacUA6yEfHnJps~On3BRwsNzGlHILfR51Cd6ueSYfE6zxOP4HrChoUCuiMmIH5nZS~jCBkHVvJN~0sr3vYvlbOPZyVM1OrDMjlihcIygwJvWp0Z1vdQ6BBM-AZ8oLoq7R0hnRLsFwaKZfOpHLiqDx-Erir6RqaDUEDZhyRRjuRln2~bL1mxeSfIp9-by-sQLAElTjbFrcNWUgu8ty51YrK6QwiiWfOXMWEC5n4xYFqJRUaqihUIH-nP8wc6F4aUARgRCG8KbfOoD64ANdOYSugsFURBylt8AMkkkxCivEMbBfa0Lrlgg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption : Make sure to add Resistors if you are connecting the LEDs in parallel to the coils

https://vimeo.com/625500502

### Sample submission which was from a student from the previous batch that used 4 AA Batteries and a bench power supply to power the motor.

The Motor in the video is running at 40 milliseconds.

https://vimeo.com/700485636

>For your assignment, incrementally reduce the `delay` in the code to see what is the maximum speed the motor can rotate. 

The current delay is placed at `1500 ms` in the code, vary it within `10ms` to `500ms` to check max speed

## -=- END

-----

>If you are unable to get the above Model of the Motor controller working, you can move to "**Phase 2 - With relays**" as that would be much easier to work with.