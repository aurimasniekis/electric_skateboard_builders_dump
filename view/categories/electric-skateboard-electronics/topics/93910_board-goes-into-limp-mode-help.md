# Board goes into &ldquo;limp mode&rdquo;. Help!

### Replies: 48 Views: 593

## \#1 Posted by: MrDGOrman Posted at: 2019-05-15T09:40:43.351Z Reads: 176

```
Hi everyone,

I've recently (about 1 month ago) upgraded my battery to a 12s6p setup. I'm still running single drive but will be upgrading to dual drive soon. I'm using the enertion focbox at the moment.

I've got everything set within the limitations of the focbox but sometimes, when I'm going up hill, the board will decide to go into some kind of limp mode. It never did this before.

I'm not entirely sure where to look. I did see that people have changed the phase wires from 14awg to 12awg but I can't imagine that would be the issue? It's an odd one for sure.

Any advice would be appreciated.

Thanks,
Dan
```

---
## \#2 Posted by: taz Posted at: 2019-05-15T09:48:18.630Z Reads: 169

```
With a single motor there is a big chance you are reaching the temperature limits on your vesc and/or motor.

What are the temperatures you are getting when this happens and what are your settings?
```

---
## \#3 Posted by: MrDGOrman Posted at: 2019-05-15T09:53:27.817Z Reads: 164

```
I thought it could be due to the temperature aswell. Sadly I can't get any data on it because for some reason my Ackmanick app doesn't work no matter that baudrate I set. The module works because I can connect to it, but the app won't give me any data :-1:

I guess it also doesn't help that I'm running 125mm wheels with 44-15t ratio!

I can't remember specifically but I think my settings are 45a batt max and 65-75a motor max
```

---
## \#4 Posted by: taz Posted at: 2019-05-15T09:55:55.632Z Reads: 153

```
I am 99% sure it is just the temperature throttling.

My board does the same with 2 x focboxes and 6374 and a lot lower gearing but I live in a very hilly area.
With one motor it would overheat in less than a minute.
```

---
## \#5 Posted by: MrDGOrman Posted at: 2019-05-15T09:58:02.346Z Reads: 148

```
So basically what you're telling me is that I should make some orders and finally get a dual system? ;)

Tbh I'm 99% sure its temperatures aswell. If I can find a cheap focbox then I'll do the conversion for sure. It's annoying because I've got a "dead" focbox spare but I don't know the first thing about trying to repair it. Or if it's even worth messing around with!
```

---
## \#6 Posted by: taz Posted at: 2019-05-15T10:01:46.340Z Reads: 137

```
[quote="MrDGOrman, post:5, topic:93910"]
finally get a dual system?
[/quote]

Yeap. However, just in case I would try and investigate the matter further (change firmware so you can see telemetry?)
```

---
## \#7 Posted by: MrDGOrman Posted at: 2019-05-15T10:04:40.609Z Reads: 130

```
I've got everything set to have PPM and UART. Is there something else I should be looking at in order to get the Bluetooth working properly?

Come to think of it, the lack of Bluetooth started when I used the new VESC Project tool to set up a new FOCBOX. It had some weird recommendations etc like 100a bat max etc so maybe the program has turned something off which is preventing the BT from working?
```

---
## \#8 Posted by: taz Posted at: 2019-05-15T10:08:37.618Z Reads: 110

```
The ackmaniac app is not compatible with the new firmware. I would use the mobile vesc tool but I am not sure it is compatible with non nrf modules
```

---
## \#9 Posted by: MrDGOrman Posted at: 2019-05-15T10:11:19.623Z Reads: 107

```
This would explain it then!

Would be interesting to know if the vesc tool works with non-nrf modules. Fairly sure it doesn't, but would be good to know
```

---
## \#10 Posted by: MrDGOrman Posted at: 2019-05-15T11:36:57.948Z Reads: 104

```
@Ackmaniac will the app be updated to work with the new firmware?
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-05-15T12:27:32.625Z Reads: 99

```
I think your focbox is overheating.

