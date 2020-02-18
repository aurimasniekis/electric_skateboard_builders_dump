# Anti spark stuck on?

### Replies: 29 Views: 600

## \#1 Posted by: marsrover001 Posted at: 2018-12-14T00:05:09.657Z Reads: 190

```
I have a "T-Rex" anti spark switch from the apparently now gone http://www.antisparkheaven.com

It worked fine for a few months. I took the board apart to add some LED's, and 2 cheap buck converters exploded in my testing. They were hooked up to the output of the anti spark switch.

So I'm putting everything back together, plug in the control switch. And the anti spark is stuck in the on state. Won't turn off. Checked continuity on the button, one common, continuity switches from one pole to the other. Tested the same thing at the connector that plugs into the anti spark switch.

So. Is my anti spark switch broken? What else can I check? 

![20181213_185741|374x500](upload://3ZboC52XfUxl5w139JVBkoXQQPK.jpeg)
```

---
## \#2 Posted by: Esk88 Posted at: 2018-12-14T00:09:26.686Z Reads: 184

```
I think that means you have a blown mosfet
```

---
## \#3 Posted by: marsrover001 Posted at: 2018-12-14T00:21:15.673Z Reads: 185

```
Any recommendations for a new one. All I see is the eskating.eu one, but shipped to me it's near $90.
```

---
## \#4 Posted by: Esk88 Posted at: 2018-12-14T00:23:48.042Z Reads: 177

```
Miami electric and @Martinsp
```

---
## \#5 Posted by: marsrover001 Posted at: 2018-12-14T00:34:41.599Z Reads: 168

```
Looked into it a bit more. I know a guy with a hot air gun and a reflow station. So I ordered 5x IRFS7730 mosfets (4 to install, one to mess up) and I'll just swap them all out. Fingers crossed it all works out.
```

---
## \#6 Posted by: Friskies Posted at: 2018-12-14T00:38:04.761Z Reads: 165

```
Honestly you need to spend more money on a good antispark or just get a loopkey. Maybe one from @Kug3lis if he still has any.
```

---
## \#7 Posted by: marsrover001 Posted at: 2018-12-14T00:51:00.199Z Reads: 154

```
If this fails I'll get one from Miami boards. They are like 3 hours from me.

I've got other boards to ride while this one is down, no big rush.
```

---
## \#8 Posted by: nuttyjeff Posted at: 2018-12-14T00:54:25.841Z Reads: 153

```
@Kug3lis has some beefy ones.
```

---
## \#9 Posted by: StefanMe Posted at: 2018-12-14T04:48:22.379Z Reads: 139

```
Everything sold out
```

---
## \#10 Posted by: barajabali Posted at: 2018-12-14T06:29:18.396Z Reads: 131

```
Where art thou @goldenHusky
```

---
## \#11 Posted by: b264 Posted at: 2018-12-14T06:37:14.537Z Reads: 126

```
We were discussing this phenomenon earlier and why they blow.

https://www.electric-skateboard.builders/t/vedder-antispark-design-problem-or-implementation-problem/77967
```

---
## \#12 Posted by: marsrover001 Posted at: 2018-12-14T08:02:44.270Z Reads: 112

```
Super interesting read actually. I don't think I can modify this switch to do the delayed resistor thing. So next time it dies I'll just hope the fat boy switch is in stock.

I do have some xt90-s on the way. So maybe that will help.
```

---
## \#13 Posted by: goldenHusky Posted at: 2018-12-14T09:18:29.675Z Reads: 106

```
Hey, I'm not very active lately so if somethings up just write me a pm so I get an email notification.

@marsrover001 I'm sorry for the defect, maybe some transient feed back of the buck converters at breakdown or normal operation exceeded the 100 Vds limit of the mosfets. Also the control switch should never be unplugged, because there is no pull down resistor, so the gates are on a undefined potential which can cause issues.

Btw, my site is not completely gone, I just discontinued the premium subscription of the shop software I used, where you can set your own domain, so the "bigcartel" phrase is included again like this: https://antisparkheaven.bigcartel.com/
```

---
## \#14 Posted by: marsrover001 Posted at: 2018-12-14T11:20:01.062Z Reads: 92

```
That might have been it, I spent a few days testing stuff by just manually unplugging the main power lead. Do you think my mosfet replacement idea will work or did leaving the switch unplugged mess up the switch sense side?

I know I'm totally out of warranty so no worries.
```

