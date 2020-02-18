# Melbourne Riders?

### Replies: 53 Views: 656

## \#1 Posted by: Koto Posted at: 2018-10-13T23:02:31.193Z Reads: 82

```
Hi, 
I’m a Melbourne based rider that wants to find someone to help to fix up my board and go for a ride with. If you are around melbourne, pm me!
```

---
## \#2 Posted by: kalebludlow Posted at: 2018-10-13T23:05:20.240Z Reads: 82

```
Hey man! There's a few dudes in Melbourne that ride esk8, but as far as I know no one really has a DIY. There's a group of Facebook called Electric Riders Melbourne, where there are weekly group rides. I'm yet to come along to a ride but can't wait to do it once I've got my board how I want it
```

---
## \#3 Posted by: Koto Posted at: 2018-10-13T23:09:06.235Z Reads: 72

```
So you’re a melbourner yourself?
```

---
## \#4 Posted by: kalebludlow Posted at: 2018-10-13T23:30:37.961Z Reads: 66

```
Geelong, but I'm up in Melbourne a few days a week for uni
```

---
## \#5 Posted by: Koto Posted at: 2018-10-14T04:55:43.304Z Reads: 58

```
Are you a DIY guy or know much about diy esk8ing?
```

---
## \#6 Posted by: kalebludlow Posted at: 2018-10-14T10:13:23.983Z Reads: 53

```
Sure do man, any particular issue I can help with?
```

---
## \#7 Posted by: Koto Posted at: 2018-10-15T06:36:42.915Z Reads: 50

```
My vesc keeps blowing, can’t find the source of why, but the drv gets blown, just don’t have any engineering background so figuring all this stuff out Ismail tedious
```

---
## \#8 Posted by: kalebludlow Posted at: 2018-10-15T06:52:33.427Z Reads: 49

```
Alright so what are your full specs and the vesc settings?
```

---
## \#9 Posted by: Koto Posted at: 2018-10-15T09:12:13.107Z Reads: 49

```
83mm enertion power wheels

Turnigy Aerodrive SK3 - 6364-245kv Brushless Outrunner Motor

Turnigy 5000mAh 3S 25C Lipo Pack

Enertion gear and belt

36t 9mm enertion drive hub

HobbyKing® ™HK-GT2B 3CH 2.4GHz Transmitter and Receiver w/Rechargable Li-ion Battery

Diyelectricskateboard esc
```

---
## \#10 Posted by: kalebludlow Posted at: 2018-10-15T09:23:58.061Z Reads: 46

```
Wait how many batteries and what config? Like are we talking 12s? BLDC or FOC? 

Also those diyelectricskateboard ESCs are widely regarded as being hot garbage, I'd avoid
```

---
## \#11 Posted by: Koto Posted at: 2018-10-15T09:28:16.691Z Reads: 41

```
yeah i learned the hard way. 2x 6s in series. BLDC. basically followed this https://www.youtube.com/watch?v=dxDXUrk-7ek.

thanks again man for looking out for a guy.
```

---
## \#12 Posted by: kalebludlow Posted at: 2018-10-15T09:40:10.960Z Reads: 41

```
What did you have your batt max set to?
```

---
## \#13 Posted by: Koto Posted at: 2018-10-15T09:42:16.138Z Reads: 39

```
21v min 19.8v
```

---
## \#14 Posted by: kalebludlow Posted at: 2018-10-15T21:19:56.441Z Reads: 36

```
Nah man sorry I meant the amps
```

---
## \#15 Posted by: Pmac Posted at: 2018-10-16T06:24:40.440Z Reads: 34

```
You are blowing the DRV due to the max eRPM.  Max should be set to 60,000 but at your 12S voltage and motor kv they would have a eRPM of 86,000 at full charge.

I have blown 1 DRV due to this issue as I had an eRPM of 68,000.

I am also in Melbourne.  SE.  Glen Waverley are.
```

---
## \#16 Posted by: kalebludlow Posted at: 2018-10-16T06:26:56.988Z Reads: 32

```
Yeah this bloke knows what's up
```

---
## \#17 Posted by: Pmac Posted at: 2018-10-16T06:34:28.378Z Reads: 33

```
Just to clarify,  do you mean you set your battery up as 6s2p or 12s1p?

2x 6s in series means 12s1p but if you meant 2x 6s in parallel that would be 6s2p.

with 6s2p you should be no where near the eRPM limit so that wouldn't cause the issue with your DRV.
```

---
## \#18 Posted by: Koto Posted at: 2018-10-17T06:13:34.884Z Reads: 34

```
Yo if you still do this kind of stuff, could definitely use your help and meeting up would be great, thanks. And also i mean i have 2 6s batteries  connected in series. 12s 1p
```