Same thing would happen on my rspec drive kit, after a while of riding (10~ minutes) stop and go, my board would go into limp mode.
```

---
## \#12 Posted by: Dirt_Bag Posted at: 2019-05-15T20:44:45.385Z Reads: 88

```
As said, its probably heat issues. When you go dual drive get the lowest kv motors you can to get your desired speed. It will help alot with heat
```

---
## \#13 Posted by: J0ker3366 Posted at: 2019-05-15T21:08:42.329Z Reads: 81

```
I just skimmed through. 

What are you upgrading from (battery wise)?
Board components?
```

---
## \#14 Posted by: Creavenger Posted at: 2019-05-15T21:18:56.408Z Reads: 83

```
Definitely the temperature, I run a single motor aswell on a steep long hill the vesc temp reaches about 80 degrees celsius (measured with metr pro) and then the boards starts to lose power.
```

---
## \#15 Posted by: maxchilton Posted at: 2019-05-16T00:51:39.253Z Reads: 72

```
[quote="MrDGOrman, post:3, topic:93910"]
I thought it could be due to the temperature aswell. Sadly I can’t get any data on it
[/quote]

Did you try touching the motor and seeing if it was hot?
```

---
## \#16 Posted by: AlanZhou Posted at: 2019-05-16T01:15:08.288Z Reads: 70

```
It's usually the vesc overheating and not the motor lol
```

---
## \#17 Posted by: myreala Posted at: 2019-05-16T01:23:38.913Z Reads: 70

```
@MrDGOrman You need a Focbox? I have a couple, can sell you one for $100
```

---
## \#18 Posted by: taz Posted at: 2019-05-16T05:07:14.386Z Reads: 65

```
How are you so sure about that?
```

---
## \#19 Posted by: Arzamenable Posted at: 2019-05-16T05:35:32.072Z Reads: 65

```
I’ve been rage posting on Instagram specifically about hot motors that put me in limp mode. 

Obvs I could change the neuter mode threshold.
```

---
## \#20 Posted by: dareno Posted at: 2019-05-16T05:45:47.347Z Reads: 65

```
[quote="AlanZhou, post:16, topic:93910, full:true"]
It’s usually the vesc overheating and not the motor lol
[/quote]

Yeah I'm quite intrigued to know why so emphatic a reply with a little ridicule chucked in there for good measure?  Please enlighten us.
```

---
## \#21 Posted by: AlanZhou Posted at: 2019-05-16T11:47:08.292Z Reads: 59

```
Both my TB vesc 4.12 and my focboxes overheated before my raptor hubs got warm (the focbox did better), the vesc is usually the bottleneck in most cases.


Both the focboxs and tb vesc 4.12 we're 70c at the Lowest....

My settings we're (30 Batt, 60A motor, -10 Batt, -30 Motor)

And 80+ when riding, the fets just can't handle the current without sufficient cool, I'm betting if I had mounted the vesc outside of my enclosure I wouldn't have the throttleing issue.

I tried Foc sensored and foc unsensored both had the same efficient, I think this proves that it wasn't the hubs overheating.
```

---
## \#22 Posted by: Sn4pz Posted at: 2019-05-16T12:10:36.446Z Reads: 54

```
[quote="AlanZhou, post:21, topic:93910"]
Both my TB vesc 4.12 and my focboxes overheated ***before my raptor hubs got warm***
[/quote]

You sure? :thinking: 😂

I agree with the TB4.12 getting stupid hot in very little time though. My mad hubs (130kv ) would be sitting at around 50c by the time my mosfets hit 90c
```

---
## \#23 Posted by: AlanZhou Posted at: 2019-05-16T12:11:19.465Z Reads: 54

```
I could touch the hubs without ever removing my hands, it felt like lukewarm water.
```

---
## \#24 Posted by: Sn4pz Posted at: 2019-05-16T12:13:24.661Z Reads: 55

```
What the f 😂

Not saying you're wrong, but I thought you ride fast? I'm sure Sean and all the other raptor owners do as well, but why wouldn't your motors heat up while theirs are dying of heatstroke 🤔
```

---
## \#25 Posted by: taz Posted at: 2019-05-16T12:17:05.339Z Reads: 51

```
[quote="AlanZhou, post:21, topic:93910"]
the vesc is the bottleneck in my case.
[/quote]

