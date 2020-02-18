# 13s BMS for 12s battery, experts please!

### Replies: 20 Views: 759

## \#1 Posted by: rich Posted at: 2019-04-10T15:07:41.925Z Reads: 130

```
So I got a 13s BMS as a gift from a friend. He asked the seller/manufacture if they sell 12s and they answered:&rdquo;13s is suitable for 12s, just don&rsquo;t connect B13+&rdquo; which seems like a joke. I guess the BMS won&rsquo;t work because then there is 0V at B13+.

![165713|690x388](upload://lbWOemN1lXVs5OuO62bFAXUXdu0.jpeg) 

This leads me to following thought, If I connect B12+ of the battery in parallel to B12+ and B13+ of the BMS it should work (beside the fact that balancing current is double for cell 12).

I think this because of another different 12s BMS I have. On the PCB B12+ and B13+ are soldered together that&rsquo;s why I asked the manufacture if I shall disconnect them because it seemed faulty to me. The answer was:&rdquo; No that is alright because they only had 13s BMS in stock and B12+ and B13+ must be connected to work with 12s.

![195839e|690x388](upload://rlBcnYnqbsxscKpDghyjX3A70v2.jpeg) 

Do you think this is legit if I do the same with the new BMS to work with 12s?

Also I wonder if it is a problem because the charging voltage is 50.4V instead of 54.6V for 13s?

Thanks in advance :grin:
```

---
## \#2 Posted by: olestra Posted at: 2019-04-10T15:28:31.625Z Reads: 116

```
seller claims it'll work as a 12 by just not connecting the b13... and you think it will do nothing, right?
what would it hurt to try that, before modifying it?
```

---
## \#3 Posted by: rich Posted at: 2019-04-10T15:53:58.104Z Reads: 108

```
I think the seller just wants to sell....

The thing is I don't like to try or play around with battery/BMS if I'm not sure if it's correct. I respect batteries for their danger or call me paranoid :laughing:.

It was not my conversation so I don't know if the answer came from a salesman (which I guess) or somebody who knows what he is talking.

I had several conversations with the seller of 2 other BMS I have (one is the mentioned 13s BMS sold as 12s). They gave me very good technical answers which seemed legit for me. That's why I think connecting B12+ and B13+ is a must but I'm no electical enginner hence I created this topic to be sure. I really don't know.

[quote="olestra, post:2, topic:90059"]
modifying
[/quote]

I wouldn't solder on the PCB, just connect the B12 & B13 balance leads to B12+ of the battery.
```

---
## \#4 Posted by: thisguyhere Posted at: 2019-04-10T15:57:03.907Z Reads: 102

```
i can't imagine how bridging the 13+12 balance leads can do anything.

usually the highest balance lead reads zero volt relative to batt+, or pack's full voltage relative to batt-.

so then this module gets the same voltage from 13 and 12 Pgroup and balances them together?

that's really odd to me, do you have a wiring schematic for this bms?
```

---
## \#5 Posted by: olestra Posted at: 2019-04-10T16:07:41.895Z Reads: 102

```
My understanding of how these things work means that it really depends on how it's programmed.

My reasoning is: if the BMS has no logic components, it wouldn't be able handle 12s on a 13s design in any fashion. either it wouldn't function or it would short if pins 12 and 13 are joined.

therefore if the same BMS hardware can handle 12 &13s, it must have some logic, a microcontroller with firmware to decide what to do, right? 

Therefore it depends on the firmware if 12&13 should be tied together or not.  If you're wrong about shorting 12&13 together -- you've got damage, If you're wrong about not shorting them together, you only get a fault and nothing happens.  

so I'm suggesting that not shorting 12&13 and using the 50.4v charger will either work or it will do nothing, and that shorting 12&13 together would either work or cause damage. I'd try the does nothing on failure option first.
```

---
## \#6 Posted by: rich Posted at: 2019-04-10T17:15:26.634Z Reads: 98

