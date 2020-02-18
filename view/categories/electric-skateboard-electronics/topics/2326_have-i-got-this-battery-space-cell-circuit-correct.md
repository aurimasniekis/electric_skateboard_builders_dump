# Have I got this battery (space cell) circuit correct?

### Replies: 36 Views: 4317

## \#1 Posted by: michaelcpg Posted at: 2016-04-13T06:56:39.972Z Reads: 202

```
Hey guys,

Been trying to work out how to wire up the space cell I bought from @onloop that I received in parts due to shipping regulations. I've drawn up a circuit diagram of everything which I've made after looking at photos of other people's space cells that've been opened up (note I've ignored the balance leads for this). Would really appreciate if someone with a bit more experience with this sort of thing could look over the diagram to see if I've made any obvious mistakes etc? Cheers

<img src="/uploads/db1493/original/2X/e/e171476507285870fbd2e077c7751bd1a216f5ee.jpg" width="690" height="453">

I've included photos of the BMS for reference.

<img src="/uploads/db1493/original/2X/e/e1d8264cc67442267bdc98e687c3a80e30091b64.jpg" width="690" height="390">
<img src="/uploads/db1493/original/2X/6/684e73177e90f7f00002d7062725922eb9530dea.jpg" width="690" height="390">

Cheers
```

---
## \#2 Posted by: onloop Posted at: 2016-04-13T09:44:25.017Z Reads: 182

```

I'm pretty sure that's not correct, I'm getting the run around from my factory! so very sorry for the lack of instructions!.... I'll disassemble a battery here and work it out. I've got to build one too for @Sporter I have also got my spot welder now!
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-04-13T10:10:02.759Z Reads: 179

```
No worries Jason, sounds like it's pretty frustrating for everyone involved. And thanks I appreciate that, even just a few good photos of the battery opened up would probably be more than enough to allow me to figure out exactly how everything goes together. I've been reading through a bunch of sites with information about BMS's but I haven't been able to come across any with the same terminal setup as this one which I found quite interesting, I've certainly learnt a fair bit though.

http://www.electric-skateboard.builders/t/space-cell-opened-up/510/38

This thread of @cmatson's has certainly helped me to figure out a fair bit of how everything goes together but the new version of the BMS has made things a bit more interesting ;P To be honest I kind of felt that the diagram isn't quite correct, it's mainly the position of the power switch and the difference in p- and p-1 terminals that I'm mostly unsure about but this was the best I could get based on some of @thomwithah's photos that he posted of his space cell with the new BMS.

Anyway, look forward to getting an update from you, can't wait to finally get this thing up an running :D
```

---
## \#4 Posted by: Sporter Posted at: 2016-04-13T10:15:39.175Z Reads: 159

```
Good to hear you have finally received the spot welder mate!!!! Looking forward to getting the space cell battery.
```

---
## \#5 Posted by: chaka Posted at: 2016-04-13T12:47:00.328Z Reads: 155

```
Your diagram looks good as long as that LCD screed can handle 42 volts. The most important part of a battery build with bms is being sure the balance wires are in the correct order.  Are you having to assemble the cells and spot weld them too?
```

---
## \#6 Posted by: michaelcpg Posted at: 2016-04-13T13:25:52.270Z Reads: 162

```
Thanks @chaka. So the power switch is in the right place? I was basically just going off what I could see from someone else's photo but tbh I don't really understand why it would go in that part of the circuit....

Do you also know what the difference would be between the p- and p-1 terminals? Again, I just did this part going off of photos of someone else's space cell but it was a little difficult to see in the photo exactly what was going where.

The LCD is just the standard one that comes with the space cell so I assume that it should be able to handle the voltage fine? Model looks to be a Jiashen JS-C30 V2.

<img src="/uploads/db1493/original/2X/f/ffa2bfb8ab493ef52bc56b72c1f043bf5812ed4c.jpg" width="689" height="390">

The cells were half spot welded but I didn't have access to a spot welder so I carefully had to solder them.

<img src="/uploads/db1493/original/2X/3/3fcd115e36f7f30ea3dc28243d58caa7a10bc394.jpg" width="690" height="390">

You can see the basic idea of how the cells are wired above. The black balance lead at the end negative terminal connects to the B0/B- terminal while the white balance lead connected to the first positive cell connection is connected to the B10 terminal on the BMS. Do I look to be on the right track here?
```

---
## \#7 Posted by: chaka Posted at: 2016-04-13T14:14:42.833Z Reads: 144

```
Based on the photo I can tell you P1 looks like it is used for discharging the pack. P seems to bypass the fets for charging. The biggest issue I see is the lack of any shunting or heat sinks on that circuit board. This tells me it is not designed for the loads we typically use. It may end up cutting power when accelerating or overheating on hills. If it gives you problems you can piggyback an order for a proper BMS on my next order to Bestech.

