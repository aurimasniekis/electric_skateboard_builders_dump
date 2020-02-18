# Good initial VESC settings for a heavy middle aged newb ;)

### Replies: 15 Views: 572

## \#1 Posted by: loiphin Posted at: 2018-06-07T20:45:54.581Z Reads: 121

```
Hey guys,

So my stats and my planned build:

Age: 43
Weight: 102kg
Experience: Skated around 30 years ago, and could do basic shit like ollies. First time on a longboard though. Have been a snowboarder for many years, but not sure if that helps? Again, I am just average on a snowboard.

Planned Build: Dual 6374 (190kv, 80A, 3150 Watts) motors, 15mm belts, 97mm wheels and 12s4p (Torque Boards) on a LY Switchblade 38.
VESC: 4.12 hw
Battery: 12s4p Samsung 30Q's with 530Wh of juice
Speed: Calculates to around 65km/h.
Use: Plan to use as mostly a commuting to bus stations, and maybe some long distance adventures.

I am no newb in electronics/software/hardware development though. I have built quite a few arduino projects, had RC helicopters for many years, robotics, 3D printers, Raspberry Pi's, hacking consoles, PC's/Macs/linux for 30 years blah blah. So no need to spoon feed me on the technical details.

I realise it's a crazy build for a newbie, but considering the import costs to Europe, I figured I will go all out and then at least I have some redundancy in case a component fails or is DOA, and I can run a single motor. I want something that wont strain up hills and burn out. 

In Norway the legal speed limit is 20km/h on a esk8. So I will probably start with an ERPM of 20000 initially. Right? I am scared shitless of going too fast in the beginning. 

While I wait for my gear to arrive, I am practising on my Switchblade, but I still have a lot to learn. 

So I am looking for medium acceleration and braking. I am a heavy guy and need some power going up hills, but also want decent stopping power. 

What settings would you recommend in the VESC's for me to start out on? Firmware variants? Hybrid mode with hall sensors attached?

I also dont want some crazy hair trigger on that nano controller. Would prefer some curves so it wont toss me off.

Thanks in advance :slight_smile:

loiphin.
```

---
## \#2 Posted by: BoostedBuilder Posted at: 2018-06-07T20:55:51.126Z Reads: 108

```
[quote="loiphin, post:1, topic:58173"]
Age: 43
[/quote]

Love this stat!! Welcome : )
```

---
## \#3 Posted by: loiphin Posted at: 2018-06-07T20:56:46.936Z Reads: 104

```
Heheh, it must be mid-life crisis. I am getting hairy eyeballs from neighbours when I am on my longboard.
```

---
## \#4 Posted by: pat.speed Posted at: 2018-06-07T20:59:42.681Z Reads: 101

```
Ok so just a tip 20,000 erpm is not 20km/h. You must work it out for your setup, erpm is the rpm of your motor x 7 (pole pair of the motor). The easiest way to do this without all the math is to go to the calc.esk8 or whatever it’s called and enter in all of your variables and see what your max speed is and max erpm. Then divide erpm by speed to get your erpm per km/h then times it by whatever speed you want, so 20 in your case. 


As for amps I would set it to batt max 25, battery min -6, motor max 40, motor min -40. These values can be increased or decreased depending on how you feel riding it. Hint: Motor amps basically means more torque
```

---
## \#5 Posted by: loiphin Posted at: 2018-06-07T21:04:21.332Z Reads: 99

```
190kv x 44v x 7pole pairs = 58520 ERPM at max speed. Around 65km/h calculated with 97mm wheels.

So 20000 ERPM is close enough for me to get around 20km/h.
```

---
## \#6 Posted by: pat.speed Posted at: 2018-06-07T21:07:27.499Z Reads: 95

```
Haha sorry mate I didn’t know you had already calculated it, for some reason I though that you thought the number in front was the speed.

Anyway I re-read the top post and I would up the batt amps from 25 to 30 as you said you were on the heavy side
```

---
## \#7 Posted by: loiphin Posted at: 2018-06-07T21:22:18.052Z Reads: 88

```
Thanks pat.speed. But was wondering why you allow the motors 40A, but limit the battery to 30A? Could you just limit the motors to 30A instead?
```

---
## \#8 Posted by: wafflejock Posted at: 2018-06-07T21:48:54.872Z Reads: 91

```
You could but basically the battery amps settings are to protect the battery whereas the motor max amps are meant for adjusting your torque (harder/softer braking/acceleration).  There can be a difference is the VESC has capacitors on it so it can dump charge out of those quicker than it is getting power from the battery (instantaneously, but not continuously).  Pretty sure this is how it works but can see from some stats from the metr module difference in motor amps vs battery amps instantaneously: https://metr.at/r/hmtOO
```

