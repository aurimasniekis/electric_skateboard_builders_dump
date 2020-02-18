# Help please - my board has a speed restriction!

### Replies: 19 Views: 1207

## \#1 Posted by: gbutcher Posted at: 2018-02-10T08:10:32.321Z Reads: 204

```
Hi,

This is my first build and I am new to VESC so looking for  some help please.  I just cannot get the expected power / speed out of my setup.  I have a dual motor, TB 6355 190Kv, 36 tooth / 13 tooth with 83mm wheels running 12S lipo,(2 * 6S 3300 mAh packs in series, 60C).  With this setup I cannot get more than 20km/ hr out of the board.  When i go up hill, there is enough power to maintain the 20 km / hr but as soon as I level out on max throttle the power reduces and I stay at 20 km / hr.  When going down hill I can max throttle but I draw almost no amps and I cannot get more speed.  

I would greatly appreciate any help thanks.

Logs and settings below.

![image|690x311](upload://uRB5rViuLTdYbCdhTSbCm65nrjD.jpg) 

![image|690x353](upload://9C3ofKiGUi52zL9qtIteTS7cj1h.png)

![image|690x356](upload://gHb4WCk3XUYLOTNNbdwiwLiTJNs.png)

![image|690x354](upload://6h4jpXVVnJNTuWwIbpYwHrlx2VE.png)

![image|690x355](upload://2WoxdYeRL1YhuMp4NB1OL1zFr6D.png)


Many thanks.
```

---
## \#2 Posted by: scepterr Posted at: 2018-02-10T08:15:19.468Z Reads: 180

```
You have soft erpm limit turned on in the ppm tab, turn it off
```

---
## \#3 Posted by: pat.speed Posted at: 2018-02-10T09:29:58.057Z Reads: 165

```
Yeah his erpm looks to be set at 15k
```

---
## \#4 Posted by: banjaxxed Posted at: 2018-02-10T10:00:21.226Z Reads: 159

```
And that is how you present your shout for help nice one
```

---
## \#5 Posted by: gbutcher Posted at: 2018-02-10T10:37:28.084Z Reads: 149

```
Ahh so the setting that says to limit my RPM actually limits my RPM ....  :)  Who would have thought ha ha

Thanks heaps for the help guys.
```

---
## \#6 Posted by: ARetardedPillow Posted at: 2018-02-10T10:55:16.751Z Reads: 144

```
"Pls help my board isnt going fest fest"
```

---
## \#7 Posted by: krloz Posted at: 2018-02-10T13:28:09.670Z Reads: 128

```
 This is a  awesome example on how to ask for help. Not a single "post your..." "upload some..." or "what is your..?".

Linking to this thread on the future when people post topics made up of a single question.
```

---
## \#8 Posted by: E1Allen Posted at: 2018-02-10T17:46:16.339Z Reads: 111

```
He also has limit ERPM with negative torque checked. Should probably uncheck that on both esc
```

---
## \#9 Posted by: Eboosted Posted at: 2018-02-11T06:09:56.252Z Reads: 99

```
I agree 100% with you, everything exposed on the first post
```

---
## \#10 Posted by: gbutcher Posted at: 2018-02-11T11:41:23.031Z Reads: 91

```
Turned soft erpm off and tried on the bench.  Crazy fast.  Decided to simply increase the ERPM limit start and ERPM limit end to give me a max speed of 35km/hr.  Went for a ride and it worked great. 

BUT

Then I did a hard brake and it looks like I may have fried a VESC.  One VESC / motor is not responding, flashing red indicating an error with a DRV8302 error whenever I apply throttle.

Could any of my settings have caused this?  I did not yet uncheck "limit ERPM with negative torque" as suggested.  Could this have fried my VESC on a hard brake?  Any other suggestions?

Anyone in AUS who can fix a VESC?

Thanks.
```

---
## \#11 Posted by: SOICDIP Posted at: 2018-02-11T11:44:46.792Z Reads: 87

```
[quote="gbutcher, post:10, topic:46018"]
Crazy fast.  Decided to simply increase the ERPM limit start and ERPM limit end to give me a max speed of 35km/hr.  Went for a ride and it worked great.

BUT

Then I did a hard brake and it looks like I may have fried a VESC.
[/quote]

![image|603x315](upload://iGBa3QQnZHudd7TqxiOHDtR1wyy.jpg)

:(

The DRV probably was fried when the voltage spiked as you braked hard.
```

---
## \#12 Posted by: Eboosted Posted at: 2018-02-11T14:48:19.081Z Reads: 84

```
Can you post a screen shot of the advanced tab?

I want to check your current ramp up
```

---
## \#13 Posted by: banjaxxed Posted at: 2018-02-11T16:07:01.870Z Reads: 82

```
12s with 190kv, eprm is getting close to limits of a vesc, what make is it?
```

---
## \#14 Posted by: krloz Posted at: 2018-02-11T17:54:25.303Z Reads: 74

```
Actually 67k erpm if I'm not mistaken
```

---
## \#15 Posted by: gbutcher Posted at: 2018-02-12T10:22:44.741Z Reads: 61

```
Thanks for the help guys.

@Eboosted  @banjaxxed 
 
I realize I'm over the 60k ERPM but my logic was by setting the start limit and end limit in the soft ERPM I was avoiding high ERPM so it would not be an issue.  This assumption may be wrong?  Especially seeing as how the issue seemed to occur on a hard brake.

Advanced tab below and updated settings which gave me a good amount of power.

I got the VESC from esk8hubs.  Their site seems to be gone so not sure what is happening there.

I have ordered a replacement chip and the electronics guys at work think it is fairly straight forward to replace.  Worth a try. for sure. 

Cheers.

![image|690x355](upload://5pmu0BpV7qRlvRgkyeZxuRVc4HQ.png)

![image|690x354](upload://23Rdkqm88BRgp4e3zBcFg2MmQ14.png)
```

---
## \#16 Posted by: E1Allen Posted at: 2018-02-12T17:23:24.999Z Reads: 54

```
[quote="gbutcher, post:10, topic:46018"]
Could any of my settings have caused this?  I did not yet uncheck “limit ERPM with negative torque” as suggested.
[/quote]


When this block is checked your skateboard will apply brakes to stop it from exceeding the ERPM limits.  That's not ideal because you're probably traveling fast at this point.
```

---
## \#17 Posted by: Eboosted Posted at: 2018-02-13T00:44:53.368Z Reads: 45

```
Get a FocBox, you will be on the endless repair loop.

The FocBox has a safety feature that cuts current avoiding it from frying when something goes wrong.
```

---
## \#18 Posted by: SOICDIP Posted at: 2018-02-13T01:28:16.092Z Reads: 40

```
[quote="Eboosted, post:17, topic:46018"]
The FocBox has a safety feature that cuts current avoiding it from frying when something goes wrong.
[/quote]


I don't think so. The FOCBOX simply has higher rated components that reduce the chance of damage. Same software and similar hardware to the original VESC 4.12.
```

---
## \#19 Posted by: Eboosted Posted at: 2018-02-13T02:28:52.913Z Reads: 38

```
All my focboxes are still working, there's only one with a burned c49.
```

---
