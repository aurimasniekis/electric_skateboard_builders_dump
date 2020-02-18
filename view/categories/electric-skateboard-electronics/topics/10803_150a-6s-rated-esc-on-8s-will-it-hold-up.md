# 150A 6s rated esc on 8S? Will it hold up?

### Replies: 30 Views: 4475

## \#1 Posted by: Jakebarnhill1 Posted at: 2016-10-08T01:56:16.681Z Reads: 226

```
Hi, I've recently finished my 2nd build with a mono drive enertion 6355 motor and i am using a 6s 150A esc, on 6s it is not fast enough around 28kp/h. I will be upgrading to 12S dual drive in the near future but until I get enough money I am stuck with this setup. I thought to give me more speed I could run it on 8s instead of 6s, which i have done once to test for 5 minutes it was wayyy faster. the esc was luke warm after the 8s test. I don't know how well the esc will stand up to the additional voltage what do you guys think?

This is the esc I'm using: http://www.hobbyking.com/hobbyking/store/__77221__RotorStar_150A_2_6S_SBEC_Brushless_Speed_Controller_AU_Warehouse_.html?strSearch=rotorstar%20150
```

---
## \#2 Posted by: rpn314 Posted at: 2016-10-08T02:05:44.006Z Reads: 218

```
If it is rated for 6s (which it looks like it is) I wouldn't go higher than that. So no go for 8s in my book. Sorry
```

---
## \#3 Posted by: Jakebarnhill1 Posted at: 2016-10-08T02:16:37.956Z Reads: 213

```
I am aware that it is rated for 6s, i was just wondering if it could handle 8s pushing it, and if anyone else had done something similar
```

---
## \#4 Posted by: Genex Posted at: 2016-10-08T02:53:30.857Z Reads: 207

```
Some people say the components of the esc's will not be able to handle it.  At the same time, I don't think anyone has ever tried it.  Most engineers make components bulkier than they need to be to hang surges and what not.  8s is roughly 8.4 more volts, which may or may not be a big deal. 

Test it for science, and get back to us :stuck_out_tongue:

I would make an assumption and say that it won't work or it will overload the components, but you never know.
```

---
## \#5 Posted by: arfintr Posted at: 2016-10-08T03:41:59.521Z Reads: 192

```
I've run a YEP 150A 6s esc on as much as 8s with no issues, I used the programming card to input the settings for 8s which isn't supposed to work, but I am guessing the esc is loaded with the same stuff as their higher range of 12s esc. I overloaded the esc in my rookie days going up a steep hill at low throttle, putting the esc on extreme load for too long and it went kaput. HK replaced mine for free and I am waiting to get new batteries so I can run faster and longer.
```

---
## \#6 Posted by: Jakebarnhill1 Posted at: 2016-10-08T07:57:45.504Z Reads: 180

```
Thats good to hear! @Genex @arfintr I will run it on 8S and keep you posted on how it goes. The main component that will be stresses out is the 5V Bec so I might have to sort out an external BEC if the onboard one fails, hopefully if it fails it won't feed the receiver with more than 5V.
```

---
## \#7 Posted by: lowGuido Posted at: 2016-10-08T08:31:53.439Z Reads: 168

```
it depends on if your ESC has a high voltage cutoff.
I know a lot of my older ESC had a high voltage cut off at ~25V so a full charged 6S at 25.2V would just manage to tip the cutoff sending it into limp mode.
if there is no high voltage cutoff then it might work. especially if it has the same firmware as the other models.
```

---
## \#8 Posted by: Jakebarnhill1 Posted at: 2016-10-08T08:36:38.408Z Reads: 165

```
@lowGuido I have done a 5min ride on 8S so it definitely has no high voltage cutoff. The esc was in a sealed container during the test and was barely warm. I should probably mount it in the airflow so it has ample cooling. But apart from that I guess that the only thing will be how long it will last on 8S, I will do a big ride tomorrow to test it out and will keep you posted on how it goes. 8S is much faster than 6S :slight_smile:
```

---
## \#9 Posted by: Maxid Posted at: 2016-10-08T08:53:00.098Z Reads: 160

