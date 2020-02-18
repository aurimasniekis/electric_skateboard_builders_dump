# Motors do weird things, I don&rsquo;t know why

### Replies: 5 Views: 468

## \#1 Posted by: Filip Posted at: 2017-06-25T19:15:54.435Z Reads: 108

```
I bought maytech hub motors (http://alienpowersystem.com/shop/brushless-motors/63mm/sensored-hub-brushless-motor-for-longboard-maytech/) and plug them to twin ESC (http://alienpowersystem.com/shop/esc/alien-150a-2-12s-car-esc-hv-twin-2/) and as power source I used 2 turnigy LiPo 3S 5000mAh batteries. When I try to start motors they sometimes start both, sometimes only one, sometimes both start and one turns off after getting some speed. I'm not sure If it's because of low voltage (6s is minimum according to specs, 12s is max.), damaged cables or maybe something else.
I'll try to record how motors work and I'll add link to video in comment (already tried to do it but motors decided to work well this time)
I'll be greatful for help :)
```

---
## \#2 Posted by: mwkeefer Posted at: 2017-06-25T20:01:04.745Z Reads: 95

```
Filip,

I'm sorry to be the one to explain this to you but I believe your gear is all working "As Designed" by the manufacturer but you may want to consider replacing your ESC.

The ESC you have from APS (I did go double check) is not a sensored ESC which means it's starting up in senseless mode, almost nothing can startup from a dead stop loaded in senseless mode without being very choppy or having a hardware slipper clutch like an RC Car.

The hub motors are sensored and very low kV specifically to enable startup from dead stop condition and have sufficient torque to get up to speed.

As an aside, the ESC your using is really just 2 ESCs which do not speak to each other and only receive a common throttle signal (PPM input), each motor needs to be configured separately and having a wealth of experience with "hub" motors, I can tell ya you likely have your timing set wrong unless you set it up specifically for these hub motors?

If you kick before applying power it should start smoothly but then you run into your 6S problem... those are 95mm skins on the hub motors I believe ?  So 95mm is 3.74" and the hub motors have a no-load kV (I emailed maytech) of 60 RPM per volt.  Now these can't be more than 85% efficient (I'm being kind) so the loaded kV will be 60 * .85 = 51 RPM per volt.  At 22.2v * 51 RPM = 1132.2 RPM at wheel / 336 = 3.36964 * 3.74" = 12.60 MPH maximum speed.

To be honest this motor issue could be caused by too long of runs and muddy BEMF which is required for senseless commutation but I think it's more likely a non-issue.

Going to 12S would likely get you into the 24/25 mph range but your never going faster unless you switch to UHV RC controllers (uber expensive) or HV eBike Controllers (6FET Infineon isn't bad, check Ed Lyen on Endless-Sphere) which are dirt cheap compared.

Sorry if this isn't what you wanted to hear and yep ill check the video out but it seems a bit more homework is needed.

Hope it helps!

-Mike
```

---
## \#3 Posted by: Filip Posted at: 2017-06-26T08:20:51.008Z Reads: 59

```
ok, I think I understand, can I exchage Twin ESC to Twin ESC sensored from APS? Will it solve the problem?
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-06-26T12:58:49.806Z Reads: 48

```
All your problem are normal since you run your setup as sensorless... Don't worry it would work just fine but you might need to give your board a little push when you start.
```

---
## \#5 Posted by: mwkeefer Posted at: 2017-06-27T01:02:50.340Z Reads: 32

```
 Yep you can either leave it the way it is and get used to pushing it to start and having someone you know non-standard or non-consistent performance between the wheels you can upgrade to censor this and get it pretty much instant start from a standstill and some better features you can of your battery pair power in order to avoid the issue that you're running into where your top speed is severely limited 

 Or as the previous poster says you can just leave it the way it is and use it, but yeah I think if you were to order the alien power system sensor controllers that would help honestly though I would pick up a pair of asks the ESC's from one of the $100-$120 order you know pricers not the Olen boards for 240 but I get a pair of them because they're much more adaptable and programmable and Set up correctly they seem to run really really well

Hope that helps

– Mike
```

---
