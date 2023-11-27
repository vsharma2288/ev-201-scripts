https://do7js0tdxrds1.cloudfront.net/8tjcfyhi25ndhdhxatv87m0uyp4f?response-content-disposition=inline%3B+filename%3D%223+pole+main+gif.gif%22%3B&response-content-type=image%2Fgif&Expires=1701080071&Signature=Hwg4hKD5AyS0TCCIeZ8-yr-hMv7pc8UT3Ko9ansCBkgk7eKFDtxDWX-t5Jb4oANBB~Hhp-75OXXddbz9JnCqkM02kmXkjBfCOYyS19bIeDe-Wo-VNAq6mPoeuvMfkXMVB~cALGkBgGOz8plTQrfcFIAJ3J1wP1HNtdRanhD-3NdHXuTwkGVSTBipkCuOrVbpgBuFYxt7RWMkanKJzDAeIPqNez0HWMeBkCE3Q7znog3NLSBJZUQ3mtXSk25DTHmv3~RUj3OkA3DzUogCN5Kfi03DEUprtLdpxb9I2dS2d9S2NpEPWnXfRZXf4MQFCPNQiKvdxvkPoJxIxUfG6EQu6Q__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption: An example 3 pole BLDC motor


Let's make an electric motor that spins using neodymium magnets and magnet/copper wire. This shows how an electric current is converted into motion.

We’re building a primitive brushless DC motor. It’s not going to win any design awards, but we like to think a simple example makes it easier to see what's going on.

Materials needed:

* Neodymium magnets x 2
* Rotor (we use a 608ZZ bearing)
* Magnet wire
* MS bolt (M8 x 25mm) x 4
* Breadboard
* Electronics - 
  * pushbutton x 3
  * LED
  * 12 volt power supply
  * Jumper wires
  * DC power Jack

The spinning part of an electric motor is called the rotor. Most brushless motors have permanent magnets on the rotor.

Our rotor spins thanks to a 608ZZ bearing stuck on an 8mm bolt. This bearing is commonly used in things like fidget spinners.

>This is different from most BLDC motors which have alternating poles facing out. This simplification will make our electronic circuitry a bit easier to understand.

### Step 2: Get Moving!
How do we get this thing spinning? We could just move it with our finger, but we're looking for a magnetic push. Bring another magnet near one of the rotor magnets, with its north pole facing the north pole of the rotor magnet. This will cause the magnets to repel, or push, setting the rotor spinning.

https://do7js0tdxrds1.cloudfront.net/k4gnf040v0ffxitf1m6i5dp2ufxm?response-content-disposition=inline%3B+filename%3D%22ezgif-6-6c89103f3574.gif%22%3B&response-content-type=image%2Fgif&Expires=1701080071&Signature=Zy2ojS1-6XPzccTBTe2ffgpYCQiyLv6MboDBOzkSnz3IzNU2Og0LU1mf8PI200t8MMUaFwcOXgf~opeFE5IkT1ZoIicLFjTTspplbwAm28LCfNjW0B4ut1zrQCXV5aFM9srUt4Xz0QqzQzW9krInPPBINJHg4nQp52VHHBCdRwFBZ9EhRZ5-DCwWUeuJBt9wyOKpWvxFFcnz4y-lHIFfCJgeBqlrPvZIYRIBZ5eRrIWyLxGaicxegt4J6vfhKgs4P4UzZijQNZy364iO2lZjB1CVg550~CK2cRXxWAWyEQ0RO~LwvXWXJNsCyPdqtPiGD8ffzQmhLNjAb~r1~5mXgw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

If we push on the magnet hard enough to spin the rotor halfway around, we can do it again to the next magnet. If we were fast enough, we could keep putting the magnet close and taking it away, spinning the rotor continuously.

This is where the electronics come in. We need to create an electromagnet that turns off and on, pushing the rotor magnets.

https://do7js0tdxrds1.cloudfront.net/xc81glj2h42clf03dwxyvu7ghwil?response-content-disposition=inline%3B+filename%3D%22N.png%22%3B&response-content-type=image%2Fpng&Expires=1701080071&Signature=d6phDSHLtc-rISi7722mQbBzfhHzp-otfXmRaqAVdI3FPdDwUaZOoJ48KRpV22PxTRenqgCAQj3EjetIKl0nKUw6ehH~0DlkEIomTopAvngKYqYiMCaNKTspMnqBeKeHm2VcSv6uMCO7bjuwfNoQw3MQAIfOaYFQ9SI7HPHU3nMSA3cKBlkS45LazrNHgHrPPwV4vtsos4FTInaapU7wSXBllyKq06qS2Y4oXM9SA2sPZS4f7QplGYLq6CrPry5-OlADuR1zdIbonoTJHBjy~DF~w8LAjJv2B5Ccxe3-FT1CZtmhfdP5idUHZQetawRqQPS1pENYjdQjPKNZg7t7Zg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

