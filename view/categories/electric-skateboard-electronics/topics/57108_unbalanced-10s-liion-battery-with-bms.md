# Unbalanced 10s Liion Battery with BMS

### Replies: 50 Views: 1837

## \#1 Posted by: markyoe Posted at: 2018-05-29T06:50:26.673Z Reads: 194

```
I built a 10s4p battery last year with 25R cells and hooked up a [SuPower BMS](http://www.batterysupports.com/36v-37v-42v-10s-30a-10x-36v-lithium-ion-lipolymer-battery-bms-p-265.html). The battery probably has 100-150 cycles on it. It hasn't been charging up to 100%. Usually it only gets to 89-90% before my charger turns off. I checked the cells' individual voltages and here's what I got. At the time I think my battery indicator was saying that I had 54%.

3.7
3.9
3.8
3.8
4.1
4
4.1
4
4.1
4

Is the BMS bad? What should I do? @barajabali in[ this](http://www.electric-skateboard.builders/t/are-my-cells-unbalanced/17235/11) thread suggested that the pack should be discharged until **completely** dead, and then charged. Is that not bad for the battery?

Thanks in advance.
```

---
## \#2 Posted by: b264 Posted at: 2018-05-29T07:08:23.760Z Reads: 184

```
What are the cell voltages after you charge it?  How long did it sit on green when you measured?
```

---
## \#3 Posted by: chinzw Posted at: 2018-05-29T07:14:15.330Z Reads: 182

```
Its a problem with how SuPower bms' work.
They over charge the cells to 4.25 and then balance down from that. The problem is that if one cell is higher than the rest it will hit 4.25v first and stop charging any other cells. So in order to get all cells to the same voltage you have to go through this cycle of getting to 4.25v and wait for it to balance. Rinse and repeat until you have a balanced battery.
Pretty crappy way to balance if you ask me.
```

---
## \#4 Posted by: Eboosted Posted at: 2018-05-29T07:15:19.862Z Reads: 174

```
Hello, this is what has been happening:

1. Your cells got unbalanced, I bet you had nickel strips connecting the individual packs. BTDT
2. The sum of all 10 packs give you the total battery voltage, if some have lower state of charge they will not charge fully and the higher state of charge won't go over 4.3v, that's why you get a lower capacity after fully charge your board. 
3. Some cells have been overcharging, this is dangerous for the cells during charging as they were being charged more than 4.2v, this could lead to eventual fire. 
4. If you have riden long enough to deplete the battery to zero (2.8v each pack usually) the lower charge packs could have gone down even lower than 2.5V (any battery going down less to 2.5v needs to be replaced), you might even  see 20% of battery remaining on the indicator.
5. Lowering any battery excessively might not kill the battery immediately but will wear it out pretty fast. 

I've been runing with my current Trampa board BMS less, one of the indicators to perform balance procedure on the packs is precisely this, checking the SOC of the battery fully charged, if it's not 100% consistently open the enclosure and check for unbalanced packs urgently
```

---
## \#5 Posted by: markyoe Posted at: 2018-05-29T07:38:12.957Z Reads: 151

```
Thanks for all the responses so far.

@b264 I'll check that in the morning. It will have been sitting green for 10-12 hours.

@chinzw So you're saying that I should look into getting a different BMS? I think a lot of people use SuPower.

@Eboosted Makes sense. Any remedy for an unbalanced pack?
```

---
## \#6 Posted by: Eboosted Posted at: 2018-05-29T07:51:30.463Z Reads: 148

```
[quote="markyoe, post:5, topic:57108"]
@Eboosted Makes sense. Any remedy for an unbalanced pack?
[/quote]

How are you connecting each battery pack? I had way too many unbalanced packs before, my assumption is that a nickel strip has too much resistance to connect packs properly, since I started using silicone wire to connect the packs they have been balanced to milivolt levels even with no bms, the Samsung 30q also have a reputation to keep balance over time.
```

---
## \#7 Posted by: markyoe Posted at: 2018-05-29T07:53:32.907Z Reads: 143

```
I used 12AWG grounding battery braid for the parallel connections and 10AWG silicone wire for the series connectors.
```

---
## \#8 Posted by: Eboosted Posted at: 2018-05-29T07:59:04.028Z Reads: 140

