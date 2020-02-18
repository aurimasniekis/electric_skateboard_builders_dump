# Talk me out of 12s setup

### Replies: 14 Views: 395

## \#1 Posted by: SqueekyCBJ Posted at: 2018-09-05T01:09:38.432Z Reads: 156

```
I'm building my first board and going for single motor, likely 6374.   I'm going to go LiPo for first build in order to save on budget.  I know however that I want to run a charge only BMS with e-switch.  I dont own a LiPo charger and figured why buy one if my BMS will do it from the get go.  

Originally I was looking into 10s BMS setup built with 2x 5s or 5x 2s.  Now I realize 12s gives me 3 different battery combinations. 

Is there any realize not to make the jump to 12s over 10s since the vesc supports it.
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-09-05T01:17:58.067Z Reads: 150

```
The vesc will support it, however there are multiple reports of DRV's blowing in the vesc when people run them on 12S as it is the peak capability of the VESC's. Focbox's and Vesc 6's seem to be able to tun them just fine. IMO, 10S is the sweet spot between power, range and speed. If you really want, you can run 11S
```

---
## \#3 Posted by: SqueekyCBJ Posted at: 2018-09-05T01:26:31.997Z Reads: 141

```
Thank you I appreciate this input, 10s BMS appear to be more redilaly available.  Now to find one in the US that has an e-switch.
```

---
## \#4 Posted by: mynamesmatt Posted at: 2018-09-05T01:30:16.959Z Reads: 136

```
https://buildkitboards.com/collections/parts/products/bestech-bms?variant=7201537687582

this guy stocks them in the US, choose 10s and it is 80A rated
```

---
## \#5 Posted by: mmaner Posted at: 2018-09-05T01:56:44.652Z Reads: 117

```
[quote="SqueekyCBJ, post:1, topic:67060"]
charge only BMS with e-switch
[/quote]

E-seitches only come on charge/discharge BMS's. You are actually bypassing the discharge function when using a BMS as charge only, so the E-switch won't work.
```

---
## \#6 Posted by: SqueekyCBJ Posted at: 2018-09-05T02:06:16.723Z Reads: 105

```
Thanks this thread has proven successful, stick with better charge/discharge BMS.  Looks like I'll go back to 10s, I'll look at 12s for the dual motor build next which will likely be li-ion.
```

---
## \#7 Posted by: SqueekyCBJ Posted at: 2018-09-05T02:08:18.101Z Reads: 100

```
To confirm with a e switch I don't need a anti-spark. I can just wire a spst.
```

---
## \#8 Posted by: mynamesmatt Posted at: 2018-09-05T02:11:35.559Z Reads: 98

```
i'm not sure if you NEED a loop key, but it is better to have one to have piece of mind that it  is completely disconnected when you're working on the board
```

---
## \#9 Posted by: mmaner Posted at: 2018-09-05T02:16:03.819Z Reads: 95

```
All you need is a 2 pole switch. The E-switch leads don't actually allow power to travese, they simply open or close a circuit which tells the BMS to either turn on or turn off the power.
```

---
## \#10 Posted by: b264 Posted at: 2018-09-05T02:24:00.202Z Reads: 90

```
I think you only need a a single-pole, single-throw on SOME antispark e-switches and a single-pole momentary on other antispark e-switches.  I'm not aware of any that need a 2-pole switch or a double-throw switch.
```

---
## \#11 Posted by: SqueekyCBJ Posted at: 2018-09-05T02:27:51.819Z Reads: 88

```
E Support Black 19mm 12V 5A Power Symbol Angel Eye Halo Car Purple LED Light Metal Push Button Toggle Switch Socket Plug Wire https://www.amazon.com/dp/B01IT0TX9G/ref=cm_sw_r_cp_apa_Y6ZJBbBWVW1D3

Going to be using this one,  my wife's board is gonna be so cool that I won't be embarrassed riding it till I can build one for myself.
```

---
## \#12 Posted by: mmaner Posted at: 2018-09-05T02:29:24.115Z Reads: 84

```
Your right, I was thinking 2 pin... Long day.
```

---
## \#13 Posted by: Eboosted Posted at: 2018-09-05T03:54:11.395Z Reads: 71

```
Please don't use 12s, it's too fun and your GF will throw you heavy things because you couldn't stop riding
```

---
## \#14 Posted by: DilatedPupils Posted at: 2018-09-05T04:40:50.895Z Reads: 60

```
[quote="Eboosted, post:13, topic:67060, full:true"]
Please don’t use 12s, it’s too fun and your GF will throw you heavy things because you couldn’t stop riding
[/quote]

And you're gonna end up building more 12S boards because they're just so awesome. So you're gonna spend a lot more money on this addiction.
```

---