We have fixed two 10 x 10 x 2.5 mm B442 neodymium magnets on the outer edge of the bearing, 180 degrees apart from one another. Both are oriented with their north poles facing out. 

A simple electromagnet beside it consists of a coil of magnet wire wrapped around a steel core. We used 25 gauge, single-strand copper magnet wire with a thin, enamel insulation. An MS bolt becomes the steel core.

When we apply a voltage to it, it becomes a magnet. With the electromagnet positioned just right, it should pull the rotor's magnet towards it. Now, all we have to do is turn it on and off at just the right moment.

https://do7js0tdxrds1.cloudfront.net/sd3l1z41v1cdt0iu2lsh4dosy4pb?response-content-disposition=inline%3B+filename%3D%223+pole+gif.gif%22%3B&response-content-type=image%2Fgif&Expires=1701080071&Signature=k4JavIJsPWqCmweKwRi5jgLARL9zZhIP4E16MhMGAJlwAFD97FUaQdZcOI2C3037pbk0zRHCibVmW74iLpuCVyysWTgh9915lUqIlx51uE~LT6lGS4uOToZFc0z3jAb440EbHnw32LhYOjNTU5MYaUxfm-0apfDk~EFJ3GXqtKEKvIpKHSp3qQnyUlnImQ9r-D6seSUaEhFauvK00VFbqC5Wxbd~xki2wZRuoZ7-2JsA-pTKKWvihAFXRhJMd431wnO7m9RLnsnV51U4LLP3rJ7OT2QPCSKgVd9c6jqsX~k17wzE5BdLICeCmngecU3LEBTBMDuPTzEL7G~16BHsww__&Key-Pair-Id=K2Q3HDJ6ZAQGFF


We want to turn the electromagnet on when it completes travel of around 120 degrees and this can be done electronically. 

But for now, let's do it manually to understand the basic concept of a BLDC motor.

## Steps to build your Motor. 

>Make sure the Base you choose to build the motor is movable and is not fixed to one place, as it will be easier to use and transport. Don't fix the motor on a table. 

#### Step 1: Get all the required materials as stated in the list above.

### Before starting, here are the Do's and Don'ts

**Do’s:**

1. while placing the coils, connect a battery it to the terminals of each coil to fix the positions of the coils from the rotor, this will help you in the coming Levels.
2. While winding the coil, make sure to distribute the wire evenly, it will help in proper working of the motor.
3. Handle magnets with care as they are powerful, letting them strike for multiple time will lead to breaking/cracking of magnets.


**Don’ts:**


1. While winding the copper wire/coil to the bolt, make sure you do not apply excess pressure/rub the coil. Else the insulation layer will wear off , and it will cause short circuit issues.
2. While fixing the coils in place using an external fixture, e.g.pipe clamp, make sure to not apply excess pressure while fixing or else it will cause a short circuit issue in the coil.

https://vimeo.com/622817168

#### Step 2:  Drill an 8 MM hole in the piece of scrap wood or a piece of plastic to fix the Bolt.

https://do7js0tdxrds1.cloudfront.net/7vpammegns210g9tlvt9ym5mwfhb?response-content-disposition=inline%3B+filename%3D%222.5+Drill+a+8+MM+hole.png%22%3B&response-content-type=image%2Fpng&Expires=1701080071&Signature=ZYmV5diD4gs8A7t600FC5dQ7bCYu8WDHM5C3V1U5PcNXTBqBXHaZnH9CDBRDMGDOIYAxDHy1VCwGeq0OBUdcg2ZasMZaOdTcxvbHlFEcgD6Xf8a4DtQSzeaygs1Tu24aj5lD2J~-YAiuD6oQ-VJvVe1wwhDMXOTwnjKA3SEVgE2fjmzBOdDhcFW1owxVHlDyPxYKmeVYF2ws2tmJQ5E-kWxa099UKUCshiajgZxHiL4r8hmvq6Wtez~Hbisei~NfimSuc2k9f308eNrDEda048D2~PZNf~JRf2IVNuwa-932dJXa1195GzsghI2YHNlCeqsHP3Ud8Y4OvKjYmasHhw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

