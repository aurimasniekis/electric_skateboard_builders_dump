# My VESC with AS5047 sensor setup

### Replies: 58 Views: 17039

## \#1 Posted by: JTAG Posted at: 2016-07-24T21:33:51.970Z Reads: 675

```
I found the connection method here:
http://vedder.se/2015/08/vesc-writing-custom-applications/

Connections being:
SCK -> HALL 1
MISO -> HALL 2
MOSI -> VCC
CS -> HALL 3

@MrEpiquad designed an awesome looking cap carrying the AS5047 developmentboard ( Mouser [985-AS5047P-TS_EK_AB](http://nl.mouser.com/ProductDetail/ams/AS5047P-TS_EK_AB/?qs=sGAEpiMZZMvc81WFyF5Eds5HfNOHCyjSQ7yI0JZudxs%3d) ):
<img src="/uploads/db1493/original/2X/b/bd90e9b9c691064d3cd39457ae0f9c08b9468a2b.jpg" width="666" height="500">
Magnet is mounted inside the pulley (shiny bit in the center).
<img src="/uploads/db1493/original/2X/5/52657812a6b0f0fe7bca41d2790846e201c77d81.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/2/29165c938104a9d1ec226bd267872003c9090f21.jpg" width="666" height="500">
PCB fits perfectly and has the perfect distance to the magnet.
<img src="/uploads/db1493/original/2X/9/9f5a04c72ae0180763831ac6aa7850e10fc25d28.jpg" width="666" height="500">
You get one magnet with the dev board.
<img src="/uploads/db1493/original/2X/5/531bef25f80458978afce47c25a9b23e13479414.jpg" width="666" height="500">
<img src="/uploads/db1493/original/2X/9/9f12417bc72a0ca8013a00feb9c423b06adc8f1b.jpg" width="666" height="500">
Everything connected :).
<img src="/uploads/db1493/original/2X/d/dc3e72f80d92c771aadf95f0292edfbc2d0b1f44.jpg" width="375" height="500">
And working!

Bottom screen is the SPI communication, I connected the oscilloscope to check if everything was working and how it looked. I discovered that upon the the first connection I swapped 2 wired, that error was easily found with the oscilloscope.

Testing encoder operation:
https://youtu.be/s3xv32vHJUk

Comparing sensored with AS5047 to sensorless (no studdering as with HALL sensors):
https://youtu.be/_gBN6H3Kumw

Configuring the AS5047 encoder on the VESC with BLDC-tool:
https://youtu.be/HtPQAW8FNcw
```

---
## \#2 Posted by: Pablo_702 Posted at: 2016-07-24T21:36:30.796Z Reads: 585

```
What does that pcb board exactly do?
```

---
## \#3 Posted by: JTAG Posted at: 2016-07-24T21:55:30.267Z Reads: 579

```
It is a development board for the AS5047 magnetic encoder chip. The chip tells the VESC the exact ( with 14bit accuracy ) rotor position, when the vesc knows this it has a far better way of applying the correct magnetic hield in the motor enabling perfect low speed (even at 0 speed ) torque control. I am now able to start very smoothly from standstill.

Yesterday we tested a setup with HALL sensors, while that was ALOT better than sensorles it still had some studdering at low RPM.
```

---
## \#4 Posted by: anon33082420 Posted at: 2016-07-24T22:05:07.793Z Reads: 552

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#5 Posted by: hexakopter Posted at: 2016-07-25T07:55:22.986Z Reads: 518

```
Great to see someone diving into the magnetic encoder support of the VESC. I have heard that the non linearity of the AS5047 leads to problems with higher RPMs. Can you confirm that? Comparing the hybrid mode (where the VESC uses the magnetic encoder for lower RPMs and then switch to sensorless mode for higher speeds) with the complete sensored mode should show that.

Isn't it bad to stick the magnet directly into the steel pulley? I think that results into a different magnetic field which maybe decline the accuracy of the encoder. 
Are you using a 6mm shaft (so a 6mm pulley) because the magnet used for the AS encoder have a 6mm diameter when I am not mistaken?
```

