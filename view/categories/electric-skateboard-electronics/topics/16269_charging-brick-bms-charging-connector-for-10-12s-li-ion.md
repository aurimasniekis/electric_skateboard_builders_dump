# Charging brick + bms charging connector for 10-12S li ion

### Replies: 6 Views: 2532

## \#1 Posted by: Atimu Posted at: 2017-01-18T16:00:31.841Z Reads: 327

```
Hi, I'm building a board that's either going to be 12s5p or 10s6p (leaning towards 12s) on a dual 190kv setup (from diy). The batteries and bms are coming in any day now but I haven't found a decent charger yet. I found this 2amp one (http://miamielectricboards.com/shop-1/12s-charger) but that would take forever to charge a 15Ah battery. There's a 4amp one here for about the same price but theyre not shipping anything out for a few weeks (http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html).

Where do you guys typically get your charging bricks? Any links would be helpful.
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-01-18T20:17:25.549Z Reads: 301

```
https://lunacycle.com/batteries/chargers/
```

---
## \#3 Posted by: Atimu Posted at: 2017-01-19T05:32:55.595Z Reads: 273

```
So I checked that link and they seem to have a good amount but nothing for 12s. Do you know if its okay to use a slightly lower or slightly higher voltage charger? Would the bms take care of that?
```

---
## \#4 Posted by: chuttney1 Posted at: 2017-01-19T06:50:33.270Z Reads: 265

```
I can give a short answer, but no insight on why. Might be a TL;DR.

The "Smart BMS" I use specifies to use a charger with a voltage higher than my battery's voltage for 10S and when done charging to pull the plug from the socket. I am not sure why I cannot use a lower voltage for charging, but probably could not. I did charge my 10S pack with an RC charger using 12 V car battery as testing to make sure my pack did not catch fire. It seemed to take some time to charge the pack up to 41 V from 36 V.  The BMS only manages the balance of each cell and limit  amperages going out. It will not charge batteries with a higher voltage than what you put in.  

For comparison, my battery pack is 12.5 Ah charged with 42V at 3 amps.  I think I was aiming for a charge time around 4 hours. A balance between speed and longevity. 

Take your time to choose a charger and get a second opinion as it seems I am the only one who responded. One thing I can say, for sure, is there is nothing wrong with charging a lithium cell for a long time such as 24 hours as long as it is not overcharged above 4.2 V a cell and not hot. 

You can also ask the community on the endless-sphere forum for help. There are some who assemble li-ion battery packs and can give a recommendation.
```

---
## \#5 Posted by: Atimu Posted at: 2017-01-20T02:42:59.135Z Reads: 226

```
Hmm that's interesting. I'm not sure if my bms would work the same if I got a higher voltage charger so I'll play it safe and get a 44v charger. 

I don't mind paying a lot but I just thought I could find a 3 or 4 amp charger for around $50 instead of a 2 amp one. That would take over 7 hours to charge my 15Ah pack, which isn't too bad I guess. 

I registered to the endless sphere forum but don't think they let new members post for a while so I'll ask on there when I can. Worst case scenario I'll go with the 2amp charger. Thanks !
```

---
## \#6 Posted by: Atimu Posted at: 2017-01-20T17:00:00.006Z Reads: 207

```
@longhairedboy I saw on a post here that you make and sell boards and that you ride a dual 190kv 12s setup, which is what I'm trying to build. Do you happen to know of any good sites to get 44v chargers from?
```

---
