# Weird noise when accelerating fast

### Replies: 25 Views: 1216

## \#1 Posted by: Ishayc Posted at: 2017-07-10T07:04:27.708Z Reads: 150

```
Hi,

I was cruising my board the other day when I suddenly noticed this weird noise when trying to accelerate. 
It is much more noticeable when climbing hills, even not that stiff.
It sounds like the belt is slipping but i'm not sure.
I tried to tighten the belt, change the belt to a new one and even to a shorter one, tighten the motor and wheel pulley bolts and not luck.
My setup:
50mm single motor, 36\12T 5M 10mm, 6s battery, 150a esc.

Help will be appreciated.

Thanks!
```

---
## \#2 Posted by: Skitzor Posted at: 2017-07-10T07:22:13.491Z Reads: 141

```
I would guess your 6s is dying under load. Your motor is not getting what it's requesting.
```

---
## \#3 Posted by: Ishayc Posted at: 2017-07-10T07:55:15.078Z Reads: 137

```
This noise started yesterday, it was fine for a couple of weeks.
I don't think it's the battery..
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-07-10T08:19:09.026Z Reads: 132

```
Maybe post a video or some photos of your setup, but like @Skitzor said, your setup is a really weak one and uses as much power as it can to bring you up a hill - it may just be too much
```

---
## \#5 Posted by: Ishayc Posted at: 2017-07-10T08:32:23.341Z Reads: 134

```
but if it needs more power then it can deliver then it just wont go fast, or i'm wrong?
It happens on flat terrain too when accelerating fast. if i do it gradually it goes fine even on hills. 
if the hill is too stiff it will climb it but slower. 
i'd be suspicious if that was the issue since day one but it is not the case.
I cant post a video for now because I took it apart and the motor pulley is stuck, but that's a different issue.
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-07-10T08:43:48.075Z Reads: 127

```
when accelerating hard on my 6s with the x-car beast, it "blocks" the power if i demand to much. Seems like a safety feature of the ESC not to overheat.
If you wanna go faster, you need to build bigger ;)
```

---
## \#7 Posted by: Ishayc Posted at: 2017-07-10T08:56:42.454Z Reads: 120

```
but are you getting this weird noise like the belt is slipping? or you just cant get it to accelerate?
sometimes i need to release the throttle and press it again to get it to accelerate fully. but this is the esc i guess(Trackstar 150a genII).
Well I don't want to go faster, I just want to accelerate as I did a few days ago :\
```

---
## \#8 Posted by: TarzanHBK Posted at: 2017-07-10T09:03:14.848Z Reads: 113

```
hmm no, I don´t have weird noises..
Maybe it´s your Trackstar... don´t know about this ESC.
Maybe switch to an other well known ESC like the X-car 150A.
```

---
## \#9 Posted by: Ishayc Posted at: 2017-07-10T09:04:43.217Z Reads: 106

```
It's actually a good esc. The noise comes out from the motor/pulley not from the esc so it's something else. 
Any more ideas?
```

---
## \#10 Posted by: TarzanHBK Posted at: 2017-07-10T09:09:10.421Z Reads: 102

```
I had a 13 tooth motor pulley before and my belt was skipping, so if you´re using a 12 tooth it´s even worse..
can´t help you any further with no pics or a video of the problem..
```

---
## \#11 Posted by: Skitzor Posted at: 2017-07-10T09:11:18.516Z Reads: 97

```
It could be a motor bearing that's not optimal. But from reading the rest in this topic I stand by the fact that it's your motor 'crying' for more juice when you ask it to accelerate faster. It may not have done this at first, but continuously pushing the motor this way could lead to those noises. 

A video would help a lot
```

---
## \#12 Posted by: Ishayc Posted at: 2017-07-10T09:18:34.275Z Reads: 92

```
Well seems too sudden to me. If I'll manage to take the damn motor pulley off without damaging the motor I'll post a video..
```

---
## \#13 Posted by: Ishayc Posted at: 2017-07-10T09:19:52.282Z Reads: 95

```
I have 15t on its way. I wonder if it will solve the issue.the motor does gets hot and the esc is pretty cold which means I'm undergearing but it's not that hot anyway.
```

---
## \#14 Posted by: Ishayc Posted at: 2017-07-11T08:00:19.170Z Reads: 72

```
Ok, so I rewired all the electronics, changed the motor pulley and the wheel pulley. 
the noise keeps coming and i'm almost sure now it's from the motor, It even happens now even when braking strong.
Got 2 different length belts scraped in 30 min of drive.
Maybe the motor is gone or I need to reassemble it? can it be that the shaft is spinning freely when loaded heavily?
```

---
## \#15 Posted by: TarzanHBK Posted at: 2017-07-11T12:57:00.815Z Reads: 67

```
Could be a short inside the motor. Try to spin it by hand - shouldn´t be much resistance. Keep spinning and wiggle a bit on the motor wires - if you feel resistance while wiggeling, thats a short somewhere.
```

---
## \#16 Posted by: Ishayc Posted at: 2017-07-11T13:32:57.303Z Reads: 64

```
I'll check it when i'm back at home.
I hope it's only the motor! then i'll have a good reason to replace it to Tacon 160 :slight_smile:
```

---
## \#17 Posted by: Ishayc Posted at: 2017-07-11T14:09:46.917Z Reads: 58

```
Checked it and no noticeable difference when wiggling the wires. The resistance seems fair enough. If the bullet connectors touch each other the resistance is greater.
```

---
## \#18 Posted by: TarzanHBK Posted at: 2017-07-11T14:17:23.810Z Reads: 53

```
Hmm do you see anything inside the motor?
Should be the motor or the ESC which is causing these problems
```

---
## \#19 Posted by: Ishayc Posted at: 2017-07-11T14:32:28.746Z Reads: 50

```
Nope, can't notice anything abnormal. I'm trying to take the motor apart. let's see how it goes.
```

---
## \#20 Posted by: Jedi Posted at: 2017-07-11T17:29:21.742Z Reads: 48

```
I had the same thing happen. I think you're right about the shaft spinning freely.
```

---
## \#21 Posted by: Hummie Posted at: 2017-07-11T17:45:24.114Z Reads: 46

```
On the Vesc tool u could check the inductance an resistance and compare to what it was in the past.
```

---
## \#22 Posted by: Ishayc Posted at: 2017-07-11T20:57:17.952Z Reads: 48

```
I think that was the problem. 
I took the shaft apart and saw that at the bottom where it is locked with a bolt the shaft is scraped.
Anyway trying to assemble it back didn't go so well so the motor is dead(bearings got broken). 
Probably will order Tacon Bigfoot 160 245kv
```

---
## \#23 Posted by: Ishayc Posted at: 2017-07-11T20:58:07.253Z Reads: 49

```
Got no vesc but esc. But I think I found the problem.
Thanks!
```

---
## \#24 Posted by: Jedi Posted at: 2017-07-11T21:05:35.445Z Reads: 48

```
Bummer, any pics? Sounds like your motor is salvageable. Maybe needs a new shaft. I wish there was a motor wizard on this forum.. someone we could send motors to for repairs. I have 3 motors that are fixable. Is the Bigfoot in stock?
```

---
## \#25 Posted by: Ishayc Posted at: 2017-07-12T03:43:09.484Z Reads: 41

```
I'll post them later when I'm near it. 
Yea it is fixable just need to get my hands on those bearings.
Yup they're back in stock :)
```

---
