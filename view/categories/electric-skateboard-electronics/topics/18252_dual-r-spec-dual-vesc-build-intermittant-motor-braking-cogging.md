# Dual R-Spec, Dual vesc build, intermittant motor braking/cogging

### Replies: 11 Views: 848

## \#1 Posted by: Jebe Posted at: 2017-02-26T04:13:43.832Z Reads: 108

```
HI All.
After about 300km's on my dual vanguard build I've started having issues where a motor is braking/cogging mid flight.
Board was performing beautifully, minimum cogging from a standstill, smooth acceleration and strong consistant braking.
Was going so well I was going to sell two of my boards.
I'm having some trouble with a build.
Running 2 R-Specs and vescs via Can bus with a GT2B on a vanguard.
 All connections were hotglued in place. 
Was performing brilliantly, top speed 43km ( more left but thats fast enough for me ) great accelleration and range.
I had about 300km's on it when I started having one motor brake while riding. This was only happening intermittantly and I was far from home. I noticed my GT2B was nearly flat so I put it down to this.
Got home and charged the board and the remote.
Next day we set off again( My fiance on the evolve GT because my DIY was kicking it's ass ).
Got around 1km away and had the braking issue again.
I thought this was a mechanical issue and tightened a belt as it was alot looser than the other one.
Not long after this the board stopped altogether.
On the master Vesc, it looks like C44 has blown. 
Once back at home I tried to connect the BLDC tool but neither vesc would power up. Interestingly the GT2B reciever does power up. No lights on the vesc .
I found this on the forum 
http://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600
and tested as per the instructions. 
Is this an accurate test? Does not look like I have a short across C25.
I then pulled apart the motors and heat shrinked them as per [this thread here](http://www.electric-skateboard.builders/t/r-spec-shorted-phase-wire-problem-solution/6474)
Found phase wires touching the frame, thought great - found it ! Love that search feature! Heat shrinked and cable tied in a way to hold the phase wires away from the framework.

Using 2 spare vescs I had for [rudolph](http://www.electric-skateboard.builders/t/rudolph-arbor-axis-gullwing-evolve-sidewinders-ollin-200kv-dual-motors-vescs-10s4p/11400) I connected it all back up again, motor detection good plugged it all in and.................
 still having this issue.. :rage:

Measuring the phase wires with the motor apart and was reading between 12 to 14 ohms.between each phase and both motors. Meter is a fluke process meter.

I think my next step will be to run one motor at a time and see if I can isolate it to one motor. Don't think it is a vesc issue as it was happening with a completely different set of vescs.

Don't have any 55 motor's spare
@torqueboards Any progress with the 220mm caliber hangers?
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-02-26T04:25:11.322Z Reads: 91

```
If you try to turn your motor by hand do you feel some kind of resistance ?

Edit: you got me with Rudolf, I was wondering who it was, then I saw the board :sweat_smile:
```

---
## \#3 Posted by: Jebe Posted at: 2017-02-26T04:30:15.709Z Reads: 88

```
no more resistance than before - It rides well, until one motor brakes.
Hit 33km/hr on a test run, thought the problem was fixed, then 2 minutes later, it cogged again. Only momentary.
```

---
## \#4 Posted by: torqueboards Posted at: 2017-02-26T04:31:39.919Z Reads: 87

```
@Jebe -- almost.. not yet..
```

---
## \#5 Posted by: Jebe Posted at: 2017-02-27T22:14:01.542Z Reads: 58

```
Looks like one motor - removed it and am going to check all the heat shrink again.
```

---
## \#6 Posted by: Jebe Posted at: 2017-03-01T09:43:08.937Z Reads: 55

```
Think I've found it - 2k run and no issue.
Much harder to regain confidence after it's been lost though, I was too scared to go above 20k/hr
Looks like a bad solder joint between the silicon cable and motor windings.
The motor windings are really short - not much room to play with.
Hopefullyu will have more of a chance to ride again this weekend and give it a good test.
```

---
## \#7 Posted by: Jebe Posted at: 2017-03-03T08:57:23.166Z Reads: 47

```
Dead again.
looks like I've blown 2 more enertion vesc's. Well one vesc and one vesc x.
was braking slowly then board went dead.
Am sick of this. thats nearly $800 aud in dead enertion vescs and all the troubles with the motor and the nano x
:rage:
```

---
## \#8 Posted by: Dedbny Posted at: 2017-03-03T20:06:48.650Z Reads: 44

```
What have Enertion support said?
```

---
## \#9 Posted by: Jebe Posted at: 2017-03-03T21:32:22.783Z Reads: 41

```
Still waiting for a response. Sent a follow up email yesterday. Don't think I'll be needing that motor bud. I've run out of vescs.
```

---
## \#10 Posted by: Dedbny Posted at: 2017-03-04T00:56:21.958Z Reads: 36

```
Read between the lines of your previous post that and te fact you didnt respond that you changed your mind. I gave up as well ofter failed vescs. Seems to be the weak link in these things. As for the motors there are known issues with the wiring close to the end of the motors as they come out. Some tend not to be wound up tight enough and come loose. A few previous posts on them. My motors fine. It was just the vescs.
```

---
## \#11 Posted by: Jebe Posted at: 2017-03-04T02:12:10.072Z Reads: 32

```
Yeah thats what I found with my motors - suprised how the motor windings finish inside the motor and don't have more length.
```

---
