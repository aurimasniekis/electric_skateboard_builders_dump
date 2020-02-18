# What happend to my R-spec hubs?

### Replies: 44 Views: 826

## \#1 Posted by: wannagofast Posted at: 2019-03-18T19:12:43.839Z Reads: 283

```
So I received my R-spec kit with the Unity in the mail a few weeks ago but was just able to install it in my board. I was extremely impressed with the performance as I began to ride it but after around 10 miles total, I stopped at an intersection and the right motor wouldn't turn without making a terrible noise. I recalibrated the motor at got this ![Screenshot_20190318-114428%20(1)|243x500](upload://3fmHvtJiN8Vayn5gYwdjNqfWttV.jpeg) .  What happened to my motor? I opened up the ESC enclosure and made sure all the connections where solid and it's still doing this.
```

---
## \#2 Posted by: olestra Posted at: 2019-03-18T19:23:14.521Z Reads: 262

```
see how high the resistance on motor 1 is?
confirm that value with a multi-meter, testing the resistance from wire 1-2, 2-3, and 3 to 1. you'll probably see one that is way outside the values of the other 2. It looks like you have one of the coil windings damaged. Normally all three will have the same, low resistance value
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-03-18T19:23:56.897Z Reads: 261

```
run motor detection again, i think i know what your talking about
```

---
## \#4 Posted by: wannagofast Posted at: 2019-03-18T19:41:48.638Z Reads: 249

```
Yep, I just checked it, thanks guys. It looks like there isn't even a connection for coil winding 3.  Damn, this really sucks, I don't have anything to commute with anymore. Would this have been a factor quality issue? Here is another reading I did before the first one. ![Screenshot_20190318-110248|243x500](upload://biQ3XlJSSE9AZKp0D2nneErubiN.jpeg)  (I know the sensor wasn't reading on the other one)
```

---
## \#5 Posted by: TowerCrisis Posted at: 2019-03-18T19:50:51.427Z Reads: 226

```
Well, a disconnect is better than a short. This may be easily repaired.

I'm guessing that the solder joint between the stator coil and the silicone wire has broken. That's good, because you can probably fix that.

Much better than two coils being shorted together, as you couldn't fix that without rewiring the entire stator.


Are these hubs easily serviceable? Can you pop open the hood?
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-03-18T19:53:59.398Z Reads: 212

```
@CarlCollins
```

---
## \#7 Posted by: Skunk Posted at: 2019-03-18T19:54:21.827Z Reads: 211

```
[quote="TowerCrisis, post:5, topic:87545"]
Are these hubs easily serviceable? Can you pop open the hood?
[/quote]

Question is will that void warranty. 
@CarlCollins 
@barajabali
```

---
## \#8 Posted by: TowerCrisis Posted at: 2019-03-18T19:55:47.382Z Reads: 202

```
I'd argue that they should already offer warranty and replace them free of charge. But I understand the allure of fixing it yourself.
```

---
## \#9 Posted by: Skunk Posted at: 2019-03-18T19:57:20.912Z Reads: 199

```
Of course,  but they also justify voiding warranty over changing xt60 to xt90 so.......
```

---
## \#10 Posted by: wannagofast Posted at: 2019-03-18T19:59:20.203Z Reads: 199

```
Luckily I've been in contact with @barajabali simultaneously and he just offered to replace it free of charge no problem! Once I have the replacement in hand I would be happy to open the other up and see what went wrong and post it here. This is probably just a rare fluke.

I just wanted to see if anyone here could give me some more detailed information. I'm not 100% certain of the mechanics of an electric motor.
```

---
## \#11 Posted by: brenternet Posted at: 2019-03-18T20:00:33.034Z Reads: 191

```
[quote="wannagofast, post:10, topic:87545"]
This is probably just a rare fluke.
[/quote]

:joy: :joy:
```

---
## \#12 Posted by: wannagofast Posted at: 2019-03-18T20:16:32.681Z Reads: 185

```
(hopefully)
```

---
## \#13 Posted by: moon Posted at: 2019-03-18T20:22:50.779Z Reads: 176

```
let me present @Seanhacker
```

---
## \#14 Posted by: DerelictRobot Posted at: 2019-03-18T20:34:21.332Z Reads: 172

```
You beat me to it.
```

---
## \#15 Posted by: SeanHacker Posted at: 2019-03-18T20:58:39.224Z Reads: 170

```
[quote="wannagofast, post:4, topic:87545"]
Would this have been a factor quality issue?
[/quote]

Yes. Every single motor I've received from them have had some sort of QC issues or just design flaws. I think I've owned around 5 or 6 pairs of them. 

[quote="wannagofast, post:10, topic:87545"]
This is probably just a rare fluke.
[/quote]

Nope. Definitely NOT a fluke in my experience with this companies motor quality over the last two years.
```

---
## \#16 Posted by: pat.speed Posted at: 2019-03-18T21:01:10.041Z Reads: 164

```
What sorts of failures have you experienced
```

---
## \#17 Posted by: SeanHacker Posted at: 2019-03-18T21:04:32.287Z Reads: 165

```
Overheating, bearings go bad after every ride because the seats are crooked, lockups (at 30mph), horribly wound windings that broke and shorted, knocking sounds, grinding sounds, stuttering, ect... All my motors have been ridden less than 80 miles. I have a basically brand new R2 that i got over 2 years ago that has around 120 or so miles on it because of these issues. It hasn't been safe and I enjoy living.
```

---
## \#18 Posted by: barajabali Posted at: 2019-03-18T21:48:09.010Z Reads: 162

```
Our latest motors are solid. Failure rate is extremely low and I know that to be true. Every batch we put out is better than the last. @SeanHacker you haven’t had a new set of motors so it’s hard for you to compare.
```

---
## \#19 Posted by: SeanHacker Posted at: 2019-03-18T21:53:59.942Z Reads: 164

```
[quote="barajabali, post:18, topic:87545"]
you haven’t had a new set of motors so it’s hard for you to compare.
[/quote]

Yes I have unless these aren't what you guys are selling now. And these suck just as bad as previous versions. 

![IMG_20190318_145218|375x500](upload://1lZmWon2M3ye4FM74AyL3Zr55CC.jpeg)

[quote="barajabali, post:18, topic:87545"]
Our latest motors are solid. Failure rate is extremely low
[/quote]

I've been hearing this same thing for two years now.
```

---
## \#20 Posted by: barajabali Posted at: 2019-03-18T22:09:34.560Z Reads: 160

```
[quote="SeanHacker, post:19, topic:87545"]
Yes I have unless these aren’t what you guys are selling now.
[/quote]


They’re not.
```

---
## \#21 Posted by: SeanHacker Posted at: 2019-03-18T22:15:16.007Z Reads: 157

```
[quote="barajabali, post:20, topic:87545"]
They’re not.
[/quote]

Yes they are. ;)
```

---
## \#22 Posted by: barajabali Posted at: 2019-03-18T22:20:07.992Z Reads: 149

```
No, they’re not.
```

---
## \#23 Posted by: SeanHacker Posted at: 2019-03-18T22:25:58.516Z Reads: 150

```
Alright dude. I see things have changed here. But yes they are. 

Can you provide the failure rates that you speak of? I'm sure everyone would be interested. If it's just a hand count, then don't bother.
```

---
## \#24 Posted by: ninTHIENdo Posted at: 2019-03-18T22:27:06.259Z Reads: 148

```
They look a little different, the new ones look like they have more “heatsinks”
![image|500x500](upload://a8FtwdbdxXQAIyWXe0JBbAN0ftO.jpeg) 

Not trying to argue against your experience, since I’m not having the best experience with them either at the moment...
```

---
## \#25 Posted by: SeanHacker Posted at: 2019-03-18T22:27:35.785Z Reads: 148

```
Different trucks doesn't mean different motors. ;)
```

---
## \#26 Posted by: ninTHIENdo Posted at: 2019-03-18T22:28:50.076Z Reads: 145

```
Takes foot out of mouth, walks away...
```

---
## \#27 Posted by: barajabali Posted at: 2019-03-18T22:35:19.223Z Reads: 144

```
No Sean. That is not a request that can be fulfilled. 

I know what has changed and I am not known to lie. I have implemented many changes myself directly to our factory. The changes are of core components, tolerances, windings and assembly processes all coming together to make our latest motors the best we have to offer. 

I know they look the ‘same’ but they’re not. I am an actual authority on this matter.
```

---
## \#28 Posted by: ninTHIENdo Posted at: 2019-03-18T22:47:43.210Z Reads: 144

```
![image|281x499](upload://l4V32KZxrUM6pXctC9CDQPw9AGy.png) ![image|281x499](upload://lynvCBGpD69890nBISnxbc7pFh.png) 

You’re not known to lie, but you said orders are fulfilled in the order received. But Carl informed me it wasn’t the case since I was a US customer, so technically you lied about shipping in the order received
```

---
## \#29 Posted by: barajabali Posted at: 2019-03-18T22:50:28.717Z Reads: 140

```
Hi Thien,

I am shipping your Unity order this Friday likely. 

Sorry if I was misinformed, I only tried to help you.
```

---
## \#30 Posted by: SeanHacker Posted at: 2019-03-18T22:53:42.843Z Reads: 137

```
[quote="barajabali, post:27, topic:87545"]
That is not a request that cant be fulfilled.
[/quote]

Figured so much. So the failure rate is whatever you guys say it is at this point. That's a real shame considering that is very valuable information to the consumer.

P.S- These are definitely the same motors though. I can drop a bomb here or leave it as is for now. I'm bored with this conversation. ;)
```

---
## \#31 Posted by: barajabali Posted at: 2019-03-18T22:56:20.555Z Reads: 135

```
Sure Sean.
```

---
## \#32 Posted by: Sn4pz Posted at: 2019-03-18T22:57:35.970Z Reads: 133

```
Damn, I hate losing faith in a company.
```

---
## \#33 Posted by: barajabali Posted at: 2019-03-18T23:02:19.711Z Reads: 135

```
@wannagofast 

Magnus, I’ve already confirmed a new motor to be shipped to you. I’ll likely have it out tomorrow or the following day. 

If you wouldn’t mind, I’d be happy to offer a shipping label to you so I can retrieve your damaged motor for investigation. This is extremely rare so I’d like to look into it.
```

---
## \#34 Posted by: CarlCollins Posted at: 2019-03-19T04:37:10.627Z Reads: 121

```
Seriously Dude? :stuck_out_tongue:
Never thought you will stick in every post and raise this method even we have addressed it more than 5 times now :blush:
```

---
## \#35 Posted by: ninTHIENdo Posted at: 2019-03-19T10:44:41.646Z Reads: 111

```
Just coming in and saying hi! 👋

I was just showing where he lied, and he apologized because he was misinformed by enertion like I was misinformed with enertion newsletters.
```

---
## \#36 Posted by: CarlCollins Posted at: 2019-03-19T11:47:57.644Z Reads: 108

```
Neither we lied to Bara or to you, the shipment related information is something which only shipment team, CS team (if informed) knows first.
```

---
## \#37 Posted by: ninTHIENdo Posted at: 2019-03-19T12:06:07.725Z Reads: 107

```
I never said he got lied to, I said I was lied to by his misinformation, which he apologized for, and stated he would get it shipped Friday when he receives the US shipment. He should receive it this week still if customs released it from the hold they had over the weekend correct?
```

---
## \#38 Posted by: Pedrodemio Posted at: 2019-03-19T12:10:00.095Z Reads: 106

```
Not trying to escalate things, but all the motors you got are replacements for the first pair? Or you bought more? And why you didn’t receive the latest motors as replacements?
```

---
## \#39 Posted by: SeanHacker Posted at: 2019-03-19T13:42:47.796Z Reads: 98

```
I've gotten warranty replacements (tons) and thought at the time I was getting lucky when I bought some motors off of a couple unhappy R2 owners. Not so lucky. The motors have always sucked no matter who/where I got them from. 

I did get the new motors (silver ones) on yet another warranty because everything they have given me to date is either half broken on arrival or doesn't work longer than a couple rides. I've seriously been dealing with this board for 2 years. It's gotten so old and I don't have the time to be constantly shipping/receiving garbage back and forth.
```

---
## \#40 Posted by: briman05 Posted at: 2019-03-19T14:08:19.567Z Reads: 99

```
https://www.irishtimes.com/polopoly_fs/1.3225232!/image/image.gif
```

---
## \#41 Posted by: CarlCollins Posted at: 2019-03-19T16:29:28.322Z Reads: 90

```
Hopefully yes
```

---
## \#42 Posted by: Kresher Posted at: 2019-08-21T07:45:17.001Z Reads: 58

```
Im really here for all this tea, but I'm also in the process of trying to design my DIY board, So my question to everyone here is. When the R-Spec motors do work as intended, do they live up to all the claims? Because, up until this point Enertion is the only company that I found that sells 2000W hub motor kits and it would be really cool if i could make my build with that.
```

---
## \#43 Posted by: linsus Posted at: 2019-08-21T08:29:04.624Z Reads: 54

```
Hi, You're better off with the new hummies. Instead of nomerous complaints there are only success stories. Live atm on kickstarter, I signed up for two sets. Created by @Hummie here on the forum. 

https://www.kickstarter.com/projects/1755906511/hummie-hub-motors?ref=user_menu
```

---
## \#44 Posted by: epss4 Posted at: 2019-08-21T17:15:48.100Z Reads: 40

```
Hi man 
I have r spec hub on 12s5p sanyo cell  with the unity
On 12S the motor dont overheat , and they are so powerful its just crazy
Ok wheel quality suck (suppose to receive the new one soon)
Ok their shipping time is really long(and they lie all the time)
But once you have them its a true pleasure to ride those , i can hit 65km/hrs on 90mm wheel
```

---
