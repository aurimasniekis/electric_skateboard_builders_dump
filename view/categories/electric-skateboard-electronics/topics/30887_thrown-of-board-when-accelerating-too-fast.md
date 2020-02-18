# Thrown of board when accelerating too fast

### Replies: 29 Views: 1408

## \#1 Posted by: TeslaAlex Posted at: 2017-08-17T15:04:19.008Z Reads: 245

```
When I pull my trigger a bit to much I get thrown of the board, because the motor stops. If I carefully pull the throttle as I am picking up speed it works fine. Is there a solution to this? I want to be able to use the throttle without being scared of falling of. 

My specs:

X-car beast 120A ESC
2x 5000 mAh 3s 20c in series
5070 Propdrive V2 270kv
```

---
## \#2 Posted by: bartroosen12 Posted at: 2017-08-17T15:20:39.669Z Reads: 234

```
Maybe buy the programcard.
What do you mean with that your motor stops?
Do you mean while breaking or that the power cutts off when full throttle?
```

---
## \#3 Posted by: TeslaAlex Posted at: 2017-08-17T15:25:16.444Z Reads: 225

```
Yea, the power cuts off if I go full throttle
```

---
## \#4 Posted by: TeslaAlex Posted at: 2017-08-17T15:26:01.148Z Reads: 213

```
I have the program card, but it seems to not be working... I'll maybe have to buy a new one
```

---
## \#5 Posted by: treenutter Posted at: 2017-08-17T15:28:32.047Z Reads: 200

```
Does this ESC have low voltage control? It might be that you're voltage-sagging those batteries and hitting a threshold programmed into the ESC, which would cut power if you draw too heavily. That would explain why you can accelerate slowly but have problems when you go full throttle.
```

---
## \#6 Posted by: mccloed Posted at: 2017-08-17T16:09:22.578Z Reads: 189

```
I am assuming you do not have sensors hooked up to the ESC. I had the same problem with my HK 150a ESC. I beleive it is a "safety" feature.My suggestion would be to use a sensored motor. This solved my issue.
```

---
## \#7 Posted by: TeslaAlex Posted at: 2017-08-17T16:14:55.511Z Reads: 170

```
Could you link me a good sensored motor for my current setup, thats also good if I would like to do some upgrades in the future (VESC, 10s or 12s)?
```

---
## \#8 Posted by: TeslaAlex Posted at: 2017-08-17T16:26:44.247Z Reads: 160

```
Could you recommend a solution? Maybe I could lower the voltage cutoff a bit?
```

---
## \#9 Posted by: psychotiller Posted at: 2017-08-17T16:27:01.020Z Reads: 154

```
https://psychotiller.com/product/sensored-5065-motor-270kv
```

---
## \#10 Posted by: TeslaAlex Posted at: 2017-08-17T16:30:23.782Z Reads: 140

```
It seems like this motor only supports up to 8s lipo. I would like something that could be useful when upgrading to higher voltages.
```

---
## \#11 Posted by: TeslaAlex Posted at: 2017-08-17T16:34:02.259Z Reads: 137

```
Im not really that happy about buying a new motor right away, I would rather like to solve it with the components i already have....
```

---
## \#12 Posted by: psychotiller Posted at: 2017-08-17T16:36:04.491Z Reads: 132

```
Check with http://www.ollinboardcompany.com/. you may need to change your mount though.

Also, you'll need to find motors with a lower kv if you're planning to go forward with 10s or 12s.
```

---
## \#13 Posted by: TeslaAlex Posted at: 2017-08-17T16:37:41.813Z Reads: 128

```
Something around 160 - 190kv?
```

---
## \#14 Posted by: psychotiller Posted at: 2017-08-17T16:38:03.664Z Reads: 125

```
The parts you have are going to limit what you can do. Start planning a new build using the parts you need to acheive your goal or buy the parts you need to make your current build work safely.
```

---
## \#15 Posted by: hornet90 Posted at: 2017-08-17T16:41:06.395Z Reads: 125

