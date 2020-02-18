# 10s FOC, why should I do it?

### Replies: 17 Views: 1146

## \#1 Posted by: flywithgriff Posted at: 2017-07-14T23:55:57.345Z Reads: 178

```
Hey guys I am currently running BLDC on two 4.12 vesc in my dual 190kv 6374 build. 
I have heard all this talk of how great FOC is and would love to know your opinion of it. I am not against going FOC and would like to try it but I am completely terrified of killing my vesc!
```

---
## \#2 Posted by: psychotiller Posted at: 2017-07-15T00:23:06.973Z Reads: 168

```
Where did you get your vescs from and when did you get them?

The reason to check out foc is because it is an ominously beautiful experience accelerating on a silent board. I think I told LHB it was like being pushed by evil spirits.  :imp:
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-07-15T00:31:47.828Z Reads: 162

```
One is from Chaka and a year old the other I purchased secondhand from LHB. I'm all for a silent ride!
```

---
## \#4 Posted by: Jinra Posted at: 2017-07-15T00:40:57.977Z Reads: 159

```
FOC gets louder with speed, but is quieter at lower RPMs. The chaka VESC should be able to handle it especially on 10s. See if you can source the LHB one, I wouldn't do it with any VESC besides chaka, focbox, or axle.
```

---
## \#5 Posted by: flywithgriff Posted at: 2017-07-15T00:42:08.783Z Reads: 155

```
Then I shall just wait until I go dual FOCBOX!
```

---
## \#6 Posted by: flywithgriff Posted at: 2017-08-26T03:53:21.065Z Reads: 117

```
Ok I have dual FOCBOX and the board is ready to setup. If I decide to go FOC which I want to, what should I be cautious of?
```

---
## \#7 Posted by: Deakbannok Posted at: 2017-08-26T04:11:14.878Z Reads: 128

```
i have focbox on FOC for awhile now and riding it abusively. ☺ For sure you will be fine with it. 
<img src="/uploads/db1493/original/3X/b/3/b384895b409d0d7de5cff6b508de92857398d3e1.jpg" width="281" height="500">
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-08-26T05:36:09.427Z Reads: 125

```
If your running sensors ... If not leave the 1 at sensorless and skip the 7-8 ... 

<img src="/uploads/db1493/original/3X/d/c/dc4f39d6676726650aae6fcc326d42f92469cc3d.png" width="690" height="365">
```

---
## \#10 Posted by: UniqueSnowflakeN27 Posted at: 2017-08-26T07:51:00.274Z Reads: 113

```
Nice!

To get FOC running correctly, this is the last step, right? First you set your battery max/min etc in BLDC and do a motor detection?
```

---
## \#11 Posted by: pjotr47 Posted at: 2017-08-26T11:57:38.431Z Reads: 101

```
I have a focbox and ride in Foc its an amazing different between FOC and BLDC... FOC is so quiet on low speed :)
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2017-08-26T13:32:27.993Z Reads: 92

```
[quote="UniqueSnowflakeN27, post:10, topic:27661"]
BLDC and do a motor detection?
[/quote]

you Don't need a BLDC motor detection to run FOC, since it's a completely different mode than BLDC
```

---
## \#13 Posted by: MontPierre Posted at: 2017-08-26T13:42:34.165Z Reads: 88

```
Does it make sense to use foc with sensorless SK3 6374 192kv? I have focbox. Would preformance be considerably worse than with a sensor?
```

---
## \#14 Posted by: Deckoz Posted at: 2017-08-26T15:05:07.063Z Reads: 90

```
Here's my take...

FOC is fine on the DIY escs on 10s.

what is not fine
-no load braking(dont flip the board upside down throttle it and brake while the wheels are moving, test throttle sure just don't brake)
-going faster then your geared speed, if you make it over 60kerpm going downhill and decide to use brakes, your gonna pop your master drv(in dual) and your slave will become non responsive. no brakes!
```

---
## \#15 Posted by: flywithgriff Posted at: 2017-08-26T15:14:26.771Z Reads: 96

```
Thank you for that layout!!!! Care to suggest starting values for min and max batt and motor? Dual 6374 190kv, dual FOCBOX, 7" pneumatics, 10s2p 150c lipo, 250# rider.
```

---
## \#16 Posted by: Deckoz Posted at: 2017-08-26T15:24:54.797Z Reads: 97

```
I have the following set up for 

Rider Weight 127lbs
Dual 6355 190kv on ackmaniacs firmware this setup is a 10s3p pack that is capable of 60Amps constant current, and 24amps max recharge current(2.5C) the values are divided between two VESCs for a total of the rated power, below is 1 esc

Motor Max 30A
Motor Min -30A
Battery Max 30A
Battery Min -12A
ABS Max 130A
Watts 1200
Throttle Curve 10.5(25), 45(50), 60(75) - edge sharpness 0

Rider Weight ~185
My friends which is dual 6374 190kv 12s4p and capable of 80A constant current, and 30amps max regen(2.5C), again this is one of two VESC's

Motor Max 40A
Motor Min -40A
Battery Max 40A
Battery Min -15
ABS Max 130
Wattage 1300w
Throttle Curve 15(25), 49(50), 63(75) - edge sharpness 0
```

---
## \#17 Posted by: flywithgriff Posted at: 2017-08-26T15:52:31.119Z Reads: 88

```
So to be clear, I need to half the values between the two focbox? In the past running this setup on BLDC I was running 50a-60a on each motor.
```

---
## \#18 Posted by: Deckoz Posted at: 2017-08-26T17:48:31.489Z Reads: 83

```
You see...

The motor max you can set to whatever you want. Just dont set battery max/min shared between two vesc outside of its constant current limits otherwise you just quickly degrade cells..
```

---
