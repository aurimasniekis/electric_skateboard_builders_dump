# Can anyone tell me what’s wrong with my pulley set up?

### Replies: 24 Views: 308

## \#1 Posted by: huntercasillas Posted at: 2019-04-29T17:45:37.671Z Reads: 123

```
Can anyone tell me what’s wrong here?

(Video Removed - problem solved motors just needed to be switched sides)

Is the motor pulley to close to the mount? Are the wheels not lined up correctly? Not sure what it’s hitting against to make this noise.
```

---
## \#2 Posted by: RedBaron Posted at: 2019-04-29T17:49:00.543Z Reads: 119

```
Sounds like a lose motor magnet or a broken sensor causing cogging.
```

---
## \#3 Posted by: huntercasillas Posted at: 2019-04-29T17:57:21.389Z Reads: 106

```
Hmmm, I bought them brand new from @JLabs and I just plugged them in for the first time. Maybe it’s something else?
```

---
## \#4 Posted by: Bobby-gg Posted at: 2019-04-29T18:06:20.560Z Reads: 100

```

 have you tried with the belts removed?
```

---
## \#5 Posted by: huntercasillas Posted at: 2019-04-29T18:12:07.827Z Reads: 92

```
I’ll do that now!
```

---
## \#6 Posted by: huntercasillas Posted at: 2019-04-29T18:17:02.106Z Reads: 90

```
Still the same without the belts
```

---
## \#7 Posted by: huntercasillas Posted at: 2019-04-29T18:23:52.643Z Reads: 85

```
Took it completely off the mounts and held it in my hand and it’s still doing the same thing
```

---
## \#9 Posted by: RedBaron Posted at: 2019-04-29T18:26:59.104Z Reads: 78

```
So its still either a broken hall sensor or a loose magnet. The only other thing i can think of is your settings might not be identical to each other. Can you post pictures of your motor settings?

Also make sure ti check that all connections are making full contact and nothing is loose. But i really think its a bad hall sensor.
```

---
## \#10 Posted by: huntercasillas Posted at: 2019-04-29T18:29:56.994Z Reads: 80

```
Yeah, I just used the unity recommended settings I believe.
```

---
## \#11 Posted by: RedBaron Posted at: 2019-04-29T18:32:17.642Z Reads: 79

```
I see. Open up the motor and check the hall sensors along with the solder job on the pcb holding the sensors. Here's a pic of what it shouldnt look like.

![20190210_131041|375x500](upload://baFDya9ACdPq1q6mdkdOvZ97BOn.jpeg) ![20190210_131124|375x500](upload://cfhZvWEVlUfPqeXbjGTUKkz8ixN.jpeg)
```

---
## \#12 Posted by: RedBaron Posted at: 2019-04-29T18:33:31.965Z Reads: 74

```
And what it should look like.

![20190426_110435|666x500](upload://4McBm9chSl0jMj47JjyEw4Un78f.jpeg)
```

---
## \#13 Posted by: huntercasillas Posted at: 2019-04-29T18:49:52.038Z Reads: 68

```
Here are the motor settings:

![Motor%20Settings|419x500](upload://cI9GovcDWzKvCaVtqVDrhAKfGev.png)
```

---
## \#14 Posted by: dareno Posted at: 2019-04-29T19:00:55.677Z Reads: 66

```
Don't open that motor until you check your warranty.  I would just contact @JLabs and get some feedback.
```

---
## \#15 Posted by: huntercasillas Posted at: 2019-04-29T19:03:05.052Z Reads: 64

```
Yeah, I haven’t touched either of them and don’t plan on opening them.
```

---
## \#16 Posted by: Bobby Posted at: 2019-04-29T19:13:41.006Z Reads: 60

```
Have you tried it with the hall sensors unplugged? Is it in foc or bldc?
```

---
## \#17 Posted by: huntercasillas Posted at: 2019-04-29T19:14:54.057Z Reads: 61

```
Yes, same thing with hall sensors unplugged although I think it’s slightly less severe jerking.
```

---
## \#18 Posted by: dareno Posted at: 2019-04-29T19:20:40.459Z Reads: 60

```
It really sounds mechanical.  Magnet or bearing.  Most likely a loose magnet.  You can check the phase wiring easily without opening it up to see if there is a short in there.
Three wires from the motor are A B and C
Disconnect the motor from the ESC 

Touch A+B together. Verify the motor has choppy brakes
Touch A+C together. Verify the motor has choppy brakes
Touch B+C together. Verify the motor has choppy brakes
Touch A+B+C together. Verify the motor has SMOOTH brakes that are much stronger

All the choppy brakes should feel the same. If one is weaker or stronger or if anything isn’t as described above, it means you might have winding issues.
```

---
## \#19 Posted by: JLabs Posted at: 2019-04-29T19:27:03.406Z Reads: 52

```
Did you try swapping the motor to the other phase leads and see if the same problem occurs? 

I’m not exactly sure what the issue is because it sounds like a loose magnet in the first video, and half a shorter phase wire in the second. Swapping the motors will rule this out. 

No matter the issue, I’ll take care of it in the end.
```

---
## \#20 Posted by: FranciscoV Posted at: 2019-04-29T19:33:39.231Z Reads: 50

```
Have you set up your unity!?   It sounds to me like you need to run motor detection and hit apply button
```

---
## \#21 Posted by: huntercasillas Posted at: 2019-04-29T19:39:48.395Z Reads: 49

```
Yes I already did that
```

---
## \#22 Posted by: FranciscoV Posted at: 2019-04-29T19:42:24.057Z Reads: 47

```
Have in mind.   App doesn’t work all that great most of the time.  Well.  At least not for me.    Sometimes after I press apply updated settings they won’t save and I have to disconnect, reconnect and run motor detection again before I can get it to work 🙂
```

---
## \#23 Posted by: huntercasillas Posted at: 2019-04-29T20:26:21.437Z Reads: 41

```
Swapping the motors worked, thank you!
```

---
## \#24 Posted by: JLabs Posted at: 2019-04-29T21:16:36.402Z Reads: 32

```
Awesome, glad that worked and nothing was up with the motors!
```

---
## \#25 Posted by: huntercasillas Posted at: 2019-04-29T22:33:13.142Z Reads: 21

```
Also! Do you have any 10s 3A chargers for sale? Last I checked it said you were out of stock. Do you know where I could buy one? :)
```

---
