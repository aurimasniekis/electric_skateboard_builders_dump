# BMS trouble and Overall Build failure

### Replies: 29 Views: 1568

## \#1 Posted by: ArsenalMain Posted at: 2018-04-19T18:49:09.234Z Reads: 134

```
Hey Esk8, I have been working on my build since mid january, picking all of my parts, and generally doing as much research as I could. Since that time, I have built a decent foundation of all the info needed to build a quality and long lasting board. Despite this, I have had nothing but trouble with my build and honestly am starting to lose hope that I will ever get it to work. 

My board has a TB sensored motor and Vesc along with a 10s bms from bestech and 5 2s batteries in series, similar to the build that @Namasaki made. Since the very beginning, I have had nothing but trouble with my BMS. 

After I first put in my BMS and finished the build, it worked perfectly, both in speed and reliability. After shutting it down and putting it away while I went to work, I came back to find that it no longer worked. Thinking it might have just been a defective BMS, I decided to switch it out and install the second one that came with my order. I had the same problem, after a short time of it working and then leaving it for a bit, it no longer worked. The worst part of this is that It wont let me charge my batteries either, with the charger just turning on and off over and over again when plugged in. 

Over the course of the past month and a half, I have been talking to Lucy at Bestech trying to solve my problem and am still no closer at figuring it out. During this time, the voltage in my batteries have dropped significantly and I am now worried that I have to buy new batteries on top of a new BMS. Do any of you have suggestions on how I should proceed? Im really lost at the moment. And this is how I wired my system.  ![152132079773915104805|374x499](upload://hV3UZv9CzsK6dyKIOPRn3R6Mciz.jpg)
And this is the steps I took while connecting it all:
Steps:
1) soldered all batteries together into series 
2)soldered the negative lead of the batteries to b-. 
3) soldered a connection for the positive battery lead to connect to the load. 
4) soldered p- to the negative lead of the load. 
5) spliced a wire onto the main positive wire and connected this to the positive terminal of the charging port. 
6) soldered a wire to the c- and connected this to the negative terminal of the charging port. 
7)  soldered switch to the two switch wires. 
8) connected balance wires in proper order
9) Connected the battery positive to the positive lead of the load. 
10) Flipped switch.
```

---
## \#2 Posted by: Namasaki Posted at: 2018-04-19T21:43:01.694Z Reads: 107

```
Just got home from work so let me see
```

---
## \#3 Posted by: Namasaki Posted at: 2018-04-19T21:47:16.910Z Reads: 114

```
The only thing I see that is wrong with your wiring diagram is that your batteries are numbered backwards.
Which Bestech BMS are you using?
The Negative out is battery 1
The Positive out is battery 5
Does the BMS turn on with the E-switch?
Are any of the battery cells at or below 3.0v?
IF the BMS turns on, is there full battery voltage at p-?
```

---
## \#4 Posted by: ArsenalMain Posted at: 2018-04-19T22:06:05.806Z Reads: 108

```
Ya, I know the batteries are labeled backwards but that was just me, I plugged them in correctly. I am using the HCX-D596 BMS. Originally, the bms did turn on with the e-switch but doesn't any longer. I'm having trouble measuring but I'm fairly certain that all of them are below 3.0v regardless of the fact that the bms has been off. And I can't even charge them because the bms doesn't work. And previously, when the bms worked, I was receiving full bat voltage at p-
```

---
## \#5 Posted by: Namasaki Posted at: 2018-04-19T22:21:25.680Z Reads: 103

```
I think you are in a Catch22 situation.
The BMS will not power up because the low voltage triggers the protection mode the instant you turn it on.
When the BMS goes into protection mode it cuts all power and has to be turned off and back on to reset.
You need to charge the battery packs individually without the bms but you will need a hobby charger to do that.
```

---
## \#6 Posted by: ArsenalMain Posted at: 2018-04-19T23:10:17.668Z Reads: 89

```
Do you think it would be worth it to order a 2s hobby charger and see if that will work? Because the thing that is holding g me is that even when the voltage was at 41v, it still wouldn't work. It worked for a short time and then randomly stopped
```

---
## \#7 Posted by: Namasaki Posted at: 2018-04-19T23:21:41.125Z Reads: 86

```
Most hobby chargers are 6s.

I'm really not familiar with that model of bms except that it is a new model and they're could be issues with it.
```

---
## \#8 Posted by: ArsenalMain Posted at: 2018-04-19T23:38:41.798Z Reads: 85

```
Can you see anything wrong with the steps I took to put it together? Like did I do something in the wrong order?
```

---
## \#9 Posted by: Jumpman Posted at: 2018-04-19T23:40:00.002Z Reads: 82

```
https://www.electric-skateboard.builders/t/bestech-hcx-d596-the-new-80a-bms-wiring/41047/14?u=jumpman
```

---
## \#10 Posted by: ArsenalMain Posted at: 2018-04-19T23:44:04.357Z Reads: 79

```
Yes, that is the process I followed while wiring my BMS, and after I had connected them, I confirmed that they were increasing in voltage across before I plugged it into my BMS
```

---
## \#11 Posted by: ArsenalMain Posted at: 2018-04-19T23:47:50.613Z Reads: 77

```
Also, I would have trouble individually charging each battery because I disconnected their connectors and soldered them together. So how would you recommend going about this?
```

---
## \#12 Posted by: ArsenalMain Posted at: 2018-04-19T23:49:17.586Z Reads: 78

```
Would a charger such as this work? 
https://hobbyking.com/en_us/turnigy-b4-compact-35w-4a-automatic-balance-charger-2-4s-lipoly.html

Or this:
https://hobbyking.com/en_us/hobbykingr-dc-4s-balance-charger-cell-checker-30w-2s-4s.html
```

