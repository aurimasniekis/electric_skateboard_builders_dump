# Calculating battery max for vesc with a li-ion pack

### Replies: 36 Views: 744

## \#1 Posted by: samr Posted at: 2019-07-14T21:28:14.132Z Reads: 146

```
Looking to upgrade my board to vesc but having some difficulty determining the continuous current from the battery. I've been watching this tutorial: https://youtu.be/_mNnHp7sOBE which seems to use a LiPo battery to calculate (with C rating). Unfortunately, I have a li-ion pack which doesn't have a C rating on it. Below are pictures of the labels on the battery. I couldn't find a datasheet online for it and I bought it second hand so I don't have the store listing.

![image|690x387](upload://nBa6NuRl7d9ya8oSPCipGH5JUsP.jpeg) 
![image|690x387](upload://5ElYcnZcsaymxBkY172Kq9T5PG2.jpeg)
```

---
## \#2 Posted by: Tinp123 Posted at: 2019-07-14T21:48:58.535Z Reads: 136

```
Your best bet would be to remove that blue wrap and see which cells are inside. Then you can google cell model and see its discharge rate
```

---
## \#3 Posted by: samr Posted at: 2019-07-14T22:11:23.119Z Reads: 133

```
I may have actually found the datasheet. http://www.hyybattery.com/Electricvehiclebattery_67.html

It says "5C discharge after full charge." So doing the calculation in the video, I would get (4ah * 5C)/2 motors = 10A max discharge? Does that seem right?

I really don't want to take off the blue tape as I will need to fly with this battery next month.
```

---
## \#4 Posted by: Tinp123 Posted at: 2019-07-14T22:19:44.539Z Reads: 127

```
Where did you see 5C discharge? All I can see is 0.5C or 2A. That is way too low for any esk8 use.
```

---
## \#5 Posted by: samr Posted at: 2019-07-14T22:23:24.441Z Reads: 123

```
This came from a paean H2B (cheap chinese board) so I would like to think that it's good enough for esk8 but you never know with these cheap chinese companies :sweat_smile:

![image|690x325](upload://xsuxQ4XwbuEIRY55n3qtE5TUmZn.png)
```

---
## \#6 Posted by: Tinp123 Posted at: 2019-07-14T22:27:41.442Z Reads: 117

```
That can't be same battery 😅 your battery has 4000mAh,this battery with 5C discharge rate has 4400mAh. That means different cells and different discharge rate
```

---
## \#7 Posted by: MysticalDork Posted at: 2019-07-14T22:40:32.458Z Reads: 116

```
Looking at the specs in the link you posted, it clearly says "maximum discharge current 2000mA." That means that you get one amp per vesc. The datasheet for the different battery lists 5C, and a maximum BMS discharge of 45A, which don't match up either with each other, or the earlier 2A number. This is the problem with buying cheap undocumented batteries likely with fake cells. You have no real idea what you have, and thus no real idea how to treat it.

I'd say limit yourself to 10A per vesc. If you want more performance/range/whatever, save your pennies and buy a proper battery from a reputable source.
```

---
## \#8 Posted by: samr Posted at: 2019-07-14T23:03:48.806Z Reads: 110

```
So then what would happen if I were to pull too much from the battery? Would it get hot and explode or would it just stop working?
```

---
## \#9 Posted by: accrobrandon Posted at: 2019-07-14T23:07:46.723Z Reads: 107

```
The cells Will get hot...depending.how long you push them past their max value a variety of things could happen...

They get over worked but not pushed past the point of no return and they die way quicker than needed...

U push them hard and then something melts amd the pack dies...

U push it to hard...they get too hot and then thermal runaway happens and then its nuclear melt down...

Probably not a lilely "explosion" like a bomb but a fire will start and you'll be like "whats happening... Why is is my board smoking... Oh shit its on fire! Run!"
```

---
## \#10 Posted by: samr Posted at: 2019-07-14T23:56:56.144Z Reads: 88

```
Oh well that's fun. Is there any way to get the settings off of the currently installed esc or is it built into the hardware?
```

