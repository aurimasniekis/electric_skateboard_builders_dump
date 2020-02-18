# New Vedder anti spark switch 1.3 FOR SALE 4pcs now WITH CONNECTORS of your choice!

### Replies: 19 Views: 1826

## \#1 Posted by: Martinsp Posted at: 2017-01-30T17:13:05.880Z Reads: 309

```
Hey guys! 
I have 9pcs of Vedders anti spark switch version 1.3 that i want to sell. I ordered 10 sets of parts and built them all. I am going to istall one of them on my board. I do this because I am pretty sure that there are a lot of people that dont have enough soldering skills (just like me a couple years ago) and still want to experience the joy of building your own custom E-board, bike etc. Buying one of these can cost you as much as 60usd plus shipping when buying from onlineshops.

I sell mine for **40€** plus shipping and **connectors of your choice! :)** **worldwide** :) With the actual mosfet switch circuit **you get the rocker switch (soldered on 10cm of cable) and silicon high strand count copper cables ready to solder connectors of your choice (5cm on either side)**. You can of course choose the way I ship it to you (last week I sent a package to china for 7€ including ensurance). I am from central europe which means that it is very unlikely that the shipping will be more than 7€. :) payments are accepted via **paypal**.

If you want more info just ask down below or PM me.

Here is a video of me testing all of them (just to ensure you that they work 100% :) )
https://youtu.be/jVjqx66iWJo
Greetings from Slovakia, ride safe :)
```

---
## \#2 Posted by: caustin Posted at: 2017-02-01T22:55:52.401Z Reads: 256

```
Can you send with xt60 connectors installed on ends (male to battery, female to esc)?
```

---
## \#3 Posted by: Martinsp Posted at: 2017-02-01T23:23:52.917Z Reads: 243

```
Hi sure i can, pm me where you are from and i will be able to tell you what the shipping cost will be :)
```

---
## \#4 Posted by: caustin Posted at: 2017-02-02T04:20:19.938Z Reads: 232

```
Great, will be to NYC. USA zip code 10012
```

---
## \#5 Posted by: Martinsp Posted at: 2017-02-06T08:46:10.982Z Reads: 214

```
Already sent :) hopefully you will receive it soon.
```

---
## \#6 Posted by: Martinsp Posted at: 2017-02-10T13:38:42.437Z Reads: 193

```
Now with connectors of your choice already soldered! :)
```

---
## \#7 Posted by: caustin Posted at: 2017-02-10T22:09:35.546Z Reads: 188

```
great,  thanks.  Will report back when they arrive!
```

---
## \#8 Posted by: Martinsp Posted at: 2017-02-15T13:42:29.914Z Reads: 186

```
Bump :D 
10 char
```

---
## \#9 Posted by: caustin Posted at: 2017-02-16T04:47:21.155Z Reads: 171

```
Haha, arrived thanks and look great. Will be gone for 2 weeks and then get a chance to try out!
```

---
## \#10 Posted by: Martinsp Posted at: 2017-02-16T18:58:29.664Z Reads: 158

```
That is awesome! Hope to hear more from you if you have any problems or suggestions! :)
```

---
## \#11 Posted by: Martinsp Posted at: 2017-02-20T11:10:23.142Z Reads: 144

```
There still is a couple more left :)
```

---
## \#12 Posted by: jonesstore Posted at: 2017-02-20T12:53:28.245Z Reads: 143

```
when i do have a good VESC, do i still need an asp? :)
```

---
## \#13 Posted by: Martinsp Posted at: 2017-02-20T13:09:51.592Z Reads: 141

```
The switch is for turning your board off and it prevnts the VESC from getting damaged due to the in rush current. Also the spark does damage your connectors slowly. And the 3rd thing is that there is not a switch or solid state relay that size that can handle the high current you need to get from the batteries.
```

---
## \#14 Posted by: halifax21 Posted at: 2017-03-05T03:43:08.974Z Reads: 132

```
Any more anti spark switch available
```

---
## \#15 Posted by: Martinsp Posted at: 2017-03-05T09:51:49.450Z Reads: 131

```
Hello, yes I have 6 available ready to be shipped tomorrow. :)
```

---
## \#16 Posted by: Martinsp Posted at: 2017-03-26T13:41:54.939Z Reads: 115

```
Hey, only 4 left guys. If you are interested just PM me :slight_smile:
```

---
## \#17 Posted by: Martinsp Posted at: 2017-06-27T14:22:15.107Z Reads: 86

```
I got time now so if anyone is interested i have like 2 left :)
```

---
## \#18 Posted by: Mike_Lemon Posted at: 2017-06-27T22:34:36.863Z Reads: 80

```
May you release the electrical schematic of that board? can it be turned on with a little 3.3v signal?
```

---
## \#19 Posted by: Martinsp Posted at: 2017-06-28T07:08:42.872Z Reads: 63

```
It is not my project. It is Benjamin Vedders open source project. 
The schematic can be found along with all of the other files here on github: https://github.com/vedderb/SparkSwitch/blob/master/Plot/Schematic.png

I doubt that it could be turned on with a voltage signal because the switch engages in both open and closed positions. But maybe you would be able to make it work but I cant really think of a solution for you. Maybe with two mosfets which would be controlled with the 3.3V signal and one of them would be open (conducting) whenever the other one would not. Like a flip flop switch with mosfets. Or simply relay that would be able to operate with 3.3V on the coil and would be normaly closed (connected P7 to P8) in the off position and when the coil would be energised the relay would connect P7 to P3 which would be on....
I honestly think that the relay version is better because it is simple and bulletproof :D
```

---
