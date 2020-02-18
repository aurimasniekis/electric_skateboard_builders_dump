# Anti spark switch stuck ON

### Replies: 15 Views: 1083

## \#1 Posted by: accrobrandon Posted at: 2018-11-27T21:42:10.596Z Reads: 154

```
So i have a Miami electric switch which ive been using for maybe the last 6mo or less. At any rate, I HAD to ride for 1mi in light rain yesterday...as I arrived to my destination the board wouldnt turn off which was weird... I assumed it was the water as my lights all fizzled out shortly after as well. Luckily I have a bestech BMS and can use that switch for now.

Upon inspection and opening the case only a small amount of moisture had gotten to my buck converter that powers the lights. I was able to clean it up with some rubbing alcohol today and get it working again. 1 point for me...

but the on/off switch which is more in the middle of the case had no moisture around it, not to mention the switch comes shipped waterproofed (basically) with what looks like dielectric grease or something. 

Anyways... the physical switch on the outside illuminates as expected, and continuity is on/off as the switch is pressed on and off.

Voltage from battery just goes through it.... 

at the pins if this helps...
- between switch neg and 12v+ pin is equal to battery voltage (48.4 currently)
- between switch positive and switch and neg voltage is 47v
- no other data for other pins based on testing various combos.


thanks and let me know if you know anything!


![1127181452_HDR|281x499](upload://c4UVkvpj67zITmavxEF8gnihQuP.jpeg)
```

---
## \#2 Posted by: longhairedboy Posted at: 2018-11-27T21:50:47.168Z Reads: 143

```
sounds like your fets locked shut. This can happen on occasion if there's a short in the mechanical switch, such as from moisture. It can also happen during extreme braking currents but that's not typical. 

Of course this is just a rebranded Flier switch and not the 300amp variety so it may have just done it for the fuck of it because those are just not reliable.
```

---
## \#3 Posted by: Sn4pz Posted at: 2018-11-27T21:53:16.981Z Reads: 138

```
On this topic, If I want a means of turning my board on and off that wont break, while supporting up to 100a, what would you do? :slight_smile:

DiebieMS has a switch, does anyone have experience with that? Is the eswitch aspect of it good? :) 

I guess I could use a loop key but I like the idea of a momentary switch(like the unity)
```

---
## \#4 Posted by: longhairedboy Posted at: 2018-11-27T21:56:17.931Z Reads: 141

```
[quote="Sn4pz, post:3, topic:76294"]
On this topic, If I want a means of turning my board on and off that wont break, while supporting up to 100a, what would you do?
[/quote]

the 300 amp variant of this exact switch from Flier. Simultaneously, that company makes both a total shit switch and a completely bullet proof switch. The 300 amp version we have used in a number of boards including ones running at 13S with ridiculous settings. 

It probably won't take a full 300 amps but it will take over 100, and we've used it in boards with 5P and 6P cell groupings in BMS bypass with a lot of success.

[quote="Sn4pz, post:3, topic:76294"]
DiebieMS has a switch, does anyone have experience with that? Is the eswitch aspect of it good?
[/quote]

It works well. Very well, and basically forever.
```

---
## \#5 Posted by: Jc06505n Posted at: 2018-11-27T21:56:37.695Z Reads: 127

```
This is the sexiest implementation of a Loopkey I've seen 

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/5852?u=jc06505n
```

---
## \#6 Posted by: Sn4pz Posted at: 2018-11-27T22:14:02.246Z Reads: 116

```
I like the idea of a key system or something that stays in, similar to a car, but i fear I would lose the loop key / regular key x) 

Or some kind of security lol.... Being at uni means I should at least make it unfriendly for whoever might try to take my stuff :laughing:
```

---
## \#7 Posted by: dareno Posted at: 2018-11-27T22:19:02.432Z Reads: 109

```
@mmaner has some nifty little 3d printed mounts for loop keys.  Make it look all nice and cuddly.  
@accrobrandon no switch I have used so far has lasted more than 3 months.  Most seem to stick on though.  I will now be frantically searching up the item @longhairedboy has so kindly mentioned.  I use the bms switch on my bestech and loop keys on everything else for the moment.
```

---
## \#8 Posted by: accrobrandon Posted at: 2018-11-28T00:22:47.234Z Reads: 97

```
what about the one on yur site? Hows that wire up?
```

---
## \#9 Posted by: willpark16 Posted at: 2018-11-28T09:14:01.669Z Reads: 81

```
Replace it @Martinsp has some good ones
```

---
## \#10 Posted by: longhairedboy Posted at: 2018-11-28T15:40:13.549Z Reads: 77

```
[quote="accrobrandon, post:8, topic:76294, full:true"]
what about the one on yur site? Hows that wire up?
[/quote]

its fine for 12S 60 amp applications and below, and it uses a standard SPDT rocker switch.
```

---
## \#11 Posted by: briman05 Posted at: 2018-11-28T15:59:42.556Z Reads: 70

```
https://www.alibaba.com/product-detail/Flier-16S-300A-power-switch-for_60768819667.html?spm=a2700.7724857.normalList.1.43c51df1raLrw9

5 qty min at $38-$48 a pop isnt to bad wonder what the shipping would be.  I feel like 300a is where to be looking since no one should every be coming close to pulling 300amps
```

---
## \#12 Posted by: accrobrandon Posted at: 2018-11-28T16:33:58.266Z Reads: 63

```
yeah I enjoy having a standardized switch, may have to reach out to them and check costs... and maybe arrange some sort of mini group buy or something.... luna cycle upped their prices on the one that is same as mine... if they were still $35 on their site i still woulda bought a new one...
```

---
## \#13 Posted by: briman05 Posted at: 2018-11-28T17:24:24.870Z Reads: 54

```
@mmaner bought one and had it die on him in a short amount of time. I just check luna cycle and when you search them is says $35 but when you click on them it says 47 someone forgot  tofix the price on the other page lol
```

---
## \#14 Posted by: mmaner Posted at: 2018-11-28T17:30:31.364Z Reads: 56

```
I got 2 experimental versions, both of which had some sort of extra fail over fets.  1 is still running, the other died in about 3 months if I remember correctly.
```

---
## \#15 Posted by: Devilmycry Posted at: 2018-11-28T17:47:04.486Z Reads: 54

```
Hi man contact me here or on the nyc diy in telegram I have one make in nyc use it on every building I make and no problem 
I test it like craze
```

---
