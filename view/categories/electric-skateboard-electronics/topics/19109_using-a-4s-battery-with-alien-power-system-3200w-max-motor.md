# Using a 4S battery with alien power system 3200W max motor

### Replies: 12 Views: 1097

## \#1 Posted by: bhaktatejas922 Posted at: 2017-03-15T19:38:26.277Z Reads: 129

```
Anyone see a problem with using a 4s2p pack with a 150A ESC(yes I know rc ESC gross)? Using 15tooth to 36tooth, 240kv motor, and I'm around 180pounds (80ish kg). I'm not looking for much speed, just like 10-12mph (college campus). I'm worried the ESC could draw too much current and burn out, but are there protections against this in an ESC?
```

---
## \#2 Posted by: Alextech Posted at: 2017-03-15T19:41:27.914Z Reads: 127

```
It's really more dependent on your battery and its discharge capabilities.
```

---
## \#3 Posted by: bhaktatejas922 Posted at: 2017-03-15T21:32:42.420Z Reads: 106

```
Assuming it can discharge to 175A max
```

---
## \#4 Posted by: OskarCastrone Posted at: 2017-03-15T22:07:43.867Z Reads: 101

```
I can not promise you that this will fail and burn, as I have never tried with a 4s setup but many on this forum have reported that using a 4s battery will need too many amps to make up for the lack of volts. Your battery might be able to supply the amperage but your ESC probably wont. Maybe if you consequently give the board some VERY big pushes to get the board to speed, and then apply throttle. That would decrease the draw of too many amps but will still be very risky if you forget, or someone else does. 

I would defined not recommend using a 4s battery. I know from experience that you will be much happier with a great board from the beginning instead of trying to find cheaper parts than suggested on the forum. I would advise you to choose some of the parts that have been recommended by the forum. Then you will not end up buying another full setup and thereafter throwing the 4s setup in the garbage.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-03-15T22:52:52.451Z Reads: 76

```
Bottom line, 6s is minimum voltage for Eskate. Even the cheapest production boards use at least 24volts.
```

---
## \#6 Posted by: bhaktatejas922 Posted at: 2017-03-16T00:08:28.340Z Reads: 67

```
Hm so escs can draw more current than they're rated for? I tested it around and I was happy with the speed. However if 4S could truly lead to too much current, I could just do 6s with a throttle limit
```

---
## \#7 Posted by: Iceni Posted at: 2017-03-16T05:45:50.847Z Reads: 54

```
RC escs usually don't have current limits built in, so if you stall the motor and pull the throttle it's going to keep pushing current through until it either moves or burns up.

If you use 6s and change the gearing to 14/36 with 76mm wheels you get around 18 mph top speed.
```

---
## \#8 Posted by: bhaktatejas922 Posted at: 2017-03-16T06:15:09.463Z Reads: 49

```
Thanks, that's the answer I was looking for. I think I will just go with the 6s with a throttle limit on campus.
```

---
## \#9 Posted by: Iceni Posted at: 2017-03-16T06:22:14.867Z Reads: 48

```
If you don't need/want it to go faster you could switch to a 200kv motor as well, with the suggested gearing/wheel size you would end up at around 15mph max.
```

---
## \#10 Posted by: kieraneboard Posted at: 2017-07-15T22:39:40.425Z Reads: 28

```
Its always a disaster to use low volts under 24V.   And you should try use 36V.
When you need a certain power say 800 Watts, the only way to protect everything is increase volts and lower the current.
You know the current power equation.
Besides, at 80 KG,  dual hub motors can always carry you at high speed.
```

---
## \#11 Posted by: IsTalo Posted at: 2017-07-15T23:17:59.270Z Reads: 27

```
Old threads, why are you reviving it?
```

---
## \#12 Posted by: kieraneboard Posted at: 2017-07-15T23:31:01.427Z Reads: 26

```
I am new on esk8, trying to help and get help back.
```

---
