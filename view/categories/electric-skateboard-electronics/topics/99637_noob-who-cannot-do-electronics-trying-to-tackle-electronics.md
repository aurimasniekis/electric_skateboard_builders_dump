# Noob who cannot do electronics trying to tackle electronics

### Replies: 6 Views: 213

## \#1 Posted by: Ben2 Posted at: 2019-08-03T10:57:39.622Z Reads: 79

```
Okay here is the rundown.
Building a board from scratch after trying to learn as much as possible about how it works etc.
What I have gathered is that, in terms of battery, most people opt for around 10s2p or better in order to get a solid range as well and a good voltage for a decent top speed. I however, am poor, and this means that my options of good Li-ions are already off the table, tried looking into building my own battery but I feel this is beyond my talent so I wanted to know firstly if the setup I plan on using will work and secondly if it will give an average performance (not looking for high end as this is just coursework).

The batteries I am looking at are these: https://www.banggood.com/2Pcs-ZOP-Power-14_8V-4500mAh-4S-45C-Lipo-Battery-XT60-Plug-For-RC-Car-Boat-Quadcopter-p-1367591.html?rmmds=search&cur_warehouse=CN
and I believe these will give me 29.6V with 4500mAh and 45C. Still not too sure what the 45C is/means but I think the range will be a bit short and the speed will be alright. Can anyone help me on this.

(Side note - will it work with: https://www.banggood.com/Upgraded-24V36V-Dual-Drive-Controller-ESC-Substitute-for-Electric-Skateboard-Longboard-Control-p-1202299.html?rmmds=search&cur_warehouse=UK because the product details on this list two voltages and mine is in the middle so I'm not sure if this is ideal or just wrong.)
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-08-04T06:08:17.901Z Reads: 59

```
Avoid batteries from sites like bangood. Try and get them from hobbyking and look for the turnigy 5000mah packs. They come in several cell counts and are tried and tested to work fine in esk8.

As for the esc, those things are sketchy at best. Just spend a little extra and buy a cheap flipsky vesc.


If you cant afford the vesc, buy the hobbywing skate esc for hub motors. Its the best super cheap esc out there atm and works very well.

https://www.ownboard.net/products/ownboard-electronic-skateboard-esc-motherboard?variant=6950811500586

Alot of companies use it now, it will look exactly like that. Sometimes it doesnt have the black resin and is a bare pcb but if it look the same, it likely is
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-08-04T06:30:44.563Z Reads: 48

```
C rating is the maximum discharge current of the battery, measured in a weird way - you have to multiply the capacity of the pack (4500mAh or 4.5Ah in the case of the lipo you linked to), times the C number. So 45 times 4.5Ah gives 202.5A. (Take these ratings with a **big** grain of salt. They are usually way inflated and you don't want to run your batteries anywhere near that number - I'd say divide by three or four to get something reasonable - 50A sounds plausible.)

If you go [here](https://calc./) and plug in all your proposed parts, you'll get a pretty good estimate of your speed, range, etc.
```

---
## \#4 Posted by: tuheeb Posted at: 2019-08-04T15:30:27.161Z Reads: 30

```
45c 4500mAh (4.5Ah) which means 45*4.5 = 202.5 Amp. Battery pack should have this number and above of that. But cells should be genuined. 

About the Esc, you could find some good deal with used VESC, learn about it to test before buying :smiley: . Minimum is Hobbywing ESC if you can find it somewhere. :hugs:
```

---
## \#5 Posted by: wafflejock Posted at: 2019-08-04T15:44:54.280Z Reads: 27

```
That ESC is for dual motor and not going to be as configurable as a VESC (can get a VESC 4.x for just under $100 typically), maybe see if anyone here has a VESC they are willing to part with if that's still too much, but think single drive is the way to go. In terms of voltage if you are in the min to max range stated by the ESC you're good, min voltage is cells in series times 3.6 (would leave the .6V buffer if cells dip below 3.0V in lipo packs it damages the cells) max voltage is 4.2 times cells in series.  8S should be usable but won't feel as punchy (I tried with 6S 12S and now ride 10S, it's a happy medium).
```

---
## \#6 Posted by: Ben2 Posted at: 2019-08-07T00:45:27.104Z Reads: 13

```
Thanks for all the advice guys. I think the battery I want to go with is: https://hobbyking.com/en_us/turnigy-5000mah-4s1p-14-8v-20c-hardcase-pack-1.html
but in a 8s1p config. I know this won't exactly be ideal and may not perform but honestly if it works it works and then later down the line I can upgrade it.

Still looking at an ESC that I can try get for under £50 but no luck yet.
```

---
