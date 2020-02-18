# SpaceCell or VESC problem? No connection, blue light on L3-100%

### Replies: 26 Views: 2735

## \#1 Posted by: racidon Posted at: 2016-07-27T09:49:06.179Z Reads: 149

```
Hi All,

Sorry if the title wasn't good enough, wasn't sure how to keep it brief but not vague.

The problem is that today I noticed that the BMS display on my Spaccell Pro 3 had the letter L and number 3, I could have sworn it was something else when I first turned it on. 
It also would sit at 96% charge after taking it off the charger. 
I suspect this was due to couriers or distributors or manufacturers having the battery turned on having it arrive at my place with about 16% I think - maybe less?
I used my board for the first time today in the morning and the afternoon. 
This was about 3-4km worth of travel. 
The battery still reads 100%.
As I was approaching home I went to continue up my hill to a friends place and the board began to loose power, and then suddenly nothing. 
The battery was still turned on (read 100%) and my controller was still on, but nothing. 
So I went home pulled it apart to test. 
The receiver had no power and the VESC had no lights on. If I unplugged the receiver it would then have a single Blue led light up. 
After eliminating the wires connecting the receiver and VESC together I connected the VESC to the PC, nothing happened, but the Blue LED began to slowly dim. 
I plugged the charger into the SpaceCell (still read 100%) and let it charge for a while. 
If I try to connect the usb I still get nothing from windows, no indication it's even had a USB connect.
Is it possible that the SpaceCell has lost part of the battery bank and the VESC isn't getting the power required? 
I'm completely lost as to what to do now. 
Short of buying another cell, vesc, motor and controller I can't really rule anything out at the moment.
I should also note I've disconnected the motor and receiver to try to connect to the BLDC tool and still nothing.

Parts list:
Enertion single motor drive system
VESC (from Enertion)
FS GT2B with receiver
SpaceCell Pro 3

Any help will be greatly appreciated as I've had a small taste so far and loved it!
```

---
## \#2 Posted by: Skitzor Posted at: 2016-07-27T10:11:49.694Z Reads: 127

```
Let's start by taking a multimeter and see what's (not) coming out the spacecell. Do you measure any voltage? 
I'm guessing not. Otherwise the vesc would show up in your bdlc tool
```

---
## \#3 Posted by: lox897 Posted at: 2016-07-27T10:17:01.137Z Reads: 124

```
This is an issue that has popped up a few times with the space cell. It is caused by the button on the back of the percentage meter being pressed down and switching to a lower cell count which means that it will think the battery is at 100%. Pull the percentage meter out and desolder the button or just make sure it isn't getting pressed down by anything. Hope this helps and your battery is working soon!
```

---
## \#4 Posted by: lox897 Posted at: 2016-07-27T10:18:13.561Z Reads: 121

```
I don't know what the issue is with the VESC though. @onloop can help
```

---
## \#5 Posted by: racidon Posted at: 2016-07-27T10:44:57.986Z Reads: 117

```
I get 42v from my multimeter
```

---
## \#6 Posted by: racidon Posted at: 2016-07-27T10:45:54.309Z Reads: 113

```
how do I reset it to 10 though? if I push the button it just cycles through showing L3 42V 100% and screen off
```

---
## \#7 Posted by: lox897 Posted at: 2016-07-27T10:59:21.677Z Reads: 106

```
Someone else can chime in here. I know someone knows the way. Try holding down the button and then pressing it to cycle through.
```

---
## \#8 Posted by: racidon Posted at: 2016-07-27T11:03:19.772Z Reads: 104

```
I measured the value for the + and - of the controller pins and got 5V and the - and Signal pins and got 3V
```

---
## \#9 Posted by: Skitzor Posted at: 2016-07-27T11:07:30.142Z Reads: 101

```
Allright. So the only problem you have is the display being in wrong settings? Does the motor still work when you accellerate?
```

---
## \#10 Posted by: racidon Posted at: 2016-07-27T11:14:25.595Z Reads: 95

```
no because once I plug my receiver in the VESC blue light turns off
and I can't get it to connect via BLDC to do a motor test there, the VESC gets very warm if I leave it turned on...
```

---
## \#11 Posted by: Skitzor Posted at: 2016-07-27T11:18:40.323Z Reads: 94

```
If you leave the receiver disconnected. Power on your spacecell. are you able to connect it with USB ?
Edit: nvm, I've read your initial post over and over again. 

Do you see any possible traces of burn on your VESC ?

Do you measure your 42V also on the lead endpoints soldered on the VESC?
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-07-27T11:25:16.658Z Reads: 92

```
Maybe the VESC throw some faults?
You can check it when you go to the terminal in BLDC-Tool and type in 'faults'.
```

---
## \#13 Posted by: racidon Posted at: 2016-07-27T11:29:41.882Z Reads: 91

```
I get the same from directly on the solder points of the VESC, is there any way to test the Caps?
I can't see any burn marks at all (checked earlier as I saw that was a common symptom of this issue)
```

---
## \#14 Posted by: racidon Posted at: 2016-07-27T11:30:14.978Z Reads: 88

```
I can't connect to the BLDC
```

---
## \#15 Posted by: racidon Posted at: 2016-07-27T11:31:57.065Z Reads: 86

```
I figured it out. Hold it down when turning the battery on on and then you can cycle through L3 -> L12 and then some voltage settings, find the one you want and turn it off and back on again
```

---
## \#16 Posted by: Skitzor Posted at: 2016-07-27T11:34:12.945Z Reads: 85

```
You need L-10, fyi.
Your other problem is definately in your VESC.

