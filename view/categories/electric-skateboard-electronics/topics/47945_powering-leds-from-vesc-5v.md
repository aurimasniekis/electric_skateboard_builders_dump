# Powering LEDs from VESC 5v?

### Replies: 13 Views: 943

## \#1 Posted by: TheFluffiest Posted at: 2018-03-02T16:27:33.411Z Reads: 136

```
Is it possible to power LED flashlights from a vesc? Specifically from the plug that powers the reciever? I have dual vescs and wanted to have one powering the receiver and the other powering some headlights... Will that burn out the vesc?
```

---
## \#2 Posted by: bevilacqua Posted at: 2018-03-02T16:29:09.573Z Reads: 136

```
yes it works, 0 issues
```

---
## \#3 Posted by: Slak Posted at: 2018-03-02T16:38:34.568Z Reads: 132

```
There is also a 5V source on the UART connector, isn't it ?
```

---
## \#4 Posted by: mmaner Posted at: 2018-03-02T16:52:40.402Z Reads: 127

```
pin 1 on the P3 (UART) header is 5v

![image|333x284](upload://rgoL1mLjB4lWwXnDITPZMSnLoLQ.png)
```

---
## \#5 Posted by: TheFluffiest Posted at: 2018-03-02T16:56:26.435Z Reads: 124

```
@bevilacqua @Slak @mmaner There's no chance of the vesc burning out? That would be a super easy solution to my problems! Thanks everyone!
```

---
## \#6 Posted by: mmaner Posted at: 2018-03-02T16:58:14.157Z Reads: 120

```
I wont say there's no chance, but I don't see any difference in using the +5v lead to power a BT adaptor and a light bar.  Personally I use it to power a LED power switch, have for months with no issues.

![latching switch - how to wire v2 110617|603x500](upload://duBulb9kdkEJ5QDAIrcGJSvQRe5.JPG)
```

---
## \#7 Posted by: thisguyhere Posted at: 2018-03-02T17:04:13.025Z Reads: 117

```
just don't draw too much amp off it, I think that 5v port is rated at 1a. 

powering two smaller 300lm led in parallel draws about <s>500a</s> 500mah so don't get carried away and overload that circuit. 

proper way would be to use a led driver, like meanwell ldd-1000h, or a buck step down,  connected in parallel to main battery pack.

[quote="bevilacqua, post:2, topic:47945"]
0 issues
[/quote]

not true
```

---
## \#8 Posted by: Scoo_B_SK8 Posted at: 2018-03-02T17:04:55.446Z Reads: 113

```
adding "options" to power source will decrease power and distance
```

---
## \#9 Posted by: bevilacqua Posted at: 2018-03-02T17:18:33.314Z Reads: 110

```
Okay for led lights up to 4W*** ;)
```

---
## \#11 Posted by: ZackoryCramer Posted at: 2018-03-02T17:26:32.589Z Reads: 105

```
I wouldn't want to rely on the brain to provide power for such a power consumptive component. I recommend getting a BEC(dc to dc converter) for the job, it’s more efficient too. 😉
```

---
## \#12 Posted by: Scoo_B_SK8 Posted at: 2018-03-02T18:54:20.667Z Reads: 102

```
"Options" = would be anything beyond the basic board (motor(s),vesc(s)/focbox(s),remote). So things like Bluetooth modules, leds, headlights, tail lights, running lights.
```

---
## \#13 Posted by: Namasaki Posted at: 2018-03-02T19:23:36.978Z Reads: 101

```
As @thisguyhere mentioned, the Vesc can only handle light duty on the signal and uart ports.
Headlights bright enough to be effective might be too much and if you burn out the buck converter, you'll have no control and no brakes.
Better not risk it, just get a separate converter as suggested by @ZackoryCramer
```

---
## \#14 Posted by: Scoo_B_SK8 Posted at: 2018-03-02T19:58:23.421Z Reads: 96

```
I agree ☝️ anything more than the modules(light duty) is nonsense
```

---
