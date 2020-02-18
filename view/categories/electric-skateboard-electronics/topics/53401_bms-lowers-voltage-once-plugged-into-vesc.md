# BMS Lowers voltage once plugged into VESC

### Replies: 25 Views: 621

## \#1 Posted by: Lumaci Posted at: 2018-04-24T22:21:49.566Z Reads: 63

```
So i got my battery pack made, all "working" i got it charged everything is fine the voltage is where it should be 41.8V Total.

When i just smack my prongs into the XT60 and read the voltage its the correct voltage but when ever i plug the XT60 plug into my VESC the voltages lowers to 3.5/3.7V.

Ive bypassed the red wire so its going directly from the pack into the XT60, do I need to do the same for the black one since it seems to be where the issue is? (Battery pack voltage is still the same no matter what only P- on the BMS lowers to the XT60.)
```

---
## \#2 Posted by: Lumaci Posted at: 2018-04-24T22:25:15.568Z Reads: 59

```
Drew a picture so it would be explained better ![image|690x292](upload://vFaAVGtNU3q8yL6j1UArOp6P7V.jpg)
```

---
## \#3 Posted by: Martinsp Posted at: 2018-04-24T23:14:25.055Z Reads: 51

```
So when you measure the voltage on your BMS output it reads low voltage even without VESC connected? or is it only with the VESC connected?
```

---
## \#4 Posted by: Lumaci Posted at: 2018-04-24T23:16:01.174Z Reads: 50

```
Only when the VESC is installed.

But i talked with a guy he tells me to just take the black wire going from the BMS and install it directly onto the battery pack so both my red and black is directly going from the battery pack into the vesc and then the bms only handles the charge part and has nothing with the rest to do.

Would that work?
```

---
## \#5 Posted by: Martinsp Posted at: 2018-04-24T23:19:46.556Z Reads: 46

```
Well I would check some stuff before doing this. There may be a problem where the VESC may be shorting the battery and triggering the BMS over current, the BMS then cycles (turns on, measures current, turns off) and these cycles may result in something like a PWM signal that your multimeter may measure on DC as 3.7 or whatever low voltage. Now this may not be the case, but it is one of the possible scenarios.

Measure the voltage on the output of the BMS without the VESC connected, also measure the resistance on the power input to the VESC. The value should be high due to the capacitors on power wires.
```

---
## \#6 Posted by: Lumaci Posted at: 2018-04-24T23:24:26.000Z Reads: 41

```
When the vesc is not connected everything is just fine 42V, but when ever its connected it drops instant down to 3.7V.

And everything else seems fine, kinda seems like a dodgy BMS but it charged it up just fine so almost cant be or can it?
```

---
## \#7 Posted by: Martinsp Posted at: 2018-04-24T23:27:36.736Z Reads: 38

```
As long as the VESC does not have a low resistance on the input wires it is ok to plug in directly to battery.

The BMS may have other problems so if it works without the bms then I would suggest changing it or possibly using for charging only. But be sure to monitor its behavior since at this point it is questionable to rely on ti keeping your batteries safe. Better safe than sorry
```

---
## \#8 Posted by: Lumaci Posted at: 2018-04-24T23:30:00.430Z Reads: 36

```
Yeah, was also really just the plan.

The battery is only meant for testing anyways so not going to be used on a board but more to tweak my vesc settings since i have no variable bench power supply anymore or one that can do a high enough amount of amps (20+)

But thanks, ill just bypass the black side as well.

It should just charge via the balance leads and the red charge lead connected to the battery just fine right?
```

---
## \#9 Posted by: Martinsp Posted at: 2018-04-24T23:33:21.335Z Reads: 34

```
Ah, okay then.

I have the same kind of BMS it seems like (10S 60A from batterysupports.com) and the charging is done using the red wire from battery directly and the P- port
```

---
## \#10 Posted by: Lumaci Posted at: 2018-04-24T23:35:53.195Z Reads: 29

```
Mine has a CH- port for charging, should be fine then.

Thanks ill give it a try tomorrow and see how it goes.
```

---
## \#11 Posted by: pat.speed Posted at: 2018-04-24T23:36:07.182Z Reads: 27

```
You must leave the b- wire connected to the battery and then run a second wire to the load, if you don’t the bms won’t function
```