Edit: with normal power, your blue (5v) and green (no idea what) led should come on. I'm guessing you're going to need to check your regulators. 

Maybe Expert @chaka can shed some light on this problem. I like to learn as much as I can about the VESC.
```

---
## \#17 Posted by: racidon Posted at: 2016-07-27T12:10:05.278Z Reads: 82

```
Would there be a circuit diagram I can look at so I can do some general tests? keen to find out if I need a new one or how to fix it, waited months to get all this for it to fail :(
```

---
## \#18 Posted by: Skitzor Posted at: 2016-07-27T12:26:26.133Z Reads: 82

```
Schematics are available from Vedders Site:
http://vedder.se/2015/01/vesc-open-source-esc/ 

Maybe this post on his forum can also be helpful for measuring points:
http://vedder.se/forums/viewtopic.php?t=195

Someone with a similar problem on the forum:
http://vedder.se/forums/viewtopic.php?f=7&t=245
```

---
## \#19 Posted by: racidon Posted at: 2016-07-27T12:58:00.854Z Reads: 89

```
Thanks a lot for all this help guys. Especially Skitzor :slight_smile:
I managed to get the VESC connected to BLDC 
I think I found the issue, not sure though. It looks like the main positive wire is being pierced by a pin on the back of a connector as the shrink tube has been done very tight. I might cut it off tonight and see what I can do with placing it all a little better
I've attached some images of bldc tool readouts incase anything is out of the ordinary.
I also get a failed to detect message when I try to detect the motor....

<img src="/uploads/db1493/original/2X/0/06e0b4a971cd83a22fe6f50670205f8d780d5d58.png" width="690" height="384">
<img src="/uploads/db1493/original/2X/6/6a62c8a0b54a1b65a47269b245aa9165e76cd7db.png" width="690" height="384">
```

---
## \#20 Posted by: Skitzor Posted at: 2016-07-27T14:56:25.727Z Reads: 82

```
Oh, you mean the bottom of the Hall sensor connector pierced your mains red cable? 
You should cut them as close to the pcb board to prevent this. I too was made aware of it by @chaka.
On a sidenote, you're lucky your vesc wasn't totalled ! And glad to help you out, or at least made you think in the right direction !
```

---
## \#21 Posted by: racidon Posted at: 2016-07-27T23:07:53.745Z Reads: 82

```
So I still think the VESC is fried as it wouldn't connect to the PC again after this and it kept failing to detect the motor. I do however have it in the state that the blue light is on and red is flashing (constantly) which is more than what I had yesterday.
I may just order another one from Enertion for now (hope that they caught up on orders) and work out getting it fixed/replaced with them in the meantime. I plan on making another board down the track so extra VESCs won't be a problem.
```

---
## \#22 Posted by: racidon Posted at: 2016-07-28T08:51:51.006Z Reads: 76

```
I was wondering if someone could confirm a suspicion for me. I think the powerdelivery is screwed in the VESC due to that pierced cable. When powered on does the VESC blue light EVER flash? or does it just stay light at all times?
I also tried removing the shrink wrap around the cables and pcb that caused it to be pushed into the pin and found that it had 2 pins actually piercing and both pierced enough to get a connection, which is odd as it doesn't even have to pierce far considering there's no protection there...
I would suggest some hot glue over these pins for anyone else.
```

---
## \#23 Posted by: chaka Posted at: 2016-07-28T13:05:41.053Z Reads: 75

```
Constant red flashing is a drv fault and it needs to be replaced. This was most likely cuased by the pins being shorted by the battery cable. The pins piercing the positive power cable is a known issue and they should have been cut flush.
```

---
## \#24 Posted by: racidon Posted at: 2016-07-28T13:19:53.314Z Reads: 75

```
Thanks for the confirmation mate. I guess I just have to wait for a email back from EnertionSupport and until the next batch of VESCs come around.
In the mean time is there any ESCs you can suggest that would work well (plug 'n' play)  with this setup?

Parts list:
Enertion single motor drive system
FS GT2B with receiver
SpaceCell Pro 3 (10s)
```

---
## \#25 Posted by: chaka Posted at: 2016-07-28T13:30:04.860Z Reads: 75

```
Not really. You need to be able to limit you motor amps with a pack that small since that motor will pull more amps than that bms can handle. The vesc is the only esc that is capable of doing this.
```

---
## \#26 Posted by: Lorenz Posted at: 2017-01-01T17:05:26.188Z Reads: 40

```
I have a big problem with my vesv too when i power my vesc and plug it into the pc the vesc lights up blue than blinks 3times red when i than press connect on the bldc tool it says no firmware read response i have the vesc v4,12 with firmware 2,18 i cant get it to connect my battery is a 6s5p 18650 without a bms only a ballance cable i am using win7 and when i go to device manager i can see the vesc i cant update the firmware becouse i cant connect what should i do pls help
```

---