As far as cell balancing it looks like you are on the right track, you seem to have figured out that the cells are labeled incorrectly. Battery negative should be cell #1 and battery positive cell #10.
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-04-13T14:29:07.412Z Reads: 141

```
i'm eagerly following this thread because i have one on my bench right now and i can't figure out this BMS either. Was hoping to have a wiring diagram sent to me by @onloop but if its posted here it would help everyone else as well.
```

---
## \#9 Posted by: longhairedboy Posted at: 2016-04-13T14:34:54.154Z Reads: 141

```
oh hang on... i think that power switch placement in line with the temp sensor might actually be correct... i'm going to have to try that when i get home. It sort of makes sense because one wire is significantly longer than the other and is interrupted by a coupling, and the sensor can also switch off the BMS so ...

Still want confirmation via official wiring diagram though. 

But i will settle for somebody tearing their existing pack apart if they have a newer one using this BMS.
```

---
## \#10 Posted by: michaelcpg Posted at: 2016-04-14T00:56:06.837Z Reads: 138

```
Thanks for all the input guys. I know it'd probably be a better idea to wait till Jason's had a chance to open a space cell for confirmation... but based on your guys feedback I'm tempted to just have a go at putting everything together now to see if it works...
@onloop sorry I don't mean to pester, but any idea when you expect you'll have time to get some photos of an opened battery? :stuck_out_tongue:

Also thanks for the offer @chaka, hopefully it won't be necessary but I guess we'll see how things go :)
```

---
## \#11 Posted by: michaelcpg Posted at: 2016-04-14T12:13:29.784Z Reads: 137

```
Ok so I decided to go ahead and put the battery together. Pretty sure I've got it all working :)

<img src="/uploads/db1493/original/2X/3/309385cbb3307113cdfd44266b46ae71306da010.jpg" width="689" height="390">
<img src="/uploads/db1493/original/2X/9/978bc414355166b30a8c7542e248494ff67e975f.jpg" width="689" height="390">
<img src="/uploads/db1493/original/2X/3/32bb5564b0095bd6830184c87afadcd8e8521350.jpg" width="689" height="390">

A few things I've noticed though... 
1. Connecting a multi-meter to the XT60 connector with the battery turned on shows 36.4V but it also shows 1.5V when turned off, is this normal?
2. The LCD doesn't seem to turn on when a VESC is connected. Is this normal?
3. When I connect the battery to a VESC and 6374 Enertion Motor, plug the VESC into my Windows 10 computer via USB and run the BLDC tool, then click connect, the BLDC tool shows the VESC as being connected for a couple seconds then says "NO FIRMWARE READ RESPONSE" and disconnects. Any idea what would be causing this issue? 

I've tried version 2.16 and 2.13 of the BLDC tool and going into Device Manager, the only COMP port available seems to be COM1. I'm connecting the VESC directly to my computer's motherboard using a very short mini USB cable (One that came with an external HDD).

Also, @chaka, do your VESC's have LEDs? I've noticed in other threads that people talk about their VESC having LEDs where as my one seems to have none.
```

---
## \#12 Posted by: chaka Posted at: 2016-04-14T13:24:58.005Z Reads: 131

```
Either the VESC is not getting power or it has been shorted out somehow. The vesc should should blink red 3 times then go solid green and blue. It is also possible that it has been wiped clean if you let it sit with an undervoltage source for too long. It is not normal to have 1.5v with the unit turned off. Sometimes it will take time for all the voltage to bleed off when you switch an inrush controller off but it should go to zero.

Does the VESC still light up with at least the blue LED? If it does not and you are sure it is getting proper voltage then it may have developed a short. 

Also check your fuse, if you reversed polarization on your source wires to the vesc then the fuse will have likely blown. 

Let me know what you find and I will help you out anyway I can.
```

---
## \#13 Posted by: michaelcpg Posted at: 2016-04-14T20:38:18.616Z Reads: 131

