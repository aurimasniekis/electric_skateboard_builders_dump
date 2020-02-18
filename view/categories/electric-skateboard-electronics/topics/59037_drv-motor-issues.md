# DRV + Motor Issues

### Replies: 16 Views: 374

## \#1 Posted by: sterlinggray4 Posted at: 2018-06-15T19:27:16.771Z Reads: 99

```
Okay, I have been working on my board for 6 months now and I had it intermittently running until I blew my DRV on my VESC 4.18. After a nice headache and a week of shipping in comes two new DRV's and after messing up the first one I got the 2nd one Soldered on my board using Hot Air. 
Everything looks good under a microscope, and when I plug it into my computer the VESCtool doesnt throw any errors. Looking good. 
But now when I plug my 6364 into my VESC and try to get it to move at all nothing happens. No matter what I do I cant get it to even make a noise.
I know that the motor works as it is easy to turn when the leads are disconnected and hard tot urn when I short two of them together.
My last Idea is that I have somehow messed up the DRV after Soldering it and I am hoping that by posting this someone who actually knows what they're doing can help me trouble shoot.
```

---
## \#2 Posted by: Eboosted Posted at: 2018-06-15T19:32:47.884Z Reads: 88

```
Save yourself a headache and buy a focbox.

When things like this happen you might end up investing a lot of time and and will go through many frustrations. BTW I suggest you buy focboxes and a replacement one in case something goes wrong with it.

BTDT
```

---
## \#3 Posted by: sterlinggray4 Posted at: 2018-06-15T19:47:31.588Z Reads: 79

```
I have seen the love for FOCBOX's on the forum but I don't understand why I should buy an extra one. It sounds like you're just saying all VESC are crap so buy two, buy ten because eventually they'll all break. I would much prefer trying to fix it as this is a DIY site after all and if Someone else can do it I feel like I should be able to. If I should buy a FOCBOX because they're better then why would I need a replacement? I appreciate your advice but I was hoping that someone had a solution to my motor not spinning.
```

---
## \#4 Posted by: wafflejock Posted at: 2018-06-15T19:50:30.574Z Reads: 74

```
Think eboosted was more saying it's good to have a backup in case things go wrong rather than you should expect things **will** go wrong (don't want to have to wait on shipping yet again or be ordering when there's some shortage or other backups in production).  Regarding time sunk into it unless you really know what you're doing (your name is @JohnnyMeduse) debugging what exactly failed is probably not worth the time (I tried once too before throwing in the towel).
```

---
## \#5 Posted by: Scoo_B_SK8 Posted at: 2018-06-15T19:53:49.754Z Reads: 72

```
9 out of 10 its user error that breaks Vesc // Focbox (IMO)

after you replace a chip usually need to reinstall everything starting with the bootloader then firmware.  also other components could have been damaged in the DRV burnout.

Edit;  if you can connect and install firmware than you shouldn't need to mess with bootloader
```

---
## \#6 Posted by: sterlinggray4 Posted at: 2018-06-15T19:54:45.683Z Reads: 62

```
Oh I haven't tried that-will do
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2018-06-15T20:18:18.517Z Reads: 64

```
Check the mosfet... you might have blown one at same time as the DRV, Also check if R48 To R51 are 100ohms (and just to be sure that they are connect properly in the circuit, you should mesure 200Ohms on the Cap C36 and C34)
```

---
## \#8 Posted by: sterlinggray4 Posted at: 2018-06-15T20:39:36.711Z Reads: 63

```
@JohnnyMeduse The resistors all are each pulling ~100Ohms and it looks like it is correctly hooked up in parallel. The capacitors also look like they hooked up in series and correctly pulling 200 ohms across them. As for the Mosfets I am not exactly sure how to measure them correctly but no matter how or where I probe them with my Ohmmeter all 6 have nearly identical behaviors weather powered on or powered off
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2018-06-15T21:11:36.780Z Reads: 63

```
First thing you could do is check if the red light flash 3 time during the boot sequence. If not there is something wrong in the drv circuit.

Second, pass over the pads of the DRV with a soldering Iron, I know they look good under a Microscope, but your never too cautious. 

Third, if your try to run a motor detection, check if the green light brighten up, if so check if R20 is good (10K)
```

---
## \#10 Posted by: Eboosted Posted at: 2018-06-15T21:31:43.077Z Reads: 58

```
[quote="sterlinggray4, post:3, topic:59037"]
I don’t understand why I should buy an extra one
[/quote]

Because it will help keep riding and enjoying the hobby when your board is out of service. It's just a good will good advice that has helped me a lot in the past.

Sorry if this isn't the answer you've been waiting.
```

---
## \#11 Posted by: banjaxxed Posted at: 2018-06-15T21:35:38.872Z Reads: 54

```
Even with hot air it’s tricky, I had something similar happen with a home brew drv replacement 

Bad ground or a solder run off the ground to the pins can do this, I’d go ahead and check the drv again
```

---
## \#12 Posted by: sterlinggray4 Posted at: 2018-06-16T16:07:26.869Z Reads: 46

```
No that's super helpful advice actually if I don't end up getting this working I'll take your advice and just invest in 2 Focbox's. Thanks.
```

---
## \#13 Posted by: sterlinggray4 Posted at: 2018-06-16T17:21:12.944Z Reads: 42

```
The red LED is not lighting up three ties during boot, and the green light is brightening and I cant get a read on R20 so I'll go ahead and replace that along with remounting the DRV
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2018-06-16T17:25:24.034Z Reads: 43

```
[quote="sterlinggray4, post:13, topic:59037"]
I cant get a read on R20
[/quote]

Well... if you don't get any read on a resistor, it sound like it could be broke
```

---
## \#15 Posted by: sterlinggray4 Posted at: 2018-06-16T18:17:05.091Z Reads: 34

```
Okay for my final attempt I replaced the DRV again using my last chip and got it perfectly aligned. Went back over the soldering connections and replaced the R20. No change still only the blue light and green light when it boots up. I think that the sign I call it quits?
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2018-06-16T19:28:15.566Z Reads: 31

```
I think true that same kind issue in one of these Video

https://www.youtube.com/channel/UCo3fMYtsfrZR82vuqvJYEuw
```

---
