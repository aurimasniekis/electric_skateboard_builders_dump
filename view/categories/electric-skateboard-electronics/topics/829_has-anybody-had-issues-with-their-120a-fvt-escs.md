# Has anybody had issues with their 120A FVT ESC&rsquo;s

### Replies: 20 Views: 5247

## \#1 Posted by: Dwswill Posted at: 2015-12-28T23:05:26.381Z Reads: 271

```
I bought a 120A FVT ESC off of Amazon for my ESK8 its a fairly cheap option and works very well for the most part but I have occasional issues when I will lose control of the motor and it will run at full speed ( believe this is a loss of signal to the ESC/Receiver) or on other occasions the ESC will give some sort of error and will give a few half speed bursts and then run at half speed for about 20 sec then shut off. I can't seem to figure out what is causing this and the ESC came with almost no instructions. One thing I have noticed it does seem to happen more with my 5500mah 5s pack than my 4500mah 5s pack. I am using the ESC's BEC don't know if that could be and issue.  Has anybody experienced similar problems or know how to trouble shoot them?
```

---
## \#2 Posted by: Kaly Posted at: 2015-12-29T12:19:55.660Z Reads: 261

```
Hi there

What are you using as your remote ? 
I was using a wiiceiver and had the same issue. 
IMO get  your self a 2.4ghz  remote. 

Here are some good ones

http://www.hobbyking.com/hobbyking/store/__31671__HobbyKing_174_8482_HK_GT2B_3CH_2_4GHz_Transmitter_and_Receiver_w_Rechargable_Li_ion_Battery.html

product/torqueboards-2-4ghz-mini-remote-controller/
```

---
## \#3 Posted by: Dwswill Posted at: 2015-12-29T15:41:30.205Z Reads: 257

```
@Kaly  I am using a the FlySky FS-GT2B 2.4GHz 3-Channel Transmitter I got it off amazon about the same as the HK one. I really think it has something to do with the ESC.
```

---
## \#4 Posted by: Kaly Posted at: 2015-12-30T18:46:28.901Z Reads: 248

```
It could be the ESC but first try to pair the transmitter and receiver again.
```

---
## \#5 Posted by: Dwswill Posted at: 2015-12-30T19:06:12.492Z Reads: 243

```
@Kaly I bought a Programming card for the ESC maybe changing some of the setting will help. Thanks for the suggestion of the Transmitter and receiver I will try that they did come with pretty decent instructions.
```

---
## \#6 Posted by: Dwswill Posted at: 2015-12-30T19:12:31.882Z Reads: 235

```
I have also thought about getting the VESC but I'm not particular good with computer and hearing people on here talk about the programing issues they have is somewhat intimidating.
```

---
## \#7 Posted by: Kaly Posted at: 2015-12-30T19:30:17.167Z Reads: 224

```
For my next built I'm considering the VESC but still not 100% onboard I have had good result with the torqueboard 12s ESC ( after installing fan ). 

The VESC it's a little more challenging to implement and more time on the computer too :-)
```

---
## \#8 Posted by: barajabali Posted at: 2016-01-06T04:47:08.970Z Reads: 217

```
That happened to me .Ive been using the FVT 120 amp on all my builds. one time my signal wires were pretty worn down so i chopped them and soldered some new ones on and it worked fine!
```

---
## \#9 Posted by: paragon Posted at: 2016-01-06T05:04:40.583Z Reads: 210

```
Did you set up the failsafe?
I run a Tacon 160 on 6s no problem with the FS-GT2B and FVT120a esc.
```

---
## \#10 Posted by: Dwswill Posted at: 2016-01-16T07:35:34.594Z Reads: 202

```
@paragon @barajabali @Kaly So I took Kaly's advice and repaired the xmtr and receiver also found that the receiver's antenna wire was loose and not making a good connection so I re-soulder it. I believe the error i was seeing where the the ESC gave me a few half speed burst and then runs at half speed was the ESC over temp. I just a few days ago recieved a programing card for the ESC tried runs with the motor timing set at the very lowest setting and the problem became more pronounced. So obviously I changed it to the highest setting and in the couple of runs I have got in the problem has seemed to go away. We will see I just ordered a 15000mah 6s battery from china. Will update when I get some really long runs with the new battery.
```

---
## \#11 Posted by: paragon Posted at: 2016-01-18T02:59:32.067Z Reads: 195

```
Are you sure you soldered it correctly? 2.4ghz receives usually have antennas made from coaxial cable.
```

---
## \#12 Posted by: Dwswill Posted at: 2016-01-18T05:36:35.505Z Reads: 191

```
@paragon nope but i will check I am out of town for work right now but i only remember seeing one connection but the wire was a little different.
```

---
## \#13 Posted by: Dwswill Posted at: 2016-02-16T20:00:12.944Z Reads: 183

```
@paragon yep I solder it wrong went back in and striped the coax properly and solder both the center conductor and shield where they were supposed to be soldered to. Since it has work great and I am pretty sure the bursts and then full speed run were an over temp thing. I have since also installed a smaller motor gear and increased the ESC timing. I did how ever catch the 15ah battery my GF got me for Christmas on fire no bueno but it think it was just a cheap battery.
```

---
## \#14 Posted by: bigben Posted at: 2016-04-27T06:13:06.256Z Reads: 178

```
Can I ask you what program card you were using? I'm guessing they're not universal?
```

---
## \#15 Posted by: GrahamZhu Posted at: 2016-06-28T16:19:32.685Z Reads: 163

```
Just bought a FVT 120A ESC and the program card. I changed some setting on the computer program but the motor acts the same as default setting. Even "reading settings" shows the same as the default. However, I was able to update the firmware. Anyone knows what was the problem and how to solve it?

<img src="/uploads/db1493/original/2X/6/6db9b67af2d468ac868f0f555d05fef9303368f6.png" width="580" height="500">
```

---
## \#16 Posted by: Mobutusan Posted at: 2016-06-28T17:33:19.296Z Reads: 153

```
Maybe @torqueboards can shed some light on this.
```

---
## \#17 Posted by: GrahamZhu Posted at: 2016-06-29T06:37:13.279Z Reads: 153

```
Need help guys. Does the usb link need driver? Does it work on windows 10? :sob:
```

---
## \#18 Posted by: dude Posted at: 2016-07-14T14:59:13.105Z Reads: 149

```
A bit late … but just stumbled over this thread.
Using it under Win10. Works.
Only downloaded and installed the USB Link software and it worked.

[Brushless Software USB Link V 1.00](https://drive.google.com/file/d/0B4mQ2EcVWaBzLWpXRUUxckdLVmM/view)
(Link source: Product page of BangGood)
```

---
## \#19 Posted by: PEX Posted at: 2017-08-16T22:44:38.003Z Reads: 60

```
I use the custom firmware provided by FVT and I have a very nive brake now

Here is the link, my settings and the firmware I used:
http://szfvt.com/en/download-6.html

<img src="/uploads/db1493/original/3X/1/6/167d33081ff22b970e2faa9b8f2f5b0a51b7494a.png" width="597" height="500">

I also made a video of my testing if you want to check it:
https://www.youtube.com/watch?v=Pynz5z984Og
```

---
## \#20 Posted by: kaspars Posted at: 2017-08-26T18:58:28.905Z Reads: 50

```
Thanks for sharing this!

I can also confirm this fixes the random acceleration issue after releasing the brakes!

http://www.electric-skateboard.builders/t/maytech-12s-esc-new-firmware-to-fix-the-brakes/13545/78
```

---
