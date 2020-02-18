# Can you hook up dual motors to a single motor esc?

### Replies: 24 Views: 6819

## \#1 Posted by: claudiofiore88 Posted at: 2015-08-30T05:44:43.689Z Reads: 350

```
Can you hook up dual motors to a single motor esc? I have a 200 amp 8s esc and am curious if splitting the motor wires between 2 motors would even be possible. What are you thoughts? Has anyone ever tried this? Would it just damage the esc and/or motors?
```

---
## \#2 Posted by: lowGuido Posted at: 2015-08-30T05:50:15.535Z Reads: 349

```
short answer: No.

answer must be at least 20 characters LOL
```

---
## \#3 Posted by: cmatson Posted at: 2015-08-30T14:51:25.498Z Reads: 343

```
ya, it wouldn't be good... you'd probably destroy both motors and esc in the progress...
```

---
## \#4 Posted by: longhairedboy Posted at: 2015-08-31T19:40:34.630Z Reads: 337

```
Once the magic smoke gets out, its really difficult to get it back in.
```

---
## \#5 Posted by: claudiofiore88 Posted at: 2015-09-03T22:30:37.192Z Reads: 316

```
Oh, ok. I figured you couldn't.
```

---
## \#6 Posted by: torqueboards Posted at: 2015-09-04T02:07:50.744Z Reads: 313

```
You could use a Y connector and it would work as it would give it voltage.

However, you wouldn't want to use it as no ESC is rated for it plus for the same price you might as well just buy another ESC.

Since we stand on it. One motor = one esc unless it's an ESC which is specifically designed for two motors.
```

---
## \#7 Posted by: longhairedboy Posted at: 2015-09-04T12:09:16.418Z Reads: 288

```
Do they even make such a beast? Wouldn't phase timing be an issue?
```

---
## \#8 Posted by: torqueboards Posted at: 2015-09-04T14:55:07.617Z Reads: 285

```
They don't make one. Usually, it's singles and you join them together. The only reason why people might suggest there is a dual esc is because of Flier ESC and their dual esc but it's pretty much just two singles with the ESC Signal Wire connected together.
```

---
## \#9 Posted by: longhairedboy Posted at: 2015-09-04T15:02:43.223Z Reads: 275

```
Every dual ESC I've ever had my hands on was definitely just two singles soldered together at the edge with jumper wires and a single heat spreader joining them together. In fact i've recently formed the opinion that two singles might just be the best most flexible option. It definitely provides a clear upgrade path when starting out as well as the opportunity (when using them in a dual setup) to create two boards from one by simply buying another battery and receiver. Not to mention when a dual burns out, both ESCs are now bad. I have two dual ESCs in boxes now that have allowed their magic smoke to escape and i'm willing to bet only one side of each of them has an issue.
```

---
## \#10 Posted by: lowGuido Posted at: 2015-09-05T00:44:26.719Z Reads: 263

```
im pretty sure if you tried the Y motor option ( Y is this even an option?) you would come into all sorts of differential problems (omg I said differential. don't kill me) 
because the wheels are almost always going different speeds the single ESC would not be able to do the different phase timing for each motor and as a result something will die.
```

---
## \#11 Posted by: mostwanted Posted at: 2016-02-17T09:26:01.417Z Reads: 234

```
i never tried it before . mine is 2 escs + 2 bldc motors . my set up are 80% ready . so i need not figure  so much to build it .  


but some expert youtubers showed positive results .
theres so many videos about 1 esc powering 2 motors .
this is one of them 

at the end of the video , the person says "...provided the load is not greater than the esc capability ...."

i'd say , good luck !

longhairedboy is hilarious ! magic smoke ! ! ! so funny .
  too bad singapore has strict rules abt weed . damn !


https://youtu.be/zeYAWqt2rIE
```

---
## \#12 Posted by: trbt555 Posted at: 2016-02-17T09:57:41.726Z Reads: 209

```
It obviously works for situations where your motors can rotate with the exact same speed. Propellers and such.
But once the speed between both motors is different, phases will get out of sync.
I wonder if on an eboard the speed differential would be great enough to cause problems though.
```

---
## \#13 Posted by: Kaly Posted at: 2016-02-17T12:59:18.970Z Reads: 202

```
For eBoard this is not possible because the motor will be spinning in oposite direction unless you put the motors on the same side of the board front and back, in short just not practical.
```

---
## \#14 Posted by: trbt555 Posted at: 2016-02-17T13:12:21.838Z Reads: 196

```
Just switch two phase wires.
```

---
## \#15 Posted by: barajabali Posted at: 2016-02-17T14:15:07.777Z Reads: 194

```
Maybe if you decided to run brushed motors somehow you could run them off one esc lol
```

---
## \#16 Posted by: mostwanted Posted at: 2016-02-17T16:18:03.491Z Reads: 189

```
i'm a smoker . indonesian clove KRETEK cigarettes .

when you mentioned the word "MAGIC SMOKE" , i was actually inhaling some , due to the hilarious term that you used , i was coughing til i cried . lols . so funny . MAGIC SMOKE ! !! ! !
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-02-17T20:40:27.941Z Reads: 183

```
its true though. if you let out the magic smoke, terrible juju happens. 

Don't think there's actual science in electronics. Its all sorcery and witchcraft.
```

---
## \#19 Posted by: JTAG Posted at: 2016-05-20T07:29:51.189Z Reads: 224

```
If the the axles can move independent; no, then both motors need unique field control.
```

---
## \#20 Posted by: aimthiazz Posted at: 2016-05-20T07:33:19.402Z Reads: 215

```
Both motors will be moving in the same direction. There won't be any speed change between motors. Both Motors will have the same RPM. If so is it possible? TIA :slight_smile:
```

---
## \#21 Posted by: JTAG Posted at: 2016-05-20T07:39:22.629Z Reads: 209

```
Axles need to be coupled and the commutation angle + motor direction should be equal ofcourse. Then and only then you have a high chance that it's going to work. It would be way easier to just buy a bigger motor :tuck_out_tongue: .
```

---
## \#22 Posted by: WeeChumlee Posted at: 2016-05-20T11:16:17.330Z Reads: 177

```
Simple answer is "NO"
You need an ESC per motor for your Eboard I am afraid.
```

---
## \#18 Posted by: aimthiazz Posted at: 2016-05-20T14:24:32.932Z Reads: 158

```
I have two identical motors. can I drive them (Sensorless Mode) using single VESC?
```

---
## \#23 Posted by: jacobbloy Posted at: 2016-05-21T07:16:04.810Z Reads: 124

```
You would be surprised how many times I get asked this on my website
```

---
## \#24 Posted by: aimthiazz Posted at: 2016-05-26T12:10:49.647Z Reads: 111

```
okay, thanks :) I didn't consider commutation will change since BEMF from both the motors won't be equal wrt to time.
```

---
