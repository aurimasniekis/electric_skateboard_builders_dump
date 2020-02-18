# Wiring, Charging, and a whole lot of newb questions

### Replies: 12 Views: 1129

## \#1 Posted by: Koto Posted at: 2016-12-05T03:35:31.807Z Reads: 129

```
Hi,
I am a newb and I dont have anything close to a mechatronics degree, so I need some help.
Some questions:

- I am getting two 5000mAh  20C 5S battery and a 70A motor. I've done some calculations and im pretty sure my battries are 100 Amp while my motor is 70 amp.
 Firstly- is that going to work 
 secondly- If my Vesc says 12 battery and motor is 10S will their be problems

- what basic wiring setup should i do. i am connecting the batteries in series, and im going to have a switch, do i still need a anti-spark loop plug or is it fine. 

- I have no Idea how charging works, do i need a balance charger, this https://hobbyking.com/en_us/hobbyking-b6-ac-dc-compact-lipo-nimh-50w-charger-eu-plug.html, or both
EDIT: because i have two batteries, is their a way to charge both. I know their is a parallel charging board but is their any other way

- 5000mAh 5S batteries are really expensive, what is it okay to go down to?

Thanks
Oscar
_xxXXKOTOXXxx_
```

---
## \#2 Posted by: ewalks6 Posted at: 2016-12-06T02:11:04.964Z Reads: 87

```
I would just suggest reading thru some LiPo builds. 10S is the optimal cell amount for VESCs, so I would stick with it. To be honest, unless your making a budget build, these batteries aren't too expensive. Look at some Li-ion packs to compare to... those are upwards of $200.
```

---
## \#3 Posted by: Koto Posted at: 2016-12-06T02:15:58.190Z Reads: 81

```
[quote="ewalks6, post:2, topic:14194"]
10S is the optimal cell amount for VESCs,
[/quote]

but my erpm goes over 60000 so i need to cut down on either battery or motor
```

---
## \#4 Posted by: mason Posted at: 2016-12-06T02:20:07.387Z Reads: 79

```
[quote="Koto, post:1, topic:14194"]
Firstly- is that going to work
[/quote]

yes[quote="Koto, post:1, topic:14194"]
will their be problems
[/quote]

no[quote="Koto, post:1, topic:14194"]
do i still need a anti-spark loop plug
[/quote]

no[quote="Koto, post:1, topic:14194"]
I have no Idea how charging works
[/quote]

learn
```

---
## \#5 Posted by: Koto Posted at: 2016-12-06T02:27:54.185Z Reads: 70

```
love your channel
```

---
## \#6 Posted by: ewalks6 Posted at: 2016-12-06T12:24:43.187Z Reads: 63

```
Yes, 10S is the optimal amount for a VESC. And if you do 10S the max motor is 200kV, so go under that. Again, there are a lot of threads that would answer your questions so just read a lot.
```

---
## \#7 Posted by: guillaume772 Posted at: 2016-12-06T14:27:04.465Z Reads: 61

```
Hi, I'm also new to building an electric skateboard, and I bought everything for it... except I forgot a charger for my battery. I have a 4000mah 5s 20-50c lipo pack, does anyone know what charger I should buy?

This is the link to my battery in case I'm not clear enough: https://hobbyking.com/en_us/turnigy-nano-tech-4000mah-5s-25-50c-lipo-pack.html 

Thanks,
Guillaume
```

---
## \#8 Posted by: mason Posted at: 2016-12-07T20:00:32.727Z Reads: 53

```
thanks man!
```

---
## \#9 Posted by: Hummie Posted at: 2016-12-07T20:37:00.621Z Reads: 50

```
12s is optimal for vesc

you can charge those batteries in parallel

battery the c rating tells what you can with little voltage sag and damage to cells and the motor amp limit is made out of thin air based on pixie dust.  just dont get the motor too hot
```

---
## \#10 Posted by: ewalks6 Posted at: 2016-12-07T21:51:42.898Z Reads: 45

```
I could've sworn I saw that... I though that was why some people use ESC for 12S...?
```

---
## \#11 Posted by: ewalks6 Posted at: 2016-12-07T21:55:00.439Z Reads: 44

```
[quote="onloop, post:4, topic:1833"]
VESC designer has said that optimum RPM for these type of brushless outrunners is 8600RPM.

That why i built my system with 10S & 190KV motors.
[/quote]

Is this not right?...
```

---
## \#12 Posted by: Hummie Posted at: 2016-12-07T22:41:34.372Z Reads: 37

```
The limit is both the erpm and voltage limit on components. Stay under both and good. With lower kv motor it's lower erpm so ur free to go higher voltage, but the components' limit is said to be no more than 12s
```

---
