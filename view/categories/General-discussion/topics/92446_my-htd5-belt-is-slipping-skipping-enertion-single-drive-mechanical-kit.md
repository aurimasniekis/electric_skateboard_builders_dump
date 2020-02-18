# My HTD5 belt is slipping / skipping ! Enertion single drive mechanical kit

### Replies: 32 Views: 403

## \#1 Posted by: guigui Posted at: 2019-05-01T16:07:50.397Z Reads: 119

```
Hey !

I have an enertion single drive mechanical kit that I had lying around for more than 2 years now and I finally decided to use it again. It had one problem, the belt skips when accelerating/braking to hard, tried to fix that today but nop, it still is the case !
I have the 16T pulley on the motor shaft, it is a Turnigy Aerodrive SK3 - 6374-192KV .
I have a  Flipsky Dual FSESC4.20 100A but I'm only using one motor, and a 6S 20C 5Ah lipo battery for the moment.

Whenever the belt skip, it does it only one time and then it stops accelerating/braking (it cuts the power), I then have to center the triger and accelerate/brake again, and still if I push it too hard it slips.
I don't know why the power cuts like that, I think it's from the VESC but what ? Two years ago when I used a hobby ESC it just kept slipping like crazy if I didn't release the trigger. 

I even tried to tension the belt way more than you are supposed to but it still skip ! :frowning:  

Here are some pictures :

https://imgur.com/a/Xjyu1UG?fbclid=IwAR1T6N51g5tL-SHyaOGxOFJQILpwYpBwuXfWrhpGGHiW1bTMjtU7qKU1oNQ

The last pic is a video where the motor is blocked and I apply as much torque as I can on the wheel with my hands, results : the belt skips even by hand (note that I have to put everything I had to do it, but it does skip !) 
So if it is slipping with my hands, I don't know how it's supposed to hold up to a 4000W motor (even though I don't use more than 1600W because of my configuration). 

So is there a problem somewhere or is it just that the kit is bad ? I mean yes there are not a lot of teeths in contact with the belt (on the motor shaft) but If enertion sell such a configuration, it's supposed to be hold the torque right ?
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-05-01T16:13:37.330Z Reads: 112

```
Try a slightly shorter belt. If oure using a 265 go to a 260, or what ever your belt size is
```

---
## \#3 Posted by: guigui Posted at: 2019-05-01T16:21:27.207Z Reads: 107

```
What is it going to change ? If the two axles get closer it's just going to engage less teeths on the motor isn't it ?
```

---
## \#4 Posted by: J0ker3366 Posted at: 2019-05-01T16:27:01.594Z Reads: 104

```
Is it possible to show video? 

Belt slippage is usual due to over sized belt, too small of a motor pulley (16t is fine), or using 3m tooth profiles. Do you know what belt you use?

Edit: in the picture it does appear to be 5m, just want to make sure.
```

---
## \#5 Posted by: guigui Posted at: 2019-05-01T16:36:11.631Z Reads: 95

```
Thank you so much for your help,
Please check the imgur the video is at the very last :slight_smile:
It's hard to see but when the camera shake it skipped. 
Yes it's a HTD265-5M, I understand the motor pulley size and tooth profiles but I really don't get why would belt size be a problem ?
```

---
## \#6 Posted by: J0ker3366 Posted at: 2019-05-01T16:39:16.233Z Reads: 89

```
Are you running a 12mm wide belt?
```

---
## \#7 Posted by: guigui Posted at: 2019-05-01T16:44:55.198Z Reads: 89

```
Yes I am !
```

---
## \#8 Posted by: J0ker3366 Posted at: 2019-05-01T16:47:59.968Z Reads: 87

```
Uh oh... That may be your problem. Im not positive as i dont have hands on you build. Anyway you can try going 15mm?

I use the same setup you have minus the mount and different belt size. Even on 15mm i still get slippage but its only under heavt heavy braking.
```

---
## \#9 Posted by: guigui Posted at: 2019-05-01T16:55:32.780Z Reads: 81

```
By it's my problem do you mean I bought something that isn't made to hold up to a lot of torque ? 

If going to 15mm will only give me a 25% increase in torque I don't think it's that good :frowning: 

I'm kind of mad at enertion, they sold it saying it was a good combo with their 2400W motor but it's not even capable to hold up to such torque.
```

---
## \#10 Posted by: J0ker3366 Posted at: 2019-05-01T17:01:38.572Z Reads: 80

```
Stop throwing % around lol. 15mm will handle the torque better than 12mm. Going dual would make it handle the torque even better. 

Diagnosis:
I do believe your problem is going to be running a single 12mm belt. 

Solution:
Uprade to a 15mm setup, have a beer/soda and call me in the morning.

I wouldnt say you bought the wrong thing or even that enertion sold you "shit". 12mm is fine if youre running a dual setup. But on a single 6374, its a little under par.
```

---
## \#11 Posted by: guigui Posted at: 2019-05-01T17:07:55.794Z Reads: 74

```
Well I don't see why the increase in torque wouldn't be linear. 15/12*100=125% So if it really is 25% I mean yes it's better but still... 

By the way, if I tweak the settings of the VESC well, I manage to get a configuration where It doesn't slip but I was looking for something more "zippy"

