# Weird sound and performance \[6374 + VESC\]

### Replies: 15 Views: 375

## \#1 Posted by: xsynatic Posted at: 2019-03-06T23:34:10.292Z Reads: 110

```
Hello,

i'm currently trying to finally set up my board but so far i'n not that happy.

Compared to other build, the sound mine makes is a bit weird. Its shrill and clicky? And second the performance. On the video without me on the board is full throttle. I'm not sure if it is configured wrong or whats the deal. Any ideas?

I also wish that i could configure 2 speed modes with my nano remote or use the reverse button, Smoother acceleration etc.

I've uploaded 2 Video to youtube to demonstrate it. One is without and one with me on the board.

I'm using a Torqueboard 6374.

Vesc 4.12

270mm 15mm belt

16T Motor Pulley and

36T Wheel pulley (Currently 3D printed.)

Running sensored.

[Youtube video 1](https://youtu.be/3E6RjlGmW18)

[Youtube video 2](https://youtu.be/9jf8h00PfSA)

Here are some screenshots if you cannot see them properly.
[screenshots](https://imgur.com/a/y2ivUyi)

![Unbenannt|690x191](upload://yi6ZOqV0dApuenOmohKA3KMqQeo.png) ![Unbenannt1|690x179](upload://wD6EAneQKA5rqBReiTbl0RxpL6K.png) ![Unbenannt2|690x184](upload://g4SwtEqSDt2dvUSsc6fI6Vnjx7y.png) ![Unbenannt3|690x182](upload://r9LZkMlMPlxQyVdjl34kx4uLB84.png) ![Unbenannt4|690x182](upload://fTrflmlm4Fz9flf0rJ6V4KkncPO.png) ![Unbenannt5|690x182](upload://k8LI9t6gAeCsZ4Msvy5zs706qS5.png) ![Unbenannt6|690x184](upload://c1RxKRshQVonjvsEQDhk9oABiYY.png) ![Unbenannt7|690x181](upload://p3U9kQtEjGrqFmLRWuy4yn8w3UW.png)
```

---
## \#2 Posted by: briman05 Posted at: 2019-03-06T23:51:02.792Z Reads: 94

```
I’m guessing you did the motor detection. Did you do the detection with the belt on? It sounds a little like the belt might be to tight
```

---
## \#4 Posted by: xsynatic Posted at: 2019-03-07T00:03:27.123Z Reads: 89

```
Motor detection Yes. With belt? Not sure to be honest.

The Belt itself has a good amount of flex still. 5-9mm is my guess..
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-03-07T01:22:00.757Z Reads: 84

```
@xsynatic  What are your voltage cutoff settings? What are your current settings? What are your settings in general? Post screenshots/pictures/descriptions.
```

---
## \#6 Posted by: briman05 Posted at: 2019-03-07T04:28:23.679Z Reads: 75

```
Well you never do a detection with the belts on probably not causing the issue but I would redo it to so you know. Like @MysticalDork said post a screen shot of your settings. Also your belt seems super long for standard mount mount and none pneumatic wheels
```

---
## \#7 Posted by: xsynatic Posted at: 2019-03-07T10:49:30.320Z Reads: 62

```
Its a 270mm Belt. I just re-did the Motor detection and setup. I'll have a look how it performs now. 

Here are some screenshots of my configuration.

[Screenshots](https://imgur.com/a/y2ivUyi)
```

---
## \#8 Posted by: xsynatic Posted at: 2019-03-07T10:52:18.604Z Reads: 54

```
Its the standart setting after giving the tool the amount of cells. it started at 20~v and ended at 18~v

[Screenshots *click*](https://imgur.com/a/y2ivUyi)
```

---
## \#9 Posted by: briman05 Posted at: 2019-03-07T14:36:39.169Z Reads: 48

```
Well one thing I noticed is you motor max is 85 and the TB's max is 80 So I would change that.  Reason I said your belt seemed big was because you stated it was 470mm in your OP. What type battery are you using I'm guessing 8s?
```

---
## \#10 Posted by: xsynatic Posted at: 2019-03-07T14:50:53.058Z Reads: 45

```
I changed to back to 75 without any noticible changes.
470mm will be my new Belts for the pneumatics, i swapped them on the post. 270 is correct.

Currently i have  a 6s LiPo connected but have a second one for either parallel or series.
[Battery specs]

Minimum Capacity: 12000mAh

Cell Count: 6 / 22.2V

Constant Discharge: 12C

eak Discharge (10sec): 24C
```

---
## \#11 Posted by: briman05 Posted at: 2019-03-07T14:56:09.774Z Reads: 44

```
Well 190kv should be ran on a 10s battery that is the nice sweet spot for 10s it will work with 12s for a 6s battery you want something with a higher kv.  How much of a charge does your battery have?

https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#12 Posted by: xsynatic Posted at: 2019-03-07T15:12:14.148Z Reads: 38

```
The battery currently has ~90%
```

---
## \#13 Posted by: briman05 Posted at: 2019-03-07T15:16:36.132Z Reads: 36

```
Well the main thing I would say is that the batteries is to low of a voltage for the 190 kv with you standing on it.
```

---
## \#14 Posted by: xsynatic Posted at: 2019-03-07T15:24:50.290Z Reads: 34

```
So, to clear maybe some things up. My build was inspired by Skatemetrics Patriot.
I basically use the same Motor,Battery and VESC. Only in a different configuration (Signle and street for now)

[Skatemetrics Video](https://www.youtube.com/watch?v=OMTzGOZPw3M)
```

---
## \#15 Posted by: briman05 Posted at: 2019-03-07T16:38:01.153Z Reads: 29

```
Ok so a few things they are using  that are different a dual motors which and the 6.6 vesc you are using the 4.12 vesc which has a max amp of 50a there is 100a per motor so that is very different and you need to change your motor max to 50 because prolonged use will probably blow the vesc. They are also using different motors than you so it is different and you may be using the same batteries but they have 2 wired up where you have one that makes a difference in the voltage.  If I did the math right your battery is capable of producing 144A so adjust your battery max.
```

---
## \#16 Posted by: MysticalDork Posted at: 2019-03-08T03:13:12.538Z Reads: 23

```
In those pics, your battery current is set very low at 20A.. I'd go with at least 40A for battery current max, probably more like 50 or 55.

190KV motors are really most suited for 10s batteries. You may want to get a pair of 5s packs, or a 4s to pair with your 6s. (Just make sure the brand, capacity, and C rating all match.)
```

---