```
Try to post a picture. 

The easiest way to balance each pack is to connect a load, it could be a car light bulb an electric fan or any other load, bring the SOC of the higher cells down to the lowest pack.

The  garage your battery with the enclosure on, so you could monitor the individual voltage of each pack, you should get 100% if all cells are still in good condition.
```

---
## \#9 Posted by: markyoe Posted at: 2018-05-29T17:19:04.155Z Reads: 123

```
The cell voltages after I charge it are:

4.1
4.1
4.2
4.1
4.4
4.5
4.5
4.4
4.5
4.4

:confused: It sat on green for several hours.
```

---
## \#10 Posted by: b264 Posted at: 2018-05-29T17:22:25.473Z Reads: 124

```
You need to bleed those that are over 4.2 down with a small 12V incandescent light bulb or something

Then once none are above 4.2, carefully remove the BMS and throw it in the trash can.

It's likely your cells are damaged.

Put a new BMS on the battery.

What charger are you using?  I'm not sure why your charger would go over 42 volts.  Are you using something besides a lithium-ion charger?
```

---
## \#11 Posted by: markyoe Posted at: 2018-05-29T17:30:00.992Z Reads: 122

```
I don't think the charger went over 42V because the total voltage was 43.2. I'm using a charger I picked up from [here](https://www.electric-skateboard.builders/t/battery-bms-and-charger-sale-take-my-stuff/22553) from @JLabs 

Ok, I'll bleed those down and trash the BMS. So SuPower is no good? Is there a BMS that you would recommend? Maybe a [Bestech](http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/) one?

![IMG_0717|500x500](upload://lhjqkNo8YJSNZKvQ8IcRm30uj2.JPG)
```

---
## \#12 Posted by: b264 Posted at: 2018-05-29T17:37:41.338Z Reads: 113

```
Do you run the discharge current through the BMS or have it bypassed?
```

---
## \#13 Posted by: markyoe Posted at: 2018-05-29T17:38:09.918Z Reads: 115

```
I bypass it
```

---
## \#14 Posted by: b264 Posted at: 2018-05-29T17:45:55.288Z Reads: 117

```
If you bypass it the Bestech 10S "D190" is a good one that I know works.

After you get your cells bled down to 4.2V each you should briefly connect the charger again long enough to measure what voltage it is sending out to the battery.  It seems to be more than 42V.  Don't leave it connected for any non-negligible amount of time.
```

---
## \#15 Posted by: markyoe Posted at: 2018-05-29T17:47:56.943Z Reads: 114

```
If I measure the voltage coming from the charger **without** it being plugged into my battery, would that be an accurate reading?
```

---
## \#16 Posted by: b264 Posted at: 2018-05-29T17:49:33.466Z Reads: 110

```
No it won't.  The charger will probably not put out its full voltage without being connected.  Certainly try, but probably not.
```

---
## \#17 Posted by: Jumpman Posted at: 2018-05-29T17:50:02.608Z Reads: 114

```
I don’t get it.  Are you using a 6s charger?
```

---
## \#18 Posted by: deucesdown Posted at: 2018-05-29T18:00:44.988Z Reads: 117

```
[quote="markyoe, post:9, topic:57108"]
4.4
4.5
4.5
4.4
4.5
4.4
[/quote]

wtf.... this is frightening and the reason I'm so scared of BMS. It looks like BMS is bypassed for charging and you're just bulk charging. Are you sure BMS is in the charger's path? It should have cut off the incoming power when any cell hits the per-cell over-voltage-protection, I think usually 4.25v. This is the BMS's primary job (protect cells from dangerous conditions, protect whole pack from dangerous conditions)

If you're connected properly, this BMS killed your pack.

supower bms has a good reputation...

Also, if your pack needs anything other than trivial amount of balancing, these bms with the tiny per-cell bleed current cannot keep packs in balance. Given the voltages you showed, your pack is likely not manageable by BMS anymore.
```

---
## \#19 Posted by: b264 Posted at: 2018-05-29T18:05:36.452Z Reads: 111

```
It's likely this is a result of the BMS not working and/or not being connected correctly, but whichever it is, it's been happening for a long time.  They have been drifting for a long time.

Not using a BMS is more risky than using one.  It just appears this one isn't working.

@markyoe Do you have photos of how the BMS is wired?
```