---
## \#11 Posted by: MysticalDork Posted at: 2019-07-15T00:26:01.401Z Reads: 88

```
Really depends on the board, but overwhelmingly unless it's based on vesc hardware/software, the answer will be either it's in hardware, or it's buried in some proprietary firmware.

Just set your vesc conservatively and check your pack during/after your test ride. If it's hot, then you're doing damage to your pack.
```

---
## \#12 Posted by: samr Posted at: 2019-07-15T00:30:04.387Z Reads: 82

```
Yeah it's one of those cheapo yiling ones that the old meepos use. I'll start it at 10A and do a test to see if I can bump it up.
```

---
## \#13 Posted by: MysticalDork Posted at: 2019-07-15T00:42:27.153Z Reads: 77

```
Honestly, with unknown cells, 10A per vesc (20A total) is probably pushing the maximum I would be comfortable with.

It's just not a very large battery, capacity/cells wise, and 10A per cell is pushing them pretty hard if they're not designed for high discharge. 

Even quality name-brand cells that aren't designed for high discharge top out around 7-10A before you start really doing damage.
```

---
## \#14 Posted by: samr Posted at: 2019-07-15T00:46:00.532Z Reads: 73

```
Oh alright. This is my first board so I don't really know what I'm doing. What would you suggest that I start at? Maybe 5A?
```

---
## \#15 Posted by: MysticalDork Posted at: 2019-07-15T00:47:10.536Z Reads: 71

```
5 or 7. You could go straight to 10, but just be careful and check to see if anything is getting hot.
```

---
## \#16 Posted by: MysticalDork Posted at: 2019-07-15T00:51:33.438Z Reads: 69

```
You should be aware that given the budget constraints and hardware you already have, this board is **not** going to perform impressively, unless you upgrade pretty much everything but the deck and wheels. There's only so much you can do with a shitty battery and the cheapest possible vescs.

Switching from a noname ESC to a vesc will make it smoother and more responsive, but you're limited by the battery, a LOT. Those vescs M.Hboards linked in the other thread are good for **fifty amps**. You're planning to feed them a maximum of **ten**.
```

---
## \#17 Posted by: samr Posted at: 2019-07-15T00:58:03.123Z Reads: 66

```
I see. If I were to upgrade the battery down the line, would I ever want to be pulling more than 50A? Just trying to decide if it's worth an extra $40 to get up to 100A.

https://www.aliexpress.com/item/32951134782.html vs https://flipsky.net/products/dual-fsesc4-12-100a?variant=9022834638908
```

---
## \#18 Posted by: MysticalDork Posted at: 2019-07-15T01:03:18.504Z Reads: 72

```
The 4.20 dual is a better design than the 4.12 singles, but with your current setup that's like asking if you need a Cummins 6.7 or a Duramax 7.8 to put in your vespa. You will not reach the limit of either, because you're limited by your battery.

My last build had a 10s4p battery with genuine Samsung cells, capable of delivering 40A per motor, and it was absolutely fantastic. More power is definitely better - not only will it improve your acceleration, but also your brakes. Your brakes will be really bad with that battery, because your braking power is based on how much power you can regenerate into the battery pack, and that pack is only good for maybe two or three amps per motor of regen.
```

---
## \#19 Posted by: samr Posted at: 2019-07-15T02:37:21.931Z Reads: 72

```
Alright, I just read through https://www.electric-skateboard.builders/t/new-user-looking-for-battery-read-this-complete-walkthrough-of-batteries/26010 and I see the problem. I think I'm going to run the current battery + esc through a clamp amp meter to see what it draws from the battery.

I guess I'm willing to put some money into this if I can make it a beast. Really all that's left to salvage are the motors. Are the ones that I have decent? I believe they're these: https://flipsky.net/collections/e-skateboard/products/copy-of-bldc-belt-motor-6374-190kv-3250w
```

---
## \#20 Posted by: Hummie Posted at: 2019-07-15T02:48:08.824Z Reads: 64

```
Look at live data on Vesc at the erpm n add a resistance, maybe a glove isn't ideal, and see what the voltage does at ten or twenty amp draw.  Maybe not a glove. Bluetooth data while riding
```

