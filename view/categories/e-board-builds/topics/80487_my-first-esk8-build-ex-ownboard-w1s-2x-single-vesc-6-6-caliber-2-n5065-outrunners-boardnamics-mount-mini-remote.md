# My first esk8 build - Ex-Ownboard W1S &#124; 2x Single VESC 6.6 &#124; Caliber 2 &#124; N5065 Outrunners &#124; Boardnamics Mount &#124; Mini Remote

### Replies: 36 Views: 1027

## \#1 Posted by: jun1208 Posted at: 2019-01-10T15:37:49.207Z Reads: 212

```
Hey guys,

I am very new to the esk8 scene and have only bought my first board from Ownboard in Nov last year :smiley:

So far I have been riding it daily for commuting to work and I kinda regretted purchasing a board before reading more in this DIY forum, so I had an idea to convert the Ownboard to a belt drive :smile:  

My parts list as below:

1. N5065 Outrunner motor - 270kv
2. Flipsky VESC 6.6 x 2
3. Extended trucks from Taobao for the motors
4. 97mm 78A flywheel clones
5. Flywheel clone pulley kit- 12/36T gear ratio

I will reuse the other parts from the W1S like the deck, enclosures, Samsung battery and my existing caliber 2 trucks for the front.

Album (I will add more pics in as the build progress :wink:) - https://imgur.com/a/d5YHG5o

I will continue to update this thread and I hope this will be helpful for the other newbies like me that wanted to learn more about building/modding their own esk8 :+1:
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-01-10T15:39:32.363Z Reads: 204

```
Ill buy your hub motors if you dont want them
```

---
## \#3 Posted by: Grozniy Posted at: 2019-01-10T15:48:33.492Z Reads: 194

```
Left motor mount on 2nd picture is apparently flipped the rong way.
Why 270kv on 10s?
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-01-10T19:57:29.092Z Reads: 167

```
You should get a motor with a lower kv, 270 kv at 10s will give roughly 70k erpm why will fry your drv because flipsky vesc 6 aren't actually vesc 6
```

---
## \#5 Posted by: Itsmedant Posted at: 2019-01-10T20:02:49.371Z Reads: 165

```
Good eye! I had to go back and look at it again.
```

---
## \#6 Posted by: J_Dizzle Posted at: 2019-01-10T20:03:08.974Z Reads: 155

```
If he runs them in foc there is no erpm
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-01-10T20:04:51.005Z Reads: 150

```
Huh im not sure about that. theres no way you could buypass the 60k erpm. 

above 60k = dead drv

focbox can safely do higher sometimes but its not guarnteed, only vesc 6 can go above and its limit is 110k erpm
```

---
## \#8 Posted by: jun1208 Posted at: 2019-01-11T01:59:37.201Z Reads: 135

```
Thanks for the offer but I am based in Malaysia, shipping is gonna be a rape :sob:
```

---
## \#9 Posted by: jun1208 Posted at: 2019-01-11T02:01:38.049Z Reads: 134

```
Good eye bro :slight_smile: the mounts are made only one side so there's not _mirrored version_ for it...
That is something I have to live with for now...

I got the 270 kv motors because I haven't been reading enough before purchasing so that was my own mistake...and I couldn't sell it off so I figure that I will use it first.
```

---
## \#10 Posted by: Sn4pz Posted at: 2019-01-11T02:02:46.980Z Reads: 126

```
Haha woops! 

Maybe you can find someone local, or save them for a backup
```

---
## \#11 Posted by: jun1208 Posted at: 2019-01-11T02:04:21.250Z Reads: 126

```
As per my reply to @Grozniy, it was an uneducated purchase lol

But I will limit the eRPM to 58000 on the VESC tool so that it won't go over :slight_smile:
```

---
## \#12 Posted by: Sn4pz Posted at: 2019-01-11T02:09:40.173Z Reads: 128

```
If you enjoy getting your hands 'dirty' you should take a look at the thread about rewinding your motors, it's pretty live right now so scrolling through the homepage should bring you right to it

For 10s, and a non true 6.xx based vesc, a good range of kv would be anywhere from 100-190

As you probably understand, the lower the kv, the more torquey and lower the top speed is (this can also depend on your gearing, so keep that in mind too)
```

---
## \#13 Posted by: jun1208 Posted at: 2019-01-11T03:04:19.505Z Reads: 115

```
Just take a light read on the topics regarding rewinding a motor, definitely _**not something**_ that I can do :laughing: 

Yea I figure that I will get a Flipsky 190kv 6354 motor after this 5065 gives way :smiley:

A 40T wheel pulley will be use also in the future for better torque :wink:
```

---
## \#14 Posted by: Grozniy Posted at: 2019-01-11T06:46:58.489Z Reads: 107

```
Don't get flipsky. You want a motor to last, get maytech or sk3 or racerstar. Maytech from forum vendors or directly through them
```

---
## \#15 Posted by: jun1208 Posted at: 2019-01-14T06:47:45.364Z Reads: 96

```
Thanks for the suggestion @Grozniy :) I'll look at ti when I am ready to replace the 5065 motors with the 6354 :smiley:
```

---
## \#16 Posted by: Scream Posted at: 2019-01-14T09:48:46.514Z Reads: 95

```
Plenty of happy campers using the flipsky 6354s - and I had a great experience with their after sales support.
```

---
## \#17 Posted by: jun1208 Posted at: 2019-01-14T11:13:26.278Z Reads: 99

```
Great to hear some positive feedback on the Flipsky motors, are you using them? Or you've jusy5heard that they're good?
```

---
## \#18 Posted by: jun1208 Posted at: 2019-01-24T01:49:49.563Z Reads: 105

```
Had this issue while trying to run the motor detection wizard...

