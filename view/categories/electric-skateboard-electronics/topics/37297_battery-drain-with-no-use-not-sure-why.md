# Battery drain with no use&hellip;not sure why

### Replies: 13 Views: 912

## \#1 Posted by: kidcisco Posted at: 2017-11-04T02:39:14.594Z Reads: 119

```
I'm having an issue with a board I'm building that I have yet to ride. 

Just got new batteries from HK (old batteries were bad) and charged them up fully, all 4.2. I left the board with the batteries hooked up (in series) to the ESC, but I kept the loop key out so there was no power to the board. 

I come back a few days later and the batteries are drained. the 6s (2x 3s 5000mah) cells look like this: 4.2, 4.2, 3.7, 3.7, 3.7, 3.7. I haven't used the board at all. I did power it up for maybe 5 minutes to program my ESC and calibrate my remote. 

Why TF are the batteries low?
```

---
## \#2 Posted by: paragon Posted at: 2017-11-04T02:46:44.804Z Reads: 112

```
defective cells/wiring?
defective charger?
Zener diode?

Hard to say for sure without a diagram of your setup.
```

---
## \#3 Posted by: psychotiller Posted at: 2017-11-04T03:10:53.603Z Reads: 104

```
Do you have a bms hooked up to your batteries?
```

---
## \#4 Posted by: kidcisco Posted at: 2017-11-04T03:21:21.274Z Reads: 99

```
I'm trying to balance charge now and it won't move the cells past 3.77v.... 

I'm attaching a basic image of how I have it wired. I've sought feedback on the wiring on here and everyone seemed to say that it was fine. Charging through the balance plugs also, which everyone said was fine also. No sparks or any problems when connecting and attempting to charge.

Charger is genuine (AFAIK) [iMax B6 from Hobby King](https://hobbyking.com/en_us/imax-b6-50w-5a-charger-discharger-1-6-cells-genuine.html).

The diagram doesn't show the proper way I have the LiPo alarm wired but it's wired correctly. When I put the anti spark loop key in everything powers up and the LiPo alarm shows me the total volts and each cell. When I pull it out everything powers off. 
<img src="/uploads/db1493/original/3X/1/6/16119bb77d1a34d88519899046145b12e492a1f9.png" width="617" height="500">
```

---
## \#5 Posted by: kidcisco Posted at: 2017-11-04T03:21:51.366Z Reads: 93

```
No bms. This is my first build so I just wanted to do it basic and keep the costs down.
```

---
## \#6 Posted by: scepterr Posted at: 2017-11-04T03:29:09.633Z Reads: 90

```
Maybe faulty lipo alarm draining them?
```

---
## \#7 Posted by: psychotiller Posted at: 2017-11-04T04:35:01.039Z Reads: 85

```
It's the lipo alarm. It's not faulty They can't be left plugged in
```

---
## \#8 Posted by: kidcisco Posted at: 2017-11-04T04:51:14.418Z Reads: 82

```
Even if it's not on? I have the negative lead from the alarm going to the negative wire off my ESC, BEFORE the loop key, so the alarm is off (unless I put the xt90 plug in). Can it still drain if the alarm is off?
```

---
## \#9 Posted by: psychotiller Posted at: 2017-11-04T04:53:04.489Z Reads: 80

```
Unless your cells are bad, I think that's the only thing it could be.
```

---
## \#10 Posted by: pat.speed Posted at: 2017-11-04T06:30:35.307Z Reads: 65

```
That wouldn't explain why they won't charge though
```

---
## \#11 Posted by: torqueboards Posted at: 2017-11-04T06:48:42.039Z Reads: 58

```
It's the lipo alarm. Don't leave them plugged in or they'll drain your batteries on a few cells. Only keep them on when your riding.
```

---
## \#12 Posted by: kidcisco Posted at: 2017-11-04T07:23:42.478Z Reads: 58

```
First and foremost I appreciate the advice from everyone. AFAIK, the LiPo alarm is OFF...the screen is dark, no beeping, not illuminated, nothing. If I plug in my loop key, it comes to life and gives me total and individual cell readings. I've left it unplugged though for a few days now. The batteries are connected in series though to my ESC and the balance wires are connected, but nothing has power (loop key has been disconnected). How else could the batteries be draining?
```

---
## \#13 Posted by: Nordle Posted at: 2017-11-04T07:29:09.005Z Reads: 53

```
It can drain power from your batterys, even if you cut the black wire and the display is off.
Thats almost sure the reason for your problem.
```

---