---
## \#6 Posted by: Ulfberht Posted at: 2016-07-25T08:16:48.739Z Reads: 493

```
@JTAG  I've been following your work on the forum here, Just when I think that you have reached maximum awesomeness, you amaze me once again. :thumbsup:
```

---
## \#7 Posted by: hexakopter Posted at: 2016-07-25T09:05:25.898Z Reads: 467

```
I think you don't get it. The support is already implemented by Benjamin Vedder. So you will see the code in his github.
@JTAG just build the supported hardware in his board.
```

---
## \#8 Posted by: Ulfberht Posted at: 2016-07-25T09:07:03.646Z Reads: 449

```
Oh yeah, I didn't check out the link before I posted! Got it. :wink:
```

---
## \#9 Posted by: JTAG Posted at: 2016-07-25T10:48:50.482Z Reads: 458

```
Yes it was benjammins work implementing the encoder. I was to lazy to design and build a PCB that fitted my exact needs so I just ordered the development boards since they were so cheap. It was surprisingly easy to make really, most of the effort went into designing the 3D model and printing it (and that was the contribution of @MrEpiquad ^^ ).

@hexakopter
Non linearity in what sense? I havent noticed anything bad, the board is now so much more fun starting from standstill. Low/zero speed is the only reason to use an encoder since at higher speed the observer does a much better job of determine the rotor flux angle.

Yes for sure the metal pully will bent/guide the magnetic field making it less ideal. I think this will result in a bit more noise on the encoder output, but hey we have 14 bits to spare xD. Yeah the magnet is 6mm and coincidentally the motor shaft is as well.
```

---
## \#10 Posted by: boards Posted at: 2016-08-30T14:56:53.607Z Reads: 404

```
Did you remove the filters on the sensor port or does it work fine without doing that?
```

---
## \#11 Posted by: JTAG Posted at: 2016-08-30T20:41:50.788Z Reads: 402

```
Yes, remove the filters like you would when using an encoder. I noticed that when using cables that have their wires right next to each other without separate shielding (like USB cables) a series resistor of 47R instead of 0R is needed to prevent cross talk (needed for the chip select and clock signal ).
```

---
## \#12 Posted by: elermetz Posted at: 2016-11-07T19:56:22.836Z Reads: 358

```
Hi JTAG,
I removed R11, R12, R13, C5, C6, C7 and replaced R8, R9, R10 by 0 Ohm resistors. Unfortunately it does not work yet, therefore the question: Is the wiring as indicated in this Image correct? Might this be a problem of Cross Talk?

<img src="/uploads/db1493/original/3X/6/b/6b5394f8fab5bc6ecb5ff12f0a2ad0e553a49ebe.png" width="690" height="460">
```

---
## \#13 Posted by: JTAG Posted at: 2016-11-07T20:41:24.006Z Reads: 339

```
[quote="elermetz, post:12, topic:6568"]
oss
[/quote]

Hmmm, everything looks OK. Did you change te sensor mode to AS5047 in the bldc tool? Cross talk is a serious problem indeed with these high speed SPI line. Also take special care in the alignment of the magnet (de datasheet / reference design manual tells the criteria).

Any easy way to verify the basic functionality is to measure on the AB (or I) output, a toggling signal should be visible when the magnet rotates.

You probably know this already, just to state the obvious: the type of magnet used has a specific north / south pole orientation, please make sure yours has something similar.

Good luck and keep us posted!
```

---
## \#14 Posted by: ykoval Posted at: 2016-11-22T00:20:17.393Z Reads: 308

```
Hi there, 
First off, let me say that i'm very impressed with the work that you've done here. So, after you've modified the VESC by essentially removing the filter and switching the resistors to around 0 ohms, what part of the code did you have to modify to allow the encoder to be recognized by the VESC? Any help will be much appreciated!

Thanks!
```

---
## \#15 Posted by: JTAG Posted at: 2016-11-22T00:55:29.289Z Reads: 303

