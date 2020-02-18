# 293 Miles in FOC to a dead DRV

### Replies: 23 Views: 1833

## \#1 Posted by: Deckoz Posted at: 2017-08-17T21:42:40.315Z Reads: 276

```
So, I built my board 18 days ago. Today I have a burned DRV. 

Specs:
10s3p
Torqueboards 6355 190kv dual
4.12 Torqueboards VESCs

I've put 293 miles on this board in the past couple of weeks in FOC and all has been fine and lovely. I go on lunch today, come back and as always - when I plug in I test motors and before I unplug I test motors at very low throttle. Anyway back from lunch get to my desk, test motors with a blip, fine. unplug work the rest of the day, goto leave, plug in, test motors, only one motor spins. DRV burnt out. I can't understand why it would burn out from the time of unplugging to plugging back in.


electric skateboard gods are killing my buzz right now.
```

---
## \#2 Posted by: Deckoz Posted at: 2017-08-17T22:02:22.534Z Reads: 270

```
After some probing the following components are dead
Tantalum Cap
<img src="/uploads/db1493/original/3X/b/b/bb1197c5d5ca7222f96f47853d60d78f4bbf5304.jpg" width="374" height="499">

Diode
<img src="/uploads/db1493/original/3X/0/9/09b62963108d9c60892dcbc45859d007642fc76d.jpg" width="374" height="499">

Diode
<img src="/uploads/db1493/original/3X/b/5/b58076bcf9a4a7f4db84d51c65685856b6ebc839.jpg" width="666" height="500">

VREG
<img src="/uploads/db1493/original/3X/d/0/d0b20cbac5b149305e43a32835b600e55f45368c.jpg" width="666" height="500">

DRV
<img src="/uploads/db1493/original/3X/0/3/031085dd73cfe9207adfddf2b1f2fa293fa068e2.jpg" width="374" height="499">

Looks to me like the originating pin on the DRV is connected to the VREG by through board VIA

@torqueboards any reason these VREGs blow??

@chaka You seem to be a wizard here, so apologies for tagging you, but any clues you could pass my way for digikey or mouser item #s and or if you think this is repairable/upgradable to prevent the VREG from failing and blowing the DRV?
```

---
## \#3 Posted by: DavidBanner Posted at: 2017-08-17T22:14:43.293Z Reads: 260

```
oh man, that sucks!

I feel for ya
```

---
## \#4 Posted by: Deckoz Posted at: 2017-08-17T22:28:54.451Z Reads: 256

```
Yea man...I don't even know why... can't really say its FOC configured improperly as I put 293 miles on it and made sure to configure both BLDC motor table as well as FOC...(BLDC motor table is used incase there is a failure on the sensors for it to fall back to)

just weird...and unfortunate...not really sure if I should replace the DRV or move to an ESC with a transistor in place to shut down the DRV so it doesn't blow... either way..more money in the money pit...
```

---
## \#5 Posted by: Jinra Posted at: 2017-08-17T23:34:22.842Z Reads: 249

```
@lowGuido doesn't call them DRVcookers for nothing
```

---
## \#6 Posted by: Deckoz Posted at: 2017-08-17T23:52:42.461Z Reads: 247

```
Confused by what you mean? My vesc have never hit above 119F in all my logs. So not sure how it cooked.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-08-17T23:59:19.316Z Reads: 243

```
yeah @Jinra  VESC are great I love that its 100% programable. I love that its designed from ground up for skateboards.

heres what it doesnt do:
protect itself.

It is literally so programable it allows you to program parameters that will kill it. 
there is no short circuit protection. touch motor wires you will kill it.
and it is literally just a circuit board (v4.12) with no shock, vibration or impact protection.
its a great ESC don't get me wrong. its just not robust. FOCBOX and newer versions might be better, but I have no experience with them.
```

---
## \#8 Posted by: saul Posted at: 2017-08-18T03:16:13.988Z Reads: 225

```
was it on canbus or split ppm?
if its canbus I'm guessing thats the slave that burnt? :thinking:
```

---
## \#9 Posted by: SORRENTINO Posted at: 2017-08-18T14:03:35.210Z Reads: 205

```
"Yes it was canbus and it was the slave that blew. Is this a known issue with canbus slaves?" I'm replying  for Deckoz.
```

---
## \#10 Posted by: chaka Posted at: 2017-08-18T15:29:30.791Z Reads: 196

```
If I were to guess, totally swinging blind here, you might have a failed or failing MOSFET. If you remove that DRV be very careful, it is probably welded to the PCB on pin #29, V-Supply. Once the drv is replaced you might find the rest of the components to be in working order.

You will need to remove all the MOSFETs to test them. Takes patience and steady heat to do it since there is a lot of thermal mass around the MOSFETs
```

---
## \#11 Posted by: saul Posted at: 2017-08-18T20:02:14.238Z Reads: 184

```
I don't think its a known issue but I'm pretty sure i've read of other slave vesc go boom for no apparent reason.

but then some people use canbus with no problems at all...
```

---
## \#12 Posted by: Deckoz Posted at: 2017-08-18T20:56:45.902Z Reads: 176

```
@SORRENTINO thanks for replying while I couldn't since my account is new..and this forum has some silly limit on responses after signing up.

@chaka tested the FETS all seem to be functional. To me the only thing I can think of is the VREG(what looks to be a vreg anyway)blew and it cascade into everything else. Not quite sure what the Tantalum cap goes to or the diode underneath the  VREG but those are blown as well. Any chance you have some mouser/digikey item #'s? As currently the ESC doesn't even power on.

