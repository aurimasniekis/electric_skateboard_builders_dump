# New vesc and 4S, nunchuck dropout, heat issues

### Replies: 16 Views: 1980

## \#1 Posted by: petter Posted at: 2016-07-18T08:37:07.750Z Reads: 172

```
So hey, just got my vesc this friday and have been riding it the weekend. And then i could not resist also installing my nyko kama nunchuck and testing that out. Soldered in and hotglued. 

Now my board is the classic don't do it this way, I have a 380KV NTM, I believe it was the lowest KV in stock when i ordered it last fall and the bearings are busted now and so on.. will be changing it soon. But because of this i use 4S, my top speed is around 28km/h as measured by GPS. 

This is not a great match for the vesc since it needs such high currents, the torqueboards 6S gave alot more power and less heat issues but this is just a design flaw from my side ;)

The bigger issue that i am thinking about is the dropouts. The connection between the nunchuck and vesc seems alright, it has good range even with the etched antenna and keeps the connection as long as the board is powered. But, it ALWAYS drops out during heavy accelerations/hills! I set the max current to 80A to get some performance from it but this is to much for the vesc in the long run, the temp protection kicks in after a few hills. I will probably lower this to maybe 55A for now to maybe be able to ride more (but sadly with less power... just until new gear arrives/is afforded).

Now my actual question is this, my guess is that the dropouts are from the high currents causing EMI that is killing the I2C to the nunchuck. Is anyone using a similar setup with similar issues? Will the dropouts go away when i go to 8 or 12S and hence lower currents?

No other problems than this with it though, for example braking works a treat, full connection and set max braking current to 48 A/24A to battery.
```

---
## \#2 Posted by: trbt555 Posted at: 2016-07-18T08:57:44.919Z Reads: 155

```
You're probably either hitting the max current cutoff or the max temp cutoff because 4S is way too low to be running an eboard efficiëntly. This has nothing to do with the Kama connection.
Go to 12S and you probably won't have the same problems.
```

---
## \#3 Posted by: petter Posted at: 2016-07-18T09:14:40.903Z Reads: 148

```
No, it's not that. And I am very sure of this because the board is unresponsive for 1 second, as per the connection loss timeout. 

For example, starting on a flat sidewalk, full acceleration. The board will start, accelerate but jerk once a second when the timeout kicks in. Inbetween these jerks i have no control of the board.

Also since the vesc is not made for these currents the temp cutoff is very familiar to me, and it's fabulous! It will gradually turn down the power as the heat rises and is very consistent on this. 

I don't think it is the max current either as then the board would not keep accelerating in between the jerks while being unresponsive. This is definitely the remote connection, the only question is if it's RF or I2C, and what is causing it. And since the brakes are fine and set at lower currents, most likely it's the high currents causing EMI that are the issue.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-07-18T09:30:06.453Z Reads: 127

```
I am betting it is the VESC with some fail safe.

When you hit a fault, like an over_current, you loose control for some seconds! Like you described! 4S does not sound healthy.... I would try it with 8S and report back
```

---
## \#5 Posted by: petter Posted at: 2016-07-18T09:39:15.254Z Reads: 128

```
Ok, fine. But then, if it is over current, why would it keep accelerating? If such a fail-safe limit is hit, the sensible thing would be to shut down to prevent damage, or, at the very least, significantly turn down the power. Not to just keep going?

The jerk in question is the board losing power for 0.1 seconds tops. Full power in between.
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-07-18T09:41:16.302Z Reads: 128

```
[quote="petter, post:5, topic:6264"]
why would it keep accelerating?
[/quote]

You never said that it keeps accelerating or i just overread it...

If it is still accelerating it cant be a failsafe of the vesc and therefore you are right with your thought that it has to be some problem with the remote.
```

---
## \#7 Posted by: petter Posted at: 2016-07-18T09:49:00.611Z Reads: 119

```
Not so easy to convey my experience in text i guess :) I have a long slope down from my house leading to a quite steep uphill. It's a smooth ride on the way down until i hit the throttle just before the incline. I get good tourque going up but for the jerks once a second. When i get to the top i release the throttle and the board keeps going full power for one second until it "hears" me and i regain control.
```

---
## \#8 Posted by: petter Posted at: 2016-07-18T12:26:45.216Z Reads: 111

