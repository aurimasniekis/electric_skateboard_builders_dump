# Handbrake Mode on Vesc 6

### Replies: 12 Views: 968

## \#1 Posted by: Dwain Posted at: 2018-03-08T11:44:23.060Z Reads: 210

```
Hi guys does anyone know if the firmware update for Handbrake mode on the vesc 6 has been released yet ?? 

And how do I activate it ?

My goal is to bring the board to a complete stop even on a slight decline .

Any help please.
```

---
## \#2 Posted by: trampa Posted at: 2018-03-11T20:54:05.706Z Reads: 131

```
Nope, not yet. 

Frank
```

---
## \#3 Posted by: b264 Posted at: 2018-03-11T21:26:23.896Z Reads: 120

```
Feel free to implement that!  It's open-source
```

---
## \#4 Posted by: Lumaci Posted at: 2018-03-11T21:57:44.205Z Reads: 112

```
It should also be pretty easy to code, we just need something like a button we can dedicate to applying constant full braking that should only work under x amount of rpm to prevent someone from flying. (We aint ready to fly yet)
```

---
## \#5 Posted by: ATLesk8 Posted at: 2018-03-11T22:06:45.020Z Reads: 107

```
Dude a handbrake slide would be so cool
```

---
## \#6 Posted by: Sebike Posted at: 2018-03-11T22:23:38.995Z Reads: 103

```
wow. can't wait.

![brake|428x500](upload://9BqPXqtfU4Dx4lRxD17wJ4wbYHw.jpg)
```

---
## \#7 Posted by: b264 Posted at: 2018-03-11T23:06:15.633Z Reads: 93

```
Just make it kick in after rolling slows to a certain amount, if you continue to hold the brake
```

---
## \#8 Posted by: amms50 Posted at: 2019-11-04T19:40:05.479Z Reads: 51

```
Still nothing?
```

---
## \#9 Posted by: JohnA Posted at: 2019-11-04T19:58:53.886Z Reads: 49

```
@amms50 not sure for esk8 Wireless ppm use, but for Ebikes you can use ADC 1 for throttle, and ADC 2 for brake. So it might be possible to hard wire a hand brake to ADC 2. Or use a break button that just shorts out the RX to ground. Alternatively short TX to ground and you can use this as a cruise control.
http://vedder.se/forums/viewtopic.php?t=419
```

---
## \#10 Posted by: RyEnd Posted at: 2019-11-04T22:18:24.707Z Reads: 43

```
Newest vesc tool on newest FW allows for reverse current braking (or whatever it's called) that applies low reverse current after you come to a stop to hold you even on a downslope. Don't have too much experience with it yet since it's new and the weather here has been bad, but seems great in theory.

edit: might be uart only?
```

---
## \#11 Posted by: amms50 Posted at: 2019-11-05T19:58:48.556Z Reads: 25

```
Unfortunately my remote will be connected with uart
```

---
## \#12 Posted by: amms50 Posted at: 2019-11-05T20:01:08.033Z Reads: 26

```
Well the problem is that I have a unity and I heard that unity only works on its own app, didn’t try it but would give it a try when my battery is built

P.s: my remote will be connected with uart so no worries 😉
```

---