```
There weren't any lights at all from what I could see. I've found that the battery outputs 1.5V even when the wire connecting the BMS to the negative terminal on the battery is cut which means the voltage is coming through the balance leads (disconnecting the balance leads removes any voltage). I double checked this morning and the xt60 cable definitely has the correct polarity as you can see below.

<img src="/uploads/db1493/original/2X/e/e9af7354347f53bb1427b7dceade7ba015fbb2b9.jpg" width="282" height="500">

This is the first time I've connected the VESC and before this it's just been sitting in its shipping packaging in my cupboard. Also something to note is that when I connect the motor to the vesc and the vesc to the battery and then turn the battery on, the motor moves just slightly for a split second so something is obviously happening. Will be interested to hear your thoughts.
```

---
## \#14 Posted by: chaka Posted at: 2016-04-15T02:08:09.984Z Reads: 127

```
I am betting the VESC got wiped clean from the sustained low voltage. Something similar happened with another customer, the VESC most likelyneeds to be reflashed. This is something that needs to be done with an st-link, you will need to send it back to me to have this done or do it yourself. If you can get Ubuntu installed on a computer and an st-link I can walk you through it.
```

---
## \#15 Posted by: michaelcpg Posted at: 2016-04-15T02:17:58.694Z Reads: 127

```
Considering we're based on opposite sides of the world I'd prefer to make an attempt at flashing it myself first. I don't have ubuntu at the moment but I can setup a VM. I'm not sure what an st-link is though. How much are they usually? Are they relatively common?
Otherwise, any idea how much I'd be looking at to return the VESC and how long it could take?

Edit: Is this what I'm after?
https://nicegear.co.nz/electronics-gear/stlink-stm8stm32-v2-programmer-emulator/
```

---
## \#16 Posted by: chaka Posted at: 2016-04-15T02:30:40.465Z Reads: 126

```
I use a discovery board: http://www.ebay.com/itm/like/262356443960?lpid=82&chn=ps&ul_noapp=true

A little pricy compared to these: http://www.ebay.com/itm/DZ399-St-link-v2-stm8-stm32-artificial-device-programmer-stlink-1pcs-/151319065969?hash=item233b51b571:g:E44AAOxyDo1TjpNo

If you get on I can help you figure out the pin out wiring order and the terminal commands.

You are definitely biting off a pretty big piece to chew for your first build. Don't stress, I'll be here for you.
```

---
## \#17 Posted by: michaelcpg Posted at: 2016-04-15T02:37:08.011Z Reads: 123

```
Thanks for the links. Would there be any advantage buying the more expensive of the two options?
Not sure if you saw the edit to my previous post when you replied but I emailed the guys at nicegear.co.nz and they have one of these left in stock:

https://beta.nicegear.co.nz/electronics-gear/stlink-v2-programmer/

Would this do the trick? Would prefer to buy from a NZ company just due to the fact that shipping should be a few days rather than a few weeks.
```

---
## \#18 Posted by: chaka Posted at: 2016-04-15T02:48:55.169Z Reads: 118

```
That should work. If you search the forums I helped another rider with a similar st-link.  They are all the same to some degree.
```

---
## \#19 Posted by: michaelcpg Posted at: 2016-04-15T02:53:43.087Z Reads: 119

```
Awesome thanks, I've just made an order so hopefully it'll be here early next week, I ordered an extra 6 F-F jumper cables as well seeing as it only comes with 4. In the mean time I'll look at getting an Ubuntu VM setup and do a bit of research into what's involved in the process. Once it arrives would you be happy to arrange a Skype call or other form of contact to help me through the process? I'm assuming there's quite a few steps?
```

---
## \#20 Posted by: chaka Posted at: 2016-04-15T03:00:11.226Z Reads: 118

```
There are a few steps but it isn't too difficult my only worry is the virtual machine but it should be fine.
```

---
## \#21 Posted by: michaelcpg Posted at: 2016-04-15T03:01:29.050Z Reads: 108

```
Ok well if you think it's less likely to cause issues I can setup a dual boot system?
```

---
## \#22 Posted by: chaka Posted at: 2016-04-15T03:05:05.803Z Reads: 113

```
No, it should be fine. I know someone used to program them on a vitual machine in the past. I do like bringing people over to the open source so if you have an old computer sitting around ubuntu can revive it. Linux/ubuntu runs great on older pc's.

Get some documentation on that st-links pin out order if you can. we will need it to arrange the connections properly.
```

---
## \#23 Posted by: michaelcpg Posted at: 2016-04-15T03:10:36.856Z Reads: 111