My order was a " MONO DRIVE MECH KIT", everything was included, I didn't buy parts here and there so if it is sold as a mono drive kit it should be able to hold the torque
```

---
## \#12 Posted by: J0ker3366 Posted at: 2019-05-01T17:12:04.341Z Reads: 70

```
You can play with throttle curves (for acceleration) and you can adjust your motor negative (battery min i believe) for when braking.
```

---
## \#13 Posted by: J0ker3366 Posted at: 2019-05-01T17:14:11.763Z Reads: 68

```
[quote="guigui, post:11, topic:92446"]
a mono drive kit it should be able to hold the torque
[/quote]

What they wont tell you is, on a single 12mm wide setup, its not par for a single 6374. 12mm is good for running dual. Sinle 15mm will work better. Single 20mm will work great. Follow?
```

---
## \#14 Posted by: J0ker3366 Posted at: 2019-05-01T17:16:37.469Z Reads: 65

```
[quote="J0ker3366, post:12, topic:92446"]
adjust your motor negative
[/quote]

Are you able to post screen shots of your vesc settings?
```

---
## \#15 Posted by: guigui Posted at: 2019-05-01T18:19:55.369Z Reads: 63

```
I'll see what I do, will give you the vesc settings when I get back, what do you want them for ?
```

---
## \#16 Posted by: brenternet Posted at: 2019-05-01T18:27:22.592Z Reads: 60

```
You're just thinking too hard here, your pulleys look fine.

The belt is probably just loose, it needs to be shorter and then it won't slip.
```

---
## \#17 Posted by: guigui Posted at: 2019-05-01T18:31:27.571Z Reads: 58

```
I tightened it like crazy once but it was still slipping. About shortening the belt, can you please explain me how it's going to affect the slipping issue ? I really don't get it :frowning:  From what I understand if I use a shorter belt the axles will be closer and it's going to engage less teeths on the motor ?
```

---
## \#18 Posted by: brenternet Posted at: 2019-05-01T18:36:07.333Z Reads: 58

```
Oh I meant either moving the motor or shortening the belt if you can't, if you've done that and it's still slipping I don't know really.. it's all pretty simple mechanics.

Bin it :smiley:
```

---
## \#19 Posted by: guigui Posted at: 2019-05-01T18:40:34.693Z Reads: 55

```
Oh okay ! Well I'll see what to do but, thank you all for your help !
```

---
## \#20 Posted by: skatardude10 Posted at: 2019-05-01T18:47:55.627Z Reads: 54

```
Are you using a bearing in your wheel pulley? It looks like you are, just to make sure... 

Adding a bearing to my wheel pulleys stopped all my skipping problems.
```

---
## \#21 Posted by: guigui Posted at: 2019-05-01T19:28:25.995Z Reads: 49

```
I do have a bearing, sadly it's not the problem here :frowning:
```

---
## \#22 Posted by: J_Dizzle Posted at: 2019-05-01T19:32:08.157Z Reads: 48

```
Maybe try using a new belt? Your current belt's teeth may be worn down
```

---
## \#23 Posted by: guigui Posted at: 2019-05-01T19:34:50.033Z Reads: 46

```
I tried 5 belts :stuck_out_tongue:
```

---
## \#24 Posted by: IndyPilot Posted at: 2019-05-02T00:53:05.183Z Reads: 43

```
Newb to eskate, but not to mechanics.  Are the motor shaft and truck axle perfectly parallel (or motor pulley and wheel pulley)?  If not, then only one edge of the belt actually is tight and you’re not getting a full width of tight belt engagement.  Or is the mount flexing to the point that they’re not parallel under power?  That’s my 2 cents.
```

---
## \#25 Posted by: Mazda_bater Posted at: 2019-05-02T00:55:33.404Z Reads: 40

```
Issue is with the vesc not the belts
```

---
## \#26 Posted by: meesie Posted at: 2019-05-02T15:37:36.547Z Reads: 35

```
Try running a longer belt with a tensioner. It makes for more contact with the pulley
```

---
## \#27 Posted by: guigui Posted at: 2019-05-02T17:16:42.155Z Reads: 34

```
I will make sure that everything is perfectly square and parallel when I get back home, thanks :slight_smile:
```

---
## \#28 Posted by: guigui Posted at: 2019-05-02T17:17:35.283Z Reads: 34

```
I thought about that but the mount is carbon fiber, I don't really have the tools to work with that
```

---
## \#29 Posted by: guigui Posted at: 2019-05-04T17:29:14.405Z Reads: 27

```
I checked everything today, it is parallel and stiff
```

---
## \#30 Posted by: TowerCrisis Posted at: 2019-05-04T19:25:30.985Z Reads: 23

```
Are you using spacers between your bearings?

If your wheel nuts are not tight because of no spacers, then your wheel pulley has potential to flex towards the motor pulley when under high loads.
```

---
## \#31 Posted by: guigui Posted at: 2019-05-04T19:49:40.376Z Reads: 24

```
I do use spacers, but thanks for the help :blush:
```

---
## \#32 Posted by: guigui Posted at: 2019-05-05T10:42:27.805Z Reads: 16

```
Ok so I tried everything I could, after tweaking the VESC settings I do get a decent acceleration (same as a meepo for exemple) and deceleration. But I though I could get something overkill with a single motor, I guess I was wrong :thinking:
```

---