```
[quote="thisguyhere, post:4, topic:90059"]
that’s really odd to me, do you have a wiring schematic for this bms?
[/quote]

I guess you mean the BMS where B12+13 are soldered together on the PCB?

The brand is RJXZS (I never used it so far)

https://www.aliexpress.com/item/12S-60A-version-S-lipo-lithium-Polymer-BMS-PCM-PCB-battery-protection-board-for-12-Packs/32860750557.html?spm=2114.search0104.3.1.5ca7bf18m6MUQr&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10068_10547_319_317_10548_10696_10084_453_10083_454_10618_10304_10307_10820_10821_537_10302_536_10059_10884_10887_321_322_10103,searchweb201603_90,ppcSwitch_0&algo_expid=16aedee1-2174-4505-ba75-b95cc8fca98c-0&algo_pvid=16aedee1-2174-4505-ba75-b95cc8fca98c

![PNG|589x445](upload://tT267mj8CbDMKF98zB8R3AYEfCJ.jpeg) 

I was digging for the conversation about the RJXZS 12s BMS so here we go:

![1|524x40](upload://zz6AhuRdDfdkF9iTcaTKmyVzARi.png) 

![2|517x330](upload://lrkR6yDSoCBdZVq87WXEwQkjGhM.png) 
![3|511x253](upload://5PNnHAGEl4q0GJdz4x1z5W6vVEj.png) 
![4|510x382](upload://tuqiWo7VZ1JvVkZzMt92w5e04JN.png) 



Just discovered a pic of a 10s BMS of RJXZS on aliexpress, it seems they bridged B10+ up to B13+ (like written in the message).

![PNG|396x164](upload://4akpTWUUZxdb3DEcSQTsWvDqJzY.jpeg) 

I use the same BMS in 10s for another build (but don't know if they bridged any pins). It works well (with well I mean I lost brakes going downhill fully charged :laughing:, unintended overcharge protection test survived). The only thing it gets quite warm after reaching full charge.


[quote="olestra, post:5, topic:90059"]
so I’m suggesting that not shorting 12&amp;13 and using the 50.4v charger will either work or it will do nothing, and that shorting 12&amp;13 together would either work or cause damage. I’d try the does nothing on failure option first.
[/quote]

Option 1 sounds good to me :ok_hand:
Maybe it's built different as you said (and the seller). Also if it doesn't work it's time for refund :stuck_out_tongue_winking_eye:


This is the red 13s BMS we are talking about (60A common port)

https://www.aliexpress.com/item/Daly-3-7V-13S-45A-60A-48V-PCB-BMS-36V-for-18650-LiNCM-lithium-Liion-battery/32932364828.html?spm=2114.search0104.3.49.34fa30c5cpMUO0&ws_ab_test=searchweb0_0,searchweb201602_1_10065_10068_10547_319_317_10548_10696_10084_453_10083_454_10618_10304_10307_10820_10821_537_10302_536_10059_10884_10887_321_322_10103,searchweb201603_90,ppcSwitch_0&algo_expid=4de2c7b4-4296-4d83-a41b-8aa8409e5f3e-7&algo_pvid=4de2c7b4-4296-4d83-a41b-8aa8409e5f3e

![Daly|646x331](upload://xOoyqZgnLF0QASL6h6WlQ5YqpPN.png)
```

---
## \#7 Posted by: Sn4pz Posted at: 2019-04-10T17:18:21.130Z Reads: 85

```
Do you have any crappy/almost dead batteries that you would be willing to sacrifice?

Could you test it with 2x 6s lipos? Or would you need another set to give you a second P group? ( just curious )
```

---
## \#8 Posted by: rich Posted at: 2019-04-10T19:43:32.611Z Reads: 81

```
[quote="Sn4pz, post:7, topic:90059"]
Do you have any crappy/almost dead batteries that you would be willing to sacrifice?
[/quote]

Yes but they are really dead :hushed:

https://youtu.be/BFk6UfeP884

I have new 3x4s Zippy's, the only 12s battery right now but need to make all connections first.

![201406h|690x388](upload://zqP5iPv3dWmJTBCzjDZqxE0PO4H.jpeg) 

I also have 2 proper Bestech BMS but huge (19cmx6.5cm)

![20171113_155615|690x388](upload://6i94071IoAfYKUr2gFPsyzVy3iL.jpeg) 

![224245h|690x388](upload://jpuJeB9hG9d0hx5Us9jyc1vRdV5.jpeg) 

compared to the others (Bestech is about as big as the red foil)

![193117h|690x388](upload://IXzYrvpv7JRBWGe6olG4Xw9G4x.jpeg)
```

---
## \#9 Posted by: Sn4pz Posted at: 2019-04-10T19:47:37.976Z Reads: 73

```
I wouldn't take the chance.... But I worry about batteries a lot 😂
```

---
## \#10 Posted by: rich Posted at: 2019-04-10T19:54:02.952Z Reads: 74

