# Replaced DRV8302, VESC won&rsquo;t turn on

### Replies: 4 Views: 530

## \#1 Posted by: rcmanchild Posted at: 2016-11-27T21:16:13.948Z Reads: 77

```
Hey guys!
I have had 2 DRV chips go bad on my VESC's lately. I'm very well versed with SMT and reflow, so I figured this replacement would be too bad. I was using full lab grade equipment and could inspect for flaws with a microscope. Replacing both chips went as smoothly as I could have expected. But now, I can't get either ESC to boot up. No LED's or USB. It looks like the micro isn't getting power.

Has anyone seen this? Did I botch it?

Thanks in advance for any help I get!
```

---
## \#2 Posted by: Blasto Posted at: 2016-11-27T21:22:43.510Z Reads: 73

```
No led mean no 3.3V, means no 5V, means you didnt properly solder your drv.

If you did not properly solder the gnd pad on the drv, the zener diode is prob dead as the output of the buck goes higher than 5V
```

---
## \#3 Posted by: rcmanchild Posted at: 2016-11-27T21:28:51.080Z Reads: 69

```
I used a reflow station till the DRV was flat with a touch of solder paste under the pad. Then, I touched up the pins with a small iron to confirm continuity. Seems unlikely I'm missing a connection since I did all this under a microscope. Very odd.  Where could I touch off to find out of I'm outputting 5V where 3.3 should be?
```

---
## \#4 Posted by: Blasto Posted at: 2016-11-27T21:30:46.403Z Reads: 63

```
Look on the silkscreen on P2 connector, 3.3 and 5V are identified, most likely your coil gets hot
```

---