#### Step 3: Attach Rotor

Pour Wood Glue (Fevicol, Fevibond, Araldite) into the hole and place the rotor assembly (MS bolt + bearing + nut) into the hole, and wait till the glue cures.

https://do7js0tdxrds1.cloudfront.net/kf0j75qwf7mb5lkhqucex0605jhp?response-content-disposition=inline%3B+filename%3D%223-resized.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701080071&Signature=h-7F~jz~JyMdPeUbMZ8WB8FclK5eKwZF8zTEgz7YFLSvz8464RH7oxZuCBqg8Hv90lf9Zn8hAbWR92FMC4xUHylXBqdZX3L15iaFx7jysbuBlf-xTzNUUrxJg4DIIPia0lXuC9AxKa~BDco3JYHXWUGHZk9Sc6GsNXymCISUKIzXX~B3tf-aPcNUl81kD5WcpIDw-9ta2T2mdQAIRL-vS03x5MGNBkijQY-qMFC4tOMkOhest4BiPw-SKaO1A8OMACJb4GuyOVN2HIIt3Z75G0R24hnRumNekhZ91UNyFe0Z1E18vLPNyo5R1HkbrHADjKjHamUa5RKpqRADkGpQfA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

### If you do not have access to a drilling machine or a piece of thick wood, follow the steps below. 

Instead of drilling a hole into the wood to place and fix your bolt (rotor), what you can do is, find a flat surface like a piece of hard cardboard, rigid plastic plate or a piece of hard foam and just rotate the bolt upside down as shown in the image below and add wood glue to it for it to stick and stick it to the surface. Some examples of glue are (Fevicol, Fevibond, Araldite, etc). Do not use fevikwik or cyanoacrylate as they do not stick to metals like steel bolts.

https://do7js0tdxrds1.cloudfront.net/mscuhlrqbky95kaxaxq0hpk37b9e?response-content-disposition=inline%3B+filename%3D%223++pole+motor.81.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701080071&Signature=dyFpJ5LJ-n0XX6bz6NHonqnyo2xgidGj1gp35l5kx4-AcOWtVsIxe1ZYEGWI2NinCGzHPt3Hp867jvoWcLglykIOFfsJdCauhWIXDUcgpCFgBY5i8o3FBbLDRi4DvyumQTLwAdjJfPLce~fdbiNM9bn2~bSS0TpS-Zf-NBEu1zbALvwia0kFxejWQcNo9NzeUVKDqLU0z7m7ZvcMsIlumWgIz~gxbQexQiY~uNvYwH~-IC~zb51ON4RXTCj-pBE0S-Fd0HulQ7SacwADqfHcviaX-JJaF2KHErdMqWwfZC5WKv167wyUW29j4f5v-1MYIPf4~teeo~AHj1VwWyrSww__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

#### Step 4: Winding the poles

Get the enameled copper wire and wrap it around the ms bolt such that 2 long ends of the wire stay out.

``` 
Make sure you count the number of turns on each bolt. 
The number of turns needs to be 200 turns on each bolt. 
We need 3 such bolts to be placed at 120 degrees each.
```

https://vimeo.com/643678159

#### Step 5: Burning/etching the winding tips

After you are done winding the copper wires around the bolts, next what you want to do is, get a lighter or a matchbox and burn the ends of those copper wires to get the enamel coating to come off.

Once you are done burning, just use a simple blade and scrape the remaining insulation off the ends.

https://do7js0tdxrds1.cloudfront.net/ccg5esn3iwsq35hk8io88fqogp4n?response-content-disposition=inline%3B+filename%3D%224.png%22%3B&response-content-type=image%2Fpng&Expires=1701080071&Signature=goaEvJ6QSIiZEeqGhHCfk-K84clV4R2yzJfz4NBfvdGffWs0Sh82nCNsV9zdofOut3X6smKmkVXqyCxmXQzmDvutSZ11P~2-Jh7nQLuLk0BxPo309~5DmuLSssreRRILyHQWYCWJuchvvtt2T09RGJdla4gEl094PMn5ha5jurBAp~pSdyU4X5saO7~D03-IOjyI4bfyXci2YcI1Eguft2i45mRKGep-oCeWG2IZ5w-hAU4WpZg7jJtDKzP~2sKPfDOotEM~8sGEkDnop9Baj7p6IBy5hUCkODxbri97a6JSmtgXB5m2-xN1LyBYgSeF5WaShYtdWBJXhn6aZDGV5w__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption: Burn and scrape the tips of the copper wires

