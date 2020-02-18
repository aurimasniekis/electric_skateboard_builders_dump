# Trouble with space cell 3

### Replies: 19 Views: 655

## \#1 Posted by: roonydagoony Posted at: 2016-11-01T20:32:50.175Z Reads: 102

```
**Setup:**
Space cell 3 pro - 10s3p
12S TB ESC with 12S rated ubec
TB mini 2.4ghz controller
16/36T gear ratio w/ 83mm wheels

**Issue:** 
Works wonders for the 1st 2 miles after a full charge
After it goes down to about 82-85% charge level (about 2 miles), it is no longer able to go faster than 5-7 mph.

I tried this with a 6S battery(instead of the space cell) and had absolutely no issues for 4 months so I'm leaning towards the fact that the BMS could be the issue.

**Note: Also noticed that when I turn off the power, it doesn't turn off for a whole minute (slowly creeping down from the charge level to 0%).**

Thoughts? Suggestions?

Any help is appreciated

Thanks
```

---
## \#2 Posted by: ThomasRBK Posted at: 2016-11-01T20:39:38.213Z Reads: 97

```
Did you change your max voltage and voltage cutoff settings on the TB ESC if that's possible? I have no experience with these ;)
```

---
## \#3 Posted by: Jinra Posted at: 2016-11-01T20:40:25.994Z Reads: 94

```
I think you can program the ESC with a programming card to dictate how many cells your battery has. If that's not done that may be the reason.
```

---
## \#4 Posted by: roonydagoony Posted at: 2016-11-01T20:52:29.241Z Reads: 84

```
Ok, I'll try that out today. I think that could be it.
Thanks @ThomasRBK, @Jinra
```

---
## \#5 Posted by: ThomasRBK Posted at: 2016-11-01T20:52:50.679Z Reads: 78

```
Happy to help :slight_smile:
```

---
## \#6 Posted by: roonydagoony Posted at: 2016-11-01T20:53:36.212Z Reads: 77

```
I've only ever programmed it directly on the card, so I guess I have to connect this to a computer with the build in mini usb on the programming card?
```

---
## \#7 Posted by: ThomasRBK Posted at: 2016-11-01T21:09:01.005Z Reads: 72

```
Maybe some pictures? Really don't know how this ESC works :sweat_smile:
```

---
## \#8 Posted by: Pantologist Posted at: 2016-11-01T21:43:17.955Z Reads: 64

```
On the card you can choose the voltage cutoff. I keep mine off because no one trusts TB 12S ESC to do proper voltage cutoff.
```

---
## \#9 Posted by: roonydagoony Posted at: 2016-11-01T21:49:39.787Z Reads: 61

```
ah, I have mine at 3.4v....What are the risks involved with turning it off?
```

---
## \#10 Posted by: Namasaki Posted at: 2016-11-01T21:53:38.591Z Reads: 60

```
Same as @Pantologist
I ran this same Esc with low voltage protection off because it doesn't work accurately.
```

---
## \#11 Posted by: ThomasRBK Posted at: 2016-11-01T21:53:43.086Z Reads: 58

```
That you need to keep an eye out yourself ;) It just doesn't cut off your lipos when the voltage per cell is too low. So if you have a voltage meter in between that'd do the same in combination with some monitoring.
```

---
## \#12 Posted by: Pantologist Posted at: 2016-11-01T21:58:40.172Z Reads: 58

```
Well... If you don't check the voltage meter on the battery or if it is not accurate either, you can damage your cells by discharging them below max discharge voltage. 

Most people don't run into this issue since they'll just look at the battery voltmeter. 

The ESC just doesn't calculate the voltage accurately. It will shutoff with voltage sag and does not detect the correct voltage for some reason.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-11-01T21:58:48.350Z Reads: 56

```
If your climbing hills, your space cell voltage is probably sagging too low. 
You need a voltage meter on top of your board so you can monitor while riding.
```

---
## \#14 Posted by: roonydagoony Posted at: 2016-11-01T22:01:21.362Z Reads: 53

```
Seems like a cheap and easy solution. I'll order one immediately and see what's up.
I do go over hills on my morning and my evening commute. About half a mile long at 5-10% max
```

---
## \#15 Posted by: Namasaki Posted at: 2016-11-01T22:03:40.419Z Reads: 52

```
10% is enough to sag the voltage.
And 1/2 mile is a long climb
```

---
## \#16 Posted by: Pantologist Posted at: 2016-11-01T22:07:21.807Z Reads: 50

```
Wait what are you ordering?

The battery should have a volt meter already.
```

---
## \#17 Posted by: roonydagoony Posted at: 2016-11-02T15:28:16.306Z Reads: 38

```
it does but it's on the space cell (below the deck)
so i'll need another one on top to monitor it while riding
```

---
## \#18 Posted by: Jinra Posted at: 2016-11-02T15:40:03.194Z Reads: 35

```
Just flip it over after hard riding. The battery doesn't recover from sag instantly, you can read out how much it sags if you check immediately after stopping.
```

---
## \#19 Posted by: roonydagoony Posted at: 2016-11-07T17:42:03.164Z Reads: 22

```
yeah my esc is fried :slight_smile: not sure how but over the weekend....poof

anyway, another issue i'm seeing is that the bms, when turned off, takes 1-2 mins to actually turn off. the screen shows it slowly climbing down from the current % down to 0%
```

---
