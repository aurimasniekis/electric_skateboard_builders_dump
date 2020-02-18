# 118kv Trampa become hot

### Replies: 12 Views: 680

## \#1 Posted by: Necromenz Posted at: 2018-05-15T17:35:48.767Z Reads: 173

```
Hi everyone,

My Dual Trampa 118kv Vesc6 Setup become over 70^C after 30min.
I use the metr App for Tracking.

Here my stats

![Screenshot_20180513-142203_metr|243x500](upload://8ZkocYvAHMAfeVbtAIYiR9ouAzc.jpg)

In my oppinion is that Not to hard.

Here my last ride

[https://metr.at/r/Cvydr](https://metr.at/r/Cvydr)

Thanks for help!
```

---
## \#2 Posted by: xclr8r Posted at: 2018-05-16T21:05:41.853Z Reads: 128

```
Maybe @trampa can offer some advice. I am running a 136kv motor and it gets pretty warm as well.
```

---
## \#3 Posted by: Pedrodemio Posted at: 2018-05-16T21:50:05.776Z Reads: 118

```
Did you setup the board or it come ready from them? if the former you probably have to configure the beta factor of the NTC sensor in the motor to have an accurate reading
```

---
## \#4 Posted by: Necromenz Posted at: 2018-05-17T06:13:11.266Z Reads: 98

```
Hi
Thx for your answers.
I bought a lot of Parts at Trampa but i Setup the Board complet by my Self.
How i have to configurate the beta factor of the NTC?
```

---
## \#5 Posted by: trampa Posted at: 2018-05-17T07:52:50.970Z Reads: 85

```
[quote="Pedrodemio, post:3, topic:55560"]
g
[/quote]

How many Amps do you push? 45A is about right. Do you use motor filters?

Frank
```

---
## \#6 Posted by: Necromenz Posted at: 2018-05-17T14:51:04.944Z Reads: 58

```
My stats

Motor max 40A
Brake -30
Battery max 40A

I Cover my Motors like yours.

![20180517_130204 1|409x500](upload://9XDPuzTxMuo8zcQv3ExBBxC5Q5C.jpg)
```

---
## \#7 Posted by: trampa Posted at: 2018-05-17T14:54:27.003Z Reads: 57

```
Try it without covers or a wider mesh. Airflow is what you want! Can't understand why some manufacturers decide to design their motors fully closed. 
Is your Belt very tight? Wheel nut to tight? Twin drive?

Frank
```

---
## \#8 Posted by: Necromenz Posted at: 2018-05-17T15:07:50.102Z Reads: 58

```
It is a twin Drive.

I will try all your proposals and give you a feedback.
```

---
## \#9 Posted by: rich Posted at: 2018-05-17T21:09:06.972Z Reads: 55

```
[quote="Necromenz, post:1, topic:55560"]
My Dual Trampa 118kv Vesc6 Setup become over 70^C after 30min.
[/quote]

When you touch the motors do they feel as 70 degrees? How long can you touch them?
Also are you hill climbing or is it on flat ground?

As @trampa  mentioned your mesh could be the problem, do you use the same mesh at the end of the cans? The holes are very tiny so there is not much airflow, if the mesh has an overlap it's even worse.

This is how my mesh looked like compared to yours, you can see through it.

![nc1|690x345](upload://t8Iwt2msX05lnzFvcFZZN5kssPs.jpg)

![nc2|690x345](upload://4XNZdzoZ477JwYNdS6GleieMjKU.jpg)

It's black painted mesh of a frying pan splash guard like Frank used in his thread. I highly recommend to use a vacuum cleaner after cutting like advised, I didn't and had parts sticking in my sole of foot, what a pain :rofl:
```

---
## \#10 Posted by: Necromenz Posted at: 2018-05-18T04:54:34.257Z Reads: 47

```
Thanks man!

I will Test it without the mesh.
[quote="rich, post:9, topic:55560"] 
When you touch the motors do they feel as 70 degrees? How long can you touch them?
Also are you hill climbing or is it on flat ground?

Also are you hill climbing or is it on flat ground?
[/quote]

The Motors dosent feel like 70 degree,i would say 45-50 degree. I can Touch the motors the whole Time without any problems.
90% of my Tracks are flat ground.
```

---
## \#11 Posted by: bevilacqua Posted at: 2018-05-18T05:47:53.423Z Reads: 44

```
then do what @Pedrodemio said ;)
```

---
## \#12 Posted by: trampa Posted at: 2018-05-18T07:36:49.708Z Reads: 36

```
You have to touch the front shield to feel the heat, not the motor can.

Frank
```

---