```
Hi ykoval, 

Thanks!
No need to change any code. AS5047 is already implemented in the latest available firmware (implemented by vedder himself).
```

---
## \#16 Posted by: ykoval Posted at: 2016-11-22T04:14:24.477Z Reads: 296

```
Hi, 
So just to confirm, I would simply select the encoder from the BLDC tool without uploading any files onto the VESC? This will then allow me to detect the encoder without any firmware changes?

Thanks again!
```

---
## \#17 Posted by: JTAG Posted at: 2016-11-22T15:26:54.275Z Reads: 283

```
Under advanced you can select the encoder type. Choose AS5047. Then do the encoder detection like demonstrated in my videos.
```

---
## \#18 Posted by: erwincoumans Posted at: 2016-11-27T00:47:55.010Z Reads: 281

```
[quote="JTAG, post:1, topic:6568"]
@MrEpiquad designed an awesome looking cap carrying the AS5047 developmentboard ( Mouser 985-AS5047P-TS_EK_AB):
[/quote]

Nice work! Do you mind sharing the AS5047 CAP 3d printer file (STL)?
```

---
## \#19 Posted by: hexakopter Posted at: 2017-02-28T23:27:21.422Z Reads: 281

```
[quote="hexakopter, post:4, topic:18155"]
Are you still driving with Encoders?
[/quote]
Maybe the question is better preserved here. Did you used the Encoders on all the kilometer driven with the board? On your other thread it looks like you are driving a lot and I am interested what your long term opinion about encoders is. Do you had any problems? Would be glad to hear about that topic.
```

---
## \#20 Posted by: JTAG Posted at: 2017-03-01T00:11:10.831Z Reads: 280

```
Hi, and my apologies, I should have replied. Unfortunately no. the cable between de encoder and the VESC broke within about 100 kilometers or so, I never found the motivation to fix it. Although the response and feel of control is way way better I don't really _need_ them.
```

---
## \#21 Posted by: jhewitt123 Posted at: 2017-03-04T14:17:57.480Z Reads: 263

```
Nice work. I am using hoverboard hubmotors now with a vesc (see below) and want to add sensors that would be better than just the 3 existing hallsensors.
Would you recommend this kind of magnetic encoder over the optical encoder method for low speed and position control, perhaps even for balancing.
I would like to know how the original hoveboard does such nice control from the gyro (acceleromter) board it uses, if you have any idea.
thanks, John@hewitt123.com
http://neurowritings.blogspot.com/2017/03/hoverboard-hack-for-electric-skateboard.html
```

---
## \#22 Posted by: jgeating Posted at: 2017-04-19T00:36:01.847Z Reads: 260

```
Anyone know what firmware versions will work for this? Since the bldc site went down, I'm having trouble finding firmware for 2.17 and 2.18. Anyone have these available for download? Thanks! I'm also up for hosting atchives of BLDC tool on my google drive if anyone has a repository. 

Thanks!
```

---
## \#23 Posted by: ykoval Posted at: 2017-05-08T21:41:20.119Z Reads: 253

```
Hi @JTAG, 
I have one more question for you and i'm hoping you could provide me some insight, or perhaps a solution. So I went ahead and added the same encoder that you've mentioned, the AS5047, removed the Capacitors and replaced the needed resistors with 10Ω ones on the VESC. But when I go into the settings, change the sensor type to the encoder option and do the detection I get a weird noise from the motor when I attempt to run them. The detection results seem to come in just fine and it gives some sort of value for the encoder, which I assume that the encoder position was successfully registered, but when I attempt to spin up the motors using the remote I get a noise that sounds like something is slipping. Would you have any insight to why this is? I can upload a video or photos of all the procedures that I've done if you're willing to look into this.

Thanks again for motivating me into attempting this!!
```

---
## \#24 Posted by: jgeating Posted at: 2017-05-08T22:17:42.629Z Reads: 236

```
I've personally had tons of issues with the encoder detection. Just because it spits out results doesn't mean they're correct. I often got a ratio of 500, which means the detection was unsuccessful. For my motor, the correct ratio was 7.
```

