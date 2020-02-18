# Battery Not fully charged ?!

### Replies: 25 Views: 1221

## \#1 Posted by: dotruongq Posted at: 2017-12-24T19:50:58.043Z Reads: 137

```
Hello folks
I recently built a 12S4p 30q samsung, I've been having an issue with that battery not fully charged. It always charges up to 49V. The Charger LED turned green ( which mean charged). I open up the battery and examine each series, only one always at 4.15v and the rest range around 4.07v.  I've seen topics like this but yet no finest solution. Im using Bestech Charge - bypass only bms, the charger model picture below. Any comment, solution is highly appreciated .
Cheers ! 
<img src="/uploads/db1493/original/3X/2/c/2c7973bd5fb78fc8f4eba8d6355ef4bf41805574.jpg" width="564" height="431">
```

---
## \#2 Posted by: scepterr Posted at: 2017-12-24T19:52:38.907Z Reads: 134

```
Which bms do you have? Seems cell unbalance is making it hit total voltage early and then dropping

A pic of the BMS would help, burned resistors can cause this
```

---
## \#3 Posted by: dotruongq Posted at: 2017-12-24T19:56:41.360Z Reads: 133

```
<img src="/uploads/db1493/original/3X/6/6/661fd1f1255ed290e28c1945ce102baa4d7afd24.jpg" width="377" height="500">

Previously I used SuPower BMS, I parted that one out and build on top of this bestech bms
```

---
## \#4 Posted by: dg798 Posted at: 2017-12-24T19:59:38.088Z Reads: 121

```
Double check balance lead from bms, make sure they are all connected and in the right spot.
```

---
## \#5 Posted by: dg798 Posted at: 2017-12-24T20:00:00.947Z Reads: 121

```
Also how many amps is the charger
```

---
## \#6 Posted by: MysticalDork Posted at: 2017-12-24T20:01:25.251Z Reads: 120

```
Sounds like a two-fold problem. First, the charger isn't going to 4.2/cell. Second, because the cells aren't reaching 4.2, the BMS isn't balancing them. 

The charger has a couple blue potentiometers on the board. One controls the final voltage, one controls the charge current. You should open it up and twiddle the pots until it outputs 50.4 volts, then charge the pack again and see if that solves the problem.
```

---
## \#7 Posted by: dotruongq Posted at: 2017-12-24T20:01:59.195Z Reads: 116

```
it 50.4V, 4Amp , I usually Unplug the charger when the LED turned green, and the pack at 49V. So i;m not sure what make the charger stop charging ( or it still charging but LED says otherwise )
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-12-24T20:02:37.254Z Reads: 113

```
Take a meter and check the voltage of the charger without anything plugged into it.
```

---
## \#9 Posted by: dg798 Posted at: 2017-12-24T20:02:57.372Z Reads: 110

```
For the future though you should probably not take the charger out until 50.2v.
```

---
## \#10 Posted by: dg798 Posted at: 2017-12-24T20:03:29.182Z Reads: 107

```
Also maybe try a different charger if you have one.
It could just be a bad charger as well
```

---
## \#11 Posted by: scepterr Posted at: 2017-12-24T20:09:30.984Z Reads: 103

```
Need a pic of the actual BMS to see if there's damage
```

---
## \#12 Posted by: dotruongq Posted at: 2017-12-24T20:27:51.714Z Reads: 101

```

<img src="/uploads/db1493/original/3X/e/c/ec0cda09b854fd97d57d924ea377bb50a4c95ec1.jpg" width="281" height="500">
- This is battery output without load

<img src="/uploads/db1493/original/3X/5/e/5e714d545442fb0b2e30816ad15ce559e08f855f.jpg" width="281" height="500">
- this is when plug in, and LED green turn on ( charged), meter measure from battery output 

<img src="/uploads/db1493/original/3X/2/7/277b66c3d31aa9980ceb9029a5aeb3e83980610e.jpg" width="375" height="500">
BMS before install 

Individual  series voltage

