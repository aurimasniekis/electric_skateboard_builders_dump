# SOLVED&ndash;Non-noob BMS Issues

### Replies: 8 Views: 472

## \#1 Posted by: Kraz3Sk8r Posted at: 2018-06-13T05:07:45.476Z Reads: 137

```
Can anyone please help me diagnose my persistent BMS issues?  My charge-only BMSs won't charge 12S liion packs past 45.3V.  I've tried 3 different 5p12S battery packs (built by me) and multiple BMSs from BesTech and batterysupports.com.  Though new to BMSs, I'm an engineer, and the skateboard otherwise works great.  I just noticed before connecting the latest BMS that the BMS instructions seem to say to connect the battery ground before the balance wires, so maybe I burned up the other BMSs by not doing so, and maybe because one of the bad BMSs charged one of the P-groups to 4.2V, the other P-groups aren't charging on the latest (presumably undamaged) BMS?  Before first charge, all voltages were 3.45v per cell.  On 7 June the P-group voltages were 3.74, 7.48, 11.22, 14.96, 18.70, 22.30, 26.50, 30.20, 33.90, 37.70, 41.40, and 45.20.  To save you the math, that means all P-groups were 3.6v-3.8v except for group 7 which was 4.2v.  Left plugged in until 10 June, the voltages changed very slightly, raising overall pack voltage from 45.2v to 45.3v per my inexpensive multimeter.

All three liion chargers output 50.4V at no load.

This is the battery compartment (with balance leads currently disconnected).![Battery%20Compartment|281x500](upload://lEH0Ev8K3t9ZwAFPIIeo7mDhYO4.jpg)  The thing under the VESC power connectors is a buck converter for powering the headlight and tail lights.

Do you think the several other BMSs were either burned out or defective, and the current one is balancing the P-groups, just extremely slowly?
```

---
## \#2 Posted by: telnoi Posted at: 2018-06-13T05:46:02.062Z Reads: 109

```
https://www.orionbms.com/manuals/utility/param_balancing_description.html

Never used a bms in my life an I am not an engineer, but I think you can deduct the following from the article above: the bms puts a load (very low - see specs of your bms) on cells that have a higher charge compared to others within a certain predefined range. Since the discharge amperage is typically super low on BMS (burns it off/turned into heat) and only meant for tiny differences, I could imagine that this takes a while if your pack is as unbalanced as yours.
```

---
## \#3 Posted by: linsus Posted at: 2018-06-13T13:17:52.547Z Reads: 85

```
Not sure how beeing an engineer applies to anything. I mean, I could be many kinds of engineer that dsnt mean it helps me to know stuff about batteries. Anyway.


Can you check if any welding spots got loose? Other wise try using a proper lab supply with appropriate settings for charging instead of a the DC brick. Usually does the trick when thers a big imbalance.
```

---
## \#4 Posted by: Jc06505n Posted at: 2018-06-13T13:38:22.730Z Reads: 83

```
[quote="linsus, post:3, topic:58713"]
Not sure how beeing an engineer applies to anything.
[/quote]

He could be an electrical engineer, meaning he's inviting others to use terms that they would normally hold back or suggest due to the diverse population on the forum
```

---
## \#5 Posted by: linsus Posted at: 2018-06-13T13:45:39.755Z Reads: 75

```
Then why not say Electro engineer.
```

---
## \#6 Posted by: Kraz3Sk8r Posted at: 2018-06-13T22:31:06.970Z Reads: 56

```
Sorry for the confusion on my "engineer" comment--I just meant to say I have some  knowledge and experience with DC circuits.  That being said, I can't figure out how I could have burned up four BMSs as long as the balance wires were in the proper order (assuming the BMSs are actually damaged).  If anyone has any ideas, please let me know.

@linsus:  Thanks--I will get and try a lab supply.  It is hard to tell since my batteries are copper on nickel on copper (three layers), but I don't think there are broken welds.
```

---
## \#7 Posted by: linsus Posted at: 2018-06-13T22:57:35.803Z Reads: 53

```
Sounds like some thick layers to weld thru tho.
Think ive rewelded all of my packs atleast once cause the vibrations usually shakes one or two Spots loose after 100 or so rides. Used hobby charged up until recently so could compare detected impendance and cell voltage imbalance easy which gives a good hint if a weld has Come loose or not. With a bms you're charging "blind" so its harder to tell.
```

---
## \#8 Posted by: Kraz3Sk8r Posted at: 2018-06-24T23:34:58.489Z Reads: 32

```
Thanks everyone for your help. I found the problem--it was a bad li-ion cell.  The BMSs were doing what they should to protect from harm.  I'm unsure of what was going on with the other battery packs since I don't have them anymore, but it seems clear what this problem was.
```

---
