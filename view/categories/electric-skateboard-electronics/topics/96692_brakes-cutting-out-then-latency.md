# Brakes cutting out, then latency

### Replies: 21 Views: 271

## \#1 Posted by: iSteeb Posted at: 2019-06-16T02:35:04.301Z Reads: 87

```
I just finished my first build (first dabble in any such project really) and it’s almost great - i’ve just been encountering a few glitches and such that need ironing out.

the big one right now is, i think, vesc related - i’ll include the info i think might be relevant at the end here. i haven’t got much data to work off (only done a couple of rides), but so far: i’ve started my ride off fine. board is working perfectly. then for whatever reason i have to do a big brake (long hill for example).

after a few seconds of braking they fully cut out and nothing responds for couple of seconds. then i get some weird shit occurring. there will be latency both for acceleration, braking and even releasing the throttle (about half a second of latency for all actions). brakes will start and then after a couple of seconds cut out, even light braking. unloaded the board will respond fine, instantaneously. this only happens when i’m actually still on the board.


12s 38120 Headway cells
Vanda VESC with Ackmaniacs BLDC tool
Turnigy SK3, 192kv, 6374 motor
VESC SETTINGS:
Motor min: -30A
Motor max: 70A
Battery max: 50A (i hope this is safe, cos i see conflicting information and very little of it for the 4.12 vanda vesc, but that’s what their website says is fine for continuous)
Battery min (regen): -30A (i had this at -20 and thought maybe the vesc can’t handle the difference when braking hard, but it occurs the exact same on both settings)
I’m currently on Current mode (brakes and reverse set up and working fine), but it also occurred with current mode brakes no reverse.

anyone have any thoughts on what the issue is?
```

---
## \#2 Posted by: iSteeb Posted at: 2019-06-18T09:50:56.756Z Reads: 63

```
bump? hoping someone can help?
```

---
## \#3 Posted by: McErono Posted at: 2019-06-18T10:13:55.339Z Reads: 59

```
How many P cells are in this 12S battery? I use battery regen -12 to -16 on my samsung 30Q 12s4p batteries. Thats about 4amps per cell and on the safe side.

Don't forget, when you charged your battery to 100% it can't handle regen current and will shut down.
```

---
## \#4 Posted by: iSteeb Posted at: 2019-06-18T10:28:35.725Z Reads: 54

```
just 1p - i just got a response on reddit and long story short i fucked up with the specs sheet on my batteries.  i’m gonna drop down the battery regen to -10 so that the cells are back to a safe 1C charging, and i’ll drop the max bat to 30 back in like with the correct safe continuous discharge for them...

oh and i don’t think the battery has even been max charged yet, i got them to 3.65v each cell at 1A charging speed, according to my iMax b6 but i think it still had a ways to go (didn’t check with a multimeter). and even so, id ridden for a few km before i braked hard anyway.

i’ll have to wait til the weekend to test because my motor pulley gear is slipping and the bitch needs to be re-filed. fingers crossed you and the reddit guy’s response solves it!
```

---
## \#5 Posted by: McErono Posted at: 2019-06-18T10:35:32.264Z Reads: 48

```
Ok 1p you have to lower the regen a lot like you suggested.

If your brakes feel weak afterwards:
* Regen = highspeed brakes
* Motor min = lowspeed brakes
```

---
## \#6 Posted by: iSteeb Posted at: 2019-06-18T11:04:11.845Z Reads: 42

```
sorry, i don’t catch your meaning about high speed and low speed?  i know there’s a bit of funky background maths going on with duty etc. with the braking but that doesn’t affect how i should set the vesc right?

would reasonable settings be:

-10 battery
-30 motor min?  and if i want stronger brakes, is there anything wrong with setting this to -40, and leaving the battery at -10?
```

---
## \#7 Posted by: McErono Posted at: 2019-06-18T11:14:46.805Z Reads: 46

```
Lets say you are doing 25mph and hit the brakes - initial braking is regen value dependent (set no higher than your battery is save with). At lower speeds until standstill the braking force is according to motor min values (highest I go is equal to battery max).

Always start with conservative settings and up them as you go.
```

---
## \#8 Posted by: captclearleft Posted at: 2019-06-18T14:56:27.531Z Reads: 40

```
@iSteeb - Great post - Thanks for bringing this up.  I am surprised that more people do not have this issue initially...  

There are actually a few factors here.  
(NOTE: I do not have experience w the VANDA product.  But I do have a lot of experience setting up VESC's)
(It would help if you had some pictures, and What remote)

You are correct on changing your regen setting, that should help. Does your vesc have a capacitor bank like this one:

![vesc|690x361](upload://6YPfntThfAxIYf7AGxMAMuxbrqm.jpeg) 

If you do not have capacitors that help manage the spikes in amperage - then your batteries are going to have to take all that load.  I noticed on the VANDA website, that the VANDA VESC did not have a capacitor bank.  Is this the case?

Second:  I would avoid any reverse with a VESC.  Reverse with an RC remote can be tricky, and latterly through you off the board if you are not careful.  

Third:  When setting up your remote - Are you able to see the PWM / PPM signals sent from the remote to the VESC in your software?  Are you maximizing the settings so that your min and max are set correctly, and that the center position of the remote is learned.?
```

---
## \#9 Posted by: iSteeb Posted at: 2019-06-18T20:27:08.603Z Reads: 35