---
## \#15 Posted by: goldenHusky Posted at: 2018-12-14T11:46:07.261Z Reads: 88

```
Replacing the faulty mosfets (could be only one or all four) will fix it, maybe the zener diode broke down too but that is rather unlikely, you can check that by measuring the voltage from the gates to ground.
```

---
## \#16 Posted by: Schulerbible Posted at: 2018-12-14T12:28:12.421Z Reads: 86

```
I can recommend Zill Boards anti spark.
![image|368x276](upload://cZCFnyhZT9VeCqpWz3h9T50nBbE.jpeg)
```

---
## \#17 Posted by: Andy87 Posted at: 2018-12-14T12:30:42.349Z Reads: 86

```
[quote="marsrover001, post:12, topic:77961"]
I do have some xt90-s on the way. So maybe that will help
[/quote]

only if you use them as loop key and forget about the mosfet switch ;)
```

---
## \#18 Posted by: bevilacqua Posted at: 2018-12-14T12:36:31.661Z Reads: 85

```
that seems like a re branded flier AS. Witch has known issues
```

---
## \#19 Posted by: Schulerbible Posted at: 2018-12-14T12:56:26.435Z Reads: 81

```
Yeah true. Was that the 120A version or 300A with the issues?
```

---
## \#20 Posted by: bevilacqua Posted at: 2018-12-14T13:11:43.987Z Reads: 79

```
not sure, @longhairedboy and @Jayx should know more
```

---
## \#21 Posted by: longhairedboy Posted at: 2018-12-14T15:30:54.458Z Reads: 70

```
if that is a rebranded genuine flier 300amp eswitch then freezing on is a defect or fluke. I've been running those in boards for a while now, they're the only ones that are really reliable. Kind of surprised at this, but i suppose it has to happen eventually.
```

---
## \#22 Posted by: marsrover001 Posted at: 2018-12-14T16:24:48.315Z Reads: 62

```
Seems like my luck.
Whoever makes the fat boy switch. Hurry up and make more. I don't mind leaving the board on all the time, but sometimes one motor stops working and it needs a reboot. I think gluing in the canbus cable and turning off traction control might have helped. Needs testing. Too much rain to test.
```

---
## \#23 Posted by: longhairedboy Posted at: 2018-12-14T17:45:14.833Z Reads: 57

```
You're going to end up with more issues, eventually the regen currents from hard braking will agitate the failure in the mosfets and you'll have to replace it anyway after it finally dies completely.
```

---
## \#24 Posted by: Battosaii Posted at: 2018-12-14T17:50:52.972Z Reads: 55

```
Is there any reliable one? I got a good one and installed it, plug and play so nothing I could do wrong and it worked beautifully. Never rode it just tested the switch and when I woke up next morning the board was stuck on and would not shut off. I look and 3 or 4 fets burned up :(.
```

---
## \#25 Posted by: J_Dizzle_2.0 Posted at: 2018-12-14T18:40:58.259Z Reads: 46

```
Do you disharge through your bms? If so just use the e-switch on the bms, that is more reliable than most anti-sparks
```

---
## \#26 Posted by: marsrover001 Posted at: 2018-12-14T18:59:43.371Z Reads: 47

```
In the name of higher amprage (and cause I bought the anti spark before I bought my bms) my bms is charge only. :expressionless:
```

---
## \#27 Posted by: J_Dizzle_2.0 Posted at: 2018-12-14T19:51:53.770Z Reads: 47

```
A 80a bestech bms for bkb is cheaper than a new anit-spark
https://buildkitboards.com/collections/batteries/products/bestech-bms?variant=7201537785886

https://buildkitboards.com/collections/batteries/products/100a-anti-spark-switch?variant=12590976598110
```

---
## \#28 Posted by: marsrover001 Posted at: 2018-12-14T19:57:48.317Z Reads: 47

```
I've got dual focbox on 6374 motors at 60a each. So the 100a switch might work, don't know I could trust an 80a bms.
```

---
## \#29 Posted by: marsrover001 Posted at: 2018-12-15T15:22:53.569Z Reads: 37

```
Update to all this. Learned some more about mosfets and poked around with a multimeter. Figured out which one went bad and desoldered it. Only had a ts100 so I did the best I could at taking it out of the circuit.

To my surprise it works again! ![20181215_101620|666x500](upload://1eMwsJpkCYLV81Znmg1VET1zeiq.jpeg)
```

---
