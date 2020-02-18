# VESC 12s bldc settings help!

### Replies: 12 Views: 1317

## \#1 Posted by: filmerskier97 Posted at: 2017-06-09T21:07:40.913Z Reads: 156

```
Hi Everybody,

I seem to be getting a lot of conflicting info on what math I should use for my bldc settings. I am running a 12s7p battery using Samsung 25R cells. I am bypassing the bms and only using it for charging. I am running dual 6355 190KV motors and vescs. I have attached a screenshot on what I think should work but any feedback is greatly appreciated! <img src="/uploads/db1493/original/3X/b/7/b7fa4564eef6b9947ec093af5fd95fca3f0d7560.PNG" width="690" height="411">
```

---
## \#2 Posted by: Jinra Posted at: 2017-06-09T21:19:58.010Z Reads: 148

```
While 28 is the max charging current for your pack, you'll want to use half the value since you have dual motors. So -14A each. Your pack also has a max continuous discharge rating of 140amps so you could probably afford to boost your battery max. You'll never pull 140 amps continuous anyway so it's nice to have the extra power. Perhaps 50 per VESC would be good (to match continuous current rating of the VESC). 

Voltage limits look good. Not sure why you unchecked (slow absolute max), I think that's usually on, but I'm not sure what it does myself.

PS. Sure hope you call your build Lucky 7 since you have 777wh
```

---
## \#3 Posted by: filmerskier97 Posted at: 2017-06-09T21:31:20.521Z Reads: 139

```
Thanks Jinra! thats the exact info I needed. I will post pics of my build soon!
```

---
## \#4 Posted by: Namasaki Posted at: 2017-06-09T23:02:09.829Z Reads: 124

```
[quote="Jinra, post:2, topic:24997"]
Not sure why you unchecked (slow absolute max), I think that's usually on, but I'm not sure what it does myself.
@filmerskier97 
**From Vedder's webpage**
**“Absolute max”** is checked in every PWM switching cycle and used in case the soft back-off strategy for the other limits doesn’t work. I usually set it way higher than the other limits because soft back-off is preferred rather than switching off the motor with a fault code, but it should never be higher than 150A.

The **“Slow absolute max”** box will make sure that a filtered version of the maximum current limit is used. This is useful if there is much noise and that fault code kicks in all the time. I usually have it ticked.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-06-09T23:09:46.691Z Reads: 119

```
Since your using Li-ion cells which can safely go down to 2.8v per cell. 
I would recommend lowering your "Battery cut off start" to 36v (3.0v per cell)  and "Battery cut off end" to 34v
Then just stop riding when you hit the Battery cut off start which is a soft back off strategy and not a total shut down.
```

---
## \#6 Posted by: filmerskier97 Posted at: 2017-06-09T23:21:15.139Z Reads: 116

```
So essentially ill get a bit more range lowering it to 34v but i should hop off when the board starts to slow down?? I would rather be safe than sorry ha ha
```

---
## \#7 Posted by: Hummie Posted at: 2017-06-10T00:09:15.193Z Reads: 112

```
12s7p wow. 

its a two tiered shut down.  you'll first feel a subtle reduction in full throttle power when you hit the first low voltage number and when you drop to the next voltage level power will drop to 10 percent maybe then its worth it to push.  I've damaged cells by trying to power the board longer as there's a voltage cliff the cells are close to when you get down there.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-06-10T02:09:58.405Z Reads: 110

```
Ok, I was under the impression that the second stage would shut the vesc down. Thankyou @Hummie for the clarification.

I agree Hummie on the cliff theory, you want to stay away from the edge. I think that 3.0v per cell should be a safe distance from the edge which is why I suggested setting the first stage to 36v and stop riding when you feel a loss of power.

It's also a good idea to mount an inline voltage gauge on the top of your board or through the deck so you can monitor your pack while your riding.
Here is an example:

<img src="/uploads/db1493/original/3X/a/9/a9134849918321ed8cc4f69e087ed36ca52143d9.jpeg" width="375" height="500">
```

---
## \#9 Posted by: Hummie Posted at: 2017-06-10T03:15:29.996Z Reads: 99

```
thats slick with the button and gauge you must get some looks.  I love how people will stop walking and turn around to look at my board.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-06-10T03:59:30.974Z Reads: 100

```
Thanks, it was inspired by the Raptor 1 with it's button and gauge on top.
```

---
## \#11 Posted by: filmerskier97 Posted at: 2017-06-10T04:55:59.273Z Reads: 101

```
@Namasaki that is genius! what did you use to cut the hole for the voltage gauge? I might be able to get that done with my dremel
```

---
## \#12 Posted by: Namasaki Posted at: 2017-06-10T05:53:04.855Z Reads: 97

```
I've done it with a Dremel with the router atachment.
Be careful what type of bit you use though. The last time I tried to use it, I had the wrong bit and it walked off the line.
I would up using a saber saw and that actually worked a lot better than the Dremel.
You just drill a hole in each corner of the square and then cut from hole to hole.
then finish it by hand with a file.
Then I used a sharpie to color the bare wood black.
For the switch hole I used wood bits to bore the dual size hole.
https://www.electric-skateboard.builders/t/diy-battery-pack-using-basen-26650-hi-drain-li-ion-cells/4973/217?u=namasaki
https://www.electric-skateboard.builders/t/diy-battery-pack-using-basen-26650-hi-drain-li-ion-cells/4973/229?u=namasaki
```

---