```
I've got multiple hard drives in my PC so it probably wouldn't hurt to setup a dual boot system with Ubuntu anyway as I've been tempted to dabble with a bit of Linux stuff in the past as well. Will see how things go and if I don't have much luck getting things setup I can always revert to just setting up a VM. 

Ok will do, thanks in advance for the help.

Edit: Found the company who produces these. They've got pin configuration info here:
http://www.seeedstudio.com/depot/STLink-V2-for-STM8-STM32-interface-programmer-p-2297.html?cPath=63_66
```

---
## \#24 Posted by: onloop Posted at: 2016-04-15T06:14:25.905Z Reads: 112

```
I could not wait any longer for the instructions to come from my factroy, so i disassembled my skateboard for you.

hope this helps


<img src="/uploads/db1493/original/2X/c/c6d4b0dd707b0343b1c30ec63995f9666ce135c7.png" width="690" height="388">
<img src="/uploads/db1493/original/2X/d/dc6ce909276e21ddf1945db83c074bfe9a1adb77.png" width="690" height="388">y
```

---
## \#25 Posted by: onloop Posted at: 2016-04-15T06:39:34.752Z Reads: 110

```
[quote="chaka, post:7, topic:2326"]
This tells me it is not designed for the loads we typically use. It may end up cutting power when accelerating or overheating on hills. If it gives you problems you can piggyback an order for a proper BMS on my next order to Bestech.
[/quote]

@michaelcpg don't listen to @chaka he is just wishing he had an awesome battery solution to sell to people, he gets a bit jealous of the enertion kit from time-to-time :slight_smile:

these BMS & batteries when they are pre-assembled at the factory get tested under load. The BMS you have is fine! it can easily handle 50A continuous

Only time you will have an issue is if you decide to design your drive train to be incredibly inefficient so that you are instantly converting watts to heat in a naive attempt to defy wind resistance whilst bravely attempting to break the land speed record with a 1-to-1 reduction ratio in 40degree(c) heat!
```

---
## \#26 Posted by: longhairedboy Posted at: 2016-04-15T17:33:52.260Z Reads: 104

```
This is exactly what i needed as well. Thank you! I can finish fixing a something now.
```

---
## \#27 Posted by: michaelcpg Posted at: 2016-04-16T01:37:28.130Z Reads: 101

```
Awesome thanks for the photos looks like I had everything correct :)
Have you found that your battery is outputting around 1V when it's turned off? I'm wondering if I should be worried that mine does this. Am also curious to know if your battery's LCD lights up when it's plugged into a VESC considering that mine didn't seem to?
```

---
## \#28 Posted by: onloop Posted at: 2016-04-16T03:09:02.353Z Reads: 101

```
Lcd should light up when you turn the power switch on. Plugging it into vesc shouldn't do anything.

Haven't measured the voltage when off.
```

---
## \#29 Posted by: chaka Posted at: 2016-04-16T13:09:07.479Z Reads: 95

```
@onloop  Get yourself a multimeter, they work great for testing voltage during assembly.
```

---
## \#30 Posted by: jrocca122 Posted at: 2016-04-18T03:24:16.778Z Reads: 89

```
@onloop Would you be able to post a wiring diagram for the space cell?
```

---
## \#31 Posted by: onloop Posted at: 2016-04-18T03:27:24.962Z Reads: 86

```
I posted a picture above, that should cover it.
```

---
## \#32 Posted by: jrocca122 Posted at: 2016-04-18T03:30:04.683Z Reads: 90

```
@onloop I was curious about the way the batteries are configured?
```

---
## \#33 Posted by: onloop Posted at: 2016-04-18T05:05:26.562Z Reads: 91

```
10S3P

is that what you want?
```

---
## \#34 Posted by: michaelcpg Posted at: 2016-04-18T09:25:02.334Z Reads: 95

```
<img src="/uploads/db1493/original/2X/0/0ff6d94ce7d5f191af9901105e5685606998aa89.jpg" width="690" height="372">

Here you go, this is how my battery is wired, based on a similar diagram that @Blasto kindly drew for me.
The diagram I drew at the top of this thread should cover everything else :)
```

---
## \#35 Posted by: rutxbikecron Posted at: 2016-05-30T16:40:40.330Z Reads: 81

```
Hi guys,

I'm thinking to make a similar space cell, 10S2P 5000mah, do you know what should be the maximum current on the BMS  I should buy? Do you know the brand of the BMS is shown on this topic?

I will install it with VESC and a Enertion big motor.

Thanks. :slight_smile:

Roger
```

---
## \#36 Posted by: Blacksheep Posted at: 2016-06-02T19:23:58.152Z Reads: 67

```
Could someone show a wiring diagram please?
```

---
