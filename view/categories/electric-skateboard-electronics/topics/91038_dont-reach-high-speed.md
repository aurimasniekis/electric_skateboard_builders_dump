# Dont reach high speed

### Replies: 7 Views: 308

## \#1 Posted by: SolarTurtle Posted at: 2019-04-18T19:31:15.744Z Reads: 158

```
Hey,

i use the 2x VESC 4.12 for a dual hub motor (from diyeboard, the 75kV).
Since i have 90mm wheels i should theoretical reach 53,4kmh, with 95% duty cycle 50,7kmh at full voltage (42V, 10S3P).

But i only reach ~37kmh with full battery. And while im cruising in this speed the VESC App shows that the motor only get a small current (<10A) and around 350W. 

Do you have a idea what could be the limiting problem? Battery current and motor current limits are much higher.

Thanks!
```

---
## \#2 Posted by: Hummie Posted at: 2019-04-18T19:36:05.431Z Reads: 151

```
Low voltage cutoff settings?  The first reduces power maybe 20 percent but the second drops it to like 5%
```

---
## \#3 Posted by: visnu777 Posted at: 2019-04-18T19:41:25.913Z Reads: 135

```
It is not 75kv. They have a lot of kv divergence these motors ;)
Edit: http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":75,"system-efficiency":85,"motor-pulley-teeth":1,"wheel-pulley-teeth":1,"wheel-size":90}|
Maybe not wrong kv but this is what you get with these, similar to my diyeboard hubs
```

---
## \#5 Posted by: SolarTurtle Posted at: 2019-04-18T19:59:23.694Z Reads: 99

```
Oh, damn. The weighted value is nearly the real value. Damn. 

I think i need some better motors in the future :slight_smile:

Thanks
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2019-04-18T19:59:32.943Z Reads: 90

```
![image|658x500](upload://6f7hs8KAaLiDDV6l5t60UCNV1uF.jpeg)

38Km is right!!
```

---
## \#7 Posted by: SolarTurtle Posted at: 2019-04-18T20:24:34.917Z Reads: 75

```
Do you know how the formula for the weighted speed is?

I know the other formula, but for the weighted?
```

---
## \#8 Posted by: Pedrodemio Posted at: 2019-04-18T20:58:29.063Z Reads: 59

```
Weighted is just a guess that you input, if you say your loaded speed is x, and your load speed is 85% just make x*0.85

For to actually calculate the weighted speed you have to first calculate the force required to overcome all losses, calculate the torque for that force and from then the current needed in each motor, and then calculate all voltage drop across all components

It’s a lot more work
```

---
