# Wanna go faast!

### Replies: 13 Views: 378

## \#1 Posted by: butt_stallion Posted at: 2018-11-17T03:36:56.639Z Reads: 190

```
Alright, so I finally finished my board a few months ago and have been riding pretty much every day.  I currently have a top speed of about 28 mph, at first I thought this was fast and I didn't think I'd want to go faster than that.  But after getting used to the board and the speed I would like to try to hit somewhere in the 30's.  
Here's my current setup:
Single FOCBOX VESC
10s5p battery
6364 190kv motor
36T wheel pulley
14T motor pulley
12mm wide belt
90mm flywheels

BLDC Settings:
75 amp motor max
-40 amp motor min
40 amp batt max
-12 amp batt min

Are there any suggestions for settings or hardware to increase my speed?
```

---
## \#2 Posted by: Fiori Posted at: 2018-11-17T03:46:44.358Z Reads: 171

```
Well you can go with a 32T wheel pulley, or even 28T, but you will pay for it in low end torque. 

What cells are you using? You can make a larger batter(10s6p?) and upgrade to a vesc6 and double you're amperage. Or, go dual motor and get another focbox and you will also have double the amperage capability. 

If you are running 10s5p 30Q, you can put out 80A safely. I would say you could even push it to 100A. You will feel the power difference.
```

---
## \#3 Posted by: butt_stallion Posted at: 2018-11-17T03:56:11.459Z Reads: 146

```
I have 10s5p 30q, so do I need to change the battery amp max to increase the power or the motor max?  I am eventually going to upgrade to a dual drive but it's not currently in the budget.  I thought the focbox was the vesc 6 it just had a different name?
```

---
## \#4 Posted by: esk8jpn Posted at: 2018-11-17T04:26:12.678Z Reads: 126

```
Let's use a larger wheel. 97mm, 107mm etc.
You lose torque and get high speed instead.
```

---
## \#5 Posted by: Skunk Posted at: 2018-11-17T04:26:42.494Z Reads: 119

```
I hear @torqueboards 110mm wheel will be available for (pre?)order on black Friday.
```

---
## \#6 Posted by: torqueboards Posted at: 2018-11-17T04:29:23.828Z Reads: 119

```
@Skunk Yeah, we'll have them for pre-order. Molds are being made now.
```

---
## \#7 Posted by: Fiori Posted at: 2018-11-17T04:34:20.854Z Reads: 119

```
Don't increase battery max to more than 50A on your single focbox. You can only go up to 80A total with dual motors and two foc boxes(40A ea box, or 50A ea box for 100a). 

Foc Box is not a vesc6. 

Cheapest upgrade would be a 32T pulley, and some 107mm flywheels.
```

---
## \#8 Posted by: pat.speed Posted at: 2018-11-17T07:10:26.353Z Reads: 89

```
That will be lacking in terms of torque using a 32t on 107s. It can be done though I would recommend changing the motor sprocket as it’s a more direct swap and also cheap as well as the teeth skipping less on braking
```

---
## \#9 Posted by: Fiori Posted at: 2018-11-17T07:31:33.192Z Reads: 89

```
He wants fast, and that will do it. I agree though, I like 16T
```

---
## \#10 Posted by: Grozniy Posted at: 2018-11-17T07:35:01.757Z Reads: 87

```
Just get 18T or 20T motor pulley and test. it's not that expensive and it's easy to change
```

---
## \#12 Posted by: pat.speed Posted at: 2018-11-17T22:53:33.079Z Reads: 46

```
That will increase his torque but he needs to change gearing to get more speed
```

---
## \#13 Posted by: accrobrandon Posted at: 2018-11-18T00:01:21.180Z Reads: 46

```
[quote="Grozniy, post:10, topic:74968, full:true"]
Just get 18T or 20T motor pulley and test. it’s not that expensive and it’s easy to change
[/quote]

I'm with this guy... I find motor pulleys cheaper than wheels.. 18/36 was my Fav...but the last 2 single drives I started with left me underwhelmed in performance... And went dual with a quickness.. @dickyho has cheap pulleys... Id buy a few for now and future dual and mess with those
```

---
## \#14 Posted by: butt_stallion Posted at: 2018-11-18T00:54:44.601Z Reads: 40

```
I'll look into going up to 80 a on the motors.  I am going to change to a dual build asap, I would really like to use the focbox unity!  For now the pulleys seem like the cheapest option!  I'm thinking of switching to @Ackmaniac  's  firmware cause I think I'd like the wattage control.  Any suggestions for that?  I know there's a lot on his original post and I've been reading a lot about it!

Edit: using the d140 BMS, direct discharge
```

---
