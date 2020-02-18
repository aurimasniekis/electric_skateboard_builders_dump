# 40+ MPH board running 12s setup

### Replies: 20 Views: 1211

## \#1 Posted by: kvboards Posted at: 2018-01-13T22:59:37.795Z Reads: 214

```
Ok guys I'm building this 12s setup and wondering if these apps I'm using are realistic as far as speed goes? If not what else will I need to make it work. This build should be finished by tonight and hopefully will have great results. ![Screenshot_20180113-165334|281x500](upload://fcpDF2770TqRdn1Lr54vUG3lHc1.png)![20180113_164732|666x500](upload://t0MjMb4KdEy4m5jjORstTv8Gyd8.jpg)![20180113_164712|666x500](upload://uTI6izvins4SQbacWmhQWqt90S6.jpg)![20180113_164758|666x500](upload://ykeB07YuIv8Ag3efOiZXd6WuJSt.jpg)
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-01-13T23:12:32.676Z Reads: 194

```
I dont think you will be able to hit 70 km/h with only one motor. With dual it is no problem though
```

---
## \#3 Posted by: kvboards Posted at: 2018-01-13T23:20:49.771Z Reads: 193

```
I thought having dual motor only allows you to reach higher speeds quicker not to actually go faster because they are still spinning at 190 KV for the motor?? Maybe I'm confused.
```

---
## \#4 Posted by: Blitz Posted at: 2018-01-13T23:27:55.516Z Reads: 188

```
Could you hit 65kmh with this 4000w motor??

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
```

---
## \#5 Posted by: FredrikHems Posted at: 2018-01-13T23:28:53.058Z Reads: 178

```
Yea in theory Thats kind of right... But to reach 70km/h you need a hell of a lot power.. I will guess something like 4kw.. Your motor probably cant do that power countinous, so your motor wont reach it max rpm Because it is simply not strong enought. By adding a second motor, each motor will only need to do 2kw (which it probably can du countinous) and can therefore spin at a higher rpm. Resulting in an higher top speed :slight_smile:
```

---
## \#6 Posted by: rich Posted at: 2018-01-13T23:31:52.909Z Reads: 164

```
The theoretical top speed of 44mph is not weighted, so when you ride it I guess you'll reach about 35mph. If you want to go faster you have to change the gearing because with 190kv and 12s you already have 59052 ERPM
```

---
## \#7 Posted by: Blitz Posted at: 2018-01-13T23:32:30.306Z Reads: 160

```
Great thing to mention,
```

---
## \#8 Posted by: FredrikHems Posted at: 2018-01-13T23:39:38.818Z Reads: 148

```
It important to remember that even with a higher gearing it not 100% sure that you reach 70km/h.. If your gearing is too high the motor will run very ineffiency and you will waste alot of power in heat.. reulting in that the motor doesnt have the torque to hit high enought rpm... If you see it like this; 
12s 190kv 90mm wheels and 1:1 gearing.. You will now have an estimated top speed of ~130km/h. This would obviously never happen, beacause of ineffiency.. I doubt you even would have hit 25km/h
```

---
## \#9 Posted by: kvboards Posted at: 2018-01-14T03:13:53.437Z Reads: 127

```
There are many good points here. I will be working on this board through the night and hopefully we'll have it up and running by tomorrow. I'm running 2 6s 10k mah
```

---
## \#10 Posted by: E1Allen Posted at: 2018-01-14T03:26:49.928Z Reads: 122

```
Does that calculator include efficiency?

I use 83% efficiency on a dual motor setup and the results are within 1mph.

![IMG_3943|281x500](upload://qAuLNpk4KLJgAcvCTLKt0SW1HRF.PNG)

http://calc.esk8.today/advanced/
```

---
## \#11 Posted by: E1Allen Posted at: 2018-01-14T03:27:32.694Z Reads: 115

```
Your batteries probably aren't the limiting factor.  What ESC?
```

---
## \#12 Posted by: kvboards Posted at: 2018-01-14T03:39:28.681Z Reads: 114

```
This the ESC
https://kvboards.com/collections/esc-controllers/products/maytech-vesc-speed-controller-board-mtvesc50a
```

---
## \#13 Posted by: E1Allen Posted at: 2018-01-14T04:25:08.568Z Reads: 104

```
Are you using a heatsink on the vesc?
```

---
## \#14 Posted by: kvboards Posted at: 2018-01-14T04:45:32.399Z Reads: 104

```
no it has air vents 2 of them on the bottom of the case.
```

---
## \#15 Posted by: E1Allen Posted at: 2018-01-14T05:19:32.711Z Reads: 98

```
If you got one of the Bluetooth modules you could monitor all your data.  See what amps that vesc can handle before thermal limiting
```

---
## \#16 Posted by: kvboards Posted at: 2018-01-14T05:34:23.546Z Reads: 102

```
Here is what it's looking like now. The holes are done for the housing and grip is installed. It's ready for test ride tomorrow.![20180113_231247|666x500](upload://8tSxp3aHl8ZYm0kNfJASRnyMRbM.jpg)![20180113_231155|666x500](upload://ZJ415YrvKiaMizYn7yMa10jVr2.jpg)
```

---
## \#17 Posted by: Ishayc Posted at: 2018-01-14T06:34:59.319Z Reads: 89

```
Maytech vesc and a 12s battery is not a good combination.
```

---
## \#18 Posted by: evoheyax Posted at: 2018-01-14T07:03:00.720Z Reads: 84

```
Have you done any analysis to see if those vents actually do anything? I found that 2 vents plus 2 fans (one sucks, one blows) that I didn't get great ventilation still. I wouldn't rely on those vents for cooling.
```

---
## \#19 Posted by: Eboosted Posted at: 2018-01-14T08:17:14.006Z Reads: 80

```
You don't want such a high speed with only one motor, the braking is really unsafe with only one motor
```

---
## \#20 Posted by: aigenic Posted at: 2018-01-14T13:25:02.361Z Reads: 66

```
Have you ever ridden that fast on a longboard?
I higly recommend you to increase the gearing ratio and forget about oging that fast, because there are many things that might happen...

the VESC might blow up, it probably wont, but its Maytech and you neveer know what to expect from maytech VESC...
You will have almost no brakes at that speed :open_mouth:
YOu might not be able to reach that speed :O 
The motor will be extremly hot!
And most of all in that speed you can kill yourself easily, unless you are experienced longboarder...

Do you ahve safety equipment?
```

---
