# Accidentally left board on for a few days and now battery won&rsquo;t charge

### Replies: 22 Views: 575

## \#1 Posted by: kaaaaahle Posted at: 2019-01-12T16:03:26.542Z Reads: 251

```
Hey all,

As the title suggests I accidentally left my @psychotiller  12s5p (charge-only BMS) board on for a few days and it got drained completely. The board won't turn on, and when I plug the charger in it flashes red for a second then goes back to green. A couple other chargers I plugged in just seem to flash red a lot. Anyone know what's going on? Did I kill the pack by draining it too much? :disappointed_relieved:

@Lunasi @skatardude10
```

---
## \#2 Posted by: J_Dizzle Posted at: 2019-01-12T16:11:36.687Z Reads: 248

```
You should be able to bring the pack back by trickle charging, just find a really low amp charger and plug it it
```

---
## \#3 Posted by: Lunasi Posted at: 2019-01-12T16:17:51.950Z Reads: 243

```
@barajabali
```

---
## \#4 Posted by: Sascha_stevenson Posted at: 2019-01-12T16:24:30.580Z Reads: 238

```
I've seen somewhere you can ask a friend to tow you with a car and with a rope turning the motors into generators. not sure if this is the best idea, but it might work. hope you get it fixed :+1:
```

---
## \#5 Posted by: kaaaaahle Posted at: 2019-01-12T16:30:18.753Z Reads: 234

```
i have a 4A charger and a 2A charger. the 4A just stays green light when i plug it in, but the 2A is flashing red (fast flash) so i guess it's at least trying to trickle charge... will report later
```

---
## \#6 Posted by: barajabali Posted at: 2019-01-12T16:39:06.678Z Reads: 230

```
Yea you may have killed it. Gotta measure voltages
```

---
## \#7 Posted by: Surfer Posted at: 2019-01-12T16:44:18.563Z Reads: 226

```
The battery voltage is under voltage recognition by your charger. Try to charge or with a hobby charger configuring it like it was a battery with less cells ( lower voltage) and then it should start charging, keep it for short period, just to get higher voltage and then use your brick charger again, as usual.
I hope it works.
Not bad idea hold until a battpro shows up.
Btw maybe next time try @Martinsp push to start and auto switch off antispark.
Is really cool idea, well you know it :)
```

---
## \#8 Posted by: Battosaii Posted at: 2019-01-12T17:08:50.269Z Reads: 213

```
You can get an adjustable power supply and trickle charger it at low amps. 

https://www.ebay.com/itm/0-5A-0-60V-10A-30V-Lab-Adjustable-DC-Power-Supply-Line-Variable-Digital-Voltage/382416128861?hash=item5909c70b5d:m:mcVpfX1fKKzjnxknJU1zMwg
```

---
## \#9 Posted by: Deodand Posted at: 2019-01-12T17:16:08.215Z Reads: 204

```
Yeah your battery will have sustained some damage (capacity will be a bit derated) but you should trickle charge it as soon as possible. Did this to one of my 10s4p packs and its still kicking. Keep a close eye when you trickle charge feeling the pack from time to time, you want to make sure there is no hotspots in the pack etc. 

One of the reasons I really like auto-turn-off on the unity because I've got a terrible memory for those type of things  :smile:
```

---
## \#10 Posted by: Battosaii Posted at: 2019-01-12T17:16:50.815Z Reads: 196

```
I have to set up the auto turn off you guys got me paranoid lol
```

---
## \#11 Posted by: Deodand Posted at: 2019-01-12T17:24:15.851Z Reads: 196

```
https://www.amazon.com/DROK-DR-US180076-Numerical-Regulator-Adjustable/dp/B01DZSFDE6/ref=sr_1_17?ie=UTF8&qid=1547313598&sr=8-17&keywords=current+limiting+power

Cheaper solution. Set to 1 amp and 30V and wait like an hour then your regular charger should work again. You would need another dc supply for this to work though actually :smile:
```

---
## \#12 Posted by: Sn4pz Posted at: 2019-01-12T17:26:36.965Z Reads: 193