https://do7js0tdxrds1.cloudfront.net/4itx3fedyits8tq2c7wl7mo8rhw6?response-content-disposition=inline%3B+filename%3D%22soldering2.gif%22%3B&response-content-type=image%2Fgif&Expires=1701080071&Signature=LI0AdrhZ4uzOZWsv35uJtWzJBjJYArRUdPdOnNwKiUZex3sCec0gogdUwra48iN1PKre-wlycmvbTKkjksowkdlKrKILncEiCUgVE3qxQDPBoqwCF49tNhgIuYdRPwH-UDF9uo0cr9SdVVGMN5-5lHZ-ym33C3X-TrpnqL~eK~JiNNfr0LtSWgzM~igY9le56hJ39-WVxgAeYeeu6dIlkGzDHIazkV2IPo9nmNKPDThtKHWuZTosZgOl0x5Q6ofbgjOMJmL0dhVomJ3NcPRov1iUEgZZt~a6EYmGPNgYBbR19MQwdI5Le8PfqxynILCvzGDFgGd-dBCD~2dnj6cOwQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

#### Step 6: Placing the poles

Place the windings on the board **120 degrees** apart from each other, but before you do that, energize your coil and check at what distance and angle the magnets from the rotors get activated (rotate) as shown in the video.

https://vimeo.com/629184717

After you do that, note down the distance between the pole and magnet, This will be the distance between the coil and the rotor. 

Once you do that, place all the 3 poles at 120 degrees to each other and fix them in place with tape as shown below.

> Tip: You can try to draw 3 lines each at 120 degrees from the rotor pointing outwards and then place the coils along the lines to achieve symmetry.

https://do7js0tdxrds1.cloudfront.net/r4fdm4nxson3acnaa8j8pjpms4oz?response-content-disposition=inline%3B+filename%3D%22IMG_20211011_201843.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701080071&Signature=PA4OL4pya56cnXdB1dZ~tyNVq8me3MAQVwUJUyLPx97udW96iwWv-JEDnX3KwkBIjHe98uB4PGsWH1kxMxnsp-sKOwI~mF196Ro86LAYGPMA7vHHFvNF60V63OYvt30QfLkZgSNhn1bu4QPKdoTm7TmielmMKClRCeW8QElAVzBZpcABcbcux9bNLIO-Wp8eSwIl09EE14UVrF70EfGSfc4fIKqBlQAEjm6jmbuSHXRZC5Dn1z7FGQBqRqy7lnPCswPOMd67ToKtKtksjEx9LwU~r78sAXgE5f~8HZstocd1mjT4Qw4witIapHcQM1QDFzprL9Px1h0XOHT2MeGrsA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Once you've placed the poles with tape, energize the individual coils as shown in the image below to check if they can make the rotor rotate a complete 360.

https://do7js0tdxrds1.cloudfront.net/jcppao11ytp7fwnxb9lparsrmx77?response-content-disposition=inline%3B+filename%3D%223+pole+gif.gif%22%3B&response-content-type=image%2Fgif&Expires=1701080071&Signature=Uw117xKzYOd9G4IpE0lDvrlYRGa-a-XXwMllKQs6zLOmaVY44PF1vMk1qo~BLV6LN-Bb-Vrqqn~lcIPvodJ3hnZ1-ESa2Tx5QRxXOMCg2scWfvm5LniW3fZKUDYUUfBM5FKwqHGX8TRIKaYIz9jSoBgSWvakbF0jBtxh~1yTSWdf6urvJmDmVkSFlLao85cgxB433k~lCvPpBElfRkLiB6OnVGFQMwWlIcZo5J4AwrcN2AMA8BgqadfVGWCV4EfdFQEMk2N62xH4Cl4XDWajlTgpTXbKI0oh4~Qo60dbToYJ-BP64EQ0WEA83aYINH6o16VYcxqnJR-Xpa32t9PcCg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Caption: Connect the battery terminals or the power supply adapter to individual coils  to make the motor rotate


After you have made sure all the poles are in the proper place, mark it and see if you can permanently fix them in place with Araldite or any strong glue.

