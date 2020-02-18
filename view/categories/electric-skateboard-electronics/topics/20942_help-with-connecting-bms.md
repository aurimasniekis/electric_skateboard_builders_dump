# Help with connecting BMS

### Replies: 18 Views: 1027

## \#1 Posted by: drnkamil Posted at: 2017-04-13T16:57:38.333Z Reads: 110

```
Hello.
Can someone help me to connect everything that is on the photo? I'm a little overwhelmed, I must admit. I would be grateful to have me show you all the schematics on what exactly to combine.
Thank you very much.<img src="/uploads/db1493/original/3X/f/2/f2d95cdcc0c66e68eae4bb8bbb78ca84259778ec.jpg" width="690" height="388">
```

---
## \#2 Posted by: pcapelo Posted at: 2017-04-13T19:03:42.503Z Reads: 98

```
Could you list everything you have in your picture?
```

---
## \#3 Posted by: drnkamil Posted at: 2017-04-13T19:11:47.565Z Reads: 94

```
From left:
LiPo 10S
BMS 10S
Antispark Switch
Charging connector
120amp esc
170KV motor
```

---
## \#4 Posted by: pcapelo Posted at: 2017-04-13T19:43:05.834Z Reads: 93

```
Ok, another question: 

Does your BMS have different points to connect charging and discharging wires?
```

---
## \#5 Posted by: drnkamil Posted at: 2017-04-13T19:51:53.134Z Reads: 90

```
http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html
```

---
## \#6 Posted by: pcapelo Posted at: 2017-04-13T20:20:03.172Z Reads: 92

```
let's start with the BMS itself:
<img src="/uploads/db1493/original/3X/8/d/8d9453a4ddb36e629ae437446439b2c45f72c5bc.jpg" width="690" height="363">

You can see how to connect the battery, the external power and the rest of your setup. based on the BMS information, this is how I see everything connected, looks funky because you have to connect the positive of the battery on the little wire on the balancing. About the balancing, I would suggest you find a Y cable to make two 5S connectors into one 10S, it would be easier to connect everything.

You should ask for aditional opinions, but thats how I see this connected:
<img src="/uploads/db1493/original/3X/0/b/0bd37c658c99959182e8be8a9287d4317bd6eb5d.PNG" width="690" height="393">


cheers
PC
```

---
## \#7 Posted by: drnkamil Posted at: 2017-04-13T20:44:27.321Z Reads: 79

```
Mostly I'm about how to connect the balancer connector to make things wrong, which balancer is to be the first, I just do not understand. I know that 1 - 3,7. 2-7.6 .... but the balancers are two, I do not know where to put the. Measure V starting with the red cable in the balancer or the other side? Sorry for haotic writing, I'm trying to explain everything thoroughly.
```

---
## \#8 Posted by: pcapelo Posted at: 2017-04-14T01:43:54.831Z Reads: 74

```
you might need something like this: https://www.amainhobbies.com/junsi-multiadapter-balance-board-2s10s-thunder-power-flight-power-losi-jun-bal-tp/p195156?gclid=Cj0KEQjww7zHBRCToPSj_c_WjZIBEiQAj8il5FPwG_XlWPXok7bxsYcIIqGmFnLl5EPRQ7bfXLMQOToaAgTH8P8HAQ

so you can connect both 5S connectors and get one 10S to the BMS
```

---
## \#9 Posted by: Namasaki Posted at: 2017-04-14T06:21:55.986Z Reads: 70

```
Where do you live, maybe someone in your area could drop by and help you.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-04-14T06:34:41.660Z Reads: 68

```
Your battery is basically  two 5s Lipos connected in series and shrink wrapped together.
You will have to find out which balance harness goes to battery 1 and which goes to battery 2
Battery 1 supplies the Negative main wire
Battery 2 supplies the Positive main wire
If the balance connectors are not marked, you will need a multimeter to find out and number the balance wires coming out of the battery.
It is critical that you get the balance wires connected correctly before connecting the main wires to the B- and P- on the bms.
```

---
## \#11 Posted by: drnkamil Posted at: 2017-04-14T07:50:15.307Z Reads: 68

```
I have a multimeter.
How and from which side to start measuring?<img src="/uploads/db1493/original/3X/7/c/7c07b8d4b15fd01550963fac42cc72bc356e48d7.jpg" width="690" height="388">
```

---
## \#12 Posted by: Namasaki Posted at: 2017-04-14T18:13:45.630Z Reads: 61

```
Ok, this is really pretty simple.
connect your negative test lead to the main negative battery wire and the positive test lead to the main positive wire to check the total pack voltage. It should be around 36v to 38v This is what voltage batteries are shipped at.
Then remove the positive lead from the main wire.
Note: The red balance wire is always the last cell in its pack. The black wire opposite the red wire, that is on the other end of the connector is a ground wire. That's why a 5s Lipo pack has 6 balance wires.
So on the 2nd wire from the end opposite the red wire check the voltage. do this on both connectors.
The one with the lowest voltage which will be 1/10 of the total voltage will be cell one of pack one.
I will add a diagram shortly.
```

---
## \#13 Posted by: drnkamil Posted at: 2017-04-14T18:38:47.848Z Reads: 56

```
<img src="/uploads/db1493/original/3X/a/3/a3687a8b653177cac7d5060f841758c23802db22.jpg" width="690" height="388">
```

---
## \#14 Posted by: Namasaki Posted at: 2017-04-14T18:59:36.335Z Reads: 56

```
<img src="/uploads/db1493/original/3X/c/9/c9d086b614ff47bb9a78b35a07b66d223bbdb331.png" width="663" height="500">
```

---
## \#15 Posted by: Namasaki Posted at: 2017-04-14T19:04:26.234Z Reads: 56

```
Looks like you got it figured out except you don't use the first black wire on each connector.
It is a ground wire for it's pack.
```

---
## \#16 Posted by: drnkamil Posted at: 2017-04-14T19:06:48.643Z Reads: 56

```
Thank you very much for picturing this connection.
Can you picture all the rest of the cables? Because I have the impression that what my colleague pcapelo presented in the photo is wrong.
I would be very grateful for your help.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-04-14T19:22:01.849Z Reads: 57

```
The illustrations that pcapelo posted look correct.
The only thing you have to check is the charge port connections.
You will need to check the output of your charger and insure the you match it's polarity with the polarity of your charge port wiring.
```

---
## \#18 Posted by: drnkamil Posted at: 2017-04-14T19:29:41.659Z Reads: 55

```
thanks guys. I greatly appreciate your help.
Regards.
```

---