```
I used that program card befor i sent it to you it is working,post pics of screen ......
```

---
## \#16 Posted by: TeslaAlex Posted at: 2017-08-17T16:45:28.978Z Reads: 116

```
<img src="/uploads/db1493/original/3X/f/8/f895fd85f16d74e572332007ae8bd4a6099e8d33.JPG" width="666" height="500">
```

---
## \#18 Posted by: darkkevind Posted at: 2017-08-17T22:01:17.309Z Reads: 89

```
Are you connecting the program card before switching on the ESC?
```

---
## \#19 Posted by: lowGuido Posted at: 2017-08-17T22:31:47.575Z Reads: 85

```
I have never used sensors and I have never had this happen with any of my ESC's 
I don't believe its a safety setting. that doesnt make sense.
I also don't change many settings on the programming card from the default. just max timing, and min punch.
I have used so many of these ESC's I have lost count. never seen this before.
```

---
## \#20 Posted by: saul Posted at: 2017-08-18T03:21:19.138Z Reads: 82

```
i got that esc on sale long long ago. it sits in a box where it belongs. :joy:
i'm sure it would be great on a rc truck doing wheelies and all. 

but yea grab a vesc. and another 3s for 9s.
or try on 6s for sure that won't throw you off anymore...
```

---
## \#21 Posted by: hornet90 Posted at: 2017-08-18T05:14:16.974Z Reads: 75

```
I done over 100 miles on a xcar 150a esc had lots of fun .....you need to get the pc program working the interface on that card sucks but useable..bet the driver didnt install with the program. Uninstall restart install restart then plug in card...see does that work
```

---
## \#22 Posted by: hornet90 Posted at: 2017-08-18T12:40:05.464Z Reads: 69

```
Go to computer right click onit go to properties
On the left hand side click on device manager
Click on universal serial bus controllers ....leave that open plug in your card and turn on your esc take a screen shot befor and after send it to me 

Thanks
```

---
## \#23 Posted by: hornet90 Posted at: 2017-08-18T12:42:54.392Z Reads: 72

```
<img src="/uploads/db1493/original/3X/2/b/2b512887e178413bd06c72a1040360c466b88671.png" width="473" height="500">

you need to get here to see if driver is installed
```

---
## \#24 Posted by: TeslaAlex Posted at: 2017-08-18T15:01:04.688Z Reads: 65

```
I got the program card to work using my brothers computer. What settings do you guys recommend?

Im still having a problem with the acceleration. Should I try to change the cutoff voltage?
```

---
## \#25 Posted by: TeslaAlex Posted at: 2017-08-18T15:37:55.682Z Reads: 61

```
<img src="/uploads/db1493/original/3X/1/3/139b91298d4ab9e326faf1ceb59a3f6e35b08ba7.JPG" width="666" height="500">
```

---
## \#26 Posted by: hornet90 Posted at: 2017-08-20T05:31:34.511Z Reads: 56

```
Hows that going for you now....are u already thinling about a 8 or 10s eboard
```

---
## \#27 Posted by: lowGuido Posted at: 2017-08-20T06:22:21.181Z Reads: 56

```
6S is fine for most things, unless you want to climb mountains. I regularly top 40 on my 6S builds. I got one that would probably crack 50
```

---
## \#28 Posted by: hornet90 Posted at: 2017-08-20T07:35:16.693Z Reads: 48

```
i have 2 10s boards and im starting a 6s ......6s  boards are great there light to carry but if u can live with 6-8 mile range there great.
```

---
## \#29 Posted by: TeslaAlex Posted at: 2017-08-20T09:17:09.263Z Reads: 43

```
I changed the cutoff voltage a bit and it works a lot better now.
Top speed flat: 22 mph
Range: 9-10 miles

Really happy with the board so far!
```

---
## \#30 Posted by: EL_PAPI_CHULO Posted at: 2017-08-22T01:35:45.370Z Reads: 36

```
change the controller for a better one i recomend you one from torqueboards.com since i had the similar problem when using a cheap one from china
```

---
