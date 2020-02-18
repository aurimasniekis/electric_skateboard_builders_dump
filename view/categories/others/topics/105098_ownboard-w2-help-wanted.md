# Ownboard W2 help WANTED :slight_smile:

### Replies: 27 Views: 217

## \#1 Posted by: dnm Posted at: 2020-01-06T17:01:24.080Z Reads: 35

```
Hi all,

I bought an Onboard W2 in August, and for the most part, I love the board. However, the board has been turning off when braking. After this happens, the board will not turn on for several minutes. The battery is around 60% or 70% when it happens. I had to bail going down a hill because of this, and luckily, only suffered minor injuries. Any advice?

Alternatively, I am in Missouri and will part ways with it for the right price.

Thanks everyone!
```

---
## \#2 Posted by: ZachTetra Posted at: 2020-01-06T22:00:38.881Z Reads: 27

```
It sounds like the controller is getting an over voltage spike maybe?  Does it happen at low battery or if you are breaking really gently?
```

---
## \#3 Posted by: dnm Posted at: 2020-01-06T22:12:49.432Z Reads: 27

```
Thanks for your help!

I usually keep my battery at around 50%. It has happened once when I was gently braking downhill, and another time braking on flat ground. I am so confused by this. I contacted ownboard and they told me to buy a new battery, but I cannot fathom why it would be a battery issue?
```

---
## \#4 Posted by: ZachTetra Posted at: 2020-01-06T22:26:16.688Z Reads: 23

```
It might be a bad connection in the pack, or the BMS is reading some fault and shutting the pack down

You can open the pack and replace the BMS or at least check for signs of damage if they won’t replace it

Alternatively you can try a different ESC, my old board started to cut out and it was my ESC going bad
```

---
## \#5 Posted by: dnm Posted at: 2020-01-06T23:12:51.337Z Reads: 22

```
Can I buy a different battery/bms? I'd like to avoid this problem from reoccurring in the future. Or do I have to use their battery and BMS?
```

---
## \#6 Posted by: dnm Posted at: 2020-01-06T23:13:15.789Z Reads: 23

```
Also, do I even need a BMS? sorry I am a noob to this.
```

---
## \#7 Posted by: ZachTetra Posted at: 2020-01-06T23:22:04.626Z Reads: 22

```
You can buy a new battery from many other sources, including forum members.  I suggest going to the new forum at forum. (you have to copy/paste the URL, the hyperlink is blocked here) to find a new battery 

You done necessarily need a BMS since you can use a balance charger, but a 10s balance charger is much more expensive so you’ll want a BMS.  You can bypass the BMS and rely on the ESC to not pull too much power and you’ll have less points of failure

If it’s not the battery, I’ve got some speed controllers I need to sell off
```

---
## \#8 Posted by: dnm Posted at: 2020-01-07T00:48:43.958Z Reads: 21

```
Again, I really appreciate you taking the time to teach me these things. Can you tell me the exact battery I'll need? Is it a 10s lipo or 10s lion?
```

---
## \#9 Posted by: ZachTetra Posted at: 2020-01-07T02:50:09.655Z Reads: 19

```
You can get any 10s battery, but the standard is using the samsung 30Q cell, you can go to the other forum and ask for someone to sell you one

Either will work, li-ion is a little lower voltage on average but has the same full charge voltage

Usually li-ion will have better capacity (in terms of weight and volume) and lipo will have better discharge.  Li-ion will have more cycles but lipo is cheaper
```

---
## \#10 Posted by: dnm Posted at: 2020-01-07T03:02:10.653Z Reads: 17

```
Ok, so if I buy a 10s LiPo without a bms, as long as I charge them properly, it should work seamlessly with the other components on the board?
```

---
## \#11 Posted by: ZachTetra Posted at: 2020-01-07T03:09:36.907Z Reads: 14

```
Sure, but you will need a 10s balance charger

Alternatively you can buy 2 5s lipos and put them in series, just make sure to charge them at different times (if you charge both at the same time with different chargers, it will short out across the ground of your wall socket power unless they are independent circuits)
```

---
## \#12 Posted by: deucesdown Posted at: 2020-01-07T14:59:37.446Z Reads: 13

```
Have you charged to 100% recently? Could be your pack is way out of balance and when you brake, one cell group goes to 4.2v (cell over voltage protection) and the bms cuts power. After a few minutes the voltage settles and bms resets.

If you charge to 100% the bms will balance the pack. If what I described is happening with the pack at 60%, it may take the bms days to balance the pack. If it's that far out of balance I'd be very concerned about pack health.
```

---
## \#13 Posted by: dnm Posted at: 2020-01-07T18:11:52.308Z Reads: 11

```
Wow, that is very interesting! I always stop charging the pack at 90%, so this could be it... So I will charge it to 100%, and then do I need to leave the board on in order to balance the cells?

Another thing I notice when it happens is that even my battery percentage LCD display goes from 60% to not even lighting up-no power to the lcd display...
```

---
## \#14 Posted by: deucesdown Posted at: 2020-01-07T18:39:26.492Z Reads: 10

```
That confirms my suspicious further.

Typically you need to keep the charger plugged in for many hours, maybe as much as 48 hours. The principle of operation (short version) is, the bms allows slight overcharge, then cuts off charging current while draining down the high cells. This repeats until the cells are more or less balanced. The pack voltage will creep up very slowly during this process. This can be seen on the board's meter. You should see it hit 90% then slowly ever so slowly climb up toward 100%. It may never reach 99%.

You're doing a good thing charging to 90%, but occasionally, say every 15-30 rides, you should charge it all the way up to keep things balanced and check out the health.

You should keep the board turned off during charging.
```

