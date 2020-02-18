# Backfire Chinese clone BMS replacement

### Replies: 13 Views: 1681

## \#1 Posted by: wariat777 Posted at: 2017-06-05T22:28:17.329Z Reads: 148

```
Hi. As i mentioned in my introduction I want to fix my Backfire Chinese board.

Do some of you guys have any idea if the wiring will be suitable for the BMS i want to use?

http://www.batterysupports.com/22v-24v-6s-60a-6x-36v-lithium-ion-lipo-battery-bms-pcm-pcb-p-478.html

There are strict instructions on the BMS product site how to connect the battery and i have no clue how the battery looks inside... Can i just put the 6pin connector in the new BMS and hope for the best or this is rather stupid idea?

Here is how the connector and the old BMS looks like:

 <img src="/uploads/db1493/original/3X/3/6/368f7e06aa51a2ffb4d878b50916e6569012cf3f.jpg" width="690" height="388">
```

---
## \#2 Posted by: sl33py Posted at: 2017-06-05T22:33:44.473Z Reads: 134

```
I'd start reading on BMS - do a few searches.  Tons of info on how to wire, and several folks who run a BMS only to charge, and bypass for discharge (to power board) so they can use an inexpensive smaller BMS for charging only.

Connector is a Deans plug.  I'd swap to XT90/XT60 - or whatever you prefer.
```

---
## \#3 Posted by: Jinra Posted at: 2017-06-05T22:37:15.092Z Reads: 129

```
While you can't see the battery you can measure the voltages on a header. For sure use a multimeter to test the leads before attaching anything.
```

---
## \#4 Posted by: wariat777 Posted at: 2017-06-05T23:14:04.450Z Reads: 112

```
So I understand, even if the connector is the same on the battery it doesn't necessarily means it's good for the new BMS?
Battery is 6s (shows 29,4V) and the specs for the BMS seems even better than the original. To make sure i should check the voltage coming out of battery through the 6pin ( dean, right? ) I already bought the BMS and I want it to work as it was -> to pass through all the power to VESC and charge with original socket charger.
```

---
## \#5 Posted by: lowGuido Posted at: 2017-06-06T00:11:40.352Z Reads: 106

```
that FET looks a bit fried.  maybe you could just replace it. its hard to tell if there is any other damage from the picture...
```

---
## \#6 Posted by: wariat777 Posted at: 2017-06-06T00:47:54.679Z Reads: 102

```
Well i tried to get it fixed by some help of retarded electrician when only ESC was fried and the guy tried to soldier something on ESC and the FET popped of like a popcorn in the microwave, I have this other BMS now, i don't know if it's safe to try to fix the old BMS ... Because i payed for the VESC quite a lot already i am a bit concerned if i should fix the FET and connect the BMS to the battery. I can't see any other damage and the battery shows 29,4V so I assume it is alright.
```

---
## \#7 Posted by: Jinra Posted at: 2017-06-06T00:59:49.108Z Reads: 95

```
yea some BMS's have 1 less pin on the balance connecting opting for a separate (soldered) connection to B-.

For example, a 6s BMS may have 6 pins on balance lead with solder on B- direct to pcb, while another BMS may have 7 pins on balance lead (6 positives 1 negative).
```

---
## \#8 Posted by: wariat777 Posted at: 2017-06-06T01:37:24.861Z Reads: 89

```
<img src="/uploads/db1493/original/3X/3/7/37b91a471aafd58080a57c55b7e48e2ff40309fa.png" width="281" height="500">

Maybe this is a little better picture to show the connections on the old BMS.
```

---
## \#9 Posted by: wariat777 Posted at: 2017-06-08T13:49:51.770Z Reads: 71

```
Ok so i chacked the voltages on  6pin output from the battery starting from 1 - 6. And it shows 
1        2       3      4        5       6
 5V   10V   15V   20V  25V   30V

5V between each connector..

Isn't it suppose to be like instruction from the BMS says

  1     -    2    -     3      -     4     -    5   -   6    
3.7V  - 7.4V - 11.1V  -  14.8V  - 18V - 22V 

Can i still use it then?
```

---
## \#10 Posted by: wariat777 Posted at: 2017-07-20T17:37:20.882Z Reads: 56

```
Ok. So I just want to inform everyone interested in the topic I created that I was able to connect Maytech VESC and 22V 24V 6S 60A 6x 3.6V Lithium ion LiPo Battery BMS PCM PCB from the website I mentioned all together and I confirm it works without any changes in the 6-pin battery control cable. It charges the battery with the charger provided with longboard and discharges normally. for safety I also set limits to 19-18V cutoff on the VESC to avoid over-discharge. 

The board now  behaves like a charm, It has better breaks and smoother start.  i had some trouble to fit all the parts together in the small compartment but I did it somehow.

If you have any questions feel free to PM me and maybe I will be able to help if you want to upgrade your chinese clone as well.
```

---
## \#11 Posted by: Zim Posted at: 2018-04-20T18:27:07.994Z Reads: 26

```
@wariat777 Hey, just looking through the posts and this is the only thing I could find online that was remotely close to what I was looking for.

I have an old Magneto electric longboard (china clone) and it looks identical to the backfire one you have listed above. You wouldn't happen to have a picture of your new bms wired up? I would be forever grateful knowing I could buy this thing and it would actually work. 

A little detail on my problem:
I have two units and one of the BMS's was working up until today when I accidentally fried it(or at least I think it is fried) 

on one of the setups, my system will turn on when connected to the charger and will run normally. When I unplug it will stay on for about 5 seconds then turn off. It will not charge or discharge on its own.

on the second skate, the battery will charge but not discharge. 

I have connected both esc to the one that turns on when connected to a charger and they both work fine. I think I just damaged both BMS when I was trying to find out why they wouldn't turn on.
!

I've attached a photo of the BMS that i need (this is the one that charges but does not discharge )

[31044097_10212153214533740_9083967710643093504_n|375x500](upload://f5eJeTYq0Lv24eaodmirqynWZAm.jpg)
```

---
## \#12 Posted by: Zim Posted at: 2018-04-20T18:27:50.383Z Reads: 25

```
![31044097_10212153214533740_9083967710643093504_n|375x500](upload://f5eJeTYq0Lv24eaodmirqynWZAm.jpg)
```

---
## \#13 Posted by: Zim Posted at: 2018-04-20T18:28:21.604Z Reads: 23

```
It might be upside down.
```

---
