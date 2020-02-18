# Power buttons/switches

### Replies: 18 Views: 457

## \#1 Posted by: MrDGOrman Posted at: 2018-09-13T08:59:42.635Z Reads: 149

```
Hi everyone,

I'm currently running 3 X 5000mah Zippy batteries and us an XT-90 antispark switch as my "on off button".

I plan to move to Li-ion batteries soon but wanted to know what on/off switch I can use. I want to be able to use it with my current setup along with a 10s4p battery.

In a nut shell - the XT-90 antispark is very attractive. I want a simple on off switch that can handle the power of the batteries. Like any normal board.

Recommendations welcome. I really like the Evolve Carbon GT on off button. Black, lights up a power logo when on and is a simple push button.

Thanks,
Daniel
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-13T11:08:27.952Z Reads: 130

```
If you wanna go by a push button you always need a relay behind which switch the main circuit.
The problem is that the push buttons usually can handle only small currents.
You have some oportunitys  
1. get a bms with built in e-switch (you can by any e-switch design you like from Ali and attach it as soon as the voltage match your bms switch voltage).
2. get a esc with a built in e-switch (same princip like with the bms, you can choose your own)
3. get an antispark switch with an e-switch
```

---
## \#3 Posted by: mynamesmatt Posted at: 2018-09-13T12:19:20.888Z Reads: 109

```
exactly what @Andy87 said. If you want it to light up you can either use a step down converter or take 5v straight from the vesc or foxbox and use that to light up your button
```

---
## \#4 Posted by: Andy87 Posted at: 2018-09-13T12:25:09.207Z Reads: 106

```
I meant a bit something different 😅
The lightning up is one thing you can sure manage from step down converter or the vesc, but the most small e-switches don’t switch high currents. You use the switch just to switch on/off mosfets or relays, which than switch the main power circuit.
```

---
## \#5 Posted by: mynamesmatt Posted at: 2018-09-13T12:42:42.702Z Reads: 103

```
correctomundo, bms' with integrated eswitches are easier than having a bms and separate eswitch IMO as it's just another element off the list that's bound to fail
```

---
## \#6 Posted by: Andy87 Posted at: 2018-09-13T12:44:01.349Z Reads: 102

```
That’s good as long as you don’t use the bms for charge only 😅 than it will not work
```

---
## \#7 Posted by: Newby Posted at: 2018-09-13T12:45:50.034Z Reads: 100

```
BMS switch is cheaper and more compact
```

---
## \#8 Posted by: Andy87 Posted at: 2018-09-13T12:48:15.172Z Reads: 99

```
Than the (ok not so good but) Flipsky 6 switch? 🤔
It’s built in the vesc and if you don’t use a bms or go with charge only it will save even more space 😅
```

---
## \#9 Posted by: Newby Posted at: 2018-09-13T12:54:26.193Z Reads: 93

```
If it cuts load reliably in a pinch then use it. Also, use a BMS. We're on a path to not get DIY boards banned
```

---
## \#10 Posted by: Andy87 Posted at: 2018-09-13T13:06:38.025Z Reads: 91

```
I will go with bms, but I think it’s not really a have too. 
There are alternatives to make your board safe too. A fuse does a good job too, in some ways even better 😬 if you get quality LiIon cells they shouldn’t unbalance so fast and you anyhow shouldn’t discharge the cells till 2.5v. I also just charge till 4.1v and monitor them from time to time to be sure all is good.
If you go lipo I think nothing bad in balance charge with a hobby charger. The cells will not crazy unbalanced under one discharge cycle.

Just my opinion.

And one thing that maybe somebody can explain me. I‘m always a bit curious about bms balancing. As long as it is not a smart bms with Bluetooth Modul it’s for me still just a Blackbox.
I can just trust that it works how it should, but what if not? Can it technically be possible that a faulty bms will unbalance my battery pack?
```

---
## \#11 Posted by: MrDGOrman Posted at: 2018-09-13T13:37:30.462Z Reads: 81

```
Okay, so ignoring the Li-Po batteries and I consider this switch for when I have Li-Ion batteries - which switch do people recommend?

If it's integrated into the BMS, which BMS do you recommend?

I basically want to have a OEM style product. Not an obvious DIY build.
```

---
## \#12 Posted by: Andy87 Posted at: 2018-09-13T13:52:43.116Z Reads: 81

```
Bestech bms d596 or similar.
If extra switch than this
https://www.electric-skateboard.builders/t/push-to-start-switch-out-now/60879?u=andy87
```

---
## \#13 Posted by: MrDGOrman Posted at: 2018-09-13T13:58:58.657Z Reads: 75

```
Thank you.

Would I need to switch on the board when charging? Sorry, I'm a little new with BMS etc. I basically want a commercially made board (Boosted, Evolve, etc) without the cost of one! And making it myself is fun :slight_smile:

Can I change that BMS switch so that it's a push button rather than rocker switch?
```

---
## \#14 Posted by: Andy87 Posted at: 2018-09-13T14:03:57.177Z Reads: 74

```
[quote="MrDGOrman, post:13, topic:67887"]
without the cost of one
[/quote]

😬😬😬be aware, in the long run you come usually more expensive 😅 

But according your question, yes the bms need to be switched on while charging, but that shouldn’t be a problem.
Yes you can use any color or design of push button as long as it works with the switching voltage of the bms (usually it’s 12v but depends from the bms)
```

---
## \#15 Posted by: MrDGOrman Posted at: 2018-09-13T14:10:47.785Z Reads: 58

```
I'm starting to see that in regards to cost! Id rather build it myself though. It's a project afterall.

Okay, so BMS has to be switched on. Any particular reason why that is? How come boards like the Boosted and Evolve don't need to have it switched on to charge? It just doesn't make much sense to me. Why have the board on to charge it?
```

---
## \#16 Posted by: Andy87 Posted at: 2018-09-13T14:14:48.307Z Reads: 57

```
The bms need power to work and balance your cells.
The boosted board bms also switched on while charging. You see the charging light flashing...it’s the same
```

---
## \#17 Posted by: Andy87 Posted at: 2018-09-13T14:17:55.841Z Reads: 66

```
And I think they are disconnected  from each other. So bms and switch is separated.
The bms is somehow always switched on in this case.
You can also use a separate switch and place it after the bms. Make a bridge on the bms switch or buy one without e-switch and you ready to go.
```

---
## \#18 Posted by: Schulerbible Posted at: 2018-09-13T14:29:56.781Z Reads: 64

```
I got this one from Zillboards. If it withstands 60-80A peaks I will be more than happy. Bottleneck on this one is most likely the wire diameter.![image|666x500](upload://eocGu84PmlDwisk7qN3YODUhb08.jpeg)
```

---