```
I have a HK 150A ESC and would like to try it with a 8S Lifepo (so full charge means 28.8V). Any idea if that could work? What brand is your 6S ESC?

Edit: nevermind I found your link. Well I have a HK Beast Car Esc - not sure if I am bold enough to try.
```

---
## \#10 Posted by: Jakebarnhill1 Posted at: 2016-10-08T09:25:47.129Z Reads: 156

```
An 8S Lifepo battery is less voltage than an 8S Lipo battery. It is only 3V more than your ESC max voltage according to the manufacturer so it should have no problem. If your ESC has a high voltage cut off it may not work but not many ESC's have it. Still no guarantees.
```

---
## \#11 Posted by: Genex Posted at: 2016-10-08T18:36:20.165Z Reads: 140

```
I have the 120A beast esc too, and tbh I wouldn't try it.  I notice mine gets warm after a series of roughly 40% braking sessions and I wouldn't want to overload it anymore.  (I'm on 6s)

Idk about you but I'm pretty disappointed in the performance of my esc.  I feel like I got a low-quality one, since I have always had problems with top speed. Running 6s on a 3:2 ratio gets me somewhere are 16 mph.  Seems weak to me.

Im switching to a vesc in the spring anyway though.
```

---
## \#12 Posted by: Jakebarnhill1 Posted at: 2016-10-08T20:38:14.012Z Reads: 128

```
@Genex my 6s ESC which is different than yours gives me a top speed of around 17mph so i don't think there is anything wrong with yours.
```

---
## \#13 Posted by: Genex Posted at: 2016-10-08T20:49:55.071Z Reads: 120

```
What is your gear ratio?

I am running a 20T motor pulley to a 32T Wheel pulley.  Almost 2:3, which is insanely close to 1:1 for a 230kv motor...
```

---
## \#14 Posted by: Jakebarnhill1 Posted at: 2016-10-08T20:53:56.130Z Reads: 113

```
Mine is 15 tooth motor pulley and 36 tooth wheel pulley, Yeah i think yours is a bit underpowered! How does it do on hill climbing? maybe the gearing is to high making the motor struggle but that is probably not the case.
```

---
## \#15 Posted by: Namasaki Posted at: 2016-10-08T22:24:03.800Z Reads: 105

```
Try to pull the shrink wrap back enough to see the voltage rating on the capacitors. That will give you a better idea.
I Would say go for it. Just keep an eye on the heat and you might want to run an inline fuse from the battery incase the Esc burns down and shorts out. Don't want it to take your battery out.
```

---
## \#16 Posted by: Jakebarnhill1 Posted at: 2016-10-09T02:50:02.263Z Reads: 109

```
Thanks for the input everyone! I went for a 10km ride on 8s this morning and it was awesome! The ESC seems to be holding up ok, it is warmer than 6s but not hot. No magic smoke yet :smile:
```

---
## \#17 Posted by: im-done Posted at: 2016-10-09T03:53:51.334Z Reads: 112

```
I had a hobbyking 80 amp esc that was rated for 4s and i thought it was rated for 6s because their paper work sucks. I ran it on 6s its whole life. The esc probably would of lasted longer but it did die in about 1 year of low use.
```

---
## \#18 Posted by: Maxid Posted at: 2016-10-09T13:01:02.847Z Reads: 111

```
I tried it as well - for science. Hooked up the 8S Lifepo (at 8*3.5V=28V) and connected the GT2B.
At first everything seems normal (the beeps count to 6S) and I can control the full throttle range. After a couple of bursts to top speed without load, the ESC starts blinking red. According to the manual this is the signal for low battery voltage ([link to manual](http://www.hobbyking.com/hobbyking/store/uploads/264719761X1465900X55.pdf)). The ESC then only allows for very little top speed as it is in low voltage mode. Not sure why it does that. My cut off is set to 21.6 (3.6V per Lipo cell) so should not be triggered with the 8S battery. 
Disappointed :cry:
```

---
## \#19 Posted by: lowGuido Posted at: 2016-10-09T17:34:16.090Z Reads: 106

```
that sounds like what mine does for over volt.
```

---
## \#20 Posted by: oren Posted at: 2017-03-08T04:27:19.705Z Reads: 89

```
Thanks for posting this @Jakebarnhill1. I'm researching my first build and just saw this post. Now that it's about 5 months later are you still using the 6s ESC with an 8s battery? I'm curious if it was able to last.
```

