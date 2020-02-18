# Battery trouble&hellip; please help!

### Replies: 29 Views: 263

## \#1 Posted by: Nicolai Posted at: 2018-09-10T20:34:03.035Z Reads: 113

```
Hey guys! 

I need to tap into the bountiful wealth of knowledge within this wonderful electric skateboard builder community for this one. I can't get my electric skateboard battery to turn on. 

Some background: I'd been happily riding my DIY esk8 (using an Enertion Space Cell Pro4, a 170kv motor, FOCBOX and GT2B controller) for a while last year until disaster struck - I went over a sidewalk while skating and the impact of the landing literally tore my truck in half. The side of the truck with my brushless out runner and wheel simply separated and got torn from the board, forcefully unplugging the phase wires from the motor and switching the board off. As I was on the cusp of a semester abroad, I thought I might as well approach the problem later. Well, now it's later and I've rebuilt everything to get my skateboard back to its former glory... except that now the battery won't turn on. 

I've attached a video detailing my problem (https://www.youtube.com/watch?v=xK1DzHaJ9m0&frags=pl%2Cwn):
- First, I thought the battery was just totally out of juice after my time spent abroad. But I just ordered a new battery charger from @JLabs and, when plugged in, my battery still won't take a charge.
- Then I thought maybe the switch was faulty. I'd already replaced the switch on the original battery, but I've ruled out the switch being the issue as the battery won't turn on even if I make contact with the two white wires going to the switch itself. 
- Now I'm thinking that it's a greater problem, like maybe the BMS was harmed during the crash, or maybe the motor being yanked out from the battery also tore out some type of solder? 

If someone out there could kindly take a look at my video and tell me what you think the problem might be, that would be hugely appreciated. Thanks in advance!!
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-10T20:49:47.926Z Reads: 96

```
The thing you don’t know what it is, is your fuse.
If you have a multimeter, take out that purple thing and measure the resistance from one leg to the other. If it’s 0ohm it’s fine.
Put it back to the holder than measure the voltage on the yellow plug. It’s the xt90 plug which gives the power to your vescs.
If it is a 10s battery pack than voltage shouldn’t be under 25v, for 12s not under 30v.
If it’s over that than it looks like your bms is broken and you need to replace it.
If it’s under than your cells probably fucked.
```

---
## \#3 Posted by: Acido Posted at: 2018-09-10T20:52:02.546Z Reads: 93

```
I didnt watch the video but make sure you open up your pack and see if all the welds still hold
if they hold and your battery works normally without the bms the bms is dead
if they do not get ta new pack or reassemble the whole pack 
How old is the pack?
```

---
## \#5 Posted by: Nicolai Posted at: 2018-09-10T20:55:44.063Z Reads: 85

```
No multimeter on hand at the moment unfortunately :/ I'll see if I can get my hands on one though.
```

---
## \#6 Posted by: Nicolai Posted at: 2018-09-10T20:56:06.937Z Reads: 79

```
I bought the pack about 2 years ago… The welds to seem to be pretty solid though. How would I go about removing the BMS?
```

---
## \#7 Posted by: Andy87 Posted at: 2018-09-10T20:58:51.561Z Reads: 77

```
Yes please. It’s the only way to make sure what’s going on with your pack.
There are cheap ones in every hobby or electric shop. Does not need to be the high end fluke...
```

---
## \#8 Posted by: Nicolai Posted at: 2018-09-10T20:59:35.493Z Reads: 74

```
Thanks a ton! I'll get on it. This is hugely helpful guys, thanks so much!
```

---
## \#9 Posted by: Acido Posted at: 2018-09-10T21:03:14.258Z Reads: 73

```
bypass it, post some pics on how it looks so we can help you but I doubt the bms is the fault here
```

---
## \#10 Posted by: Jake2k17 Posted at: 2018-09-10T21:08:31.272Z Reads: 71

```
When your truck snapped did you actually turn the board off? The phase wires disconnection would disconnect the motor but the board would remain on.
```

---
## \#11 Posted by: Nicolai Posted at: 2018-09-10T21:30:07.632Z Reads: 63

```
@Jake2k17, I did turn the board off when the truck snapped off. However, my brother just told me that while I was away, he noticed that the board was actually on for a couple days, and that he didn't think twice about it and then after a couple days it was off... weird that he didn't think to try to turn it off.

