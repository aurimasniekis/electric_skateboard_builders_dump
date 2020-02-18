# How to download linux on a mac

### Replies: 10 Views: 939

## \#1 Posted by: mcoyle Posted at: 2016-04-28T02:18:38.638Z Reads: 66

```
I'm trying to download linux for my Macbook Pro to use the BLDC tool (it was recommended to me to use linux rather than mac os since I'm having trouble connecting), but can't find any great places to get the software from. Can anyone help redirect me there? Or maybe help me figure out why it isnt working?
The battery is on and working, plugged into my dual VESC and then off to my two motors. I can't figure out why it wont work when I accelerate the trigger or connect to my computer.
```

---
## \#2 Posted by: dacc34 Posted at: 2016-04-28T02:25:19.820Z Reads: 62

```
Oh hey, something that I'm actually good at. I haven't used Linux on a Mac before, but this looks like a good tutorial for it: http://computers.tutsplus.com/tutorials/how-to-create-a-bootable-ubuntu-usb-drive-for-mac-in-os-x--cms-21253

You could probably just boot it from the USB and use the BLDC tool without even installing it if you wanted.
```

---
## \#3 Posted by: mcoyle Posted at: 2016-04-28T02:34:20.958Z Reads: 55

```
I'm having trouble connecting with the VESC. It won't recognize the USB as an option to connect to, so I've been redirected towards linux, since apparently the BLDC tool works better with it.
```

---
## \#4 Posted by: laurnts Posted at: 2016-04-28T03:10:06.151Z Reads: 50

```
If mac BLDC tool doesnt work for you then you cant have linux on a bootable usb. You will need a dual boot mac most likely. Maybe @jacobbloy could shed some light for you.
```

---
## \#5 Posted by: jacobbloy Posted at: 2016-04-28T03:54:33.622Z Reads: 49

```
I'm not sure why you can't connect with your mac it's only ever Windows that has a problem!

What version of OS X are you using? And have you tried a different cable?
Do you have your vesc powered via a battery?

Send me a pm I'll offers a support session for you! Usually it is some thing really basic and gets fixed in no time at all
```

---
## \#6 Posted by: massy Posted at: 2016-04-28T13:14:59.954Z Reads: 35

```
It should be fine with a bootable USB as long as the same steps are taken as on the regular version. Myself I installed an Ubuntu VM on my mac. Works like a charm!
```

---
## \#7 Posted by: laurnts Posted at: 2016-04-28T14:29:56.690Z Reads: 27

```
I'll try with my VM'ed ubuntu. This is very interesting to be able to compile directly those files without sing BLDC tool especially if I would like to change / adjust some parameters. Thnx for the info
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-04-28T14:41:11.301Z Reads: 25

```
Yeah i would totally run Linux off of a USB stick rather than installing over your Mac. The mac is already running a very nice flavor of Unix and it would be a shame to waste it. 

i'm putting windows back on my linux laptop and just stocking up on all the older and newer BLDC windows versions i can find.
```

---
## \#9 Posted by: mcoyle Posted at: 2016-04-28T14:59:35.675Z Reads: 26

```
What would be the best route for me? I'm not really sure how to do any of this but I'll learn whatever I need. I can't get the BLDC to recognize and connect to my VESC. I haven't tried another wire (can someone link me one?), I'm not really sure if the VESC is even lighting up (or where it lights up from), and I want someone else to tell me that I should try linux before I go and download it.
```

---
## \#10 Posted by: Bobfandango Posted at: 2016-04-28T18:16:03.131Z Reads: 21

```
I would *not* try Linux just yet at all since you haven't eliminated all the potential problems..  I use a MacBook Pro as well, and it has no trouble whatsoever connecting to the vesc.  First, make sure the VESC is indeed powered.  There are LEDs on the board that should light up if it is powered up.  If you have power to the VESC, the go ahead and try a different USB cable to see if that helps.  I suppose you could also try a different USB port on the mac, but that doesn't seem like a likely issue.

Anyhow, until you are 100% certain you need to deal with dual boot or a USB stick, I wouldn't go to the trouble.  Jacob's OSX build of the BLDC tool works just fine.
```

---
