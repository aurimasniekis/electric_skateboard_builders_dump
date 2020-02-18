# Motor Setup Help

### Replies: 17 Views: 177

## \#1 Posted by: LaCocoRoco Posted at: 2019-05-06T11:36:19.743Z Reads: 64

```
Hi, i need guidance from experienced builders.

This is my current setup:
- Tramper Carver 14ply
- Tramper Gummis 124mm 
- Battery 12S4P
- Pulley 14/44 

First i thought to use an 6374 190KV ~3000W Motor.
But after reading through many projects probably the KV is to high.
Should i go for 150KV?
I am grateful for every recommendation.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-05-06T11:39:52.722Z Reads: 62

```
You can calculate your top speed here

https://calc./#/0

Depending on what you aim for both will work. 150kV will give you more torque, 190kV more top speed. Both will work.
```

---
## \#3 Posted by: Komamtb Posted at: 2019-05-06T11:40:28.961Z Reads: 58

```
I run 12s with 170kv motors on gummies, 16/60 ratio, seems to be a good medium.
```

---
## \#4 Posted by: LaCocoRoco Posted at: 2019-05-06T12:56:19.270Z Reads: 50

```
@Andy87 The main reason for the board is to get fast from one village to the next. But i dont know if i ever will say "Ok, i am fine with 30mph+". So probably buy recommended Motor with xxx KV and replace other components.

@Komamtb Do you have a link to the motors?
```

---
## \#5 Posted by: Komamtb Posted at: 2019-05-06T13:01:48.976Z Reads: 47

```
I use Alien motors, but would not recomend them.
```

---
## \#6 Posted by: trampa Posted at: 2019-05-06T13:04:15.788Z Reads: 45

```
Motor KV does not matter so much. If you have a proper ESC like VESC 6, you could go for 190KV with ease. For ESCs that are HW4.12 based, featuring only two low side shunts, higher KV has the potential to turn out more problematic since the amp flow in the system is higher.
```

---
## \#7 Posted by: Andy87 Posted at: 2019-05-06T13:09:34.219Z Reads: 43

```
[quote="trampa, post:6, topic:92955"]
Motor KV does not matter so much
[/quote]

@trampa but why you than just sell low kV motors?
```

---
## \#8 Posted by: trampa Posted at: 2019-05-06T13:17:33.074Z Reads: 41

```
Low is relative. The MTBs have 160 KV and with 9" tires and 1:6 gearing that is good for 50Km/h which is plenty for an off-road setup. 
Usually you choose the KV according to top speed. Lower KV outputs more torque at a given Amp flow. If you want to keep the amps low, you calculate the top speed you want to achieve and then choose the KV accordingly. For a street board with low rolling resistance and quite powerful motors KV has not so much of an impact if you look at the average amp flow. Question is: How fast do you want to go?

If the ESC features only two shunts, lower KV is better.
```

---
## \#9 Posted by: LaCocoRoco Posted at: 2019-05-06T13:18:43.025Z Reads: 39

```
Ok that sound legit. I will use VESC 6. And if i am not wrong, it should be possible to switch the Trampa Motormounts Pullys & Belt to 16/66 if necessary. This solved my doubts.
```

---
## \#10 Posted by: Andy87 Posted at: 2019-05-06T13:20:29.854Z Reads: 38

```
Ok than i might understood your first comment  wrong. As your latest comment just explained that the kV matters when you think about which performance is the right for your board.
```

---
## \#11 Posted by: Andy87 Posted at: 2019-05-06T13:22:09.544Z Reads: 37

```
@LaCocoRoco keep in mind that gummies will restrict your clearance. 66th is a big pulley.

Edit: that’s 66th on 8“
![image|510x500](upload://aE6Vx4mtrQ745FtuhrhiDB4JO3Y.jpeg)
```

---
## \#12 Posted by: trampa Posted at: 2019-05-06T13:26:33.713Z Reads: 35

```
It depends on copper fill. For the motor it doesn't matter, the ESC sees more amps with higher KV.

For the setup with Gummies and 14/44 transmission: 170 KV gets you to 53Km/h, which is already way above the speed I would ever go on a carver.
```

---
## \#13 Posted by: Andy87 Posted at: 2019-05-06T13:32:29.670Z Reads: 34

```
[quote="trampa, post:12, topic:92955"]
Gummies and 14/44 transmission: 170 KV gets you to 53Km/h,
[/quote]

Depending on your battery for sure.

I had 15/44 with 190kV on 11s and I wouldn’t go that high in kV or better to say so low with wheel pulley teeth. 50-55th would work better for me in this case.
```

---
## \#14 Posted by: LaCocoRoco Posted at: 2019-05-06T14:38:29.184Z Reads: 29

```
Thanks for this information!
I will reconsider everything first.
```

---
## \#15 Posted by: professor_shartsis Posted at: 2019-05-06T15:18:57.054Z Reads: 27

```
[quote="LaCocoRoco, post:1, topic:92955, full:true"]
Hi, i need guidance from experienced builders.

This is my current setup:

* Tramper Carver 14ply
* Tramper Gummis 124mm
* Battery 12S4P
* Pulley 14/44

First i thought to use an 6374 190KV ~3000W Motor. But after reading through many projects probably the KV is to high. Should i go for 150KV? I am grateful for every recommendation.
[/quote]

the left chart shows "how fast you could go" with the following assumptions:

250lbs, 2 motors, 190kv, 0.05ohm, 45.6v battery, 124mm tires

the right chart shows what gear ratio is necesasary to achieve the maximum possible up-slope speed:

https://i.ibb.co/0F2v1Mx/12s-124mm.jpg

^it turns out if you are willing to change your gearing ratio, you could get nearly identical performance from your board whether you select a 190kv or 150kv motor... but you would need to use different gear ratios than are shown on this chart if you select a 150kv motor.

whether you choose 150kv or 190kv, and regardless of tire size, a gear ratio that gives a no load wheel speed of ~36.7mph will give you a peak uphill velocity of about ~34mph on 25% slopes assuming you use 60a battery current limit per motor.

https://i.ibb.co/VWj0Jdz/124mm-25percent.jpg
```

---
## \#17 Posted by: Resonant Posted at: 2019-05-06T16:26:57.996Z Reads: 16

```
How can I see a predicted graph like this for my future build? You should make a website to input such variables and output them like these graphs.
```

---
## \#18 Posted by: professor_shartsis Posted at: 2019-05-06T16:27:44.219Z Reads: 16

```
@Resonant you can download the spreadsheets I built for that here: 

https://www.electric-skateboard.builders/t/racing-calculator-for-esk8/92437
```

---