Motor was detected fine but won't spin at the 2nd test...just stutters like you see in the video below...

https://youtu.be/g2rbr6zPsIM

I've tried swapping the phase wires around and make sure not cables are touching each other but it still produce the same result...

Swapped the motors and VESC around and can confirm it's _not_ the VESC's issue, since the other motor works just fine on both VESC...

Any idea guys?
```

---
## \#19 Posted by: jun1208 Posted at: 2019-02-13T01:07:58.288Z Reads: 99

```
Finally got the mounts from @Boardnamics and they are really much more polished than the cheap chinese mounts that I have previously !

![](https://imgur.com/VCRMflL.jpg)
![](https://imgur.com/4ZPwUxD.jpg)
![](https://imgur.com/EuDnPLq.jpg)
```

---
## \#20 Posted by: eboardquebec Posted at: 2019-02-13T18:55:58.495Z Reads: 86

```
What kind of motor you build ?
```

---
## \#21 Posted by: Sn4pz Posted at: 2019-02-13T18:57:38.700Z Reads: 84

```
I didnt build any motor, I was hoping to buy his :) 

However, I have ownboard Hub motors if thats what youre asking
```

---
## \#22 Posted by: jun1208 Posted at: 2019-02-14T14:50:29.293Z Reads: 80

```
Mine is a generic N5065 outrunner motor from China, plan to change to Flipsky 6534 motors once these dies :+1:
```

---
## \#23 Posted by: chrischo1996 Posted at: 2019-02-14T15:07:07.222Z Reads: 75

```
Can you link your rear trucks? How does the quality seem on them?
```

---
## \#24 Posted by: jun1208 Posted at: 2019-02-14T15:48:23.567Z Reads: 74

```
Here you go 👍🏼

https://item.taobao.com/item.htm?id=584738329905
```

---
## \#25 Posted by: chrischo1996 Posted at: 2019-02-14T16:05:37.616Z Reads: 71

```
Wow those are really long. No problems with fitment for the Boardnamic mounts?
```

---
## \#26 Posted by: jun1208 Posted at: 2019-02-14T17:35:07.413Z Reads: 69

```
So far they fix with no issues, haven't mount it on my deck yet but they are indeed much longer than normal caliber 2 :laughing:

Even the extended trucks from TB is not as wide :wink:
```

---
## \#27 Posted by: Grozniy Posted at: 2019-02-14T22:36:08.703Z Reads: 65

```
Be careful. If regular cheap 10' trucks break, longer ones are even more prone to it.
```

---
## \#28 Posted by: jun1208 Posted at: 2019-02-15T00:09:18.687Z Reads: 63

```
Yea man, I was aware of the cheap DIYe truck breaking fiasco :frowning_face: 

Will be more careful with it, but this seems to be a custom made trucks by the seller himself as I've never seen anyone else selling them :+1:
```

---
## \#29 Posted by: Grozniy Posted at: 2019-02-15T09:12:26.608Z Reads: 50

```
DIY sells them also for AT setup
```

---
## \#30 Posted by: jun1208 Posted at: 2019-02-15T11:16:22.063Z Reads: 47

```
You got a link for that bro? Do you mean DIYe the Chinese site or DIYelectricskateboard aka Torque Board?
```

---
## \#31 Posted by: Grozniy Posted at: 2019-02-15T11:18:03.522Z Reads: 50

```
The Chinese DIY store
```

---
## \#32 Posted by: chrischo1996 Posted at: 2019-02-15T13:58:25.929Z Reads: 48

```
I don't believe they're the same ones, the diyeboard ones have a round profile while these ones have a caliber style shape.
```

---
## \#33 Posted by: jun1208 Posted at: 2019-02-15T14:22:41.455Z Reads: 47

```
Wait, you're saying that DIYe selling the one I'm using too?
```

---
## \#34 Posted by: Grozniy Posted at: 2019-02-15T14:44:08.089Z Reads: 44

```
This one?
http://www.diyeboard.com/9-at-truck-kit-for-our-6-airless-allterrain-wheels-p-623.html?zenid=69b7b773ca49100c2ee5fc635c5bf084
```

---
## \#35 Posted by: jun1208 Posted at: 2019-02-15T14:49:51.550Z Reads: 46

```
Can't see clearly in the pic but the trucks does looks a bit similar so I can't be sure...
```

---
## \#36 Posted by: jun1208 Posted at: 2019-02-19T06:51:29.983Z Reads: 40

```
I just checked again, the DIYe ones are 9" whereas mine is 10" :slight_smile: 

So it is not the same one :+1:
```

---