---
## \#25 Posted by: ykoval Posted at: 2017-05-08T22:17:59.833Z Reads: 232

```
@JTAG
Here is a link to the video of me configuring the encoder settings and attempting to run the setup with the encoder: https://drive.google.com/open?id=0B-CnAwEu9O1ndW55QjVkcTM0R0U
```

---
## \#26 Posted by: JTAG Posted at: 2017-05-08T22:43:49.403Z Reads: 227

```
Hi,

Your received / detected ratio looks quite low. Mine was 7, but on the other hand your motor is also different so it might be correct.

Somewhere in BLDC tool you can read/visualise the encoder output. Can you try if the encoder output graph still shows encoder data when you select sensorless in FOC? If so check the noise on the encoder signal (when motor is actuated), it sounds like the motor actuation / current is corrupting your encoder signal. If not obvious that that might be the problem please share a picture.

Good Luck!
```

---
## \#27 Posted by: ykoval Posted at: 2017-05-08T23:05:23.454Z Reads: 240

```
That did the trick! It looks like there was too much noise in the line and by simply readjusting the connector cable I was able to get a clean signal! Thanks again! I'll try to insulate the connectors so that they don't cause such issues down the road. 

Noisy Signal: 
<img src="/uploads/db1493/original/3X/f/a/fa5424d5a4ef028824f4f55f0d7b56fb6d5ec532.JPG" width="666" height="500">
Slightly Cleaned up signal
<img src="/uploads/db1493/original/3X/4/e/4e21bf91eff60238d1c76354d9c116f551621d7a.JPG" width="666" height="500">
Connector: 
<img src="/uploads/db1493/original/3X/4/0/401df38793b61e8dac846aac6c17bf58ce90ca21.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/f/c/fc72a6153684af1b44e9379a24248397e59bcee7.JPG" width="666" height="500">
```

---
## \#28 Posted by: JTAG Posted at: 2017-05-08T23:34:14.786Z Reads: 230

```
Awesome!

I ended up using shielded cable, that got me to a 99.9% clean encoder signal, more then enough for a nice riding experience :grin:.
```

---
## \#29 Posted by: Pantologist Posted at: 2017-05-09T00:00:48.632Z Reads: 228

```
So this is basically what Boosted uses I guess? 

Are there any benefits to having the sensor monitoring the shaft position compared to being inside the motor instead?
```

---
## \#30 Posted by: JTAG Posted at: 2017-05-09T00:07:14.095Z Reads: 227

```
Hall sensors in the motor have multiple 100's times lower angular resolution then the AS5047, therefore the low RPM flux angle has a way higher accuracy resulting in a way way smoother start from standstill.
```

---
## \#31 Posted by: yhao1 Posted at: 2017-06-06T02:11:26.713Z Reads: 232

```
Hello, Danny

@JTAG 

Thank you very much for positng this great work here. I'm actually also working on a VESC encoder position control project. Can I ask you some questions about it?

Where can I purchase the motor in your video? Can you provide a link to it? My motor does not work with VESC encoder detection. It keeps giving me 0 ratio and the detection only stops when the detection is timeout. The BLDC-tool does not response after the detection. I have to restart the VESC and reconnect to the BLDC-tool. So I'm thinking use the same motor as yours. 

Which firmware version did you use for VESC? Did you use version 2.18?

I watched the Benjamin's video about position control. He used version 2.10, and also it is a bin file. So I'm really confused about which software to use right now. 

Thanks very much

Michael

<img src="/uploads/db1493/original/3X/1/2/121453ed90cd12382c2928652a7df443b08fdfb0.jpg" width="637" height="425">
```

---
## \#32 Posted by: yhao1 Posted at: 2017-06-06T02:39:42.100Z Reads: 221

