# First build / single sk3 6374 kv192/ 2 x 5s1p 20c/ maytech vesc

### Replies: 28 Views: 1188

## \#1 Posted by: Starymis Posted at: 2018-03-13T22:35:41.931Z Reads: 171

```
Hi everybody, 

I diced to build a eskate with motor sk3 6374 192kv, 2 batteries 5s1p 20c and maytech vesc (i have it). 16/48t, 83mm wheels
What do you think? 
I see that the batteries have bullet connectors, motor too, the vesc hasn't any conexións( it's possible?).  Can you  recommend me which typ of conexions will be ok (keep the bullets and put to vesc too of change everything for xt60 /90)?

Thanks for your help
```

---
## \#2 Posted by: RedEagle Posted at: 2018-03-13T22:38:32.390Z Reads: 170

```
Both xt60 and xt90 are okay. I would go for the xt90's just in case. Bullet connectors are also an option.
```

---
## \#3 Posted by: dg798 Posted at: 2018-03-14T13:09:04.031Z Reads: 142

```
I’d go with 90mm wheels at least as they give u some more ground clearance as well as higher top speed and more smooth over bumps
```

---
## \#4 Posted by: dg798 Posted at: 2018-03-14T13:09:46.731Z Reads: 139

```
I would then use a 36/16 pulleys if u are going with 90mm
```

---
## \#5 Posted by: Jammeslu Posted at: 2018-03-14T21:36:54.050Z Reads: 119

```
Use whatever connectors you want, just insulate then properly
```

---
## \#6 Posted by: Starymis Posted at: 2018-03-15T04:30:24.969Z Reads: 110

```
Thanks a lot for answers!
I would like to use some anti spark conexións.  How many i'll need?  Only one,  between battery and vesc?  Or all battery's outputs?
```

---
## \#7 Posted by: Starymis Posted at: 2018-03-15T06:22:54.424Z Reads: 103

```
![bf28d9944b2db1183fe647244eaf|500x500](upload://Abs9X2RULPAitopVGUEFHlcEUpN.jpeg)

This will be enough to connect 2 batteries?
```

---
## \#8 Posted by: dg798 Posted at: 2018-03-15T13:01:45.247Z Reads: 87

```
As long as ur 2 batteries both have xt90 female output connectors and the vesc has an xt90 male output then yeah
```

---
## \#9 Posted by: Starymis Posted at: 2018-03-15T14:25:52.946Z Reads: 82

```
The batteries have bullet 4mm and the vesc any connection. I know that i will have to solder. 
I like to change baterries conexion for xt90 but i dont know,  buy only one anti spark and put it before vesc or 3 (2 for batteries and one for vesc)?
```

---
## \#10 Posted by: Sebike Posted at: 2018-03-15T14:37:10.744Z Reads: 80

```
48t sounds big for 83 mm wheels. Gives you 3,5mm clearance without belt.
```

---
## \#11 Posted by: RedEagle Posted at: 2018-03-15T14:47:01.852Z Reads: 77

```
You have to put the antispark between the battery and the vesc on the positive side(red wire). You only need one antispark per board.
```

---
## \#12 Posted by: Starymis Posted at: 2018-03-15T15:19:00.251Z Reads: 70

```
48t has 59mm (I hope. It's written on the seller's page) . So give me 12mm clearance
```

---
## \#13 Posted by: Starymis Posted at: 2018-03-15T15:20:04.770Z Reads: 71

```
Big thanks! 

And also other big thanks for everybody!
```

---
## \#14 Posted by: Sebike Posted at: 2018-03-15T16:49:31.811Z Reads: 70

```
Sounds weird. Do you have a link? Must be some weird pitch and certainly not 5mm or stated diameter is wrong.
```

---
## \#15 Posted by: dg798 Posted at: 2018-03-15T17:18:56.235Z Reads: 67