---
## \#15 Posted by: dnm Posted at: 2020-01-07T18:56:56.509Z Reads: 8

```
So, to reiterate, I need to charge my board for 48 hours, and my BMS may actually not be broken?
```

---
## \#16 Posted by: ZachTetra Posted at: 2020-01-07T19:13:32.030Z Reads: 8

```
Possibly, if one of the cells is at a low voltage while the pack is still charged it will trip the safety and cut power
```

---
## \#17 Posted by: dnm Posted at: 2020-01-07T19:19:39.154Z Reads: 10

```
Ok, are there any precautions I should take while charging the pack since the pack may be unhealthy?
```

---
## \#18 Posted by: deucesdown Posted at: 2020-01-07T19:59:00.478Z Reads: 12

```
Since electric skateboards are kind of like lipo RC stuff with respect to battery, the normal precautions are
- be in the same room while charging. Stop charging if you leave the room.
- consider charging outdoors
- have a path planned to outdoors
- have a fireproof blanket to grab the thing with and toss it outside
- fire extinguisher, bucket of sand

Extra precautions you could take, and this is totally up to you:
- take enclosure off
- check temperature of cells, wires, connections, bms during charge (it's normal for the balance resistors of the bms to get quite hot, but not melting stuff hot)
- if anything besides the balance resistors get more than warm, disconnect, worry a lot, read a lot, keep monitoring, store pack outside until you figure out what's up
- check individual p-group voltages often. If any go above 4.3v unplug and be worried. Be careful when measuring -- it's easy to short out multimeter leads
- put a watt meter between charger and pack so you can see how many watt-hours and amp-hours have gone into the pack, and see pack voltage at a glance.

---

It's worth noting, your pack may have a weak/damaged p-group that drains down faster than the rest of the pack, and triggers bms cutoff. Ownboard's advice might have been correct. It's worth doing some diagnostics/maintenance to confirm though.

And I agree with just about everything @ZachTetra has said too.
```

---
## \#19 Posted by: ZachTetra Posted at: 2020-01-07T20:18:31.932Z Reads: 11

```
Follow deucesdown's instructions, he's way more careful then I would ever be, after the pack is charged you'll want to give it a while to balance then charge it again to make sure it's correctly balanced 

If after a couple rounds of that the battery voltage is 42.xx (depends on the exact charger) you're probably good to ride again.  If not you're gonna have to open the battery and check the voltage of each group, be very careful when opening it to not touch anything with metal (I.e. scissors or knives)

If the charge port is a 5.5x2.5 jack I suggest connecting a short length of wire to the probe ends and only stripping the last 1mm so you don't short the port out, normally I use alligator clips to connect everything

Probably much safer and easier to take the battery out and charge it on a kitchen table with the windows open so you can chuck it outside if it starts venting smoke
```

---
## \#20 Posted by: dnm Posted at: 2020-01-08T20:40:55.279Z Reads: 9

```
@ZachTetra and @deucesdown  So I charged my board for a long time and its at 41.8v do I keep charging until 42v+?
```

---
## \#21 Posted by: ZachTetra Posted at: 2020-01-08T20:51:18.838Z Reads: 9

```
Hmm, that's close enough I think it's the voltage drop across the BMS

Define a long time
```

---
## \#22 Posted by: deucesdown Posted at: 2020-01-08T20:57:08.505Z Reads: 9

```
I say if you came this far keep going. Is your charger 42.0 at the charge port?

Also curious how long it took.
```

---
## \#23 Posted by: dnm Posted at: 2020-01-08T22:58:12.883Z Reads: 9

```
It took like 4 or 5 hours to achieve 41.8v, but the board touched 100% battery in the normal amount of time (say maybe 1hr or 1.5 hrs) to go from 60% to 100%.
```

---
## \#24 Posted by: dnm Posted at: 2020-01-10T15:27:28.130Z Reads: 9

```
@deucesdown @ZachTetra   

Update: after another 3 or 4 hours, I've gotten it to 41.9v. Does this seem balanced to you?

Since it may have balanced relatively quickly do you think that my BMS is what's wrong, or could it still have been unbalanced cells?

Thanks so much for all of your help. I am not very skilled in the art of electricity, but I have had a passion for boarding ever since I could walk. :)
```

---
## \#25 Posted by: ZachTetra Posted at: 2020-01-10T15:57:34.907Z Reads: 9

```
Yeah it's probably balanced, go for a ride and drain completely, wear safety gear for it.  Let us know what happens
```

---
## \#26 Posted by: deucesdown Posted at: 2020-01-11T00:30:43.789Z Reads: 6

```
You might have another 4 hours to get to 42v? If so it took a decent amount of time. But to be honest I think it wasn't that badly out with the info you gave. Cell low voltage cutoff right have been a false alarm. I'd charge until the pack voltage matches the charger voltage just to get a 100% baseline, but you can do that in the future.

Pad up and see if it still tosses you off. :slight_smile:

If it still does cutoff, it might be worth the trouble to measure each p-group's voltage on the spot. Or at home but before charging again.
```

---
## \#27 Posted by: dnm Posted at: 2020-01-14T23:51:51.492Z Reads: 5

```
Rode it all day today with no problems, thanks homies!

Since I suspect I wont be ripping into her again, I also finished my board art. :slight_smile:

![pickle%20board|666x500](upload://9Mzrh5uzmXAsa0EiwLC1UhDCkRQ.jpeg)
```

---