---
## \#20 Posted by: markyoe Posted at: 2018-05-29T18:08:34.038Z Reads: 115

```
Charger not plugged into battery: 45.8V
Charger plugged into battery: 45V
I also tested a different charger that I borrowed from a friend and it was putting out 44.5V not plugged into the battery...

I'll take pic of the wiring and try to find the diagram I followed.

@Jumpman No, he had a couple 10s chargers available in addition to a 6s one.
```

---
## \#21 Posted by: b264 Posted at: 2018-05-29T18:09:49.135Z Reads: 113

```
Something is wrong with your charger.  What charger did you borrow?

Measure a brand new Alkaline AA cell.  What voltage do you get?  Is your measuring device the thing that's not right?
```

---
## \#22 Posted by: deucesdown Posted at: 2018-05-29T18:12:59.988Z Reads: 109

```
[quote="b264, post:19, topic:57108"]
Not using a BMS is more risky than using one.  It just appears this one isn’t working.
[/quote]

That's the issue, you can't easily tell if it's working or not. At minimum it needs a fault indicator, loud beeping or blinky lights...

And bypassing BMS for discharge gets rid of 50% of the safety factors.

I've been thinking about this for a long time and trying to convince myself, but I'm still not convinced. :)

I'm going to wet my toes with one of those bluetooth Smart BMS, just to monitor voltages. Then add it to the charge circuit. Then maaaybe add it to the discharge.

[quote="b264, post:21, topic:57108"]
Is your measuring device the thing that’s not right?
[/quote]

This is like the "I used to know what time it was until I got a second clock". :slight_smile: I ended up buying a voltage reference...
```

---
## \#23 Posted by: Acido Posted at: 2018-05-29T18:23:25.040Z Reads: 99

```
li ion cells are safe from blowing up all up to i think 5.x volts (i read this on some paper can not find it now)
higher than 4.2 is just slowly ruining them
```

---
## \#24 Posted by: markyoe Posted at: 2018-05-29T18:38:07.620Z Reads: 101

```
Didn't have a brand new AA, but I measured a brand new 9V and got 10.33V.... I then switched out the battery in my multimeter and read a 9V as 9.58V which from what I read is ok. I measured my charger again and it's 42.1V.

SO the multimeter was reading incorrectly. Here are the new readings from my 10s pack.

3.8
3.8
3.9
3.8
4.2
4.2
4.2
4.2
4.2
4.1

Much better, but why would some of those be lower?

Anyway, here are some pictures of the wiring, like @Eboosted wanted to take a look at.

![IMG_20180529_111558|666x500](upload://pHSqQNtKdY3ljg9amwHAjX99Vor.jpg)![10s4p BMS bypass|496x500](upload://wtDwpBtDnpwEHth032HJw1y4PzZ.jpg)![IMG_20180529_111612|666x500](upload://tOCmAtC3CRIY4nFJ6mj7ZDz83c4.jpg)![IMG_20180529_111643|666x500](upload://qFP8UV8n3DHcdz5dPBlxc8D1Jyo.jpg)![IMG_20180529_111619|666x500](upload://7FiAzocihVpLst0FwLxbD46fYQN.jpg)
```

---
## \#25 Posted by: b264 Posted at: 2018-05-29T19:18:21.054Z Reads: 89

```
This is great news. :smiley: So your charger and BMS may be working correctly after all -- but not your multimeter :rofl:

So I would let it sit on green for 10 more hours and see **if any of the low cells go up, or if they don't**.  That would determine the next steps

Maybe check after 15 minutes, 1 hour, and 4 hours

To be clear, you're looking for a 0.2V jump because 0.1V is the resolution limit and could just be rounding errors.
```

---
## \#26 Posted by: egzplicit Posted at: 2018-05-29T19:23:57.409Z Reads: 91

```
The difference is so big a bms won’t be able to balance them back. I would manually discharge the higher ones to get them close to 3.8v (use a light bulb connected to the individual groups that are high in voltage).

Once you manually balance them, if the bms works it should keep them in sync.
```

---
## \#27 Posted by: deucesdown Posted at: 2018-05-29T19:26:55.614Z Reads: 90

