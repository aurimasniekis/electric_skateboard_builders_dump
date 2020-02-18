# VESC Regen breaking with a BMS

### Replies: 6 Views: 2493

## \#1 Posted by: Sharkface Posted at: 2015-11-17T23:17:55.998Z Reads: 176

```
Hello All, 

still solidifying my knowledge in electronics here, so I am probably missing something stupid obvious....

I am taking a look at various BMS systems for building my own Life battery. For sake of conversation lets refer to this guy here:
http://www.alibaba.com/product-detail/battery-bms-48v-for-lifepo4-cells_613150704.html?spm=a2700.7724857.29.48.SZkiiZ

so that guy has the positive lead for charging/discharging, a negative lead for charging, and a negative lead for discharging. Obviously only two leads are coming off of the VESC. So when trying to get use out of the regen brakes, wouldnt i need to put the negative lead from the vesc into two spots on the bms? If so, wouldnt I have to be worried about one of those negative leads being used for discharge while its connected to the charge negative lead port?


I am probably doing a really bad job at putting into word what I am trying to understand here. Wasnt sure if I should hijack the FAQ page about BLDC tool setting for regen brakes.

Thanks for the help, i love you all!!!!
```

---
## \#2 Posted by: lowGuido Posted at: 2015-11-18T03:05:24.581Z Reads: 166

```
you would hook up the VESC to the output of the BMS. 
when you charge with the charger it would connect through the BMS
regen does not go through the BMS it just goes straight into the battery

edit: My language in this post can be a bit misleading, I have elaborated below.
```

---
## \#3 Posted by: Braylon31 Posted at: 2015-11-18T03:19:46.026Z Reads: 158

```
Have you got it put together yet? Im thinking about doin 5he same thing?
```

---
## \#4 Posted by: Sharkface Posted at: 2015-11-18T04:27:26.650Z Reads: 159

```

[quote="lowGuido, post:2, topic:504"]
regen does not go through the BMS it just goes straight into the battery
[/quote]

I am a complete idiot here so correct me if im wrong.... but in the circuit itself the leads go through the battery, into the bms, then to the vesc. To my understanding thats just how it works. Getting the regen to come back into the battery on this bms requires a different lead to be soldered to the bms. If i solder the same negative lead from the vesc and splice it to the two point on the bms what would be the point of having a second port on the bms? If i bypass the bms for regen then the bms would be in parallel thusly causing the vesc to just run straight from the battery. That sounds wrong to my basic electronics. Do i need to find a bms where it also only has the two leads?
```

---
## \#5 Posted by: lowGuido Posted at: 2015-11-18T06:35:35.310Z Reads: 149

```
there are BMS and then there are BMS.
If you have a BMS that is monitoring charge and discharge currents and limiting them to pre determined safe levels then your regen will be limited and controlled by that.

If you have one of the cheaper BMS that's basically just a built in balance charger then when you plug in your "dumb charger" it balances the cells and limits charging currents etc.

the VESC also has configuration where you can control the regen current, so its not really a big deal either way.

even if you did regen direct to the battery (via the FETs and CAPs to be technically correct) its not a big deal.
my cheap chinese single-board-BMS on my Ebike blew up early in the piece and I have been charging (and discharging) my LiFePO4 battery directly with no problems for 3 years now.

edit: Im rambling here. let me cut to the chase.
the BMS should have: 
 +ve terminal that connects to the most positive of the cells.
 -ve terminal that connects to the most negative of the cells.
"managed -ve" which is the negative terminal that you connect to your load (VESC) and also the negative terminal for your charger.
then it will have a lead for the +ve terminal of every individual cell in the battery.
```

---
## \#6 Posted by: Sharkface Posted at: 2015-11-18T08:07:07.314Z Reads: 139

```
[quote="lowGuido, post:5, topic:504"]
(via the FETs and CAPs to be technically correct)
[/quote]

That was my suspicion, so thanks for confirming that!

[quote="lowGuido, post:5, topic:504"]
LiFePO4 battery directly with no problems for 3 years
[/quote]
Yep, with the new job came access to a lot of manufacturing/maker equipment so I am already going through the motions to get access to the spot welder so I can build myself up a LiFePO4 battery. LiPO for my plebeian self for the time being as its what i have on hand.

[quote="lowGuido, post:5, topic:504"]
+ve terminal that connects to the most positive of the cells. -ve terminal that connects to the most negative of the cells."managed -ve" which is the negative terminal that you connect to your load (VESC) and also the negative terminal for your charger.then it will have a lead for the +ve terminal of every individual cell in the battery.
[/quote]
so the BMS I linked is pretty much useless since it the "managed -ve", "managed +ve", and a third -ve labeled as "charge terminal". Thats basically what I am hearing here. Thank you for your clarifications!!! that should help out a lot!!!

[quote="Braylon31, post:3, topic:504, full:true"]
Have you got it put together yet? Im thinking about doin 5he same thing?
[/quote]
Sorry I missed you bud!
At this time no, I am waiting up on a VESC or three from enertion/onloop. Once those are in hand itll still be a bit before i am working with a BMS. lol Slow but sure the shark combs the ocean looking for the choice eats, nomsayin?
```

---