---
## \#21 Posted by: Jakebarnhill1 Posted at: 2017-03-09T00:41:56.280Z Reads: 84

```
@oren , unfortunately it didn't last that long on 8s, I probably got about 2 hours out of it. I am now using the yep 120a HV ESC on 12cells, it is great because the active freewheeling enable the esc to generate less heat at partial throttle, which makes it efficient to run it on 12S, compared to other hobby esc's. The only bad thing on the yep esc is the brake, which is very hard.and the variable brake is to soft.
```

---
## \#22 Posted by: oren Posted at: 2017-03-09T08:18:16.482Z Reads: 79

```
@Jakebarnhill1, thanks for the followup! It was tempting to try because the 6s ESCs are usually much cheaper than HV. The price especially adds up when buying 2 of them for dual hub motors. Now I know it's not a good idea.

The YEP 120A HV sounds like a good option. I actually just ordered a pair of VESCs from a company called Maytech through AliExpress. They're kind of expensive (I paid $110 USD each) but everyone seems very happy with VESCs. The braking was one of the main reasons I'm trying VESC. I bought them with a pair of 70mm hub motors for a shortboard I'm building. This is going to be my first build so I'll find out soon how well they work.
```

---
## \#23 Posted by: marcoramires Posted at: 2017-04-10T10:20:54.505Z Reads: 66

```
Curiosity here. Which remote control are you using? I have the same ESC and I can't get any binding or throttle with a few different remotes. However, it connects and works fine when using a servo tester.

Cheers Marco
mcoboards.com
```

---
## \#24 Posted by: Jakebarnhill1 Posted at: 2017-04-10T10:57:02.813Z Reads: 65

```
I'm using the gt2b. Make sure throttle isn't reversed on the remotes your using. And also if the reciever isn't bound to the radio it won't work. Once you know the reciever is bound to the remote (the red light will be solid on) try reversing the throttle channel if it doesn't work when it isn't reversed. 

Good luck
```

---
## \#25 Posted by: bartroosen12 Posted at: 2017-04-10T12:38:41.130Z Reads: 63

```
Hi man,
Are you sure about that 16 mph? I have also had the boat esc, very bad braking but the speed was pretty stable, max speed was around 24 mph.
It's very strange if you have 230Kv on 6S with 32T and 20T pulley you can only go 16mph...
If you have a wheel diameter of 70mm the max speed MUST be around 21mph.
If you have a larger diameter, the max speed would always be higher so...
```

---
## \#26 Posted by: marcoramires Posted at: 2017-04-11T00:27:32.696Z Reads: 61

```
Thanks mate. I will give it a go with the gt2b ;)
```

---
## \#27 Posted by: marcoramires Posted at: 2017-05-09T23:23:18.870Z Reads: 57

```
Hey man,

I am trying to setup the esc using the gt2b and there is no confirmation beep from the esc. Both transmitter and receiver are bound correctly. I made a video showing what's happening... Would you be able to tell if I am doing anything wrong please?

[https://www.youtube.com/watch?v=t6_Pw7QY_hA](https://www.youtube.com/watch?v=t6_Pw7QY_hA)

I got in touch to Hobbyking and that was their response:

> Alex, May 9, 21:12 HKT:
> Hello,

> The YEP 150 is not designed to be used with a car transmitter. Since the end points are not the same as a standard helicopter or airplane transmitter the ESC will not initialize.

> Regards.

> Alex
```

---
## \#28 Posted by: Jakebarnhill1 Posted at: 2017-09-10T04:40:53.473Z Reads: 36

```
Hey mate I somehow missed your notification... 


anyway did you get it working?
```

---
## \#29 Posted by: marcoramires Posted at: 2018-02-21T03:18:23.611Z Reads: 25

```
Hey mate,

I sort of parked the project for a while. I might get a new vesc this time. I tried all different controllers and none will pair with esc.

Thanks anyways!
```

---
## \#30 Posted by: Jakebarnhill1 Posted at: 2018-02-21T10:34:04.450Z Reads: 21

```
one last suggestion :) did you have the programming wire plugged into the receiver instead of the throttle wire??
```

---