```
Hello ykoval,

@ykoval

Thanks very much for posting your video here. I actually have similiar problem as yours. My motor does not even work with the encoder detection. I'm using an ABI encoder which is 1000 pulses per revolution. The BLDC-tool can detect the ABI encoder and show the degree on the BLDC-tool. 

Did you use Maytech 6374 motor in that video? Have you solve your problem now?

Best

Michael
```

---
## \#33 Posted by: ykoval Posted at: 2017-06-06T10:05:12.048Z Reads: 212

```
Yes, I was able to successfully solve the encoder issue. As JTAG pointed out, I was getting too much noise in the signal which the BLDC tool didn't like and which is why I wasn't able to detect the reported encoder position properly. Just make sure that the BLDC tool is reporting a single clean line when it shows the encoder position. Those regular six pin connectors don't seem to work well, which is why I replaced them with shielded wires. If your VESC can detect the motor parameters without the encoder, it should detect it with the encoder. That is of course if the encoder is wired correctly.
```

---
## \#34 Posted by: yhao1 Posted at: 2017-06-06T15:56:11.663Z Reads: 211

```
@ykoval
Yes. I tried AS5048A encoder today and got a lot of noise. If you don't mind, could you please post a picture of your wiring, connections and other stuffs so I can know how to fix my hardware?

Best

Michael
```

---
## \#35 Posted by: yhao1 Posted at: 2017-06-07T08:36:36.011Z Reads: 213

```
@hexakopter

Hello,

How you solve the spi noise problem? Did you just use normal wires? 

Thanks very much

MIchael
```

---
## \#36 Posted by: ykoval Posted at: 2017-06-08T03:49:51.187Z Reads: 216

```
I implemented twisted pair aka an ethernet cable which provided a ground for each signal wire. <img src="/uploads/db1493/original/3X/0/c/0cd3217f1ff313eb8af516f2ad474f2866e07249.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/9/9/995dfd771eb32d352e3fcc2f2480743121682403.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/1/e1265656e7a41e7ebaf0f29f6b4a5c2d8aa82837.JPG" width="375" height="500">
```

---
## \#37 Posted by: ykoval Posted at: 2017-06-08T04:00:47.996Z Reads: 217

```
As you can see, my original motor had hall sensors which I snipped. <img src="/uploads/db1493/original/3X/2/3/233fcfa9cfbe6efc40a1c51bb59beb3847c21221.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/f/c/fc401a420fa20e19345bfd49381dd38e6445d0d2.png" width="503" height="500">
<img src="/uploads/db1493/original/3X/1/3/136e1213a48035e555b779c507f9ddf1c9f9d4d2.JPG" width="666" height="500">
The original encoder wires were replaced with twisted pair ethernet.
<img src="/uploads/db1493/original/3X/3/4/347cf96b93a6a3f4beef449a55057d808cd85565.png" width="665" height="500">
Encoder cap reference to the actual wheel.
```

---
## \#38 Posted by: Luuke Posted at: 2017-10-26T17:55:54.692Z Reads: 199

```
That Senor sounds super cool!
Can you tell me, why you are using AS5047P-TS?
There are other options as well AS5047P-ATSM, AS5047P-ATST, AS5047D-TS, AS5047D-ATSM.
```

---
## \#39 Posted by: Okami Posted at: 2017-10-26T20:26:00.043Z Reads: 200

```
Nice wheels btw.. are these onda wheels?.. Also the cover, which also holds encoder looks really nice.. Do you pour epoxy into a mold to make these?
```

---
## \#40 Posted by: ykoval Posted at: 2017-10-26T20:43:31.801Z Reads: 200

```
The encoder covers were 3D printed and the motor mounts were CNC machined and yes those are Onda wheels
```

---
## \#41 Posted by: SORRENTINO Posted at: 2017-11-03T18:47:41.045Z Reads: 184

```
@JTAG  Does anyone know if this encoder can work with the focbox without any modification to focbox? Would I just have to use the latest firmware from Vedder?
```

---
## \#42 Posted by: JTAG Posted at: 2017-11-03T23:19:50.158Z Reads: 185

