# ESC capable of super high erpm? 80-100k?

### Replies: 15 Views: 1054

## \#1 Posted by: Deckoz Posted at: 2017-08-26T14:34:22.840Z Reads: 145

```
So, I've blown another VESC - this time my master. I believe the culprit is erpm.

39mph freewheeling downhill, tapped the brakes, and fried the DRV. To my calc with gearing that's 67k erpm... 7k over the limit, and less then a millisecond to pop.

Can anyone that does fast downhill and esk8 chime in with a ESC that is capable of 45mph freewheeling on 36/16 (2.25) gearing and not going to pop if I decide to use brakes vs sliding?

This is getting silly, esk8 made to go fast, but you can't go faster then your geared speed freewheeling downhill or you risk popping vesc and having no brakes...
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-08-26T16:07:02.511Z Reads: 133

```
$100+esc usually don't have problem with erpm. but then they occasionally pops for using burst amp
go with brand or proven esc.

just to note that it's not very efficient to run over 60k. I found with gear ratio u can pretty much achieve any usable speed. 

and it's hard to believe it broke for braking on high speed. cuz erpm limit is for acceleration. that means if u go above the erpm limit board will auto brake?
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-08-26T16:11:15.325Z Reads: 130

```
and tell us ur set up too. everyone smarter than me will help u out better
```

---
## \#5 Posted by: onepunchboard Posted at: 2017-08-26T16:24:42.562Z Reads: 119

```
I see well that's bummer. I can recommend hobbywing ezmax series. or fvt I believe maytech produce these. many seems to use as alternative to vesc
```

---
## \#6 Posted by: Namasaki Posted at: 2017-08-26T17:30:09.153Z Reads: 110

```
I think I may have the answer your looking for. 
You don't need to give up on the Vesc. 
You just need to set up your gearing for downhilling. 
Basically, you need to build a board to use specifically for high speed down hill. 
Large wheels with a small wheel pulley and a large motor pulley. 
Or better yet. Direct drive hub or in wheel motors that will give you a 1:1 ratio.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-08-26T17:37:28.030Z Reads: 108

```
Here are s couple belt drive examples
<img src="/uploads/db1493/original/3X/9/b/9b00bf63d3537e9540cb2c36e46bf1052033ff25.PNG" width="281" height="499"><img src="/uploads/db1493/original/3X/e/4/e44a993903667abf85989ac1787d0322273eb8c1.PNG" width="281" height="499">
```

---
## \#8 Posted by: Namasaki Posted at: 2017-08-26T17:42:10.346Z Reads: 103

```
Here's example with Carvon V2.0 145k

<img src="/uploads/db1493/original/3X/4/9/495c9c71406a4befb339e9ff5bc42823160e7ee2.PNG" width="281" height="499">
```

---
## \#10 Posted by: Namasaki Posted at: 2017-08-26T17:53:47.789Z Reads: 98

```
The Vesc6 might be your answer if it in fact does have a 150k limit. 

What I was suggesting is that if you want to do high speed downhill with Vesc 4.12, then you need to build a board specifically for that purpose.
```

---
## \#11 Posted by: onepunchboard Posted at: 2017-08-26T17:54:02.295Z Reads: 93

```
vesc 6 does 150k. trampa spoke himself. tho it's  beta and 300euro... I saw occasional focbox 80k from endless sphere but can't grantee it won't die. 
or u can buy physical brake or use servo to brake in downhill.
```

---
## \#12 Posted by: Deckoz Posted at: 2017-08-27T03:58:20.602Z Reads: 83

```
@trampa would I have these issues on the VESC 6?
```

---
## \#13 Posted by: BigBoyToys Posted at: 2017-08-27T04:01:28.235Z Reads: 79

```
+1 for the VESC 6 👍
```

---
## \#14 Posted by: chuttney1 Posted at: 2017-08-27T05:43:09.507Z Reads: 71

```
Which VESC did you have?
```

---
## \#15 Posted by: Deckoz Posted at: 2017-08-27T05:48:09.310Z Reads: 71

```
Torqueboards 4.12.
```

---
## \#16 Posted by: trampa Posted at: 2017-08-27T10:05:57.202Z Reads: 61

```
You should not use the motors as a brake system to rely 100% on. Especially high speed downhill riding is problematic. If you are a pro skater that can slide the board sideways, the motor brakes will act as an additional system assisting you to control the speed. Higher ERPM are possible with Vesc Six.

Frank
```

---
## \#17 Posted by: Deckoz Posted at: 2017-08-27T13:37:06.292Z Reads: 52

```
Hey @trampa,

I don't rely 100% :). When the brakes failed I slid and then foot braked to a stop at the bottom. Mostly just looking for confirmation that if I decided to brake like I did the VESC 6 won't blow out. As walking back uphill with a 19lb board isn't to fun all because of a brake tap.  And even better since esk8 could be miles from your car and now have a push board with lots of resistance vs not having the belts on lol. Thanks for your input :)
```

---