I'll get a multimeter by tomorrow and let you all know what's up.
```

---
## \#12 Posted by: Sn4pz Posted at: 2018-09-10T21:36:15.052Z Reads: 60

```
you almost certainly had the issue I did, you left it on and now the pack is flat. You can sometimes revive flat li ion batteries with trickle charge until its at a safe voltage again..... make sure you monitor everything please.
```

---
## \#13 Posted by: Nicolai Posted at: 2018-09-10T21:52:58.410Z Reads: 59

```
@Andy87, turns out my housemate has a multimeter that I borrowed. The fuse read 0.6![IMG_6051|375x500](upload://tGUkDSsFHYTMjW3McUUvddEDw8f.jpeg) 
And when I checked the voltage on the battery at the xt90 plug, I couldn't get any reading at all...
```

---
## \#14 Posted by: Nicolai Posted at: 2018-09-10T21:56:57.022Z Reads: 57

```
Is it worth trying to rebuild the battery? How can cells become "fucked"? I assume that means they're not fixable, at which point it sounds like rebuilding the battery is kind of pointless...?
```

---
## \#15 Posted by: TowerCrisis Posted at: 2018-09-10T21:58:37.746Z Reads: 59

```
The cells themselves may have been damaged from being overdischarged.

Open up the battery and measure the individual cell voltages. If they're below 2.5V you've got issues.

Make sure to probe with the multimeter at the actual cells themselves.
```

---
## \#16 Posted by: Spatt Posted at: 2018-09-10T22:14:37.400Z Reads: 49

```
You should check the voltage not on the xt90 but directly to the main positive and the main negative directly on the pack! This to exclude bms fault, actually the bms should have protected cells from discharging.
Check the voltage directly to the +and - and then if you have 0 it means for sure broken series connections
```

---
## \#17 Posted by: Jake2k17 Posted at: 2018-09-11T01:15:32.243Z Reads: 49

```
@Nicolai 

I saw this cool thing these guys did with the boosted board, it was way over discharged, and one drove a car really slow and the other held onto a rope that was attached to the car and then he towed him until the rechargeable brakes powered the board on enough to charge
```

---
## \#18 Posted by: Nicolai Posted at: 2018-09-11T02:41:43.474Z Reads: 51

```
So here are some photos of my battery. @Spatt could you please specify where I should check the voltage? 

![image|374x500](upload://ojaYT1e9nocsoelL1agfAEOzv3C.jpeg)![image|666x500](upload://jQ5nJwGK41McVlMlSUfzuZk6VBH.jpeg)![image|374x500](upload://uVrgrxxqZrRzAe75ozdZRRpbpWP.jpeg)
```

---
## \#19 Posted by: Nicolai Posted at: 2018-09-11T02:43:49.249Z Reads: 50

```
Interesting idea. I assume the board could turn on though before being pulled by the car? And wouldn’t the battery cells be able to charge up normally with the wall charger that I have? Why the need to “trickle charge”?
```

---
## \#20 Posted by: Andy87 Posted at: 2018-09-11T03:38:01.818Z Reads: 48

```
Sorry my bad..yes can be the bms don’t give you to read any voltage.
So you need to measure on the last cells of your pack. There is in the picture on the left side the big red wire and on the right the big black wire connected to the pack. Measure there the voltage.
```

---
## \#21 Posted by: Nicolai Posted at: 2018-09-11T03:42:04.329Z Reads: 45

```
Yeah I'm still getting a voltage reading of 0 when I measure there...
```

---
## \#22 Posted by: hyperIon1 Posted at: 2018-09-11T04:07:44.015Z Reads: 42

```
Do you have anything to check your meter on. 
If it’s not your meter. 
Your pack is dead
```

---
## \#23 Posted by: lrdesigns Posted at: 2018-09-11T04:21:03.918Z Reads: 42

```
Check here. 
![image|413x500](upload://puuAOBo9RnLutzZqiCXuhzb0WIj.jpg)
```

---
## \#24 Posted by: Nicolai Posted at: 2018-09-11T04:23:19.344Z Reads: 43

```
Yeah I checked there @lrdesigns... nothing. Not even an uptick at all in the voltage... Sounds like my battery might be toast...
```

---
## \#25 Posted by: lrdesigns Posted at: 2018-09-11T04:25:29.652Z Reads: 41

```
:bread: + :fire: = TOAST!
```

---
## \#26 Posted by: Nicolai Posted at: 2018-09-11T04:30:34.551Z Reads: 41

```
NOOOOOOOO!! Damn... Looks like I gotta get myself a new battery setup.
```

---
## \#27 Posted by: Andy87 Posted at: 2018-09-11T04:35:45.119Z Reads: 42

```
Yeah looks like... 😬
But, just to make sure, you set your multimeter to dc voltage not ac right?
Can you check if it’s functioning properly on a aa battery or so? Just to be sure it’s not the multimeter.

And the very last thing you could check. Is there a lose nickel strip somewhere in your pack?
From the pictures it doesn’t look like but that’s the last thing why it could be 0v
```

---
## \#28 Posted by: Nicolai Posted at: 2018-09-11T04:40:04.226Z Reads: 40

```
Yeah, my multimeter is working fine, I just checked it on a AA battery. And all the connections are still soldered on and everything too. Damn, that's a real bummer.
```

---
## \#29 Posted by: TowerCrisis Posted at: 2018-09-11T05:00:55.751Z Reads: 40

```
I wouldn't give up hope QUITE yet.

Check between these of the same color. I've color coded them.

if I'm right about how this pack is constructed then you PROBABLY should see between 6.4V to 8.4V between each spot of the same color.

I chose these because they seem like the most easily accessible to measure.

If you see 0V between ALL of them then you've got a serious problem... the cells are 100% dead if that's the case.

BUT if you see voltage between any of them then you've got hope. If three work or even one, then it's likely that you've got a break between the cells. That's fixable :smiley:

if you'd like to be more thorough, you can unplug the white plug that all the red cables lead to. Check the voltage between each pin. All pins that are directly next to eachother should read a minimum of 3.2V.

If you see voltage across some but not others then it's possible that you can repair it.

If they all read 0V then it's burnt :fire: :bread:.

![d8bf6d733cf69b755377779455b322818c6cfafb|374x500](upload://xI51N2HFq2fbinoaqmYbbIOkiXJ.jpeg)
```

---
## \#30 Posted by: Eboosted Posted at: 2018-09-11T05:12:14.921Z Reads: 36

```
That battery pack is a 10s4p, meassure the voltage of each group of 4 cells, if they all read 0 then your battery pack is toasted, but I highly doubt about that
```

---
