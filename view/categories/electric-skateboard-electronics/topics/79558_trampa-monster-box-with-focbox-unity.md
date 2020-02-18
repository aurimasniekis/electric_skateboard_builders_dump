# Trampa Monster Box with Focbox Unity

### Replies: 19 Views: 659

## \#1 Posted by: JKUK Posted at: 2019-01-01T20:36:19.603Z Reads: 188

```
Hi All,

I am after some advice if possible for my first build.

I have been looking at the following configuration but combining it with a Focbox unity

![24683|690x308](upload://2QUUamtE1268GK0MBbdlSyh6BqM.jpeg) 


I am struggling on how to connect the power to the focbox unity though. 

![edit|690x308](upload://AVydU0hHzILwp2hO4158N1d1L3.jpeg) 

I'd really appreciate it if someone could point me in the right direction for the best way of connecting the batteries to the unity and also connecting the LED display please.

Thanks in advance, complete noob here btw so please be patient :slight_smile:
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-01-01T20:43:12.211Z Reads: 168

```
Uhhhhhh it has it should have an xt60 on the opposite side of phase wires. Unless you have to add them. But that would void the warranty. 

Yeah. There's an xt60 connection for power. I guess they didn't show it in that picture you have.
```

---
## \#3 Posted by: StefanMe Posted at: 2019-01-01T20:45:56.948Z Reads: 162

```
https://de-m.banggood.com/XT60-Parallel-Adapter-Harness-Connector-Converter-p-938168.html?gmcCountry=DE&currency=EUR&cur_warehouse=CN&createTmp=1&utm_source=googleshopping&utm_medium=cpc_bgcs&utm_content=zouzou&utm_campaign=pla-deg-toys-mb
```

---
## \#4 Posted by: J_Dizzle Posted at: 2019-01-01T20:46:06.461Z Reads: 155

```
![image|375x500](upload://p7HdobKqDYFM4CwWnMPI6rKSi5a.jpeg) 

So you have 2x 12s1p batteries, wire them in parallel, with both positive leads going to the positive of the unity and both nagetives going to the negative of the unity

Edit: to do this use the parallel connector in the post above :arrow_up: :arrow_up:
```

---
## \#5 Posted by: J0ker3366 Posted at: 2019-01-01T20:52:48.158Z Reads: 146

```
Oh yeah lol. Like that.
```

---
## \#6 Posted by: JKUK Posted at: 2019-01-01T21:02:22.080Z Reads: 142

```
Ah thanks very much.

![edit|690x325](upload://qM0v8t3IDEXnjZ3hUvjUGTztqQ9.png) 

Diagram updated with a loop key that would connect to the unity from the batteries. 

So next couple of questions.

1. How can I connect the battery LCD display?

2. Also how can I charge the batteries? Is there a way of charging all 4 batteries without removing them from the enclosure?

Thanks again
```

---
## \#7 Posted by: JensSjogren Posted at: 2019-01-01T21:08:40.366Z Reads: 135

```
The easy way to connect a battery indicator without an bms is simply to cut a small hole in the silicone on the battery wires after your parallel connector, one hole on the positive and one on the negative, after that you solder the cables of your battery indicator to the battery wires, positive on positive and negative on negative naturally.

You can also attach a BMS to your lipos to charge them in place via a DC port, otherwise a balance charger for 6s batteries is what you need
```

---
## \#8 Posted by: pjotr47 Posted at: 2019-01-01T21:14:44.332Z Reads: 124

```
The unity has a extra output for wiring stuff. You can connect you lcd to those ports
```

---
## \#9 Posted by: J_Dizzle Posted at: 2019-01-01T21:29:26.267Z Reads: 119

```
LiPo balance boards often help with charging lipos in parallel
```

---
## \#10 Posted by: JKUK Posted at: 2019-01-01T21:53:24.042Z Reads: 115

```
I'm now considering the BMS option. I've taken someone else's diagram and edited it for what I need.

Can anyone see any issues with the below design and the kit in the shopping list?

![battery|690x424](upload://74byZpSnFNPy7wKGuvmCuMkvK9w.png) 

**Shopping List**
4 x https://hobbyking.com/en_us/zippy-compact-6200mah-6s-40c-lipo-pack-xt90-1.html

1 x 12S BMS https://www.ebay.co.uk/itm/44-4V-80A-Li-ion-Li-Battery-BMS-LFP-PCM-SMT-12S-12x-3-7V-eBike-Board-12x-4-2V/153102683271?hash=item23a5a18c87:g:TeIAAOSwuehbTWF-:rk:4:pf:0

1 x Charge port https://www.ebay.co.uk/itm/1pc-Iron-5-5x2-1mm-DC-Power-Female-Jack-Socket-with-Waterproof-Cover-Ring/282413905239?epid=20002838221&hash=item41c12e3557:g:ya4AAOSwPCVX63VZ:rk:1:pf:0

2 x Harness cable http://www.trampaboards.com/12s-battery-harness-to-make-12s-power-from-2x-6s-batteries-premium-top-quality-strand-copper-with-highly-flexible-silicone-coated-cable-kit-with-50-amp-fuse--beast-or-monster-box-p-25905.html

1 x loop key http://www.trampaboards.com/monster-box-loop-key--fixes-into-the-lid-of-the-monster-box-to-make-the-power-connection-p-25909.html

Any recommendations for a charger that will do the job?


Thanks again
```

---
## \#11 Posted by: topcloud Posted at: 2019-01-01T22:06:24.864Z Reads: 103

```
Fully endorse Graupner, after personally wasting money on AliExpress, Hobbyking and the like:

http://www.trampaboards.com/graupner-ultramat-18-charger--capable-of-charging-2x-6s-batteries-at-once-with-balancing-cables-p-25648.html

Good hunting
```

---
## \#12 Posted by: mikenyc Posted at: 2019-01-01T22:11:37.864Z Reads: 100

```
This is the charger I’m using on my top mount. I’m not using a BMS. Are you in the states?

https://www.amazon.com/dp/B07DR8HW19/ref=cm_sw_r_cp_api_i_fv-kCbY3WHRFC
```

---
## \#13 Posted by: JKUK Posted at: 2019-01-01T22:35:23.895Z Reads: 93

```
Thanks.

Could I use one of those chargers with a BMS later on to charge via an XT90 port? Instead of the charge port in my last reply.

That way I could use one of those for now and later on introduce a BMS whilst using the same charger.
```

---
## \#14 Posted by: JKUK Posted at: 2019-01-01T22:37:40.392Z Reads: 88

```
I'm based UK doesn't look like that hobby mate is available here
```

---
## \#15 Posted by: JensSjogren Posted at: 2019-01-02T09:41:46.076Z Reads: 80

```
Maybe theese batteries are worth to consider (https://hobbyking.com/en_us/turnigy-high-capacity-battery-20000mah-6s-12c-drone-lipo-pack-xt90.html)

They also come in 12ah and 16ah versions, the 12c rating on a battery of this size should in theory be more than enough to supply you with the amps that you need. You would only need to deal with two cells instead of four and with the 20AH version you would increase your capacity with 8AH for that raaange. 

I'm considering buying theese aswell to use as a extended pack on top of my 12s5p 30Q pack that i currently use on my trampa mtb, that pack gives about 25-30km range which is fine for normal use but riding heavy offroad i doubt it would give more than 10km. With your current 12AH option you will be even more limited than i am. 

I can be dead wrong about theese cells but they seem like an excelent option for a great price, anyone has experience with the multi rotor lipo packs?
```

---
## \#16 Posted by: Andy87 Posted at: 2019-01-02T09:58:18.669Z Reads: 71

```
I don’t have personal experience with them, but I could imagine they similar to the big multistar lipos. They advertised with 10-12c but in real life they only can handle 3-4c.
This packs not made for high drain applications, more to charge up your lipos while you on the fields.
If you want high drain high capacity lipos, I would go with tattu lipos only.
```

---
## \#17 Posted by: JensSjogren Posted at: 2019-01-02T12:14:17.987Z Reads: 59

```
Hmm i see your point, however they seem to use the 12AH version of this pack on the patriot board and from the videos they posted it looks like it's performance is good. 

http://skatemetric.com/index.php/2018/12/16/patriot-build-tutorial/
```

---
## \#18 Posted by: Andy87 Posted at: 2019-01-02T12:27:32.900Z Reads: 57

```
Aren’t those this guys who get 9000watt out of two 6374 Flipsky motors? 🤔
How ever... they sure will work, the question is just how good and how long and if you would get cheaper with better lipos in the long run.
But that’s everybody need to find out for his own.
There also people happy driving with the multistar lipos.
```

---
## \#19 Posted by: JensSjogren Posted at: 2019-01-02T12:41:08.345Z Reads: 52

```
Yes they are atleast claiming that they are getting 9000 watts which means 180 amps in total system power. Anyways not here to change the discussion of this thread 🤔
```

---
