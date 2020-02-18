# Problems Building VESC

### Replies: 21 Views: 2470

## \#1 Posted by: Weberp7593 Posted at: 2016-10-11T23:17:37.987Z Reads: 185

```
Hey guys,
I have 3 questions who don't let me finish my VESC.

1 In which direction should the 8Mhz Quarz look?
(He got 4 pins)

2 In which direction should the LEDs look?
(Can't see on my plan)

3 A resistor (the number e.g R16) is hiding so I can't see on the plan:
See here:
<img src="/uploads/db1493/original/3X/3/5/358110896e990116ab883f3574a9da1ef72aef1b.png" width="281" height="499">

I am using this one:
<img src="/uploads/db1493/original/3X/5/8/586e851c6e0d219dca6a1ed8cc59a6a1d06d01de.png" width="326" height="500"><img src="/uploads/db1493/original/3X/a/d/ade0ac1676165fe824ccaabfd061a23293327641.png" width="296" height="500">


I would be very happy if someone could helpe me :) 

Regards!
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-11T23:29:20.643Z Reads: 175

```
maybe check the schematics? you can get them from vedder's github
```

---
## \#3 Posted by: rpn314 Posted at: 2016-10-12T07:14:05.150Z Reads: 167

```

1. I believe I put it so the text on the chip was right side from how you have the PCB oriented in the picture above, but the truth is that it doesn't matter. Given the orientation of the crystal I am almost positive it will work either way (just not upside down) since it's a crystal that just oscillates (doesn't have polarity) and the grounds are in opposite corners. I can check it in the morning for you to be sure, if no one beats me to it.  edit: The spec sheet (found via Mouser [here](http://www.mouser.com/ds/2/3/abm3b-39910.pdf) indicates that usually pad 1 has a slight chamfer (think "cut corner"), on the inside, as you can see in this screenshot from the spec sheet.<img src="/uploads/db1493/original/3X/4/9/4909d224218ef7c029498de05ba6a2101e9c4480.png" width="690" height="175"> Pad 1 is the one that goes in top right of the board in the orientation of the pictures you posted (the closest pad to C5)

2. Gnd is up. Here's a screenshot I just took from Vedder's schematics. Just note that it shows them in the mirror as you see them (D1 to D3 right to left, instead of left to right as is seen from that side of the board) . <img src="/uploads/db1493/original/3X/f/d/fd540bba631f249c54ed5caa6bd363361ddab8e6.png" width="661" height="500">

3. The one right above R401 is R17, and the one just to the left (in your picture) is R18. <img src="/uploads/db1493/original/3X/4/c/4c878e7474ab2e3d6cc66b2254de7bc0355769a2.png" width="690" height="407">
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-10-12T12:45:49.417Z Reads: 138

```
There no right way to place the crystal, it's symmetric.

Also these might picture might help you with the placement (they are suppose to be in Vedder files)

<img src="/uploads/db1493/original/3X/c/b/cb9e4d40cb81ca015590b0edd4463a6a71a1ba02.jpg" width="690" height="453"><img src="/uploads/db1493/original/3X/1/c/1c0492c1ad50ea2215a5162a5b41d9d4cd4a5870.jpg" width="690" height="456">

You need to cross-reference it with the BOM.
```

---
## \#5 Posted by: rpn314 Posted at: 2016-10-12T13:32:16.374Z Reads: 125

```
Tried to check what I did, but I can't see through my shrink wrap and behind my red wire....but I'm still fairly confident that it doesn't matter, just as @JohnnyMeduse said.
```

---
## \#6 Posted by: Weberp7593 Posted at: 2016-10-12T20:05:03.649Z Reads: 116

```
Thanks to all of you! fot searching and figuring out the problem.
You helped me a lot.
I was too stupid to check the shematics...

I try to continue with the last few components next week.
then i will give a feedback ;)

Regards
```

---
## \#7 Posted by: rpn314 Posted at: 2016-10-13T00:09:26.771Z Reads: 100

```
You got it! I built two for myself and helped diagnose an few issues a friend of mine had after he built his, so feel free to reach out!
```

---
## \#8 Posted by: Weberp7593 Posted at: 2016-11-23T21:48:49.241Z Reads: 85

```
@rpn314 thank you maybe I will write you an PN if I get stuck again.

I soldered mine today. And I hope now I am finished.
So I can Programm in a few days.

Do you program with Linux or windows?
```

---
## \#9 Posted by: rpn314 Posted at: 2016-11-23T23:54:48.928Z Reads: 80

```
To flash the VESC with the bootloader and default firmware I used Windows 10. I think the stlink software I found first ran on windows, so I wen with it, but I've done stuff since with Linux. I flashed my nunchuckrf in ubuntu.
```

---
## \#10 Posted by: Weberp7593 Posted at: 2016-11-24T09:46:48.073Z Reads: 75

```
Ok thanks, then maybe you can help me.
I have the ST-Link2 the withe one.
And I also want to flash with windows.
But I don't know where I can get the hex file for the 4.12.
And also someone said I need 2 hex files one for the software and one for the bootloader.
Other ones said there is a single hex file with both.

How do you do it?
And can you maybe upload the hex?
Or give me a link :slight_smile:?


Regards!
```

---
## \#11 Posted by: Weberp7593 Posted at: 2016-11-24T16:40:55.645Z Reads: 64

```
 Problems problems problems 

 I hope someone of you can help me...
@rpn314 @JTAG  

<img src="/uploads/db1493/original/3X/4/d/4d1742ae9ca4b34a1cf22b333194c049127eff15.JPG" width="690" height="429">

 Today I tried to connect the controller and tried to program it.
 But it doesn't work :frowning2:
I measured some things  and saw that the power input of the programer was not 3.3 V   It was 1.5 V 
Also there was no high signal on reset pin while programming.

And I know that the ST link is fine because I programmed some other electronics with it 

That's what I get when I try to connect...
<img src="/uploads/db1493/original/3X/a/d/ad2af1f596be42594cab710893fa519575ee3dfa.JPG" width="690" height="422">

What can I do next?
And If i did not get it will someone buy the VESC from me? Otherwise it will lay around years :smiley:
Or maybe could check the problem? I would buy for it...
(I am from Germany)

My job is electronics and i have equipment.
So if u have an advice what to measure I can do it with oscilloscope e.g.


Best Regards!
```

---
## \#12 Posted by: rpn314 Posted at: 2016-11-24T16:47:22.158Z Reads: 60

```
I followed this: [VESC firmware/bootloader flashing windows stlink
](https://www.youtube.com/watch?v=H4sbDhRcaOQ) (credit to @jacobbloy)

Did you find the hex file? I think there's some with the bootloader (to allow to flash over USB in the future) and some without. At the bottom of that video, he has this link to hex files: http://vesc.net.au/flash/
Just double check after flashing if they have the current ramp bug, cause I think they might....and it'll fry your drv. If it does have it, just reflash with the USB to a known good ones (no need for hex now, since the bug isn't in the bootloader). That's pretty much what happened to me, but I fried my DRV before I found it cause I was stupid and didn't check after flashing.

You don't see a light on the VESC do you? The blue light should come on if I remember...
```

---
## \#13 Posted by: Weberp7593 Posted at: 2016-11-24T17:37:47.269Z Reads: 59

```
No i can't see any reaction when I connect to the St Link programmer.
That's what i did:
Connect:
<img src="/uploads/db1493/original/3X/6/8/684d184c50d58e5e6c9b27eefd91f36a78636a10.PNG" width="281" height="499">
Connect...
3,3v to pin 1 - MCU VDD
CLK to pin 9 - SWCLK
DIO to pin 7 - SWDIO
RST to pin 15 - NRST
GND to pin 3 - GND(2)

Then connect the VESC to the programer via Cables, then connect programmer via USB, then start ST Link Utilities, then press Connect -> Error

No flashing LED on VESC...
Only 1.5V on MCU VDD
No High Reset pin 
(STM need high at flash progress I think)

But now I see...
Do I connect to the wrong GND? There is a (2) behind and it sais:
Connect:
Connect to GND for noise reduction.?...
```

---
## \#14 Posted by: Blasto Posted at: 2016-11-24T17:41:43.061Z Reads: 54

```
[quote="Weberp7593, post:13, topic:10988"]
No i can't see any reaction when I connect to the St Link programmer.
[/quote]

you probably don't have 3.3v coming from the stlink

you can try to connect your vesc to a power supply
```

---
## \#15 Posted by: rpn314 Posted at: 2016-11-24T17:43:04.371Z Reads: 52

```
Yeah, you definitely need 3.3v coming from the ST-Link. Which one do you have exactly? I used one of those super cheap flash-drive looking ones
```

---
## \#16 Posted by: Weberp7593 Posted at: 2016-11-24T17:46:38.559Z Reads: 51

```
Jeah I will try, then I will see how much amps will flow :smiley:.
Maybe i have a Shorting (short-circuit) on the PCB.
But I don't know...

But then I see where it's getting hot and can find the problem :smile:

But don't know what to do else, because it's a ST Link In our company they program every day with it... so it should work
```

---
## \#17 Posted by: Weberp7593 Posted at: 2016-11-24T17:47:35.252Z Reads: 52

```
@rpn314
<img src="/uploads/db1493/original/3X/8/e/8ed702042e94e37461d4acc5b9a59ce4ca6db255.PNG" width="281" height="499">

The left one ;)
```

---
## \#18 Posted by: rpn314 Posted at: 2016-11-24T17:58:42.137Z Reads: 49

```
Try Pin 19 for vcc instead of pin 1. Page 12 [in the manual](http://www.st.com/content/ccc/resource/technical/document/user_manual/65/e0/44/72/9e/34/41/8d/DM00026748.pdf/files/DM00026748.pdf/jcr:content/translations/en.DM00026748.pdf) for that st-link unit shows that pin 19 is 3.3 on the target.
```

---
## \#19 Posted by: Weberp7593 Posted at: 2016-11-24T18:07:39.369Z Reads: 52

```
@rpn314 thanks i will try :slight_smile: and write tomorrow if it worked.
```

---
## \#20 Posted by: Weberp7593 Posted at: 2016-11-25T16:09:32.599Z Reads: 46

```
Ok thanks to all!
@rpn314 @Blasto @JohnnyMeduse @chinzw    
It is now working!
The problem was the connection of the programer.

<img src="/uploads/db1493/original/3X/9/6/96c83f3b3807970bae26469a347d7f2c02854ba0.JPG" width="666" height="500">

But I have one more question...
Is it normal that I got misfires with that little BL-Motor? 2000kv or sth.
I only had that one around and tested it with it.
And when I give throttle the motor stops at highspeed. Then won't move. First I must go back to zero then I can throttle up again.
What could that be? Or do you think it's only because this little motor is too fast?

<img src="/uploads/db1493/original/3X/5/2/521c05e3cef60261a9df2ff8afc15e6bf40f73de.JPG" width="666" height="500">

Regards!
```

---
## \#21 Posted by: chinzw Posted at: 2016-11-25T17:47:25.214Z Reads: 42

```
Well, it could be you're hitting the ERPM limit. Usually its set to 100k or 60k by default, i cant remember of the top of my head.
So if you're using a high kv motor, this could be the case.
```

---
