# VESC Questions Thread

### Replies: 4 Views: 460

## \#1 Posted by: Esrapp21 Posted at: 2017-01-15T02:41:20.119Z Reads: 61

```
Hi guys, I have been on this forum for a few months now and one thing I notice is how many VESC question threads there are. I just received the majority of the parts for my first build, so I figured I would, too, have plenty of questions. So, I'll start with a few questions and feel free to comment any of your questions below!

My experience:
I have a SPACE Cell 3, single carvon v2.5 hub, and a carvon VESC. Jerry sets up some of it for you, so I figured why not! Anyway, I was wondering about the current and voltage limits. Is there like a formula for each of these, I.e. Cutoff start is 4x-3 where x is battery voltage?
Also, I have one of the Bluetooth modules that connect to your phone that allow you to monitor your board, how could I set that up?

I don't know if this topic will catch on, but hopefully this becomes a convenient thread to post your VESC Questions!
```

---
## \#2 Posted by: lox897 Posted at: 2017-01-15T03:07:56.654Z Reads: 55

```
[quote="Esrapp21, post:1, topic:16122"]
Also, I have one of the Bluetooth modules that connect to your phone that allow you to monitor your board, how could I set that up?
[/quote]

You will need to set your baud rate on your vesc and wire the bluetooth module to the vesc. Also select PPM + UART if you are using a ppm remote
```

---
## \#3 Posted by: NickTheDude Posted at: 2017-01-15T03:25:58.538Z Reads: 50

```
Voltage cutoff depends on your cells chemistry. For my lipos I started the cutoff at 3.6 per cell and end at 3.4 per cell, so 36 and 34 volts on my 10S pack. That could be a little conservative but I'd rather be on the safe side. 

Also, out of curiosity could you share the max motor/battery amps that the carvon VESC comes configured with?
```

---
## \#4 Posted by: Esrapp21 Posted at: 2017-01-15T03:54:43.813Z Reads: 44

```
Yeah, I should get it within a week or two, I will be sure to check that.
```

---