```
Does anyone have an idea how to isolate if this is an radio or I2C issue? Wires from vesc to receiver is some 2cm, which basically means that it's placed almost between the battery and motor cables. Pretty much the worst place to put it for radio but that would be an easy fix to just use longer wires and place it in the other end of compartment, where i had my old receiver for PPM. 
OTOH, if it's a problem with interference on the I2C, long wires just means more interference! And there is not really a solution for this, since it's connected to the vesc and that is what is generating the EMR. Shielding is sort of fiddly for a 2 cm cable..

So my guess would be I2C because of the way it's acting, i would expect the receiver to return a 0 upon signal loss and therefore cut the acceleration. But then this would be implementation specific so it might just be the radio anyways.
```

---
## \#9 Posted by: brun Posted at: 2016-08-09T05:43:47.013Z Reads: 88

```
I was (still am somewhat) having this same issue.  I shortened the wires from VESC to motor and VESC to receiver and it's helped a lot.  Im not sure which change caused the improvement.  Shortening both sets of wires could have reduced I2C (wire) noise...but shortening the VESC-to-motor wires could also have reduced RF noise interfering with the bluetooth signal.  There isn't much more I can do now.  I only have 6s batteries.  

Has anyone had a GOOD experience with using the nunchuck?   Previously I was using my own NRF2401+ radio that was connected to the VESC PPM port and had no issue with interference.  My problem with NRF/PPM setup was that the BLDC software doesn't seem to have the same nice-ramping acceleration and braking management when using PPM.   Has anyone used the VESC native NRF inputs?  What is the protocol...what numbers is the VESC looking for?
```

---
## \#10 Posted by: petter Posted at: 2016-08-15T12:41:24.277Z Reads: 79

```
Tricky situation. How is your reception otherwise? i had a very good signal as long as i was not doing full throttle. Also i was running on low batteries, i just had them in the receiver for 6 months but never used it, they still got drained. So new ones sort of made it better but not perfect. 

I was also using a standard RF remote before and never ever had any signal problems. But i will get my new motor this weekend(hopefully), going from 370 -> 190 KV should bring down the current to half and hopefully i can sort this out then ;) But well see, signal loss is not very nice
```

---
## \#11 Posted by: brun Posted at: 2016-10-03T05:30:41.937Z Reads: 59

```
Hi Petter...any improvement to the signal loss problems?
```

---
## \#12 Posted by: petter Posted at: 2016-10-04T14:41:34.280Z Reads: 52

```
Nope, sorry to say... Had ALOT of shipping issues with my order for a new motor so i only just got it last week but, tried it, didn't work any better. In fact, it seemed much worse than before! I wonder why it would do that, maybe there is some ground/power issue to the nyko receiver?

Has anyone tried the [wiiceiver](http://austindavid.com/jm3/index.php/hardware/3-wiiceiver)? I wonder if that would give a better signal, being more designed for it and also giving better power distribution/ability to place it anywhere with super short signal path for i2c and PPM carrying the signal to the vesc and possible the "trouble zone".
```

---
## \#13 Posted by: XIII Posted at: 2016-10-17T19:11:29.232Z Reads: 40

```
I have the exactly the same thing happening too me with my NYko KAMA, on high load the torque stutters. 

My receivre was placed just behind the Caps and still this problem occured. 
i'm running a 10s battery with max amp motor 60A and max battery is 20A 

I saw somoene using aluminium foil and apply it around the entire vesc and phase wires to avoid EMI. 
His problem was completely solved!! 
Make sure if you try this to have sufficient heatshring between your aluminium and vesc to not have shorts! 

I'm gonna try this in the weekend!
```

---
## \#14 Posted by: Goombaacez84 Posted at: 2016-10-17T19:15:57.081Z Reads: 40

```
Is this the thread that you're referring to? 

http://www.electric-skateboard.builders/t/fiona-vanguard-3-3d-print-pulley-sk3-245kv-vesc-vac-enclosure/11251/5

If so, I think a clarification from @whatthejess used might be needed. We discussed EMI shielding tape by 3M in that thread and they also mentioned they had aluminum tape on hand as well. I would imagine that aluminum is too permeable, but I don't want to rule it out if that's what was used in the thread. Needless to say, I'm going to give the EMI shielding tape a shot as well when my VESC comes back.
```

---
## \#15 Posted by: XIII Posted at: 2016-10-17T19:21:59.410Z Reads: 39

```
I couldn't find this thread anymore ! THANKS ! 

Mine is soldered on , this should be the other problem with nyko kama. But since I don't have this, it can only be EMI

Or maybe a bad potentiometer? but this seems strange because braking works like a charm
```

---
## \#16 Posted by: petter Posted at: 2017-04-21T09:33:39.995Z Reads: 20

```
pot would be unlikely, at least if you board works on the bench :) i switched back to my RC remote and then got a nano x... Works great so far, no cutouts.
```

---