```
[quote="Acido, post:23, topic:57108"]
slowly ruining
[/quote]

IMO not slowly at all at 4.5v. But whew!

[quote="egzplicit, post:26, topic:57108"]
Once you manually balance them
[/quote]

Still begs the question of why they went so far out of balance.

The balancers on BMS, once they trigger, do they run until all cells are in balance no matter how long it takes? Or only if charger is still supplying power?

Where I'm at right now in my understanding is, the charger has to deliver full pack voltage, but not enough to trigger pack over-voltage-protection. The balancing will be triggered when one of the cells reaches the balance-start voltage (probably 4.25v on this bms?). As long as charger is still supplying power, the BMS will attempt to drain all cells down to the voltage of the lowest cell.

The charger will continue to supply power until the entire pack's voltage hits its setpoint. This should not occur until all cells are balanced and full.

If something goes wrong, the BMS will open the charger circuit, cutting off power, and the pack will not be balanced or fully charged. One of the possibilities here is the charger is supplying power faster than the BMS can drain the high cells down. This should not happen if cells are close in voltage, as the charger will not provide a lot of watts to the pack when the pack is near full.

Someone correct me if I'm wrong.
```

---
## \#28 Posted by: Acido Posted at: 2018-05-29T19:36:09.164Z Reads: 85

```
this depends on the bms
some bmss balance all the cells to be at the same voltage every time like on 4.2, 2.8 or 3.2v
and some only on full charge as i know
```

---
## \#29 Posted by: deucesdown Posted at: 2018-05-29T19:40:11.804Z Reads: 87

```
[quote="Acido, post:28, topic:57108"]
balance all the cells to be at the same voltage every time
[/quote]

[quote="Acido, post:28, topic:57108"]
some only on full charge
[/quote]

Either way, I'm thinking if you use a CC/CV power supply instead of a lithium ion charger, once the pack is full you'll be constantly running the balancer until you pull the plug? More BMS caused premature wear, if you don't have full understanding of your BMS behavior?
```

---
## \#30 Posted by: b264 Posted at: 2018-05-29T19:43:37.627Z Reads: 87

```
Let's wait until all the facts are in before we rush to judgement

We still need experimental results else this could be speculation
```

---
## \#31 Posted by: Acido Posted at: 2018-05-29T19:44:14.445Z Reads: 85

```
theres a whole discussion about this on here
https://www.electric-skateboard.builders/t/programmable-supply-power-60v-15a-35/36797
```

---
## \#32 Posted by: markyoe Posted at: 2018-05-30T16:40:38.780Z Reads: 82

```
Ok I let it sit with the charger on green for about 16 hours. Not much changed.

3.8
3.8
3.9
3.8
4.2
4.2
4.2
4.2
4.1(decreased .1)
4.2(increased .1)

Instead of hooking up a light bulb to the higher voltage packs, could I use my Imax B6 charger and charge them all individually to balance?
```

---
## \#33 Posted by: b264 Posted at: 2018-05-30T16:42:17.326Z Reads: 76

```
You could use the B6 on each P-pack yeah

Somehow your setup is not balancing your cells.  It's like the charger is not doing the CV part of the CC/CV cycle.

Those two changes could be rounding errors.  If the minimum granularity of your measuring device is 0.1V then you need to see a 0.2V jump to be certain it has actually changed.
```

---
## \#34 Posted by: b264 Posted at: 2018-05-30T16:44:04.010Z Reads: 74

```
I would borrow a charger and try the same experiment again.  If you get the same result then I would change the BMS.

The balance charging part of the cycle is not happening
```

---
## \#35 Posted by: b264 Posted at: 2018-05-30T16:46:22.535Z Reads: 75

```
Honestly I WOULD NOT use the B6 to manually balance the cells.  The reason being is because that will work once, but you want to fix the problem, not kick the can down the road.  If they are all perfectly balanced you won't be able to test the balance charging...
```

---
## \#36 Posted by: markyoe Posted at: 2018-05-30T16:55:09.587Z Reads: 73

```
I'll hook up another charger for a while. I just sent an email to Lilian at battery supports to see what she thinks.
```

---
## \#37 Posted by: markyoe Posted at: 2018-05-31T12:14:02.660Z Reads: 68

```
Would have discharging through the BMS helped keep the P-packs more balanced?
```