---
## \#19 Posted by: kalebludlow Posted at: 2018-10-17T06:31:44.631Z Reads: 33

```
Yeah 245kv is way too high for 12S, I've got 190 and that would be the max when using a 4.12 vesc
```

---
## \#20 Posted by: Koto Posted at: 2018-10-17T09:54:03.648Z Reads: 32

```
so how should i fix this problem
```

---
## \#21 Posted by: kalebludlow Posted at: 2018-10-17T10:06:52.682Z Reads: 30

```
If money isn't an issue then get a Flipsky FSESC6.6
```

---
## \#22 Posted by: Koto Posted at: 2018-10-17T10:16:40.895Z Reads: 29

```
[quote="kalebludlow, post:21, topic:71139"]
If money isn’t an issue
[/quote]
 wheewwwwww i mean damn i thought i was covered but thats pretty expensive ngl, what other options do i have
```

---
## \#23 Posted by: kalebludlow Posted at: 2018-10-17T10:28:14.457Z Reads: 28

```
Either lower kV motors, lower voltage battery
```

---
## \#24 Posted by: kalebludlow Posted at: 2018-10-17T10:29:33.030Z Reads: 29

```
Also do you have a single or dual motor setup? You can get a FSESC6.6 on eBay for $200aud
```

---
## \#25 Posted by: Koto Posted at: 2018-10-17T10:57:51.485Z Reads: 28

```
hmm ok single motor
```

---
## \#26 Posted by: kalebludlow Posted at: 2018-10-17T11:09:00.744Z Reads: 26

```
Yeah my recommendation would be the FSESC 6.6 then especially cos it will work without issues (probably) and will allow you to use FOC as well
```

---
## \#27 Posted by: pat.speed Posted at: 2018-10-17T11:15:38.484Z Reads: 32

```
Just gonna put this out there but if you need a cheaper solution, get a 190kv keda motor from HK, limit the vesc to 58k erpm (just to be extra safe) and you'll be riding in no time. I have two of the smaller versions running on 12s with TB vescs and it works perfectly.

Edit: that is assuming you have a working vesc

Edit 2: An even cheap solution is to just limit the erpm and keep the same motor you have now, should work fine. It will be a little more inefficient but that won't stop it from working
```

---
## \#28 Posted by: Pmac Posted at: 2018-10-17T23:30:32.316Z Reads: 34

```
Like @pat.speed said the cheapest way is to limit the erpm.

If you are very new and need help with the BLDC tool.  If you go to the video you linked that you followed at the 1 minute mark it shows on the video the part of the screen with the eRPM.  the erpm limit box is ticked which should be left ticked and then in the boxes change  min erpm to -58000 and the max erpm to 58000.

I would also change your volatge settings to 12s as with the current voltage settings you would kill your batteries if you allowed them to get that low.

Cheers,
Patrick

Edit:  Just to give you an idea.  I am running my board at 9s (i have 6 3s 5000mah LiPo's with 9s2p).  I have 2x 260kv 6354 motors running on the Flipsky 4.2 dual.  So the erpm is 68000 but I limit the erpm to 60000 and with a 12t pulley on the motors and a 40t pulley on the 83mm wheels i get a top speed of ~40kmh.  I have never hit the top speed as I get to 30kph and chicken out according to the GPS.

![IMG_20181005_233246|690x393](upload://zOoNCWPlS9XcyBTmoWHFCg74JLz.jpeg) 
![IMG_20181005_233317|690x393](upload://wP1Fyh2GNE6o9wbAXLeqOgIKHwG.jpeg) 
![IMG_20181005_233329|690x393](upload://uZQMHBXNBSJ6FA1dD4DLIBWkqPG.jpeg) 

I've got 2 more builds that I am planning.  Another 9s (still deciding on batteries whether liion or lipo) with 2x 270kv 5060 motors and 2 HK SK8 VESCs.  Will be running on 12t and 40t pulleys on 83mm wheels.  I have all these parts (other than the batteries) sitting around and a spare deck which I will use.

The other build will be 10s with 2x 190kv 6364 running on 6" pneumatic wheels.  haven't decided on the other parts yet.
```

---
## \#29 Posted by: Jamesk8 Posted at: 2018-10-18T01:55:33.298Z Reads: 31

```
i'm based in Melbourne and this exact thing happened to me but my vesc went too. waiting on my 190kv motor clearing customs then should be up and running :)
```

---
## \#30 Posted by: Koto Posted at: 2018-11-02T22:58:35.883Z Reads: 27

```
hey so can i use a vesc like this https://flipsky.net/collections/new-accessories/products/mini-fsesc4-20-50a-base-on-vesc-widely-used-in-eskateboard-escooter-ebike ? because its a bit more in my price range
```