---
## \#21 Posted by: MysticalDork Posted at: 2019-07-15T03:57:49.176Z Reads: 59

```
Oh yeah, those will be pretty good. 

My list of motors goes like this:

Single 5055: Double Meh.

Single 5065 Meh.

Single 6355: Good.

Single 6374: Very Good.

Dual 5055: Good.

Dual 5065: Better.

Dual 6355: Great!

Dual 6374: Overkill!

You won't quite get to "beast" territory with 5055s, but it will be really fun.
```

---
## \#22 Posted by: samr Posted at: 2019-07-16T05:01:42.591Z Reads: 52

```
Alright I've got the VESCs, remote, and misc connectors ordered. Now on to the battery. I need to stay under 160Wh to take it on the plane and I want to buy a premade pack - any suggestions? Ideally, I would stay somewhere around $150 but I can spend a little over $200 if needed. Since those ESCs are in parallel, the maximum that they will pull from the battery is 50A right?

Also, I have one of those battery meters (with 4 LEDs), is there an easy way to hook this up to these VESCs?
```

---
## \#23 Posted by: Hummie Posted at: 2019-07-16T14:09:44.300Z Reads: 48

```
 @samr  U didn't figure what cells they are and are assuming they won't cut it.  Why not run them at a certain load and see what the voltage does like I said above and then u will know what amount of current u can comfortably pull from them.  Your brakes could be fine.  Regen current is for a short time and u could set up the motor regen higher and battery lower to compensate at least. 

If you hook up a clamp amp meter it should read similar results to what the Vesc records and don't see the point unless ur seeing how accurate the Vesc is recording that

The max the escs will pull is determined by ur settings and load.

 if youre trying to get it plane possible it will either have to be made with super powerful cells or else 100 watthour packs that can be disassembled.  you can have two that are 160 watthours I read
```

---
## \#24 Posted by: MysticalDork Posted at: 2019-07-16T20:48:37.599Z Reads: 41

```
You can set the vescs to draw whatever current you want. Anything up to the physical/thermal limit of the vesc/motor/battery.

You don't hook up the battery meter to the vesc, you hook it up to the battery. Specifically across the battery wires after the loopkey.

@Hummie it was my own homemade pack with INR18650-25R cells. As for regen, I played around with low battery and high motor settings. They're awful.
```

---
## \#25 Posted by: Hummie Posted at: 2019-07-16T20:56:52.167Z Reads: 42

```
O I mistaken posted the last message to u but meant It for Sam related to his unknown pack he could see what it was by watching voltage sag
```

---
## \#26 Posted by: MysticalDork Posted at: 2019-07-16T21:10:00.768Z Reads: 42

```
Ahh right. Yeah a clamp meter is a wonderful tool to have. I've got a little Uni-T AC/DC one that's great!
```

---
## \#27 Posted by: samr Posted at: 2019-07-17T19:20:43.612Z Reads: 40

```
Yeah I'm just waiting for that clamp meter (ordered it on Amazon) so I thought I would spec out a battery in case I need it.

My plan is to hook the battery up to the stock ESC and run full speed forward as well as some brake tests. I'll take peak current draw and post them here.

I should have the meter on Monday and I'll post my readings here and you guys can let me know what you think.
```

---
## \#28 Posted by: samr Posted at: 2019-07-22T05:40:41.092Z Reads: 37

```
I just got my VESCs today and noticed that they didn't come with a CAN cable (JST-PH 4-pin). Is that the best way to connect them or should I split the PWM output from the remote? Also, I thought that CAN just used 2 pins, why does this connector have 4?

I'm still waiting on the battery measurements (the clamp meter that I bought only measures AC :frowning: I'm going to borrow one from a friend on Tuesday)
```

---
## \#29 Posted by: MysticalDork Posted at: 2019-07-22T05:57:04.953Z Reads: 37

```
The connector has power ground and two data pins - You only need the two data pins, the middle ones IIRC.

Split PPM works but you only need the signal wire to go to the second vesc, if you have all three (power, ground and signal) you can have problems with ground loop.

Yeah, not all clamp meters measure DC. I have a Uni-T UT210E that works great if you decide to get one in the future.
```