---
## \#12 Posted by: Lumaci Posted at: 2018-04-24T23:37:39.039Z Reads: 27

```
Like this?
Thats how i planned to do it, wire a new black wire on the battery that goes directly to the vesc and leave the one connected to the BMS

Dont mind the white stuff and black wire, only the battery to bms part is what im doing.
![image|257x500](upload://3egMFEMWeXSeUoWhtykom1kU7lS.jpg)
```

---
## \#13 Posted by: pat.speed Posted at: 2018-04-24T23:39:29.882Z Reads: 24

```
![image|690x292](upload://eDsIBL4qr9zXVaJuD0amuw9Z6Th.jpeg)

Like this

Edit; yep yours is right
```

---
## \#14 Posted by: Martinsp Posted at: 2018-04-24T23:40:46.542Z Reads: 23

```
That looks correct.
The path for black should be from battery to BMS whichever port it uses (refer to diagram of your BMS) and out of the BMS charging port to your charging plug. Red goes straight from battery. Of course balance leads have to be connected too.
For discharge, just both red and black directly from battery
```

---
## \#15 Posted by: Lumaci Posted at: 2018-04-24T23:41:56.611Z Reads: 24

```
Perfect, going to sleep now ill hook it up tomorrow and see how it goes.

Anyone know the amp limit of an Evolve Bamboo GT battery? I read somewhere its max 45Amps only gonna do 20 on it though but just to be safe so i aint blowing stuff up.
```

---
## \#16 Posted by: pat.speed Posted at: 2018-04-24T23:43:42.551Z Reads: 23

```
You could try increasing amps until the battery sags a lot then you’ll know your close to the max amps limit
```

---
## \#17 Posted by: Martinsp Posted at: 2018-04-24T23:44:18.179Z Reads: 22

```
I unfortunately dont, maybe try asking someone who is rebuilding the batteries. Someone is providing it as a service here on the forum, maybe they will be able to tell you more.
```

---
## \#18 Posted by: Lumaci Posted at: 2018-04-24T23:44:29.899Z Reads: 21

```
So just read voltage on +/- op the amp a little and see if i get huge dips?
```

---
## \#19 Posted by: Lumaci Posted at: 2018-04-24T23:46:19.129Z Reads: 22

```
Found this on the Evolve Forum:

"Our motors are rated at 3000w, and batteries at 36v. 3000 / 36 = 83 amps"

83amps cant be true can it?
```

---
## \#20 Posted by: pat.speed Posted at: 2018-04-24T23:46:31.158Z Reads: 20

```
Yeah, do you have a Bluetooth module for the vescs? Otherwise @darkkevind might know


Those amps would be peak not constant
```

---
## \#21 Posted by: Lumaci Posted at: 2018-04-24T23:47:35.568Z Reads: 19

```
Yep, got a Metr module.

So sounds like it safe to assume the battery can supply around 40amps and 80peak.

Same i read else where
```

---
## \#22 Posted by: pat.speed Posted at: 2018-04-24T23:56:35.476Z Reads: 19

```
Yeah I would says that’s a pretty safe assumption. I wouldn’t go much more than 20-25a per Vesc
```

---
## \#23 Posted by: Lumaci Posted at: 2018-04-25T00:11:29.951Z Reads: 20

```
Yep, only using single drive myself so way under the maximum but better safe then sorry.

20amps is what i plan on using the board at for the rest of its life and just using the battery pack i made now to get it up and running so when ever i get the money for a real pack i no longer would have to worry about vesc settings and i can just enjoy it or if im super lucky and get a good offer on the complete without battery the buyer wont have to do anything else either :-)
```

---
## \#24 Posted by: darkkevind Posted at: 2018-04-25T00:43:17.958Z Reads: 22

```
Yes. The Evolve BGT, CGT and GTX will pull a max of around 80A peak for a few seconds... It can't sustain it for any longer. It pulls around 40A continuous though. Even then it will overheat and restrict current if you do that for too long...

Cheap Chinese parts unfortunately. Not even good Chinese parts! :confused:
```

---
## \#25 Posted by: Lumaci Posted at: 2018-04-25T09:38:38.723Z Reads: 19

```
Sooo it works now flawless and hooolyyy fuuuc my board has a lot of power now.
```

---
