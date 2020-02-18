# Using resistors to lower voltage?

### Replies: 28 Views: 642

## \#1 Posted by: TeslaAlex Posted at: 2018-04-17T12:58:34.374Z Reads: 101

```
Hi guys!

Has anyone here used resistors to lower the voltage of the main battery, to power lights etc? 

Im currently using a step-down module that works great, but I cant use my [hobbyking reciever switch](https://hobbyking.com/en_us/turnigy-receiver-controlled-switch-1.html) since it requires a common ground wire. 

I got some help from @Ishayc with the calculations and I´ll be using two 5W 300ohm resistors in parallell from my main 12s battery. The lights are running on 10-16V and 0.23A. 

Im excited to try this out, but until then it would be nice to see if anyone else has done it. :slight_smile: 

Thanks!

/Alex
```

---
## \#2 Posted by: laurnts Posted at: 2018-04-17T13:44:37.656Z Reads: 87

```
You can buy directly a HK universal SBEC. It can bring around 24v to 5 / 9 / 12 volts with 10A discharge.
```

---
## \#3 Posted by: Skitzor Posted at: 2018-04-17T13:52:50.351Z Reads: 84

```
Yup, go for an SBEC or UBEC. Why? Your resistor solution will work, but will always consume power. Even when nothing is used. Whereas the BECs mentioned will store this energy as efficient as possible (always losses)
```

---
## \#4 Posted by: TeslaAlex Posted at: 2018-04-17T13:58:10.637Z Reads: 79

```
I guess the SBEC will have to be rated at 12s (50,4v)? I thought about going this route at the beginning but I simply bought a stepdown module since it was cheaper. Could you guys link me a cheap SBEC that will work with my 12s battery?
```

---
## \#5 Posted by: Martinsp Posted at: 2018-04-17T14:00:53.855Z Reads: 72

```
The resistor idea is not a good one. Apart from the fact that it will consume your battery power passively, it will be only able to provide 0.168A due to the resistor and all that with significant voltage sag so your lights may not perform as desired.
I unfortunately dont have an SBEC to recommend, sorry :/
```

---
## \#6 Posted by: TeslaAlex Posted at: 2018-04-17T14:02:58.949Z Reads: 63

```
Okay, thanks for the good info. I´ll search around and see if I find a good SBEC :slight_smile:
```

---
## \#7 Posted by: TeslaAlex Posted at: 2018-04-17T14:07:50.147Z Reads: 62

```
What about this [SBEC](https://hobbyking.com/en_us/turnigy-multistar-twin-output-5-10-amp-6-50v-sbec-for-lipoly.html)? It´s on the high end with price, but is rated up to 13s. Would I be able to use my reciever switch with it? :grinning:
```

---
## \#8 Posted by: mmaner Posted at: 2018-04-17T14:11:16.601Z Reads: 59

```
Where does it require a common ground?  If you are using a normal RX you shouldn't have an issue.  THe power connections on the turnigy switch only use the POS and the 3 wire connector connects to the 2nd chanel on the RX.  

![turnigy reciever controlled switch 072417|533x407](upload://abCpzV0Fo834ksyAwyvhQhSzqqv.jpg)
```

---
## \#9 Posted by: TeslaAlex Posted at: 2018-04-17T14:16:04.659Z Reads: 56

```
I tried conneting the switch using that exact diagram, but it did not work. Here is the diagram that came with the reciever switch:

![IMG_1328|666x500](upload://m1L3DgrsFGvWMjJYCMbc9Tr4NUj.jpg)

![IMG_1329|666x500](upload://j9pOPVflLmEb09NVuwnaqIUgn56.jpg)
```

---
## \#10 Posted by: mmaner Posted at: 2018-04-17T14:24:01.625Z Reads: 50

```
Those instructions are for using the switch with a BEC, my diagram is if you are using a step down converter.  Do this...

    1. Connect the POS In the the Step Down Converter
    2. Connect the POS Out to the lights or whatever
    3. Connect the Step Down Converter NEG to the Lights
    4. Connect RX CH2 to the 3 wire plug on the switch
    5. Power up the board and hit the remote switch
```

---
## \#11 Posted by: TeslaAlex Posted at: 2018-04-17T14:26:05.907Z Reads: 51

```
Ok, give me a second to open up the enclosure.
```

---
## \#12 Posted by: Ishayc Posted at: 2018-04-17T14:26:46.210Z Reads: 49

```
My first board is running a 6s pack so I series connected two 12v LED light and it's working beautifully.   
The Idea of the resistor might not be the cleverest or the most sophisticated  but it's the simplest and should work(tried it in a different project).

@Martinsp he can always make a switch before the resistor to stop it's consumption when not used.
```

