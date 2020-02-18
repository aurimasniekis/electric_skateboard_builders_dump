# Raptor 2 increasing max current settings

### Replies: 11 Views: 1625

## \#1 Posted by: Eboosted Posted at: 2018-01-25T04:44:39.395Z Reads: 226

```
I wonder if the FocBoxes on the Raptor 2 have a different version of @ackmaniac firmware.

I was able to increase battery max from 30A to 40A, board feels better but I'd like more torque, on all my boards I ran between 80A and 100A with no issues at all and I'm quite happy with the performance, however I wasn't able to increase the motor max from 80A to 90A using Vesc Monitor App, it just topped at 80A.

[img]https://i.imgur.com/rdJXJDe.png[/img]

Is there any built in feature that is preventing to change that parameter for safety reasons?
```

---
## \#2 Posted by: SeanHacker Posted at: 2018-01-25T05:53:33.865Z Reads: 203

```
Pretty sure its custom firmware made specifically for the R2. So that could definitely be why the limitation. 

I'm guessing for warranty purposes, if we flash something else we would be out of luck. Unless Enertion provides this firmware somewhere I don't know about.
```

---
## \#3 Posted by: Eboosted Posted at: 2018-01-25T06:16:55.077Z Reads: 196

```
@ackmaniac did you wrote a specific FW for the Raptor 2?
```

---
## \#4 Posted by: ninja Posted at: 2018-01-25T10:32:43.173Z Reads: 176

```
[quote="Eboosted, post:1, topic:44608"]
on all my boards I ran between 80A and 100A with no issues at all and I’m quite happy with the performance
[/quote]

So you run even higher amps than motor max is allowed for those motors? I mean, for an example, sk3 is rated to 70A, but you using 80-100A for those motors with no problem!!? 

Thing is that I have sk3 and now I'm running 70A like it is rated for those motors, but I wanted to feel more power, just afraid to go beyond rated mot max. How do you think, it will not cause problems if I rise amps like to 80 or 90 since max rated amps is 70?
```

---
## \#5 Posted by: egzplicit Posted at: 2018-01-25T12:55:16.057Z Reads: 166

```
U won’t have any issues. It’s peak anyway and it will get to 80-90 only when starting from a stand still or going up a hill. I used to have Racerstars 5065 rated at 42A and pushed 60A and even 80A motor max with no issues at all.
```

---
## \#6 Posted by: egzplicit Posted at: 2018-01-25T12:59:03.513Z Reads: 161

```
[quote="Eboosted, post:1, topic:44608"]
I was able to increase battery max from 30A to 40A, board feels better
[/quote]

How much better? I have a 10s4p 30Q with bat max set at 30A and wondered how much more torque you get if you push it to 40A/vesc. 30Q cells are happy at 20A discharge continuous so 40A bat max that you only reach for a few seconds shouldn’t cause too much stress on the cells... but I wonder what the impact is on torque / acceleration.
```

---
## \#7 Posted by: Surfer Posted at: 2018-01-25T13:01:49.728Z Reads: 156

```
Yes, it is specific firmware 0.80 version if i'm not wrong, made it to work with enertion vesc-tool. Remember if you change firmware warranty will be void. In another hand, you are a jonkytorquey man!!! Mucho power from the R2!!
Edit: I have this firmware if you want it @SeanHacker
```

---
## \#8 Posted by: Eboosted Posted at: 2018-01-25T15:32:47.859Z Reads: 145

```
The 30Q have been tested my mooch to hold 20A of discharge each so 80A for a 4P setup is pretty spot on, no stress on the batteries
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2018-01-25T15:58:34.023Z Reads: 141

```
80a divide by 2 motor is 40a 😉

Edit: and event at 40a I’ve screw a few battery pack because of over discharging, so 30a is the safe way
```

---
## \#10 Posted by: Eboosted Posted at: 2018-01-25T18:31:58.624Z Reads: 127

```
So the ESC failsafe didn't activate when discharging? How you went low enough to screw them?
```

---
## \#11 Posted by: Surfer Posted at: 2018-01-25T19:06:53.935Z Reads: 119

```
I have 10s4p 30q's for a year, asking them 80a in vesc's settings and I can see they aging quite fast, still good range, but acceleration wise is noticeable lower than my R2 pack in the same config. It will be nice to have a temp sensor on the batteries, just to know how much stress we put on them, looking forward for the new 2170 40T!!
```

---
