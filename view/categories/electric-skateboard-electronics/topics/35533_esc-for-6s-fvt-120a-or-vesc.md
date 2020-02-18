# ESC for 6S, FVT 120A or VESC?

### Replies: 11 Views: 1286

## \#1 Posted by: daniel309 Posted at: 2017-10-14T22:06:41.283Z Reads: 113

```
Hi everyone, I have been going back and forth on this one and would appreciate your comments. 

I build my own 6s7p battery (NCR18650) which takes up so much space that I will very likely never go above 6s. Given that, what would you recommend, the FVT120A or the HK VESC ("turnigy esk8 esc")?

Other parts
- 70mm wheels (will upgrade to 90mm eventually)
- HK motor mount + pulleys. 15mm belt. Gears: 15 (drive), 36 (wheel)
- SK3 6364 245kV

Been running all that through the esk8 calculators out there, amp draw, top speed etc. are all within limits and ok for me. 

However, 
I keep reading 6s is at the Amp limit of the VESC, so higher risk to fry it (already seems quite high risk anyways...). The VESC mosfet's limit is 50, and I want to be able to draw at least 50 or 60 battery amps to have enough power for the board. So I would definitely operate at the limits, especially when I upgrade to 90mm wheels. Is the VESC with 6s worth the risk? 

I am guessing the FVT 120A with the "161214" (brakeLine / linear brake) firmware will hold up better with 6s. At least there seem to be many more 6s builds out there that use this one instead of the VESC. 

I dont mind losing the configurability of the VESC, if I get better reliability in exchange for less options  and features. 

So, whats your take on this one?
```

---
## \#2 Posted by: JLabs Posted at: 2017-10-14T22:12:38.902Z Reads: 110

```
I would not run the VESC on 6s.. you pull too many amps. I have had good success with the FVT 120a on my first build (not sensored) and the new firmware. Some others have blew the FVT but I believe most of them were running sensored.
```

---
## \#3 Posted by: pat.speed Posted at: 2017-10-14T22:37:01.760Z Reads: 103

```
The X-car beast esc is another tried and true 6s esc that works great I have it on my build. The only problem is the screeching brakes
```

---
## \#4 Posted by: Namasaki Posted at: 2017-10-14T23:17:14.050Z Reads: 101

```
running sensored and trying to start from a dead stop pulls too many amps doesn't it?
```

---
## \#5 Posted by: Colson003 Posted at: 2017-10-14T23:38:23.652Z Reads: 93

```
I'm running my VESC on 6s in sensored FOC with TB 130kv hub motor. Just switched to FOC this week, the rest has been this way for a month.
```

---
## \#6 Posted by: bigben Posted at: 2017-10-15T06:58:49.926Z Reads: 81

```
http://www.electric-skateboard.builders/t/skywing-120a-esc-review-after-very-short-term-use/35380/31
This guy seems keen on this solution? For the price it could be worth a go?
```

---
## \#7 Posted by: daniel309 Posted at: 2017-10-15T09:23:32.405Z Reads: 73

```
yes, this one is interesting too. Ill have a look. Not sure however if I am adventurous enough to try this one yet.
```

---
## \#8 Posted by: daniel309 Posted at: 2017-10-15T09:34:44.128Z Reads: 71

```
Thanks everyone for the feedback, really appreciated. Just wondering if there are more happy 6S VESC users out there, in addition to @Colson003?
```

---
## \#9 Posted by: Colson003 Posted at: 2017-10-15T17:10:31.150Z Reads: 57

```
@daniel309 FYI I'm running a TB VESC
```

---
## \#10 Posted by: daniel309 Posted at: 2017-11-23T22:59:11.176Z Reads: 47

```
update: I bought the FVT 120A, and disasembled it to remove the original caps and solder new ones horizontally, removed the fan and the top case to reduce overall height to about 20mm (want the enclosure to be nice and flat...). 

Doing so, I took a picture of the PCB with the MOSFETs there, and found their datasheet: 

<img src="/uploads/db1493/original/3X/8/1/810b799875af6bd2e42eff8eb04d713691dd3588.jpg" width="375" height="500">

The MOSFETs on the board are **IRFH5301**. Each FET can sustain 100A continuous at max 100 °C. Max temperature is 150 °C. Pulsed drain current can be up to 400A. https://www.infineon.com/dgdl/irfh5301pbf.pdf?fileId=5546d462533600a40153561b477b1ebe

This gives me comfort that for 6S and a 6463 (245kV) motor, I should be good with this ESC.
```

---
## \#11 Posted by: daniel309 Posted at: 2017-12-21T23:03:29.008Z Reads: 35

```
Ok, I should have read the VESC's MOSFET datasheet before I posted. Clearly, the MOSFETs there are much more capable than the ones on the FVT 120A. 

The VESC's IRFS7530-7PPbF sustains 240A continuous, 1450A (!) pulsed @10V and 100 °C (175 °C max) and can dissipate 375 W of power. 
http://www.mouser.com/ds/2/196/irfs7530-7ppbf-1228415.pdf

One thing that may make a difference though is that the FVT 120A ESC has a total of 24 power MOSFESTs (12 on the front and on the back), the VESC has 6. 

I am wondering where these recommendations come from that the VESC does not like 6S and will overheat because of too much current. Are there any users out there where the VESC actually overheated at 6S?
```

---