---
## \#31 Posted by: kalebludlow Posted at: 2018-11-02T23:02:15.658Z Reads: 27

```
Sure can, just don't use FOC, only BLDC. I have blown one of those ones using 12S FOC, which was 100% my fault
```

---
## \#32 Posted by: Koto Posted at: 2018-11-02T23:23:09.269Z Reads: 26

```
alrighty sounds good thanks man
```

---
## \#33 Posted by: notepad Posted at: 2018-11-02T23:25:47.237Z Reads: 26

```
>Title: Melbourne Riders?

*Lives in city Lincoln UK*
*On street*  **Melbourne Way**
:disappointed_relieved::disappointed_relieved:
```

---
## \#34 Posted by: Koto Posted at: 2018-11-02T23:32:11.269Z Reads: 25

```
Ugh that sucks, sure there are riders around your spot. Just ask like i did!!
```

---
## \#35 Posted by: notepad Posted at: 2018-11-03T00:06:06.364Z Reads: 25

```
ive Only ever seen one other person with one.   It’s sad but at the same time it’s a nice ‘we are a rare breed’ feel to it.
```

---
## \#36 Posted by: Koto Posted at: 2018-11-04T00:08:11.209Z Reads: 24

```
Yeah, a wholesome feeling
```

---
## \#37 Posted by: Koto Posted at: 2018-11-16T05:27:29.522Z Reads: 22

```
Hey, 
The new vesc came in! What do you recommend for a tutorial on how to set up the FSESC 6.6 (I dont want to break it this time haha)
```

---
## \#38 Posted by: kalebludlow Posted at: 2018-11-16T05:39:10.042Z Reads: 18

```
Just use the tutorial on the vesc website, that's what I used
```

---
## \#39 Posted by: Koto Posted at: 2018-11-16T05:43:26.539Z Reads: 19

```
alright thanks what tool should I use
```

---
## \#40 Posted by: kalebludlow Posted at: 2018-11-16T06:08:34.452Z Reads: 20

```
Just the most recent version of vesc-tool will be fine
```

---
## \#41 Posted by: Pmac Posted at: 2018-11-16T06:35:45.814Z Reads: 21

```
Great choice!

max erpm of 150,000!  so there should be no issue running your 245kv motor on that ESC!

in terms of tools I like @Ackmaniac's tool as it has an awesome max watt mode and works with a cheap BT adapter and his own android app.  I set up multiple max watt outputs so I can lower the wattage for beginners trying my board with just a click in the app.
```

---
## \#42 Posted by: Koto Posted at: 2018-11-16T09:21:48.563Z Reads: 20

```
Holy shit they make it a pain to download
```

---
## \#43 Posted by: kalebludlow Posted at: 2018-11-16T09:41:19.733Z Reads: 20

```
Yeah man it sucks ass
```

---
## \#44 Posted by: Koto Posted at: 2018-11-16T11:19:54.192Z Reads: 20

```
hmm my vesc isnt getting sensed
```

---
## \#45 Posted by: moone Posted at: 2018-11-16T11:34:18.627Z Reads: 21

```
News team. Assemble. 
@Andy87 @moon @Wraith
```

---
## \#46 Posted by: Andy87 Posted at: 2018-11-16T11:38:30.512Z Reads: 18

```
so you have a FSESC 6.6 (single one) right?
it´s connected to the batter but not recogniced by the pc, or what is your problem now?
```

---
## \#47 Posted by: Koto Posted at: 2018-11-16T11:44:00.763Z Reads: 20

```
wow fixed itself
thank u thhough
```

---
## \#48 Posted by: Wraith Posted at: 2018-11-16T12:08:01.810Z Reads: 19

```
Well @Andy87 took care of that quickly lol
```

---
## \#49 Posted by: moone Posted at: 2018-11-16T12:42:31.300Z Reads: 17

```
When the esk8 mafia gets involve we just scare shit into working. @Andy87 @Wraith
```

---
## \#50 Posted by: Wraith Posted at: 2018-11-16T12:45:41.605Z Reads: 17

```
It doesnt always work with our own boards though i think lol
```

---
## \#51 Posted by: Koto Posted at: 2018-11-16T22:12:01.501Z Reads: 17

```
 @Andy87 @moone One thing though, evem though my ppm transmitter is connected to the receiver, the vesc isn't recognising any throttle in the ppm mapping part of the VESC tool
```

---
## \#52 Posted by: Andy87 Posted at: 2018-11-16T22:45:38.551Z Reads: 16

```
Are you plugged in the right channel?
```

---
## \#53 Posted by: Koto Posted at: 2018-11-16T23:04:07.329Z Reads: 16

```
nup im a retard thx
```

---