---
## \#38 Posted by: ARetardedPillow Posted at: 2018-05-31T12:31:45.183Z Reads: 68

```
Probably not, I used that exact same BMS once and after around 2 months of running it without being bypassed the thing blew up on me.
```

---
## \#39 Posted by: pedro Posted at: 2018-05-31T14:02:31.704Z Reads: 67

```
so what i seeing, the bms stop charging after just 1 cell is reached 4,2 V and the others lower than 4,2 stop charging.... this is a shit. maybe the discharge is the same, when a cell is 3V, the discharge close, and you can't ride anymore if the others 9 cells is 4V...
```

---
## \#40 Posted by: pedro Posted at: 2018-05-31T15:28:05.376Z Reads: 65

```
Achivement!!
Welcome
This badge is granted when you receive your first like on a post. Congratulations, you've posted something that your fellow community members found interesting, cool, or useful!


I want to say thanks to my mom, dad, and all my friends who stay with me in my bad and good momens, and a big thanks to my follwers. 
I love you <3
```

---
## \#41 Posted by: b264 Posted at: 2018-05-31T15:31:13.430Z Reads: 64

```
[quote="pedro, post:39, topic:57108"]
so what i seeing, the bms stop charging after just 1 cell is reached 4,2 V and the others lower than 4,2 stop charging
[/quote]

NO, we don't know that yet.  It's a possibility.

@markyoe still needs to try a different charger

And it's possible maybe the charge needs to be on N- port
```

---
## \#42 Posted by: chinzw Posted at: 2018-05-31T17:51:27.225Z Reads: 60

```
I have that exact bms, and that is the behaviour. One cell hits 4.25, that's it, no more charging.
```

---
## \#43 Posted by: deucesdown Posted at: 2018-05-31T23:40:41.112Z Reads: 61

```
I think this is proper behavior. That cell I. Already high at 4.25.f it lets charge keep going there's a good chance the high cell overcharges. The tiny bleed resistor which can do 50-100ma has to compete with the charger which can be throwing as much as 4a/10cells==400ma at the cell assuming a 4a charger and 10s pack.

When this happens, does it start balancing? Discharge all cells to the same voltage as the lowest cell?
```

---
## \#44 Posted by: chinzw Posted at: 2018-05-31T23:54:35.883Z Reads: 56

```
It should stop charging and start bleeding the higher cells to match the lower ones and start charging again, but this doesn't happen.
That's why some of us moved from analog BMS to digital ones. Much more customization, better charging/balancing algorithms, etc.
```

---
## \#45 Posted by: b264 Posted at: 2018-06-01T05:37:35.123Z Reads: 54

```
~~Just an idea, what is the N- port for and what happens if you connect the charger negative to it~~

~~Warning: I don't know for-sure that's safe, but if I was in your position I would try it, closely monitoring EVERYTHING and see what happens.  Maybe first through a fuse.~~

edit: I was just told by Bestech that if a BMS has a N- it's probably the charge port.

@markyoe So try moving that black wire from P- to N-
```

---
## \#46 Posted by: markyoe Posted at: 2018-06-01T07:31:38.574Z Reads: 53

```
Well dang, lol. Thanks for checking in on that. I was about to email Lilian to ask about that. I'll do that and report back what happens.
```

---
## \#47 Posted by: markyoe Posted at: 2018-06-03T06:48:13.851Z Reads: 50

```
I manually charged the P-packs with my B6 before I knew to change the negative cable to N- so I'm not totally sure if changing it was the solution. I'll be using the board quite a bit the next fews weeks so we'll see if the BMS will actually keep the packs from drifting.
```

---
## \#48 Posted by: b264 Posted at: 2018-06-03T09:34:29.198Z Reads: 48

```
I would drain one pack down a little bit just to see if the BMS will correct it...
```

---
## \#49 Posted by: Sender Posted at: 2018-06-03T11:58:04.744Z Reads: 45

```
Awesome job on the troubleshooting assist @b264.  I have been follwing this just to see how it all turns out.  Hopefully it is all sorted now @markyoe
```

---
## \#50 Posted by: Z4MSupreme Posted at: 2019-09-08T20:47:59.260Z Reads: 15

```
Any updates on how the BMS is performing? I've been having a problem with my bestech BMS and unbalanced P-groups. How did you fix it?
```

---