```
Good question. Since the original 4.12 VESC needed changes and the FocBox is based on that design I would assume it needs some modifications as well. But I am no expert on the foxbox so I don't know for sure :( .
```

---
## \#43 Posted by: SORRENTINO Posted at: 2017-11-04T01:39:06.207Z Reads: 181

```
Ok then it's a good bet to say it probably needs some  modification.
```

---
## \#44 Posted by: Raess Posted at: 2018-03-31T12:42:37.635Z Reads: 163

```
So lets get this thread active again. :) Trying to setup an AS5048A.

I modified the VESC (flier model) removing R11-13. Solder jumper on R8-10 and removing C5-C7.

The encoder works and I can run the encoder detection, I receive the values: ofs: 264.10 Rat: 7

Problem is when I try to run the motor it makes very funny noises. And I don’t know where to start the troubleshooting?

For encoder count on advance tab in BLDC tool. what should I set this value to? I put 16384.

Any suggestions?
```

---
## \#45 Posted by: Raess Posted at: 2018-03-31T12:47:53.094Z Reads: 165

```
Some videos:
https://youtu.be/70IOnsneilw 
https://youtu.be/nq8IzenI9Lw
```

---
## \#46 Posted by: barajabali Posted at: 2018-07-01T22:49:59.394Z Reads: 150

```
Does anyone have the developmental board on hand? Looks like it’ll be a while on mouser, does this one work as well? https://www.digikey.com/product-detail/en/ams/AS5047P-TS_EK_AB/AS5047P-TS_EK_AB-ND/5452344 


How do I get a hold of it now?

@JTAG thanks
```

---
## \#47 Posted by: Pimousse Posted at: 2018-07-02T08:07:19.417Z Reads: 139

```
I have 2 of them (the one you linked), but I didn't try yet.
```

---
## \#48 Posted by: Charles_Chan Posted at: 2018-07-14T08:54:29.913Z Reads: 132

```
@JTAG  Do you know how can i get 50rpm on my VESC with AS5407? Thanks
```

---
## \#49 Posted by: spork Posted at: 2018-11-22T03:03:47.184Z Reads: 106

```
I just added hall sensors internally and have them working.  This is the first I've heard of removing filters.  Is this necessary when running in hybrid sensor mode (in which case I believe the sensors are ignored beyond the threshold speed)?  Can you tell me why we would want to remove the filters, and where I can learn more about this?

Thanks!
```

---
## \#50 Posted by: JTAG Posted at: 2018-11-22T09:18:14.625Z Reads: 101

```
If you use HALL sensors you should not remove the filters and not configure the AS5047 section but the HALL sensor section. 

Both rotor sensing methods use the same inputs on the VESC, the sensor signal is different and therefore you should configure them different.

Good luck!
```

---
## \#51 Posted by: spork Posted at: 2018-11-22T10:04:40.479Z Reads: 100

```
Thanks very much.  I just noticed that I misread one of your comments further up.  You mentioned removing the filters as you would when using an encoder.  For some reason I read "encoder" as hall sensors.  D'OH!

So I think I'm good.  I've got both motors modified, and both VESC's properly configured and working with the hall sensors.  It sounded like maybe there was something more I should do that might further improve the performance.
```

---
## \#52 Posted by: JTAG Posted at: 2018-11-22T10:06:01.751Z Reads: 96

```
If it works, don't touch it :nerd_face:. Just kidding, good luck!
```

---
## \#53 Posted by: spork Posted at: 2018-11-22T10:27:05.446Z Reads: 95

```
I go with the old saying "if it ain't broke, fix it until it is" :slight_smile:
```

---
## \#54 Posted by: vlabs Posted at: 2019-07-11T22:42:24.294Z Reads: 60