---
## \#9 Posted by: Mathias Posted at: 2018-06-07T21:49:02.218Z Reads: 92

```
At first on my board I just went with the max specs of all components and that was a scary thing to step on as a noob and it almost threw me off a few times. The two things that did the trick for me were reducing motor amps, and finding a good positive/negative ramping time for the PPM. 

Like @pat.speed said, the motor amps limit the torque, which means the force that you feel under your feet. 
Second thing is ramping time for the PPM. I found the default values 0.9 s for positive and 0.3 seconds for negative really weird. This almost threw me off a couple of times in the beginning when I let go of the trigger too fast while accelerating hard. I found 0.6/0.6 s felt much more natural, and much less twitchy under my feet. You'll need to try what fits you well here. 

As for hall sensors: if you have them, use them. But they only matter for take-off from stand-still, which is smoother with sensors. After you reach something like walking speed the VESC switches to sensorless mode anyway. Typical beginners mistake: if you use BLDC mode with sensors, you should select "hybrid mode" not "sensored mode". 

I wouldn't worry too much about limiting the ERPM. It won't just "happen" to you that you stand on your board, cruising at 10 km/h, pull the trigger too hard, and wooops you're going 60! As long as you have a good control over the torque, and a good feeling for your trigger, the control of the speed comes quite naturally even for a beginner, I would say. 

[quote="loiphin, post:7, topic:58173, full:true"]
Thanks pat.speed. But was wondering why you allow the motors 40A, but limit the battery to 30A? Could you just limit the motors to 30A instead?
[/quote]
The motor amps and battery amps have a different meaning. Battery amps limits the total power, motor amps the max torque. So at low speeds you can have high torque with little power, and at high speeds you need high power to get decent torque. You don't really "feel" a too high battery limit, because what you feel is the torque. 

This is why I'm not a big fan of limiting the battery min to small values. I mean this won't matter so much at low speeds. This only limits the braking power. But if you eventually DO go to higher speeds, or you want to brake going a steep downhill street, you want your brakes to get to the full torque that you set with the motor min. Battery min is nothing that will throw you off when you set it too high if you set a decent motor min.
```

---
## \#10 Posted by: shrimpwhisperer Posted at: 2018-07-01T22:58:27.462Z Reads: 57

```
wow i just read you post and im thinking i knew what to do about my build however hearing that hall sensors play a factor in smoothness on start and breaking so i should run in foc mode on my vescs and use a sensor wire and then config the motors 2 6374  190kv 12s3p battery from torqueboards
```

---
## \#11 Posted by: Sn4pz Posted at: 2018-07-02T00:23:46.487Z Reads: 50

```
depends on your esc, foc could pose a problem unless youve got a premium vesc
```

---
## \#12 Posted by: shrimpwhisperer Posted at: 2018-07-02T00:30:58.701Z Reads: 49

```
are the vescs from torqueboards -  premium ? and is foc a mode in the vesc like bldc is ? im really trying to figure this out !
```

---
## \#13 Posted by: Sn4pz Posted at: 2018-07-02T00:56:18.061Z Reads: 53

```
theyre middle ground as far as vescs go, above that would be the focbox and then above the focbox I would guess only the 6.XX that benjamin and Trampa have going

foc is indeed a mode just like bldc :)

personally I wouldnt use foc on a toruqeboards vesc, there have been alot of people who have had their vesc malfunction because of it ( although i seem to be an exception? MY tb vescs have been golden, except** in the heat department)
```

---
## \#14 Posted by: shrimpwhisperer Posted at: 2018-07-02T01:31:24.824Z Reads: 50

```
focbox is by enertion right? and that lets me run sensored so if i did 2 torqueboards 6374 190kv motors would i need to plug the focbox into a pc and configure it "is that a thing with focbox?",and if thats the case how does one put two motors together master and slave i know you cut the voltage in half when you run two and have a can bus connector and then do i need a sensor plug for the focbox to the motors for the sensor or is that built in ?
```

---
## \#15 Posted by: Sn4pz Posted at: 2018-07-02T01:53:31.742Z Reads: 46

```
so 

enertion does make the focbox, correct :) 

all vescs come with a sensor plug ( any decent ones, anyways) 

all vescs are configurable via usb and should be adjusted to whatever your paramenters are so both you can the electronics can stay safe

as for connecting the two, theres a debate between split ppm and canbus which can be found here( https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461)

for master and slave youve just gotta set the vescs to numbers 1 and 0, and make vesc number 1 forward its "stuff" (data?) over canbus

please make sure that when you connect your stuff ( if you do go the canbus route, that you have both vescs plugged in at the same time or else one will fail)

edit sorry to jack ur thread @op :) 

ill move this to pm if there are any more questions
```

---
