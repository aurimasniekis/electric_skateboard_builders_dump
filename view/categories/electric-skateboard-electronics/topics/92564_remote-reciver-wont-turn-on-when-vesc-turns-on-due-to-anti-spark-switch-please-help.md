# Remote reciver won&rsquo;t turn on when vesc turns on due to anti spark switch. Please help!

### Replies: 21 Views: 365

## \#1 Posted by: M.Hboards Posted at: 2019-05-02T15:56:23.216Z Reads: 81

```
So iv been useing a Loopkey on by board for the past few weeks and its been perfectly fine but last night i installed a anti spark from @JLabs (made by @Martinsp) and once i did that my remote reciver (flipsky vx1 through uart) would no longer power up. (The rest of my setup would) Sounds craze that the anti  spark somehow caused this but when i take out the antispark and power the vesc (flipsky 4.12) up straight from the battery the reciver powers up perfectly fine. Another piece of info that may help solve the mystery is that if I unplug the receiver and then plug it back in while the anti spark is on it will then power up but once I shut off the anti Spark and Power the board backup the receiver won't turn back on.

If anyone could help me solve this issue or knows what the issue may be please let me know @blasto @Deodand @Martinsp 

Heres the wireing diagram for the reciver if it helps-
![Screenshot_2019-05-01-23-14-43~2|690x477](upload://nE8bc56AFkp7v4LFOtMF9PAF47b.png)
```

---
## \#2 Posted by: Andy87 Posted at: 2019-05-02T16:16:16.329Z Reads: 76

```
Do you have a picture how you actually wired up the anti spark in your circuit? Did you have the xt90s loopkey before on the plus or minus?
```

---
## \#3 Posted by: M.Hboards Posted at: 2019-05-02T16:24:04.376Z Reads: 74

```
@Andy87 Anti spark is wired like any Normal antispark and i belive  the antispark im useing interups the negitive side just like my Loopkey did.![0502191223_HDR|690x328](upload://HJiYrdRtdZRCcU1q53EKzdEDGg.jpeg)
```

---
## \#4 Posted by: Deodand Posted at: 2019-05-02T19:05:25.798Z Reads: 64

```
Your receiver probably has some form of safe start voltage regulator on board, the soft start  of the antispark is probably putting it into a latched fault mode. If you get me a good enough photo of the ICs inside I might be able to guess what's going on if they are labeled.
```

---
## \#5 Posted by: M.Hboards Posted at: 2019-05-02T19:17:23.097Z Reads: 57

```
 @Deodand What is an ics and is it on the antispark or reciver?
```

---
## \#6 Posted by: Mich21050 Posted at: 2019-05-02T19:21:31.508Z Reads: 57

```
[quote="M.Hboards, post:5, topic:92564"]
ics
[/quote]

Ic stands for integrated circuit. Those small black "boxes". :slight_smile:. In short @Deodand wants a good picture of the receiver PCB.
```

---
## \#7 Posted by: M.Hboards Posted at: 2019-05-02T19:22:35.323Z Reads: 56

```
There on the remotes reciver correct?
```

---
## \#8 Posted by: Mich21050 Posted at: 2019-05-02T19:22:51.337Z Reads: 56

```
Yes.
10char
```

---
## \#9 Posted by: M.Hboards Posted at: 2019-05-02T19:39:07.599Z Reads: 54

```
![0502191532|690x328](upload://hejlWb3gWU32n0xuk7SEgMpHx9u.jpeg) 

The small black box on top of the yellow box i belive says LG33 with what looks like an underscore between the L and G and the larger box / chip says pan163CX
1902CAa
```

---
## \#10 Posted by: Deodand Posted at: 2019-05-02T20:12:24.503Z Reads: 53

```
https://www.google.com/url?sa=t&source=web&rct=j&url=https://cdn-shop.adafruit.com/product-files/3081/mic5219.pdf&ved=2ahUKEwjF0frV0_3hAhXT6J8KHSFEAFwQFjAAegQIAxAB&usg=AOvVaw01f0t1pEEkpVxkZzFphFFY

This is the voltage regulator... Simple ldo not sure why it would not be booting.

Does the issue persist when you disconnect the battery sensor?
```

