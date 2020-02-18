# VESC FAQ &#124; Easy VESC Configuration in Windows / Mac for Noob

### Replies: 23 Views: 14153

## \#1 Posted by: laurnts Posted at: 2016-05-07T02:41:49.580Z Reads: 1506

```
For all new members who are interested in VESC and have been reading alot and still have questions about it because it might seems to difficult, **I tell you it's not**. In fact **it's almost as straight forward as doing programming with program card**. It provides more options, but **you don't need ALL OF THEM!**

You only need to configure 3 Basic Things! (BLDC mode)
1. Configure your Battery Voltage and Amps
2. Configure your Motor
3. Configure your Remote

And if you seen VESC from Vedder and ohh crap I need to instal linux with some command line and then compile things and so on.... That is only if you want to recompile your own code and or you just finished soldering a VESC that you need to insert the firmware.

**If you buy a pre-made VESC from Ollinboard / Enertion / any valid / known members here, they all came preinstalled with firmware already. So you don't need linux, you don't need ST Link V2. You only need a pc / mac with usb port.**

Then get your self a pre-compiled BLDC tool from http://vesc.net.au specially made by @jacobbloy. Provide the guy with love "donation" and you only need to install them. It takes you minutes to get BLDC tool up and running detecting your VESC.

There are videos how to configure VESC from Vedder / Enertion / Vesc.net.au / other sources how to do so. It's really really easy.

**Trust me, I got NO LINUX and I got NO ST LINK V2**
```

---
## \#2 Posted by: onloop Posted at: 2016-05-07T02:44:20.972Z Reads: 1390

```

GREAT WORK!, it's what this community needs, more user generated content to help people build better eboards....
```

---
## \#3 Posted by: treenutter Posted at: 2016-05-07T03:25:59.256Z Reads: 1337

```
@laurnts I think that a lot of people needed to hear this!
```

---
## \#4 Posted by: Mobutusan Posted at: 2016-05-07T04:25:03.677Z Reads: 1258

```
@laurnts Thanks for posting this. It's reassuring that when I finally do jump on the VESC train, I'm gonna be able to program it without destroying it.
```

---
## \#5 Posted by: jacobbloy Posted at: 2016-05-07T05:30:44.431Z Reads: 1121

```
Next update will have online firmware updates with a tick box for vesc hardware version and maybe auto hardware detection so no confusion, I'm also going to make a quick start wizard.
```

---
## \#6 Posted by: lilracerboi Posted at: 2016-05-07T05:52:33.859Z Reads: 989

```
Awesome.

I don't have the VESC yet, because of the current delays, but I just downloaded the BLDC Tool to take a look at.
Also can't donate now, but will in the near future when my summer hours pickup.
```

---
## \#7 Posted by: evoheyax Posted at: 2016-05-07T21:23:05.041Z Reads: 871

```
I think we should have some topics like this pinned to the top of the forum. This will get buried and newbs will come ask questions answered right here.

Or better yet, one that links everything together that is pined to the top. People are a) lazy and b) don't always know what term to search for. I think that would help :)
```

---
## \#8 Posted by: anoop54 Posted at: 2016-08-05T22:23:27.765Z Reads: 719

```
Hey new member here wanted to ask, I have a 12s battery supply and a 12s 170kv motor. What parameters do I need to set? In bldc mode, like besides the motor config where is has all the volatge and stuff what do i change? Also is it okay to us the 12s supply to program the vsec? I've herd i need a external supply.
```

---
## \#9 Posted by: Pablo_702 Posted at: 2016-08-11T00:50:14.922Z Reads: 685

```
depending on were you got ur vesc from, the reason why some recommend to use a power supply is becasue most of them are not tested and there might be some shor in the vesc from factory i got mine from ollin board wich is by far the best vesc out there and they test each one of the vescs leaving there warehouse when i got mine i plugged mine straig to my fully charged 12s and everything worked just fine
```

