# Board no longer responds

### Replies: 18 Views: 231

## \#1 Posted by: Pafrican Posted at: 2018-09-23T04:27:58.557Z Reads: 98

```
I recently assembled my board, here are the specs:
VESC from diyelectricskateboard
Turnigy 6364 245kv BLDC motor
(x2) Turnigy 5s 5000mAh lipo batteries connected in series
FS-GT2B 2.5GHz transmitter and receiver

I used the new VESC tool to set up my board.. the Motor Setup Wizard and Input Setup Wizard (in FOC mode) worked like a charm.

I rode my board for a few days with no issues until today... the motor wouldn't spin when I throttle. Disconnecting and reconnecting the batteries didn't help. I double checked all connections and everything seems solid. The VESC and receiver are properly powered so it seems like the problem lies between the VESC and the motor.

I reconnected to the VESC tool and checked my input setup; the receiver and transmitter were working properly. Next I went into the Motor Setup Wizard and tried to redo the motor detection.. that's when I started noticing problems. 

When I click on RL detection I can see the VESC LED's blinking but nothing happens. The program either records insanely high values or it'll give me an error. When I do the Lambda detection the motor does not spin and outputs a failure error.
(None of this had happened the first time I set-up the motor a few days prior.)

Did I fry something on the VESC that communicates with the motor? Maybe the motor itself went bad? 
The problem occurred when I applied some throttle to the board while it was laying on its back, so there was no load on the motor. 

Please help. I'm not sure if this is a programming issue or a hardware issue.

Thanks!
```

---
## \#2 Posted by: threebysix Posted at: 2018-09-23T04:31:42.201Z Reads: 88

```
TB Vescs aren't really meant to be run in FOC mode. If you use the search function you would find posts talking about TB 4.12 vesc not working in FOC.  Weird things can happen to it like sudden death syndrome. Try BLDC mode and see if it still works.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-09-23T06:36:37.157Z Reads: 75

```
Open your vesc tool, switch on everything.
Than read out faults unter „Terminal-print faults“
Post a picture of the faults, than we can maybe say what it is
```

---
## \#4 Posted by: Komamtb Posted at: 2018-09-23T07:11:10.458Z Reads: 69

```
This will not help, but I had nothing but trouble regarding TB vesc, and the support in my case wasn't great either, I had some similar issues, ended up with them blowing dvrs.
```

---
## \#5 Posted by: Pafrican Posted at: 2018-09-23T14:28:29.235Z Reads: 57

```
What is the DVR responsible for on a VESC?
```

---
## \#6 Posted by: mmaner Posted at: 2018-09-23T15:01:10.418Z Reads: 54

```
[quote="threebysix, post:2, topic:68922"]
TB Vescs aren’t really meant to be run in FOC mode. If you use the search function you would find posts talking about TB 4.12 vesc not working in FOC.
[/quote]

You will also find plenty if posts where they do work in FOC mode. That is a myth your spreading. I've got 2 single motor builds using TB VESC's running I'm FOC, there are litterally hundreds.
```

---
## \#7 Posted by: mishrasubhransu Posted at: 2018-09-23T15:04:54.257Z Reads: 50

```
I am running foc too on TB vesc
```

---
## \#8 Posted by: Andy87 Posted at: 2018-09-23T15:09:14.559Z Reads: 49

```
If you ask because you have a drv error than 😬
You will need to replace it. It’s sure not only a sw fault
```

---
## \#9 Posted by: Pafrican Posted at: 2018-09-23T18:33:17.589Z Reads: 43

```
Is it possible for the VESC to break when throttling with no load? Can the rush of current fry a chipset? 
If so, these things are way more delicate than I thought.
```

---
## \#10 Posted by: Pafrican Posted at: 2018-09-23T18:35:43.870Z Reads: 44

```
I'm asking cause @Komamtb above said he's blown the DVR's on his TB ESC's
```

---
## \#11 Posted by: Andy87 Posted at: 2018-09-23T18:41:23.110Z Reads: 43

```
Yes you can fry your drv with a Full charged 12s battery and a motor with kV over 190.
It’s even more likely as you will hit the max erpm limit more easy without load than with load.
```

---
## \#12 Posted by: dareno Posted at: 2018-09-24T23:06:49.700Z Reads: 30

```
that set up will spin up over the erpm limit on the bench.
```

---
## \#13 Posted by: Komamtb Posted at: 2018-09-25T12:38:05.114Z Reads: 27

```
Well my story is a bit different, my drvs blew while programing the VESCs. Short story - everything worked, I wanted to change the settings, fast forward to BLDC tool, took the same steps as before, only wanted to change motor parameters, they started spining once I pressed "Next" in the BLDC tool and KABOOM. i personally see no way, how this could be a user error, since I did not take any other steps besides the usual ones. I have contacted TB, but got no answer that would make sense. I'm not even talking about refund/replacing whatever. This was the first and will be the last time I have bought anything from them.
```

---
## \#14 Posted by: ARetardedPillow Posted at: 2018-09-25T12:41:51.516Z Reads: 24

```
I think I've fried about 9 tb vescs, 2 of them are user error and the rest is just unkown. Long story short they're not reliable, had to do many walks of shame.
```

---
## \#15 Posted by: Pafrican Posted at: 2018-09-25T14:57:20.113Z Reads: 16

```
I tried doing motor detection in BLDC mode (instead of FOC) and got the same problem.. motor is not responding at all.
VESC tool is not listing any faults either, which leads me to believe that the VESC is fine (green and blue LED's light up as they should, I haven't seen any red LED lights flashing). Maybe my motor went bad?

One of the reps from diyelectricskateboard told me that using a 245kv motor and a 10S setup may have caused the problem. Apprently I should be using a motor with 190kv or less when using 10S. Can anyone explain to me why this is? How does this relate to ERPM limit?
```

---
## \#16 Posted by: Andy87 Posted at: 2018-09-25T15:43:47.277Z Reads: 14

```
You can calculate your max erpm here
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":245,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":90}|

With the combination 10s 245kV you could theoretically hit the 60 000 max erpm for hw4.12 vescs
```

---
## \#17 Posted by: Pafrican Posted at: 2018-09-25T19:04:35.736Z Reads: 13

```
And if I hit this 60,000 erpm then I blow a DVR?
```

---
## \#18 Posted by: Andy87 Posted at: 2018-09-25T19:05:22.870Z Reads: 12

```
That can be the result yes
```

---