1 x 4.18v 
11x  4.07v
```

---
## \#13 Posted by: dotruongq Posted at: 2017-12-24T20:28:33.154Z Reads: 93

```
what charger you reccomended
```

---
## \#14 Posted by: dg798 Posted at: 2017-12-24T20:33:15.891Z Reads: 93

```
I’d go with a standard 3-5 amp ebike Charger.
```

---
## \#15 Posted by: scepterr Posted at: 2017-12-24T20:41:13.424Z Reads: 92

```
Lol need to see the BMS as it is now 😉, specifically the PCB underneath with the balance resistors

Look for something like this
<img src="/uploads/db1493/original/3X/a/6/a6368fb780df1a2aab7751651eaa41e026bb23ee.jpg" width="374" height="500">
```

---
## \#16 Posted by: pat.speed Posted at: 2017-12-24T21:27:43.765Z Reads: 87

```
Hey mate, I think @MysticalDork is right here. And what is happening is when you plug it into charge the voltage is dipping slightly down to 49v. Oh and Merry Christmas everyone
```

---
## \#17 Posted by: Deckoz Posted at: 2017-12-24T21:29:04.121Z Reads: 89

```
This is definitely his charger being undervolted

You need to turn one of the blue pots inside to make the end voltage 50.4 when the light turns green. 

With the charger unplugged from the pack
-Remove the top

-hook up meter to the plug

-find which blue pot changes the voltage, if the pot doesn't change the voltage, put it back and move to the next

-once you find the next that does voltage, hook up the meter to the pack and play in the charger. Once the charger turns green if the pack is still under 50.4v, turn the pot in the direction 1/4-1/2 turn at a time, and allow the pack to charge until the light is green, if the voltage is still not 50.4 repeat. Do this until the pack reads 50.4v, and the charger is green. 

-put hot glue or something on the pot to keep it from moving, close the charger back up. Your charger may read 50.6 or 50.8 while unplugged, but will only supply 50.4 under load due to the resistance of the pack. All changers should be calibrated after you buy them before completing the board

Example of the end result
<img src="/uploads/db1493/original/3X/4/a/4ac083c3e733822cfcb5903cc163c173ee8a12e5.jpeg" width="666" height="500">
```

---
## \#18 Posted by: scepterr Posted at: 2017-12-24T21:31:28.175Z Reads: 85

```
It could be also that, but for new cells to get that unbalanced something has to be draining them unevenly
```

---
## \#19 Posted by: Achmed20 Posted at: 2017-12-24T21:35:41.190Z Reads: 84

```
i've read somwhere here that the bestech BMS starts balancing when its finished charging (basicly liek every lipo charge does). so if you leave it on, it might actualy solve your inbalance problem automaticaly.
no idea if this information is correct though
```

---
## \#20 Posted by: scepterr Posted at: 2017-12-24T21:40:27.394Z Reads: 83

```
It can/will balance when it hits full charge, assuming there's nothing wrong with the actual BMS that caused the unbalance
```

---
## \#21 Posted by: dotruongq Posted at: 2017-12-25T00:14:20.285Z Reads: 75

```
I checked the bms, seems to be fine, i just dont want to screw top pcb off for now. What I notice for a test run today that from 49V to 45.4V ( 3 miles ). Not sure If this is normal ? what the lowest I can run the 30Q to. My set up is 190kv 6374 dual. and big offroad wheel lol. If this drainage isnt normal than i have to think of i have a bad cell somewhere within the pack
```

---
## \#22 Posted by: dotruongq Posted at: 2017-12-25T00:15:05.167Z Reads: 74

```
chaka mentioned it would take weeks to let it auto balance.
```

---
## \#23 Posted by: dotruongq Posted at: 2017-12-25T00:15:37.531Z Reads: 74

```
ill try this out
```

---
## \#24 Posted by: scepterr Posted at: 2017-12-25T00:18:38.058Z Reads: 72

```
That amount of drain is normal for your config, assuming cells are balanced, 45.4 means 3.78 per cell which means you haven't even hit nominal voltage yet, the part where it levels off

I would drain the 1S that's higher than the rest to as close as you can to the rest, then balance
```

---
## \#25 Posted by: ShutterShock Posted at: 2017-12-25T20:54:35.188Z Reads: 62

```
Have you tried leaving the charger plugged in for about an hour after it turns green?  Sometimes even when the charger turns green, it can still be balancing the cells.  Leave it plugged in and check the cells periodically after it hits "full".
```

---