---
## \#10 Posted by: D3rax Posted at: 2016-10-13T20:59:43.585Z Reads: 576

```
How do you power up your vesc when programming? I did read somewhere on this forum that a special power suppley is only nesceseray when the vesc-x is booted for the first time? 

And how is this with the newer vesc-x?
```

---
## \#11 Posted by: TarzanHBK Posted at: 2016-10-14T10:47:18.126Z Reads: 556

```
some people selling vesc test them prior to shipping, so they´ll do that for you. After that you can just throw your normal batterys on there.
If you buy somewhere else or want to go 100% safe, power it up with a low voltage battery, like one 3s or like @chaka mentioned somewhere, use two 9V batteries in series.
```

---
## \#12 Posted by: D3rax Posted at: 2016-10-14T15:35:26.948Z Reads: 538

```
Great, thanks for clairfying that. Makes the vesc a lot more usable for me.
```

---
## \#13 Posted by: rfschmidt1 Posted at: 2017-05-16T23:50:43.606Z Reads: 397

```
When I click on the link it says that the Service is Unavailable. Is there something i'm missing???
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-05-17T07:32:55.999Z Reads: 391

```
the site is down. I recommend you get Ackmaniacs BLDC tool instead:

https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#15 Posted by: Bugist Posted at: 2018-08-24T06:24:44.258Z Reads: 122

```
Okay, if I go to test with 2 9volts in series, how do I know if something is actually wrong? Assuming there is a fault in using 18 volts so the fault is indicated by heat and not by fire or sparks correct?
```

---
## \#16 Posted by: TarzanHBK Posted at: 2018-08-24T06:34:25.890Z Reads: 119

```
where did you get your vesc from?
Nowadays they should all be able to be powered up with your normal "ride"-battery.
If you stil wanna be 100% sure, power it up with 18V, connect to a pc and get it connected to a vesc-tool.
There will be no sparks or something ;)
If a vesc is damaged it´s really rare that you have a minimum of smoke because of a damaged resistor, but that´s all.
```

---
## \#17 Posted by: Bugist Posted at: 2018-08-24T14:43:47.665Z Reads: 106

```
I got mine from flipsky, they have no reviews and don't say that they come tested so I really don't know what to expect
```

---
## \#18 Posted by: TarzanHBK Posted at: 2018-08-24T14:45:30.397Z Reads: 100

```
should be ok with your normal battery, but like i said, if you´re unsure, start with the other battery to power it up the first time
```

---
## \#19 Posted by: Bugist Posted at: 2018-08-24T14:46:41.053Z Reads: 99

```
Okay, if something is damaged the vesc tool will show a fault code?
```

---
## \#20 Posted by: TarzanHBK Posted at: 2018-08-24T14:47:42.805Z Reads: 100

```
if you go to terminal and type in "faults" yes
```

---
## \#21 Posted by: Bugist Posted at: 2018-08-25T14:54:08.292Z Reads: 91

```
So, my VESC didn't come with a micro usb cable and i dont think ive seen one in 5 years... Is it a bad idea to replace it with a mini usb from an old android phone? Or should i find the right cable?
```

---
## \#22 Posted by: TowerCrisis Posted at: 2018-08-25T15:31:47.831Z Reads: 91

```
I think you've got those flipped, it uses a mini and Android's have used micro.

Besides that, no definitely do not replace it. You're risking damaging the vesc before you ever even get to use it.

It also uses a mini because it's a very robust connection to the PCB. It's just in general stronger, which is important for an expensive device that could be effectively bricked for the end user if they don't have a way of fixing it.

Just get the right cable. they're more common than you might think, plenty of Arduino based boards use it, and just DIY electronics in general. Some even use usb B type connectors.
```

---
## \#23 Posted by: Bugist Posted at: 2018-08-30T21:43:15.544Z Reads: 74

```
Okay so I've got 18 volt, the negative of the battery going to the negative of the vesc and the vesc plugged into the computer but there are no option coming up under "port" and the auto connect feature won't work either...
```

---