```
@JTAG or @ykoval I appreciate you two sharing your journey with the AS5047. 

I'm trying to achieve low speed smooth rotation by integrating the encoder with my FlipSky FSESC6.6 dual right now and not able to connect the dots. Hope someone here can help. I wired the AS5047P-TS_EK_AB dev board to the VESC using SPI, using the 3V3 power supply, and confirmed that I'm getting reliable sensor input when rotating the motors.

I can't for the life of me figure out what my settings in the VESC Tool need to be in order to achieve PID speed control using the encoder. I've read and re-read this topic, reviewed others on Esk8. Several people post about their hang-ups from the sensor to the VESC, but few people have mentioned any issues happening after they get a reliable signal from the encoder. Maybe I'm missing something obvious?

Clicking the FWD button on the Local VESC (Motor Settings > General > General > Refresh > FWD) rotates the motor about 1/4 rotation, then jitters violently as can be seen below.
![image|690x364](upload://tjQo00JIei9pc6L86qAR1Yd0OvY.png) 

Watching the video ykoval posted of his problem, he ran into a similar issue of not getting correct commutation. His symptom was a locked rotor, less jittery than mine. JTAGs suggestion of running the motor in sensorless mode and watching the encoder output didn't seem to help either. Using the FWD button again, the motors spun up as expected and the encoder output below looks as would be expected. The post suggested that noise would be visible but I don't see any noise - it's smooth like the image above.

I've tried sensorless, and sensored (PID Speed control, current control, DC). I can't use the keyboard arrows to spin up the motors without a bunch of jitter either.

Am I missing something obvious? How did y'all who have been successful with the AS5047 encoder get smooth control? Would love to understand the settings involved in VESC Tool to get my motors to work as expected and share that with the community here for anyone else trying to make this work. Thanks!
```

---
## \#55 Posted by: jgeating Posted at: 2019-07-12T01:06:28.583Z Reads: 57

```
If it won't spin smoothly with keyboard input (duty cycle and current control modes), I doubt your problem has anything to do with PID settings. I've used the AS5047 with FSESC 6.6 single several times now successfully in both position and speed control modes, and before tuning the PID gains, it always rotates smoothly with the keyboard in duty cycle or current control modes. If it doesn't do that correctly, then I know something else is wrong and I run the motor setup again. I've had the luxury of spare motors, controllers, and encoders, and usually switching one of them fixes the problem if it gets that far. Usually just running commutation again fixes the problem though. 

One jitter problem I've had similar to what you're describing was related to sensor wire harness EMI. I was using unshielded jumper wires, and simple moving the wires around made the encoder signal go from tons of noise like you're showing, to perfectly stable. Motors were uncontrollable and the temporary fix was to empirically tape one of the wires away from the rest. It worked rather well, but shielded cable might help. I'd move the sensor wires in question around and see if it affects the signal. It was the same result with multiple harnesses, so I don't think it was a loose wire problem. 

Can you confirm that when you say "I'm getting reliable sensor input", the encoder setup is successful, and as you rotate the motor by hand it shows smooth, 14 bit data that doesn't jump around? Also, what motor are you using? I had some issues a while ago trying to drive small motors with the VESC 4.8, because the current sensing shunts don't do well with small currents.
```

---
## \#56 Posted by: vlabs Posted at: 2019-07-15T20:07:30.070Z Reads: 47

```
Thanks for the reply. I'm using a pair of FlipSky 6368 / 140KV outrunners. The sensor data looked smooth and consistent for the entire rotation.

I believe I found the solution. Once I had setup the encoder and ran the calibration, the part I was missing was to rerun the FOC motor setup with sufficient d and I values to commutate the motor. I thought I only had to run the motor setup first, then the encoder setup, but it seemed to work better for me the other way around.

Thanks for the help @jgeating! Hope this helps the next person stuck in troubleshooting mode.
```

---
## \#57 Posted by: jgeating Posted at: 2019-07-16T02:58:55.598Z Reads: 40

```
Hmm. I don't think I've ever run encoder setup prior to motor detection, with similar sized 6374/80-150kV motors. But whatever works - I'm glad the problem is fixed.
```

---
## \#58 Posted by: eve Posted at: 2019-08-15T23:29:48.491Z Reads: 28

```
Good Day, Did you make a holder for the magnet also. Do you have the stp files by chance. I would like to try it out.
```

---