Fixed it for you.

Just because in your experience it is the vesc that is overheating first that in no way applies to "most" cases.
Your experience relies on one type of motor (raptor hubs), in your type of terrain (?) for your way of riding (?) your settings (30 Batt, 60A motor, -10 Batt, -30 Motor) and your body weight (yesterday's lunch).

So it would be good to rephrase your statement and not generalize with such a small sample.

FWIW I have had both the motors and vescs overheat on various setups. Depending on the way you ride the vesc or motor can overheat first even on the same board.
```

---
## \#26 Posted by: AlanZhou Posted at: 2019-05-16T12:18:45.804Z Reads: 54

```
[quote="taz, post:25, topic:93910"]
(raptor hubs), in your type of terrain (?) for your way of riding (?) your settings (30 Batt, 60A motor, -10 Batt, -30 Motor) and your body weight (yesterday’s lunch)
[/quote]

Was doing max speed tests so stop and go, I weigh 115 and managed to overheat

I noticed it if  I do normal riding it overheats less.

Also noticed overheating on a raptor 2
```

---
## \#27 Posted by: AlanZhou Posted at: 2019-05-16T12:25:37.577Z Reads: 54

```
My TB 4.12 was also overheating on my dual 6374 setup when I had them.

Can't remember if I had overheating on my 6355 setup that I had
```

---
## \#28 Posted by: taz Posted at: 2019-05-16T12:33:23.970Z Reads: 53

```
My dual 6374 SK8's overheat when my vesc 6 don't even exceed 45C .

Therefore in most cases it is the motors that are overheating.:roll_eyes:
```

---
## \#29 Posted by: AlanZhou Posted at: 2019-05-16T12:36:12.354Z Reads: 51

```
We'll vesc 6 has a beefed up heatsink... 🤣
```

---
## \#30 Posted by: AlanZhou Posted at: 2019-05-16T12:38:44.664Z Reads: 49

```
[quote="taz, post:28, topic:93910"]
6374 SK8’s
[/quote]

Also sk8's are known to overheat.
```

---
## \#31 Posted by: taz Posted at: 2019-05-16T12:39:29.441Z Reads: 46

```
I am going to be blunt.

You are either thick or trolling. Whatever the case, I am done answering to you.
```

---
## \#32 Posted by: AlanZhou Posted at: 2019-05-16T12:45:30.524Z Reads: 47

```
Alright that last comment was trolling 🤣 but other then that I agree with you that it depends on the case.
```

---
## \#33 Posted by: briman05 Posted at: 2019-05-16T12:46:00.224Z Reads: 47

```
It is several things.  First it is the simple fact that you are going up a hill with a single drive.  Depending on your motor it might be too steep for it to handle. Dual drive will immediately make a difference as your motors will run cooler because it isn't having to work as hard to power itself up a hill.  It could also be the kv on the motor is to high and you do not have enough torques in the motor to power you up the hill.
```

---
## \#34 Posted by: Jinra Posted at: 2019-05-16T13:59:55.253Z Reads: 48

```
Fwiw i had an Olllin vesc and at the time a single 5065 in 2.25:1 gearing. The motor got insanely hot (no motor temp sensor) and i never got performance throttle. I burned my hand touching the motor for a sec
```

---
## \#35 Posted by: murloc992 Posted at: 2019-05-16T14:55:52.903Z Reads: 48

```
@MrDGOrman

Check your focbox for this classic move:

![15|690x388](upload://pQQGu1iqLCF8vHEdQcwt9Alk8CQ.jpeg) 

This film shouldn't be on your focbox thermal pad. Kind of beats the purpose of the heat transfer pad beneath it.
```

---
## \#36 Posted by: Jinra Posted at: 2019-05-16T16:57:21.199Z Reads: 45

```
The amount of times I've seen that on prebuilt PC's lol
```

---
## \#37 Posted by: murloc992 Posted at: 2019-05-16T17:14:56.730Z Reads: 44

```
I was surprised when I decided to clean used focbox I purchased and found this. Prebuilt and beginner DIY CPU cooler vibes..
```

---
## \#38 Posted by: MrDGOrman Posted at: 2019-05-16T21:15:17.215Z Reads: 43

```
Okay so this is what I've gathered from everyones comments:

It could be the motor, it could be the vesc. It's not possible to tell without realtime data. Going dual will make a difference as the load is shared. I could potentially have the bat/motor max levels too high for a single drive. My gear ratio could be the cause of the problem because this never happened with my old lipo setup that used a 15-36 ratio.

In short - fix the Bluetooth (@Ackmaniac???) and do some testing.

Also, @murloc992, it wouldn't be that because I've moved the speed controller from the standard heat sink to a 3dservisas dual one. The thermal pad is there, although I might replace it to see if that helps keep that area cool.  

Cheers everyone. Much appreciated :slight_smile:
```

---
## \#39 Posted by: lrdesigns Posted at: 2019-05-17T02:48:33.766Z Reads: 38

```
If your motor does not have temperature sensors built in then the hot motor limp mode can not be activated by the vesc. But it can still get hot it just won't slow you down till it has full melt down. So you can eliminate that depending on which motor you have. Not many have temp sensors. 

When I have an issue with my dual setup that puts me on a single motor, there is hill on my way home and the vesc will always go into low power about half way up the hill. 

You could try a high gear ratio (lower top speed) this should put less load through the system, or limit amps in the vesc.
```

---
## \#40 Posted by: MrDGOrman Posted at: 2019-05-17T09:29:49.354Z Reads: 36

```
I use the eskating 6374 motor which is sensored.

https://eskating.eu/product/eskating-pro-motors-6374-190kv-waterproof-sealed-and-sensored/?v=7516fd43adaa

I'm going to order the VESC Project Bluetooth module now.
```

---
## \#41 Posted by: lrdesigns Posted at: 2019-05-17T12:49:48.060Z Reads: 32

```
Sensored usually means only angle sensor. Not temperature sensor, it would mention that if it was a feature.
```

---
## \#42 Posted by: taz Posted at: 2019-05-17T12:56:43.790Z Reads: 31

```
The eskating (maytech) motors also have a temperature sensor.
```

---
## \#43 Posted by: lrdesigns Posted at: 2019-05-17T13:00:08.607Z Reads: 31

```
Really? That’s nice then. 

Well you can check the can with your hand and see how hot it is when it goes into protection mode. If it’s not too hot that you can keep you hand on there for a while you could turn up the protection temp in vesc tool. Sometimes the reported temp can be 20c off the actual temp and needs some calibration.
```

---
## \#44 Posted by: MrDGOrman Posted at: 2019-05-17T13:34:32.358Z Reads: 29

```
I've made an order for a second motor mount to go dual and the Bluetooth module from trampa. Hopefully that'll give me some insight.

Either way, dual is on the way so that's bound to help!
```

---
## \#46 Posted by: taz Posted at: 2019-05-17T13:45:08.829Z Reads: 29

```
Not in my experience. As soon as the temperature of the motors exceeds the one set with the vesc tool, the power is slowly reduced by the vesc.

The vesc tool nowadays not only monitors motor temperature, there is also a feature that allows for power reduction at a lower temperature between acceleration and braking. That way you don't end up without brakes at the top of a hill before going down.

@deckoz  You have been out of the game too long Brad. Time to update your focboxes :wink:
```

---
## \#48 Posted by: taz Posted at: 2019-05-17T13:55:39.103Z Reads: 27

```
![03|690x388](upload://xByT54CcxPiCXQJ4jzyidkz6WZ0.png) 

On some of my boards the vescs overheat first and on some others the motors.\
On my Trampa with VESC6 the motors always overheat before the vescs. This is not motor specific since I had Trampa 6364, Maytech 6374 and now sk8 6374 motors on it.

Do the update, a lot has changed for the better.
```

---
## \#49 Posted by: Keevaan Posted at: 2019-05-17T14:02:40.645Z Reads: 27

```
I’m also going into limp mode, due to motor temps.
What is the solution to this?
```

---
## \#50 Posted by: Sender Posted at: 2019-05-17T14:57:03.055Z Reads: 26

```
Absolutely makes a huge difference! I have done it on all my  builds since as well and have had no overheating issues even in the Alabama heat!
```

---