---
## \#13 Posted by: mmaner Posted at: 2018-04-17T14:28:57.224Z Reads: 51

```
[quote="Ishayc, post:12, topic:52540"]
but it’s the simplest
[/quote]

I disagree, the simplest solution is using tested hardware specifically manufactured to perform a given task, not reinventing the wheel.
```

---
## \#14 Posted by: TeslaAlex Posted at: 2018-04-17T14:30:02.178Z Reads: 49

```
Ok, here is my enclosure:

![IMG_1321|690x325](upload://edCT8DiNHJ5gmzUYjsEkTa6q52d.jpg)
```

---
## \#15 Posted by: Ishayc Posted at: 2018-04-17T14:31:09.551Z Reads: 48

```
Using a resistor to lower a voltage is reinventing the wheel?  Hmm tell that to all the old school engineers I’m working with.
```

---
## \#16 Posted by: mmaner Posted at: 2018-04-17T14:34:13.063Z Reads: 49

```
Anything is reinventing the wheel when have a proven reliable piece of equipment to perform a given task...but build something less reliable to do the same job.

I am an old school engineer.  Keep it simple, reliable and bullet proof.
```

---
## \#17 Posted by: Ishayc Posted at: 2018-04-17T14:39:14.100Z Reads: 47

```
I’m pretty much a new engineer so I’m not in position to argue about that but i’ve used both method to regulate voltages and both worked well. 
Glad we think different, that’s a good way to learn :)
```

---
## \#18 Posted by: mmaner Posted at: 2018-04-17T14:41:57.029Z Reads: 45

```
[quote="Ishayc, post:17, topic:52540"]
Glad we think different, that’s a good way to learn
[/quote]
There's a time for engineering a solution and a time to use a pre-engineered solution...specifically if the pre-engineered solution falls within spec, conforms to cost, voltage & space requirements and is proven to be reliable.  

I'm not saying your wrong, Im just saying that since he has the switch and has the drop down module it doesn't make sense to re-engineer the solution when there is one already available that will be far more reliable than the boy scout method :slight_smile:
```

---
## \#19 Posted by: mmaner Posted at: 2018-04-17T14:44:42.513Z Reads: 44

```
Also...

[quote="Ishayc, post:17, topic:52540"]
I’m pretty much a new engineer so I’m not in position to argue
[/quote]

I'm gonna call BS on that, being a new engineer is the best time to argue.  It gives yous additional perspective, experience without investment, new ideas and either helps to prove or disprove your own theories.  Plus engineering school is fuggin expensive, so arguing is free entertainment :slight_smile: 

And there's this...
![image|410x500](upload://mQFb5H4ley88pTsfvG3aH57tPqf.jpg)
```

---
## \#20 Posted by: TeslaAlex Posted at: 2018-04-17T14:53:28.675Z Reads: 41

```
Does not seem to work, it might be the remote? Im using a nano-x
```

---
## \#21 Posted by: Ishayc Posted at: 2018-04-17T14:54:32.909Z Reads: 41

```
Haha that’s actually true, I do enjoy arguing 😂. 
@TeslaAlex the nano-x’s 2nd channel needs to be activated first.
```

---
## \#22 Posted by: TeslaAlex Posted at: 2018-04-17T14:56:30.114Z Reads: 38

```
How?

10char
```

---
## \#23 Posted by: Ishayc Posted at: 2018-04-17T14:58:05.366Z Reads: 36

```
Not sure how. Saw it somewhere here.
Let me search
```

---
## \#24 Posted by: TeslaAlex Posted at: 2018-04-17T14:58:33.489Z Reads: 35

```
Okay, thanks a lot! This is probably the problem :thinking:
```

---
## \#25 Posted by: Ishayc Posted at: 2018-04-17T15:12:21.532Z Reads: 36

```
No luck finding it. 
Maybe @CarlCollins can help with this.
```

---
## \#26 Posted by: TeslaAlex Posted at: 2018-04-17T16:08:51.730Z Reads: 34

```
Okay, I got the switch to work. But there is a problem.

I push the button on the remote for about 5 seconds, and the the light bar does a quick flash and then powers off. 

What is wrong?
```

---
## \#27 Posted by: TeslaAlex Posted at: 2018-04-17T16:19:00.307Z Reads: 36

```
Ok, no problems guys. I had to remove on of the "loop-pins" on the reciver switch so that it was set to mode 3: **Switch ON**

![IMG_1329|666x500](upload://4Kpc1oWCbUEM7lvZbBzHho353CI.jpg)

Thanks for all the help guys, this community is awesome! :grinning:
```

---
## \#28 Posted by: CarlCollins Posted at: 2018-04-17T20:45:49.340Z Reads: 31

```
I guess I am late, Issue is already resolved :stuck_out_tongue:
```

---