```
If all they are 4mm bullets buy this:
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F390416857132

Then buy this xt90 anti spark:
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F231516850545.

Then you need to buy either a pair of hxt bullet connectors to solder to ur vesc so u can connect the series connector to the vesc or buy this hxt to xt90 adapter:
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F332552024879.

This is how u would wire everything up with antispark:
![image|608x500](upload://r3YdL6SNlErLpv8c1TFE2vsyZJZ.jpeg)
```

---
## \#16 Posted by: dg798 Posted at: 2018-03-15T17:22:01.318Z Reads: 64

```
Just remember, use the male part of the xt90 anti spark on the wire and then the female acts as a key to close the circuit and gouge power. The female key needs to be bridged with wire like this:
![image|592x500](upload://7G8c23lTDxX2q8lqnFWPfTI8E2G.jpeg)
```

---
## \#17 Posted by: Starymis Posted at: 2018-03-15T18:29:38.676Z Reads: 59

```
Thank you! 

So in the "+" i can solder directly male xt90 for sparks?
```

---
## \#18 Posted by: RedEagle Posted at: 2018-03-15T18:32:10.623Z Reads: 59

```
Yep. 10char
```

---
## \#19 Posted by: dg798 Posted at: 2018-03-15T19:16:11.118Z Reads: 57

```
But remember that the mere are 2 batteries so the positive and negative of each are going to be connected to make the series connection and then the positive from one battery and negative from other battery is going to go to the vesc and u have to make sure to solder the xt90 antispark to the wire coming from the battery that has the + wire.
```

---
## \#20 Posted by: dg798 Posted at: 2018-03-15T19:17:12.419Z Reads: 55

```
Also if I were u go with 90mm flywheel ones and use a 36t wheel pulley and 16t drivetrain
```

---
## \#21 Posted by: Starymis Posted at: 2018-03-15T19:26:39.412Z Reads: 51

```
And about charching? Imax b6 mini will be enoguht?  It's possible to charge two batteries in serie on the same time?
```

---
## \#22 Posted by: dg798 Posted at: 2018-03-15T19:27:45.835Z Reads: 48

```
I wouldn’t do that if I were u as there can be many complications and can ruin ur batteries. I would either use 2 imax and charge each one separately or look into getting a charge only BmS.
```

---
## \#23 Posted by: Starymis Posted at: 2018-03-15T19:34:45.982Z Reads: 49

```
But to charge battery by battery imax will be ok?
```

---
## \#24 Posted by: dg798 Posted at: 2018-03-15T19:36:07.743Z Reads: 47

```
It should be. Just make sure that you have the proper connectors and power supply for it.
```

---
## \#25 Posted by: dg798 Posted at: 2018-03-15T19:37:59.503Z Reads: 52

```
It would just be cleaner and easier to do a BMS but good old fashion imax will do the trick. And remember never use a higher current while charging then 1c of ur batteries unless u want to decrease the life of ur batteries. Basically if let’s say ur batteries are 5000 mah, don’t charge more then 5 amps but stay within the 2-4 amp range
```

---
## \#26 Posted by: Starymis Posted at: 2018-04-20T22:59:46.752Z Reads: 43

```
Hi everybody, 

I still waiting for few things to finish my board. 
I have few questions:
This indicator will be ok for lipos? 
https://m.banggood.com/es/12V24V36V48V-8-70V-LCD-Acid-Lead-Lithium-Battery-Capacity-Indicator-Digital-Voltmeter-p-1209820.html

And also can i change vesc's connecion with the motor?  Are 5,5mm bullets and motor had 4mm bullets. 

Thanks for your help!
```

---
## \#27 Posted by: Starymis Posted at: 2018-06-13T01:50:02.940Z Reads: 30

```
<a href="https://www.fotosik.pl/zdjecie/e00312369ba57b53" target="_blank"><img src="https://images83.fotosik.pl/1092/e00312369ba57b53.jpg" border="0" alt="" /></a> 

Can you confirm that is all right?
```

---
## \#28 Posted by: dg798 Posted at: 2018-06-13T02:11:44.924Z Reads: 30

```
you dont need the middle connector. it just adds resistance.
you want all the wires as short as possible with the least connections possible.
i can draw you up a diagram tommorrow if u want
```

---