https://do7js0tdxrds1.cloudfront.net/e5kidepl1gxhl7yqcipzndemldd2?response-content-disposition=inline%3B+filename%3D%22IMG_20211004_213026-resized.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701080071&Signature=Hffs~vR1mkkRaAJkXc92TkDV30mcrFnu0jDaMUivWO303IkU1ap7UDJ8XXf9PPCwoD0Q7aae1pjNOaUgcu3JwKaMPp7h-oPAFUe66~bEYXU8VDnJRPi24wdPxnCpaz6oVN9HTxkC48TNap~mhSn1RZPZFzcVB0FE~-Qvq7QpW0hIpKUkndqYz5uUHUrJrTs3j9TyFScBJGNppnkHllbf5~fK1~ERMdiQGXlXeivf5~DGOHhfs-W5hYkh3TL7cEOYzm6IQiW-su5OKb1AiWYkWsurrvz1ygdj-V8UymXyq8kLkA7PKyvYvCY2zc8Kl0-~4rhlTsy9HI3eBfp00rD5Gg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

![7.jpg](https://www.pupilfirst.school/markdown_attachments/4278/un3m-JGSkBdFfVpW9W9W9A)

#### Step 7: Wiring

In order for the motor to work, you need to energize the individual poles when a magnet is near it.

We do this by,
1. Soldering all the ends of the copper wires for better connectivity.

2.  Locating all the negative terminals of the windings. Our end goal is to attract the magnet towards the coil as shown in the video below.

3. Once located, mark all the terminals as shown in the video.

### Soldering the copper windings for better connectivity

https://vimeo.com/629103047

https://do7js0tdxrds1.cloudfront.net/zolvty8yozr9lvogcngzg8c13msc?response-content-disposition=inline%3B+filename%3D%22WhatsApp+Image+2021-10-11+at+5.30.45+PM.jpeg%22%3B&response-content-type=image%2Fjpeg&Expires=1701080071&Signature=oVkF2Clh74uU797zCQufviwFv1nRKBDFnBDHiYHtry9x9DeCEfuYWftCBnvmYSdxOpTQWBDoRKfbozFjMU1wGnW0ngSl2p1yIUMOmImo8P~jEh--Qw0Xa-3SZqL4-JW0FHtDl9hdzuwg6QB6AsmBb7456IHimRUJHR8VD0VxIYD3U9rBgAX8QhrvMTQJG7sEcpqOuna-OfDKi9pD3aZh4SYd7gNCbOFISUhU7adsKczXNI6A7YpxeLIFkXXcn90CquBglZ62sKsNwuXuKdSoGdXb-jA~GSILmZJBVQtDKJnF-9ruJUFcATLKV-Y8C0FP0lhTs3NnVybHA2dec395Wg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

https://vimeo.com/622876745

#### Step 8: Running the motor.

Our main goal here is to individually energize the poles whenever the magnet is near it to attract the magnet towards it and make it rotate.

This is the simplest configuration of a motor and is very easy to understand as well. 

Let's move forward to manually running the motor by individually switching on the poles in this chapter to keep things simple.

> We will be building a motor controller that automatically increases or decreases the speed of the motor in the next level.

https://vimeo.com/643675443

>If you have access to a 12 volt power supply, connect the power supply

https://do7js0tdxrds1.cloudfront.net/7vshjtwdyeuh8ds2fh2z0xez6yga?response-content-disposition=inline%3B+filename%3D%223+pole+breadboard_bb+new.png%22%3B&response-content-type=image%2Fpng&Expires=1701080071&Signature=OzZbuWmK6eb3nX54Crq0I0uT3brTGeo8wz21DYIupufQk7ieDi7Sas6~Zm~S3uqFsFPegl1C9nan2zb24MDAbU~S3McwoAF5SxlBQtN-zFOIKo5rr6uPMIcuV1CvIQLKGQs7b8CHQ1~ePPs~pyFIYzevDZDVgRrubLoOXn5bsByKKY~NnpzYgP6BgJBmox5xEIRhhV1cNLMOLmXaQh7g-xC7hljwy~odJY4sZTWUy92XpeeVzHo40cge~5nBTSfo6rfcQwicgwu57OysNBkbv2X5PD84HFDGI0JRCRlQPrmulPu2OF6bsnMpYa981sqxa7n2JwgBINlXlkw-Rn-6jw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

https://vimeo.com/625382866

> Submission: Upload a video of you running the 3 pole motor by activating each pole.

#### Example video submission by Nandhu Suresh (Teaching assistant),

https://vimeo.com/639656819