```
thanks for the response!

1. yes it has a capacitor (not a bank, just one)

2. the reverse mode works really good with ackmaniacs implementation. it’s a brake until you’re really slow then you release and pull down again and it becomes reverse.  has there been issues with it in the past?

3. yeah ive set up the remote correctly. it’s one of these cheap asian ones: https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com.au%2Fulk%2Fitm%2F202074456495
```

---
## \#10 Posted by: captclearleft Posted at: 2019-06-18T21:56:00.696Z Reads: 32

```
I guess if it's a big enough capacitor - That should be fine.  It all depends on your weight, battery setup, motor setup.  

Something to consider...
If your using Lion Cells, and you only have 1 pack (12s1p), and you have a fresh charge (98% or better), and you start rolling down hill - 
There is no where for the electricity to go.  Your VESC would try and put that electricity into the batteries. The capacitor/s would take the initial hit.  The batteries would take the rest,  but once they are full - You are relying on the VESC to dissipate that charge.  It works fine for small hills, and just slowing down.  

Reverse - that's fine I suppose.  Post a video of you riding in reverse (sounds like a lot fun). :slight_smile:   

Most RC reverse applications are such that a second hit on the remote in the "brake" direction commands reverse.  This would be dangerous on a skateboard.  If your software and the VESC are smart enough and never fail, that's awesome.  When I am riding down hill - I don't hold a constant brake... Its small hits...  If your VESC knows that you are not commanding reverse, and it's not sending opposite power to the poles - I guess that is fine.  While braking and reverse are similar - They are not the same.  Commanding reverse while going forward could (or could have) damage the VESC. 

Let us know if you get it working correctly with any of the mods.  Super helpful topic!  :+1:

That remote seems fine.  I have used those before.
```

---
## \#11 Posted by: Sebike Posted at: 2019-06-18T22:13:52.237Z Reads: 28

```
did you check for any fault codes in the terminal after the cut outs? if so, post them here. if not, next time this happens, check for fault codes before turning the vescs off after the ride and post.
```

---
## \#12 Posted by: strattos Posted at: 2019-06-19T03:37:54.145Z Reads: 25

```
A ks firmware version has a maximum erpm reverse setting so it only goes into reverse under a certain wheel speed when you move the remote from neutral to brakes.

You can come to complete stop holding down reverse/brake and it won't reverse till you release the brake/reverse and re-engage it.
```

---
## \#13 Posted by: iSteeb Posted at: 2019-06-19T04:13:24.436Z Reads: 24

```
that’s for the super helpful response. glad to hear the remote is okay.

definitely have considered that with the charged battery - not the case here (hasn’t been fully charged, and was ridden a fair bit before braking big anyway).  your braking technique sounds like a good plan going forward too though.

reverse is great!  it’s a really smart implementation - it won’t activate reverse unless you are going at below 4000ERPM (a customisable value as well). i plan on posting a full build thread when everything is complete and i’ll  include pictures and videos for ya!
```

---
## \#14 Posted by: iSteeb Posted at: 2019-06-19T04:14:30.639Z Reads: 23

```
i tried but im still learning this stuff and couldn’t see any but i might have been in the wrong spot. it’s in the BLDC tool terminal right?  all i saw was “VESC connected” type messages.
```

---
## \#15 Posted by: Friskies Posted at: 2019-06-19T04:28:26.003Z Reads: 22

```
Never heard of this Vesc clone before but your problem may stem from it being not that great a quality of a Vesc. If you are trying to set it up in FOC mode I would suggest you try BLDC instead and motor settings no more than 25 and -15/-20 and similar settings for the battery. It sounds like you may be getting drv errors and the controller is rebooting. I've seen this happen a lot with cheap clones :frowning:
```

---
## \#16 Posted by: iSteeb Posted at: 2019-06-19T04:41:19.378Z Reads: 24

```
strangely i found very little mention of them on these forums. the Vanda vesc from my reading online looks to be better quality built than most vescs and definitely better than the flipsky. taiwan manufacture instead of cheap shoddy chinese work.

definitely not using FOC, read too much about people frying their vescs with that
```

---
## \#17 Posted by: McErono Posted at: 2019-06-19T09:10:20.313Z Reads: 21

```
Using FOC on my 4.12 Torqueboards VESC on 12s4p for over a year now.

Flash new firmware, set up FOC and never switch to BLDC.
```

---
## \#18 Posted by: rusins Posted at: 2019-06-19T10:11:08.054Z Reads: 20

```
What remote are you using btw? I had something similar happen to my board once, but was unable to reproduce it, and ended up blaming my APS remote because I might have been holding the trigger down while turning it on. Not fun having a 0.5 to 1 second latency while stuck in heavy traffic. :grimacing:
```

---
## \#19 Posted by: Sebike Posted at: 2019-06-19T14:39:27.375Z Reads: 15

```
yes, in the BLDC tool terminal you should type "faults" (without citation marks) and push enter

fault codes are not stored, so if this happens again you need to read the fault codes off your vesc before shutting the board off
```

---
## \#20 Posted by: deucesdown Posted at: 2019-06-19T17:41:14.626Z Reads: 11

```
The behavior sounds like "abs over current" which is usually followed by a reboot which takes 3 seconds. Get a bluetooth module and ackmaniac's app. The app will usually be able to capture the fault even if the vesc resets.
```

---
## \#21 Posted by: Sebike Posted at: 2019-06-19T19:07:39.376Z Reads: 11

```
screen shots of your vesc settings would help as well
```

---