---
## \#11 Posted by: M.Hboards Posted at: 2019-05-02T22:47:45.938Z Reads: 50

```
 @Deodand I uplugged the voltage sensing wire.  (The one that goes straight into the battery's positive right?) And still no luck however don't know if this means anything but regardless if the voltage sensing wire is attached or not when i shut off the switch and then wait around 10-30 sec. When i power it back on the reciver will turn on like normal but if i leave the switch off longer then i need to unplug and replug the reciver to get it too power on.
```

---
## \#12 Posted by: M.Hboards Posted at: 2019-05-05T01:06:48.053Z Reads: 41

```
@deodand I'm not sure if you missed my last post in this thread or not but if you have any other idea to what the prob may be or a possible solution if you can let me know it would be greatly appreciated thanks.
```

---
## \#13 Posted by: M.Hboards Posted at: 2019-05-06T18:49:40.382Z Reads: 33

```
Bump 

Someone please help


@Deodand @Martinsp
```

---
## \#14 Posted by: M.Hboards Posted at: 2019-05-07T17:41:16.210Z Reads: 33

```
Update problem still occurs even in ppm mode.
```

---
## \#15 Posted by: b264 Posted at: 2019-05-07T17:51:03.070Z Reads: 30

```
Have you asked the remote receiver manufacturer, or are they simply outsourcing customer service to us?

What did they say?
```

---
## \#16 Posted by: M.Hboards Posted at: 2019-05-07T17:54:45.725Z Reads: 32

```
I have yet to ask flipsky  but i do plan on it asked here first.
I don't think it's defective as it works fine with a Loop key. I think it's something to do with what @Deodand said above.

[quote="Deodand, post:4, topic:92564"]
Your receiver probably has some form of safe start voltage regulator on board, the soft start of the antispark is probably putting it into a latched fault mode.
[/quote]
```

---
## \#17 Posted by: mythe00 Posted at: 2019-09-26T16:55:32.312Z Reads: 9

```
I suspect I have the same issue as you.  I have an anti-spark switch, VESC, and Flipsky VX1 remote+receiver.  Ever since installing the anti-spark switch, which has a noticeable precharge that lasts almost a full second, the receiver will only turn on some of the time.  It seems to be completely random, sometimes the receiver will work fine after days of inactivity and other times it just won't turn on for 10 reboots in a row.

I have an idea to put a zener diode between the controller and the receiver, so that the receiver will only receive >5v.  Does anyone know if this is a sound plan?  I think it's either that or a physical switch so that I can turn the receiver on after the controller is switched on.  But I'd rather not have to hit an extra power switches every time I use my board.
```

---
## \#18 Posted by: M.Hboards Posted at: 2019-09-26T17:33:24.894Z Reads: 6

```
Yeah I think it has something to do with long pre-charge times. What company anti spark Are you useing?
```

---
## \#19 Posted by: mythe00 Posted at: 2019-09-26T17:48:34.251Z Reads: 7

```
I'm using the BKB 100a anti spark.  There's about a 1 second pause between depressing the button and the LEDs going from partially to fully lit.

I'm going to test the voltages going to the receiver this weekend with a multimeter to confirm my suspicions about the low voltage setting off a fault mode.  If that's the case it seems like the zener diode should fix the issue.  I have very little circuitry knowledge though and only found out about these components from a Google search, so it would be nice if someone could weigh in on how sound an idea it is.  I wouldn't want the receiver cutting out during use.

Update:  Zener diode isn't the right component to use.  I didn't know that the diode subtracts that amount of voltage from the circuit.  I instead used a small 5v relay.  The relay only triggers after the ESC gets full power and then connects the receiver to the ESC.  Everything is working perfect so far but I haven't been able to do too much testing yet.
```

---
## \#20 Posted by: M.Hboards Posted at: 2019-09-26T18:01:05.741Z Reads: 7

```
Thats the same antispark I had the issue with.

I now have the maker-x antispark and its working fine with the vx1 but I haven't done all that much testing yet.
```

---
## \#21 Posted by: mythe00 Posted at: 2019-09-26T18:29:17.104Z Reads: 6

```
Good to know, I might give that antispark a shot too, thanks.
```

---
