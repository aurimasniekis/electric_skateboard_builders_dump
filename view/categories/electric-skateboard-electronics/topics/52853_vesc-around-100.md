# VESC around $100

### Replies: 21 Views: 1480

## \#1 Posted by: BoiltheOil Posted at: 2018-04-20T00:34:55.549Z Reads: 133

```
I'm looking for a VESC around $100 to upgrade from a cheap, garbage, Chinese substitution. Right now I'm looking at these 3:

 products/torque-esc-vesc-bldc-electronic-speed-controller

https://hyper-ion-systems.myshopify.com/collections/esc-vesc-contollers/products/maytech-super-esc-brushless-controller

https://vandaelectronics.myshopify.com/collections/electronic-speed-controls/products/vesc-motor-controller-custom-cables-and-connectors

Which of these 3 would be the best? Is there another VESC I should consider? I'm running a 6s battery and a 270kv motor (at least that's what it says. It's also a cheap Chinese part but I haven't had issues with it).
```

---
## \#2 Posted by: JLabs Posted at: 2018-04-20T00:38:31.684Z Reads: 125

```
Personally I don’t recommend a standard 4.12 VESC for a 6s setup. I have had success using an FVT 120a ESC, but some others have had them blow smoke. 

So personally for me, I would look at getting a 6s “car” ESC and changing the firmware if possible.
```

---
## \#3 Posted by: BoiltheOil Posted at: 2018-04-20T00:44:56.115Z Reads: 117

```
How do I change the firmware of an esc? They don't have USB ports, do they?
Also, are you talking about something like this:
https://www.ebay.com/itm/FVT-120A-Waterproof-Brushless-Sensorless-ESC-For-1-8-1-10-RC-Car-Skateboard-ESC-/152964419469?_trksid=p2385738.m4383.l4275.c10
or this:
https://www.ebay.com/itm/FVT-BOAT0120-120A-Brushless-Senseless-BOAT-ESC-Speed-Controller-Waterproof-5V-5A-/222696420062?_trksid=p2385738.m4383.l4275.c10
```

---
## \#4 Posted by: JLabs Posted at: 2018-04-20T00:56:33.920Z Reads: 100

```
The first one, and the make a little programmer that you can plug into it.
```

---
## \#5 Posted by: BoiltheOil Posted at: 2018-04-20T01:04:24.579Z Reads: 97

```
Can you post a link to the programmer?
```

---
## \#6 Posted by: JLabs Posted at: 2018-04-20T01:06:00.879Z Reads: 94

```
https://www.rcjuice.com/lcd-program-card-for-fvt-car-esc-s.html
```

---
## \#7 Posted by: BoiltheOil Posted at: 2018-04-20T01:07:26.291Z Reads: 89

```
Thanks, is it similar to VESC software in the sense that you input different values depending on the specs of your motor and battery?
```

---
## \#8 Posted by: JLabs Posted at: 2018-04-20T01:09:11.827Z Reads: 84

```
Not really, you can change dome values but no where near the amount as the VESC software
```

---
## \#9 Posted by: BoiltheOil Posted at: 2018-04-20T01:09:37.736Z Reads: 83

```
So what all can you change?
```

---
## \#10 Posted by: JLabs Posted at: 2018-04-20T01:10:41.664Z Reads: 83

```
It allows you to upgrade the firmware to a more eSk8 style (still not great) and the timing values
```

---
## \#11 Posted by: BoiltheOil Posted at: 2018-04-20T01:13:02.321Z Reads: 79

```
Ok, I will defiantly keep this in mind. I really like the idea of the BLDC software though, so I might go with a VESC still, but if I don't find something that I like, I will certainly go with this. Thank you very much.
```

---
## \#12 Posted by: JohnTakesPhotos Posted at: 2018-04-20T01:17:59.016Z Reads: 79

```
My Maytech speed controllers have been alright - you just have to be more careful with them compared to something like a FOCBOX or VESC6. I seriously regret not buying focboxes when I was shopping for speed controllers, I only saved like 100 NZD with the maytech ones. Save and get a FOCBOX, don't be like me :joy: Also don't even consider a hobby car speed controller, just don't cheap out at all for such an important component.
```

---
## \#13 Posted by: BoiltheOil Posted at: 2018-04-20T01:22:08.234Z Reads: 73

```
Is it worth buying used parts? That could definitely cut cost some, but I'm not sure how bad the wear can get. Ideally it shouldn't matter because it should be good enough to last a long time. If I it's worth buying used, I'll get a FOCbox, but if not, I might just go with a different VESC.
```

---
## \#14 Posted by: JohnTakesPhotos Posted at: 2018-04-20T01:27:35.337Z Reads: 69

```
I'm all for well looked after used components (though all of my eskate stuff has been new). For a speed controller though unless you have a desperate desire to run motors with FOC it's probably better to just buy new so you get a warranty and all that good stuff. Maytech swears by the "high quality components" they use and I haven't had any issues with their customer support (especially with me bugging them about their lack of boot loader :joy: ) so that's probably the best option for you.
```

---
## \#15 Posted by: BoiltheOil Posted at: 2018-04-20T01:29:14.607Z Reads: 68

```
OK, I'll most likely go with the Maytech VESC then. Have you had any issues with their VESC at all? I live in the south and overheating could be a problem.
```

---
## \#16 Posted by: JohnTakesPhotos Posted at: 2018-04-20T01:34:35.742Z Reads: 66

```
How far south is south? I'm in Christchurch, NZ and I've never had an issue but we only have 25-30C summers. I don't have any cooling on it and have it in a pretty much watertight enclosure (I hope).
```

---
## \#17 Posted by: BoiltheOil Posted at: 2018-04-20T01:36:31.924Z Reads: 65

```
United States deep south, around 35C (95F) in the summer, every day.
```

---
## \#18 Posted by: lrdesigns Posted at: 2018-04-20T09:28:11.512Z Reads: 58

```
I have maytech, they have been good to me although I am on 12s dual setup. Only running 12amps per esc. 

It works good for me but a few occasions when I had one motor down, my commute home it would overheat and throttle the speed to make it really slow. Slight up hill for 15 minutes. Hot climate. 

On 6s the heating will be worse as you will need a much higher amp setting. 

Will you run single or dual and how heavy are you, plus back pack?
```

---
## \#19 Posted by: BoiltheOil Posted at: 2018-04-20T10:51:23.095Z Reads: 55

```
Single, motor probably 130 with backpack. I use it to get part of the way home from school.
```

---
## \#20 Posted by: lrdesigns Posted at: 2018-04-20T11:34:45.257Z Reads: 49

```
I’m over 200, but I still think at 6s vesc might be a bad choice unless you get a heat sincked direct fet. Like focbox but that is $155
```

---
## \#21 Posted by: BoiltheOil Posted at: 2018-04-20T13:32:51.668Z Reads: 42

```
I've got a cpu heatsink that should be more than enough cooling
```

---
