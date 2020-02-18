# 40 Cell Li-Ion 10s4p

### Replies: 19 Views: 3833

## \#1 Posted by: paragon Posted at: 2016-03-27T05:41:02.929Z Reads: 248

```
Hello,
For my next single motor mountainboard build, I'll be building a Li-Ion pack using either LG INR18650HE4 or LG ICR18650HE2 cells. The pack will contain 24 cells in 8s3p configuration and will be housed in these:
https://www.fasttech.com/products/3827700
This pack should handle 60a continuous. Which bms would you guys recommend?
I've been looking at this one:
http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html
```

---
## \#2 Posted by: torqueboards Posted at: 2016-03-27T06:06:01.623Z Reads: 244

```
Nice mountainboard build. I'll be working on one soon as well. Can't wait.. I want to hop onto and off curbs :smile:

You should go 12S for a mountainboard :smiley:

- As for the BMS it looks fine. I've heard of a few people using them but I haven't tried them myself.
- Do those fasttech cell holders have a max amp?
```

---
## \#3 Posted by: paragon Posted at: 2016-03-27T06:35:04.808Z Reads: 235

```
I would, but I'll be running a Tacon 160 245kv (I bought 3 at the $50 when they were in stock last year) and according to this http://www.electric-skateboard.builders/t/vesc-faq-when-to-use-low-voltage-vesc-configuration/1965 I shouldn't go above 10s with a VESC and this motor.
I couldn't find the max amps of the sell holders, but they do look like keysone 1048.
```

---
## \#4 Posted by: delta_19 Posted at: 2016-03-27T06:39:04.535Z Reads: 213

```
oh shit son you're making a pack like mine
[enter link description here][1]


  [1]: https://www.youtube.com/watch?v=OKv0Kb0v8o4

those contacts say copper and gold so they should be fine, mine are nickel plated steel.
```

---
## \#5 Posted by: torqueboards Posted at: 2016-03-27T07:04:25.705Z Reads: 199

```
@Paragon That's only setup for motor detection. I believe, you can run at 12S. I'll be doing more testing. I like me 12S! 8600rpm was only a suggestion as well.
```

---
## \#6 Posted by: NerijusM Posted at: 2016-03-27T14:00:29.809Z Reads: 189

```
And go with biggest reduction as possible - like 6:1 or 7:1. I`m using 6:1 with 192KV and 12S lipo - quite good, but thinking about 7:1.
```

---
## \#7 Posted by: paragon Posted at: 2016-03-27T15:11:56.246Z Reads: 185

```
With my current 5.5:1 gearing, I'd break 47mph on 12s 😂
```

---
## \#8 Posted by: Hummie Posted at: 2016-03-27T15:25:46.719Z Reads: 189

```
Really? I was reading Chaka saying here that doing 8600/voltage= max kv     And thought it was important to keep under that.  Maybe if u never end up at top speed u could have a higher kv but I thought the commutation was too quick for the vesc.  

Delta the thread on es about spot welding 18650...I think the nickel covered steel is high resistance. More so than nickel.  https://endless-sphere.com/forums/viewtopic.php?f=14&t=68005&hilit=Spot+weld+18650    Nickel isn't so good either.  All compromises so that they are weld able.  And ur not welding either I think.

Lg hg2! Maybe more expensive but more energy.  I got 48 from some vape store
```

---
## \#9 Posted by: chaka Posted at: 2016-03-27T15:31:11.900Z Reads: 179

```
Running the Tacon 254kv motor at 8s will need an 80 amp max to run well and have sufficient power I would run at least 8s4p with 20amp cells. 10s would be better for the VESC, less chance of overheating. 

Running a motor with a kv higher than 200kv at 12s can induce some drv8302 fault codes. When I get a chance I will see if I can replicate the fault that others have reported. It may be possible to limit erpm to eliminate the fault code/failure.
```

---
## \#10 Posted by: paragon Posted at: 2016-03-30T12:14:18.336Z Reads: 165

```
Thanks for the info.
I ordered enough cells to build a 10s4p battery with lg he4 cells.
```

---
## \#11 Posted by: paragon Posted at: 2016-03-30T14:45:52.645Z Reads: 162

```
Also, because I'll be running a bms, will I be able to charge the pack with a higher voltage charger?
My pack will be 42v when full, but my charger is a 48v charger (I think it charges up to 58.8v).
Perhaps I could use a dc step down?

Otherwise I'd have to build a 7s5p pack to use with my 24v charger.
```

---
## \#12 Posted by: chaka Posted at: 2016-03-31T14:23:40.662Z Reads: 159

```
You need to pair your charger with your target voltage. You have a charger for a 14s pack, get a 10s charger, 42v. They run anywhere from $70 on up $$$. Note that you don't want to charge them too fast either so do some math and be sure you are not trying to drive to many amps into your pack otherwise the bms will not have the needed time to balance the pack as it reaches full charge. This is all determined by the wattage of the charger.
```

---
## \#13 Posted by: paragon Posted at: 2016-03-31T15:25:28.770Z Reads: 148

```
Would a "hoverboard" charger suffice (42v 2a so kinda slow)?
I'll be using a bms so no need for an expensive balance charger.
```

---
## \#14 Posted by: chaka Posted at: 2016-03-31T17:08:07.309Z Reads: 145

```
That would be a little under 0.5C charge rate so it should work fine,  almost ideal for long life if you can make it work.
```

---
## \#15 Posted by: paragon Posted at: 2016-04-01T00:44:04.672Z Reads: 136

```
Has anyone tried splitting their li ion packs, using two bms, then connecting in parallel?
Then I'd be able to get 2 small 10s 40a bms instead of a single large 80-100a bms.
```

---
## \#16 Posted by: Hummie Posted at: 2016-04-01T16:40:13.249Z Reads: 137

```
You could...
Do what I do and get a "power supply" as Apposed to a charger Meanwell sells adjustable ones or hoverboards as u say for like 20 bucks off amazon.  Mine does 1.5 amps and for a bit more and a bit bigger there's some that do 2.5.  This is 48 volts though and maybe 10s be easier.  I'd get a wattmeter and add it to your board main power and then you can see what's coming in as well as going out.  
bms or rig up a battery-medic or some other resister to do it.
```

---
## \#17 Posted by: longhairedboy Posted at: 2016-04-01T16:57:15.911Z Reads: 135

```
Something else you could do is just split the cells into two groups and run extension wires for the mains and balance leads and just keep one BMS on one side. 

but then again i don't know what the use case here is. If you want to allow flex in the deck, either situation would work. You could also just allow a little bit of space between each cell group or even box them individually in a sort of ribbed configuration to allow flex to happen.
```

---
## \#18 Posted by: paragon Posted at: 2016-04-02T00:08:12.515Z Reads: 130

```
No flex. It's just that two 10s 40a continuous bms can be bought for $40-50, but one 80a cont. will cost $80-100 and be bulkier.
```

---
## \#19 Posted by: Hummie Posted at: 2016-04-02T00:34:09.364Z Reads: 126

```
Sorry I was answering some other question above. I don't know about bms and splitting the pack.
```

---
