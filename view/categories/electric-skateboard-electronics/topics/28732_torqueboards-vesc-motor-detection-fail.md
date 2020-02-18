# Torqueboards VESC Motor Detection Fail

### Replies: 12 Views: 735

## \#1 Posted by: gottagoslow Posted at: 2017-07-27T05:58:50.371Z Reads: 94

```
Hey all,

My motor seems to fail detection but it does spin during the operation but it is very choppy as seen in the video

[https://youtu.be/TafaMeXmc2k](https://youtu.be/TafaMeXmc2k)

Yes I've followed a lot of guides and other posts but they don't help.

I'm using a Torqueboards VESC with firmware 2.18 and Torqueboards 5065 260kv motor.

Here are my settings:

[http://i.imgur.com/LUX1bYJ.png](http://i.imgur.com/LUX1bYJ.png)

Any help would be much appreciated!
I'm very tired of this after frying my first motor with a 150A RC ESC.
```

---
## \#2 Posted by: jammin Posted at: 2017-07-27T06:01:11.769Z Reads: 85

```
Does your motor behave like this only during motor detection? Try press + holding the arrow keys, does your motor move smoothly then?
```

---
## \#3 Posted by: Namasaki Posted at: 2017-07-27T06:38:17.706Z Reads: 81

```
Remove the motor pulley while doing detection.  make sure nothing is rubbing like the shaft C-clip on the mounting plate.
If your using a sensored setup, try unplugging the sensor cable and see if it will detect without sensor.
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-07-27T08:30:47.147Z Reads: 76

```
You´re running 6s lipos?
Check if nothing is shorting inside the motor. How long are your wires and how long are your motor mounting screws? (the last guy had the screws too long, they touched the windings inside and so his detection didn´t work properly.)
```

---
## \#5 Posted by: GrecoMan Posted at: 2017-07-27T17:55:04.814Z Reads: 63

```
@TarzanHBK Hahaha that was me... Btw all four of my screws were replaced and now everything is running smoothly with my board
```

---
## \#6 Posted by: gottagoslow Posted at: 2017-07-28T03:26:34.408Z Reads: 54

```
@jammin They also behave like in the video when I use the arrow keys

@Namasaki Removed it and retested, still no go.

@TarzanHBK Yes I'm running 6S. WELL DARN, the provided hex screws from the @torqueboards 50mm motor mount kit caused this. I unscrewed them so that the motor is freely moveable in the mount, retested the motor detection and walla!

Now I really think this caused my last torqueboards motor to fry, cause the tips of the motor mount screws were charred!
Now I need to find a way to sand down these hex screws.....
```

---
## \#7 Posted by: TarzanHBK Posted at: 2017-07-28T06:15:57.978Z Reads: 49

```
there you go. Just buy shorter ones ;)
```

---
## \#8 Posted by: flywithgriff Posted at: 2017-07-28T06:19:28.606Z Reads: 48

```
@gottagoslow send @torqueboards a message and tell him what is going on. I'm sure he will help you out.
```

---
## \#9 Posted by: GrecoMan Posted at: 2017-07-28T12:01:42.111Z Reads: 48

```
Aha I see this is more common than I thought
```

---
## \#10 Posted by: torqueboards Posted at: 2017-07-29T02:55:37.846Z Reads: 44

```
@gottagoslow I think this is a specific issue with the 5065 since it's a smaller motor. 63mm doesn't have this issue but thanks for bringing it to my attention.
```

---
## \#11 Posted by: gottagoslow Posted at: 2017-07-29T03:30:55.712Z Reads: 39

```
Okay, I've scavenged some M4 phillips screws that are like 8mm long and they work perfectly!
Motor detects and I've been contacted by Torqueboards.
```

---
## \#12 Posted by: GrecoMan Posted at: 2017-07-29T11:02:28.197Z Reads: 30

```
Yup, I had the same problem
```

---