```
So this will for sure never happen when using the Unity and the built in power switch? :thinking:

Very nice if so :smile:
```

---
## \#13 Posted by: Deodand Posted at: 2019-01-12T17:31:47.278Z Reads: 190

```
Never is a strong word, I'll say shouldn't ever :smile:

I guess if you turned the auto-off timer way up then kept powering up the board over and over on dead battery, or if you held the power switch in (got pressed in lodged in your trunk or something) those are two scenarios where over-discharge could occur.  @Blasto made a little circuit for low power BMS where you can take the discharge signal from the BMS and and even get cell-level turn-off etc. That is what we use in the raptor 2 bms.
```

---
## \#14 Posted by: kaaaaahle Posted at: 2019-01-12T19:39:15.417Z Reads: 174

```
OK so my battery is charging again normally with the 2A charger!! It really was doing a "trickle" charge, with the flashing red light. But the light is solid red now. Good thing I have multiple chargers cause the 4A wasn't doing anything. Case closed!!!
```

---
## \#15 Posted by: psychotiller Posted at: 2019-01-12T19:59:36.762Z Reads: 161

```
Batteries dead dude....Edit...now i've read all of the thread. Forgive me.  I would definitely keep an eye on the pack now though as some (or just one) of the cells could be severely damaged.

Let me know!!
```

---
## \#16 Posted by: Psmrman90 Posted at: 2019-06-19T17:54:44.254Z Reads: 98

```
I have a 11s3p 30q with charge only bms that I drained to 1%, maybe lower.  I plugged it into my charger as soon as I got home and let it charge overnight.  Now when I plug it into the charger, the charger only charges it to 42% and then goes green like it's at 100% but my ackmaniac phone app tells me it never gets above 42%.  Any advice on how to fix it?  Is the bms fried?  Should I charge it past 42% by going down a big hill and using regen braking?
```

---
## \#17 Posted by: kaaaaahle Posted at: 2019-06-19T18:21:51.860Z Reads: 88

```
Sorry man but the battery pack is done for. The pack won't charge fully because some of the cells are damaged and are below their nominal voltage. you'll have to take out each cell and figure out which ones are damaged if you want to repair it.
```

---
## \#18 Posted by: Psmrman90 Posted at: 2019-06-19T18:59:42.264Z Reads: 82

```
Well that sucks, at least it charges almost halfway, still get 8 miles out of it if I'm careful. Lets say I don't have the know how to repair it (dont have a welder and never wired a battery before) what are my options? Send it to someone who can fix it?  Dismantle it and sell the indiviudal cells for a ciulle bucks each?  Use this as a chance to learn about the battery and try to take it apart since there not a lot to lose?
```

---
## \#19 Posted by: bartroosen12 Posted at: 2019-06-19T19:49:10.597Z Reads: 76

```
Hi man,

First measure the voltages of each cellgroup, maybe there's just 1 cellgroup which is already 4.2V while the other cells are like 3.8V so the charger will stop charging to prevent overcharging.

Then charge every cellgroup seperately, maybe set your max battery current a bit lower because slightly damaged cells can't deliver full power and will cause outbalancing again.
```

---
## \#20 Posted by: mishrasubhransu Posted at: 2019-06-20T04:08:33.985Z Reads: 51

```
If the discharge was a very low current, the battery doens't suffer from much damage(i.e. Internal resistance doesn't go up much) and can be brought back by trickle charging(like charge it at 0.01C, where C is the capacity of battery). I have have that mistake on couple different battery packs and got it back that way. I didn't observe any significant reduction in capacity or significant increase in IR.
```

---
## \#21 Posted by: clistpdx Posted at: 2019-08-18T23:28:58.227Z Reads: 37

```
did you get your battery running again? I've got an 11s3p that I had on my shelf for the last 6 months and despite charging it overnight it still only puts out about 2V. Wonder if you found any success or just scrapped the battery
```

---
## \#22 Posted by: kaaaaahle Posted at: 2019-08-19T14:12:28.758Z Reads: 27

```
nope. i just scrapped the battery
```

---