@torqueboards as always no input and ignoring customers. you haven't even refunded the faulty anti-sparks my friend and I ordered and shipped back weeks ago... so should I expect any less, your support is about as low as it can get lol. 

@saul interesting. I use traction control, which can't be done over y splitter....ugh its a shame if this is the case - but it seems most people burn out the can chip - which mine seems to be fine... it all looks to have started at the linear voltage regulator(or what appears to be a linear vreg)
```

---
## \#13 Posted by: torqueboards Posted at: 2017-08-19T00:10:32.272Z Reads: 155

```
@Deckoz - Obviously, I have no idea who you are from your screenname. But you can email me at dexter@ and I can check up on it for you.
```

---
## \#14 Posted by: saul Posted at: 2017-08-19T04:07:54.935Z Reads: 157

```
[quote="Deckoz, post:12, topic:30922"]
I use traction control, which can't be done over y splitter
[/quote]

i'm pretty sure traction control is the problem.
all it does is set the current equal, which is not good in many cases.
```

---
## \#15 Posted by: Deckoz Posted at: 2017-08-19T17:00:12.279Z Reads: 150

```
@torqueboards I told my buddy @pshaw to email you since it was his PayPal for the antisparks... 

I'm the guy your support argued with over a week about a $700 order and sending motors and vescs all of which had 5.5mm barrels - except one motor had 4.5mm barrels and all ya had to do was ship me 3 male 5.5s to correct it, which after way to many conversations with Mary, you finally did. Then my buddy and I ordered two antispark switches from you. We literally plugged them in turned them on and they never turned off again(failed open first time it ever switched lol). 

The trucks I ordered from y'all, well they seem nice until you realize the kingpin hole is way off center and turning in both directions isn't even and needs to be cored out to even feel right.

Kingpin holes as received <img src="/uploads/db1493/original/3X/3/3/33025d848d0bf4c45773826d3d4e90a1b63a634b.jpeg" width="690" height="414">

Centering milled & fixed
<img src="/uploads/db1493/original/3X/6/2/62f2a0a8b7abeaf99fae71fb89e9c4b195b83c90.jpeg" width="295" height="500">
Centering fixed with riot plug after milling.
<img src="/uploads/db1493/original/3X/7/e/7e71fd0408990423fac1fb2badb929977071aa08.jpeg" width="295" height="500">


The motor drive pulleys received inter rim is pressed on vs tac welded. So this happens until you tac weld it on.
<img src="/uploads/db1493/original/3X/f/c/fc57534f6f48c5b82ebf094b7c65e25a4017ab2e.jpg" width="374" height="499">

And now a bum VESC that started at the voltage regulator - which shouldn't have even happened as its way within the limitations of the VESC(10s 42V)



@saul I'm not sure that  is an accurate statement. The rpm data is compared. Over CAN throttle signal manipulates the VESCs independently until a rpm signal is received that is greater then the Traction control Erpm threshold. At which point it limits the motor current with higher rpm from accelerating to infinity from traction loss but is not making the current the same.  You can see how traction control behaves at the end of this file in the "//Traction Control" segment.

https://github.com/vedderb/bldc/blob/master/applications/app_ppm.c
```

---
## \#16 Posted by: Deckoz Posted at: 2017-08-30T19:06:07.367Z Reads: 123

```
Can anyone provide the part number for this diode?

D5?
<img src="/uploads/db1493/original/3X/7/9/79b7d9f0dae8f22822be2a0475a0ad931dbbb755.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/d/f/df132c2bcee4661bca6e3bdddce9a601c4085da5.jpg" width="375" height="500">
```

---
## \#17 Posted by: sl33py Posted at: 2017-08-30T19:46:48.455Z Reads: 116

```
Have you looked on Ben's github at his BOM which should note exact specs so you can find on mouser/similar?
```

---
## \#18 Posted by: Deckoz Posted at: 2017-08-30T20:06:23.388Z Reads: 116

```
I just found the BOM thanks.

Also found out after replacing the DRV my suspicions were right

D4, L1, C33, are all downstream of D5. 
<img src="/uploads/db1493/original/3X/0/c/0c94cae0ed5b17a6a6dc3c88558a4e771c6337b8.png" width="627" height="217">
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2017-08-30T20:07:52.311Z Reads: 118

```
Did the diode blow after you replace the DRV... if so, you're 5V is probably at 8v, and the ground plane under the drv is not properly solder
```

---
## \#20 Posted by: Deckoz Posted at: 2017-08-31T00:52:03.861Z Reads: 110

```
The components were dead before the DRV replacement. ^ from posts above. I'm getting 5v at that pad
```

---
## \#21 Posted by: SORRENTINO Posted at: 2017-09-22T17:44:51.239Z Reads: 82

```
So looks like 6 vescs from DIY Electric dead all within 2 months or riding. Pretty shitty if you ask me. Sounds like a bad batch. Pretty pissed about it.
```

---
## \#22 Posted by: Chewie Posted at: 2017-09-22T18:10:18.624Z Reads: 82

```
Yup, Was just riding sub 10mph in the parking lot and poof, no brakes, no power FAULT: FAULT_CODE_DRV8302
```

---
## \#24 Posted by: Mikenopolis Posted at: 2017-09-22T19:57:32.745Z Reads: 65

```
probably less than ONE mile with my vesc-x using FOC and I just got FAULT_CODE_DRV8302. I didn't even notice anything until I opened up the enclosure to change something and saw a blinking light. gave no faults until I reflashed the FW, reconnected and checked faults again.
```

---