---
## \#13 Posted by: Namasaki Posted at: 2018-04-20T00:13:54.147Z Reads: 65

```
It's gonna be tough without the original balance connectors on the Lipos.
You could try charging one pack at a time with 2s charger without balance but keep a close eye on the cell voltage with a multimeter.
```

---
## \#14 Posted by: ArsenalMain Posted at: 2018-04-20T00:38:34.689Z Reads: 63

```
I still have the original balance connectors connected(I never removed them, but the positive and negative wires are soldered onto their counterpart on either side.
```

---
## \#15 Posted by: Namasaki Posted at: 2018-04-20T01:19:20.128Z Reads: 59

```
Your in luck then. You can balance charge each pack individually with a hobby charger. 
Disconnect all of the balance connectors from the bms harness then remove the shrink tube from the series connections and use alligator clips to connect to the main wires. Do one pack at a time.
```

---
## \#16 Posted by: ArsenalMain Posted at: 2018-04-20T01:26:16.582Z Reads: 56

```
Is there any hobby charger I should look into specifically? And im trying to not spend more money if I have to end up buying new BMSs

Do either of the ones I posted work?
```

---
## \#17 Posted by: Namasaki Posted at: 2018-04-20T01:34:13.868Z Reads: 57

```
A hobby charge is a maintenance tool when you use Lipos. It’s an investment. 
I still have my dual bank 6s Lipo Charger  
I recommend you spend a bit more. 
https://www.amazon.com/dp/B072V7PNJV/ref=cm_sw_r_cp_api_xqu2AbNGM80BD
```

---
## \#18 Posted by: ArsenalMain Posted at: 2018-04-20T01:38:26.497Z Reads: 57

```
See, I already got this one to be able to charge my batteries in series:
https://lunacycle.com/36v-4amp-luna-mini-charger/
So i am just reluctant to buy another expensive charger considering I might not have enough to buy another round of BMS's if I cant figure it out.
```

---
## \#19 Posted by: b264 Posted at: 2018-04-20T01:42:43.739Z Reads: 56

```
[quote="Namasaki, post:17, topic:52809"]
A hobby charge is a maintenance tool when you use Lipos.
[/quote]

A hobby charger should not be any more necessary for Lipos then it is for lithium-ion cells.

A hobby charger is needed when you are trying to avoid using a BMS, which is not recommended
```

---
## \#20 Posted by: ArsenalMain Posted at: 2018-04-20T01:44:27.586Z Reads: 54

```
So what would you recommend?
```

---
## \#21 Posted by: KTMinni Posted at: 2018-04-20T01:45:52.763Z Reads: 50

```
In this case it does sound necessary because he can't charge through bms. It's a good thing to have either way.
```

---
## \#22 Posted by: b264 Posted at: 2018-04-20T02:27:51.970Z Reads: 48

```
[quote="ArsenalMain, post:20, topic:52809, full:true"]
So what would you recommend?
[/quote]

Firstly measure all your P-packs with a multimeter.  As long as none are near 4.2, put the charger directly on the battery ends for 5 minutes (charging directly, bypassing the BMS), then check all 10 P-packs again.  Never leave it connected unattended and just do it for short times, and keep checking voltages with the multimeter.

Bring it up high enough for your BMS to work, but don't exceed 4.2V on any one cell.
```

---
## \#23 Posted by: ArsenalMain Posted at: 2018-04-20T02:41:46.384Z Reads: 44

```
Would either of the chargers that I posted work or no? Also, I have access through my school to a straight power source if that would work. With that line of thinking, if i set the power source to release a 7v output at 4A, would that be viable for charging each of my 2s batteries? If i followed the steps you outlined? Or would you recommend just sticking with a charger?
```

---
## \#24 Posted by: Namasaki Posted at: 2018-04-20T03:01:48.278Z Reads: 40

```
[quote="b264, post:19, topic:52809"]
A hobby charger should not be any more necessary for Lipos then it is for lithium-ion cells.
[/quote]


It's just a handy tool to have around in case of a situation like this with Lipos and could also be handy for maintenance charging of Li-ion cells or P groups individually.
```

---
## \#25 Posted by: deucesdown Posted at: 2018-04-20T03:03:06.175Z Reads: 41

```
[quote="b264, post:19, topic:52809"]
A hobby charger should not be any more necessary for Lipos then it is for lithium-ion cells.
[/quote]

Gotta disagree. Many lipo packs have cycle life in the 50-150 cycle range. As they age you might want to check capacity, internal resistance, etc etc.

But then I'd feel the same way about li-ion packs...
```

---
## \#26 Posted by: b264 Posted at: 2018-04-20T03:14:52.210Z Reads: 41

```
[quote="deucesdown, post:25, topic:52809"]
But then I’d feel the same way about li-ion packs
[/quote]

That's the point I was making
```

---
## \#27 Posted by: ArsenalMain Posted at: 2018-04-20T03:17:08.958Z Reads: 40

```
Do you think the method that I suggested would work?
```

---
## \#28 Posted by: b264 Posted at: 2018-04-20T03:20:33.379Z Reads: 41

```
The most important part is stopping VERY often and checking the voltages.  You cannot exceed 4.2V or go under somewhere around 3 volts.  You can cannot charge OR discharge any of them at too high a rate, which the 7V 4A one might do
```

---
## \#29 Posted by: Namasaki Posted at: 2018-04-20T11:49:09.989Z Reads: 37

```
[quote="b264, post:28, topic:52809"]
The most important part is stopping VERY often and checking the voltages.
[/quote]

@ArsenalMain 
It’s much easier and safer to do this with a hobby balance charger. 
And the cells will be balanced when charging is complete. 
And it is important for the cells to be balanced before reconnecting them to the bms.
```

---