---
## \#30 Posted by: samr Posted at: 2019-07-24T02:29:41.056Z Reads: 35

```
Alright so I just got back from the "dyno" and unfortunately, I was only able to test the power out and not the recharge. When testing, the motors stalled out when the ESC pulled 22.5A from the battery. Since my VESCs are going to be in parallel, I will be dividing the current by 2 so a good place to start would probably be 7A each? If all goes well with that, I might try and bump it up to 8 or 9. Does this sound like a good way of going about this?

The next thing that I need to determine is the brake/recharge current. The charger that came with the board is rated at 2A so I know that I can at least put 2A back into it. I was thinking of starting it at 2A and logging battery temperatures while I go down some hills. Then I'll slowly bump it up and repeat the test. Will the battery heat be a good indication of what the battery can take?
```

---
## \#31 Posted by: MysticalDork Posted at: 2019-07-24T02:51:41.001Z Reads: 34

```
7 and 2 (per motor) should be a good conservative starting point. Heating is a good indication in terms of discharge, but unfortunately won't tell you much about regen.
```

---
## \#32 Posted by: Hummie Posted at: 2019-07-24T03:42:41.310Z Reads: 34

```
  if you want to figure what cells they are and what charge and discharge they can take, cant you open them up a bit and see their color?  if that isn't possible you should be able to tell by seeing what the voltage drop is under a certain load like I said.   that seems the easiest best revealer really beyond the wrap.   

regen current is for such a short time and not the same as a full charge cycle and the cell's rating on that.  even that can be taken with salt when at a low state of charge especially.    I think heat is the indicator of a lot of damage that is done to a cell whether charging or discharging and you really have to get to some highly untouchable temps to be in danger in danger I think.
```

---
## \#33 Posted by: samr Posted at: 2019-08-04T19:47:30.464Z Reads: 22

```
I've got everything wired up and I put new firmware on the VESCs. Just waiting for the CAN connectors to come in the mail and then I should be ready to ride.

I also ordered one of these to use with the VESC skateboard apps: https://www.aliexpress.com/item/32962465399.html?spm=a2g0s.9042311.0.0.39bf4c4dBMt89X. That uses the same serial COM port as the receiver. Is it possible to connect both of these through the same COM port or will I only be able to use one? Would it be possible to connect the receiver to the master VESC and then connect the bluetooth module to the follower VESC? I couldn't find anything on the forum but I'm sure this has been asked before.
```

---
## \#34 Posted by: samr Posted at: 2019-08-06T00:53:01.158Z Reads: 18

```
I've got it running but it's hitting the 7A limit when trying to move without a person on it. Should I bump it up or is there something wrong? It could move a little bit (with no rider) but only if I very slowly ramp up the speed that I'm feeding it.

Based on this video: https://youtu.be/LzXEtWjkj4g?t=350, I think I'm going to try and bump it up to (on each esc):

    Motor current max: 15A
    Motor current max brake: 10A
    Absolute max current: 20A
    Battery current max: 20A
    Battery current max regen: 10A
```

---
## \#35 Posted by: samr Posted at: 2019-08-07T02:03:34.454Z Reads: 14

```
Well it looks like I might need to replace the battery pack :frowning:. I think the "random esc shutoff" was because of low voltage.

The VX1 shows only one red light and after riding for a few mins, it starts flashing.

I fully charged the battery and then checked the voltage and got 40.3V. According to https://batteryuniversity.com/learn/article/charging_lithium_ion_batteries, that's about 70% capacity. Are there any other measurements that I should take to figure out if this battery is bad?
```

---
## \#36 Posted by: Santino Posted at: 2019-08-07T16:32:13.777Z Reads: 12

```
I suggest you to read and learn more about batteries and the different set ups for Esk8. If there it is something I do not want to play and push limits, and have a problem, it is with batteries. Why? Because a fire could kill you and others... You need to learn....read....and then buy or build...This is a serious matter, and I wish you to play safe...
```

---