```
I plan 2 battery packs in the near future. The 12s5Ah Lipo above and a 12s6p. So I need 2 BMS and I wanted to use the cheap ones because of the space :thinking:
```

---
## \#11 Posted by: Fiori Posted at: 2019-04-10T20:35:36.627Z Reads: 72

```
I am not sure for this BMS specifically. But it is generally normal for BMS's to cover a ranged of voltages. I don't think its that abnormal at all. 

If you look at the differences in pictures of 10s, 11s, 12s, 13s BMS's it's usually the same unit, just with different wiring setups.

The only thing i'd be worried about is that the firmware settings/software version may be different between different voltages.(10s, 11s, 12s ect..) 

I'm assuming bridging the b12 and b13 pins changes the firmware settings for end-of-charge voltage. After you solder those pins, I would check to make sure that the overcurrent protection still works by connecting a higher voltage charger and seeing if it actually shuts off.
```

---
## \#12 Posted by: pjotr47 Posted at: 2019-04-10T20:40:38.376Z Reads: 70

```
The soldered 13s pin to the 12s is no problem for reading the voltage from each cell and balancing it. The most important this is that the Chinese company had to change the setting from the BMS. 

Overcharge voltage must be 50,4v and not the 54,6v from the 13s battery. Same for voltage cut-off if you are going to use it with discharge.
```

---
## \#13 Posted by: Fiori Posted at: 2019-04-10T20:49:33.731Z Reads: 68

```
^^^This. 

#10characterssssssssssssss
```

---
## \#14 Posted by: rich Posted at: 2019-04-10T23:47:03.796Z Reads: 66

```
[quote="Fiori, post:11, topic:90059"]
The only thing i’d be worried about is that the firmware settings/software version may be different between different voltages.(10s, 11s, 12s ect…)
[/quote]

True.... and I'm getting more and more confused that's why I wrote the manufacture a message, hopefully I get an answer soon.

[quote="pjotr47, post:12, topic:90059"]
Overcharge voltage must be 50,4v and not the 54,6v from the 13s battery. Same for voltage cut-off if you are going to use it with discharge.
[/quote]

That's exactly what I thought first but on the other side the overcharge and over-discharge voltage is always shown for a single cell in the specs. I think the protection is for each cell no matter the total voltage of the pack, the same for overcharge protection.
```

---
## \#15 Posted by: rich Posted at: 2019-04-11T11:46:21.610Z Reads: 55

```
Meanwhile I got a reply from the official manufacture how to connect this 13s BMS for 12s

![reply|300x144](upload://4ksnKMUDOjgT2nf1i1uA8J9zRN4.png) 

:rofl: So basically the same answer "not to connect B13+" just more destructive.
```

---
## \#16 Posted by: sk8l8r Posted at: 2019-04-11T12:08:31.547Z Reads: 53

```
I saw a review for a 13s smart BMS I own (yet to use) that apprently works with less than 13 when not connected (going to dig it out make sure I'm not lying)
```

---
## \#17 Posted by: sk8l8r Posted at: 2019-04-11T12:19:46.111Z Reads: 54

```
yup 

https://youtu.be/ClGmMY0kXvQ?t=194
```

---
## \#18 Posted by: pat.speed Posted at: 2019-04-11T12:25:10.184Z Reads: 55

```
@rich @pjotr47

The sellers are correct, all that is needed is to disconnect the last balance lead. I’ve done this twice now with two different bms modules. The way is works is the bms only monitors the cells that give off a voltage, when disconnected there is 0 volts thus the bms doesn’t recognise that a cell should be connected.

To answer the worry about charge and discharge cut offs it is not an issue as the bms module doesn’t/ can’t measure full battery voltage. It only measures the voltages between the balance leads. Thus it doesn’t matter whether the cell is missing or not
```

---
## \#19 Posted by: rich Posted at: 2019-04-11T13:00:05.444Z Reads: 52

```
Thanks for your answer and I like it :grin: :partying_face:

So it seems the silver RJXZS is made different where the pins 12+13 must be shorted on the PCB.
```

---
## \#20 Posted by: pat.speed Posted at: 2019-04-11T22:19:18.588Z Reads: 40

```
Yes, I have never seen the pins shorted before. For example one of my bms modules actually has the possibility to use up to 16s but the connector only takes 13s so the remaining 3 contact points on the pcb are left in connected
```

---
