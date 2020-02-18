# ACTON Blink board with VESC?

### Replies: 19 Views: 2169

## \#1 Posted by: Tomer Posted at: 2017-04-18T09:01:53.465Z Reads: 167

```
Hey there,

I have the ACTON Blink board (belt version) almost 8 months. Right now the board is not operating well.
The belt motor and the battery pack works just fine, it's just the ESC which does not work well.

I was wondering if is it possible to use my ACTON's belt motor and battery pack with DIYElectric VESC?

Things that I am trying to think of, for example, is that the ACTON Blink belt motor brakes are just terrible. 
They give you 100% braking even if you pull very gently the brakes from the control, I was wondering if
I will be able to configure the motor brakes through the BLDC tool.

I will be very thankful for any clarification about this topic.

Thanks.
```

---
## \#2 Posted by: aigenic Posted at: 2017-04-18T14:51:45.932Z Reads: 144

```
If you use vesc, the brakes will be much better...
The only problem that would confuse me is BMS and reciever as I already mentioned in public Chat...If you could take down the enclosure and send picks of battery and all electronics...it would be great if I could see what exactly is inside and then I will help you...
I have already seen some pics so I think it will definitely be possible...
```

---
## \#3 Posted by: Tomer Posted at: 2017-04-18T18:13:57.740Z Reads: 129

```
I think that the BMS is inside the battery pack. 
I disconnected the battery from the ESC, and the battery was about 90% charged. I plugged it into the charger and there is a Red LED indicator which states that the battery is not fully charged. After about 10-15 minutes the indicator LED turned to Green which means that the battery is fully charged. So yeah, I think the BMS is already in it.

Anwyas, here are the pictures that you have requested. Please let me know if you need any more pictures to be shared.

Thank you my friend. 

<img src="/uploads/db1493/original/3X/c/5/c56d9a88763cab170f0dc8df26be3013330c9d1c.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/e/2/e2429e4ca2de80b9e945a51ae979c05f3c2f4883.jpg" width="375" height="500">
```

---
## \#4 Posted by: aigenic Posted at: 2017-04-18T18:25:33.041Z Reads: 117

```
Ok...the ESC is connected just by 2 wires so the BMS is probably inside :) charging cable leads also directly to the pack :)
It will deffinitely be possible...Is there a reciever of the remote or not? it doesn't look like that from your pictures...
Do you have voltmeter? could you charge the battery to max and then measure the voltage? If not try to search google/reddit/this forum to find the voltage...
```

---
## \#5 Posted by: mmaner Posted at: 2017-04-18T18:37:48.879Z Reads: 116

```
Most power supplies will charge to a specific voltage and then stop fast charging and go trickle charge.  That could just be the power supply detecting the full charge.  Post a pic of the power supply.
```

---
## \#6 Posted by: Tomer Posted at: 2017-04-18T18:52:13.892Z Reads: 112

```
Try to zoom in the first picture that I uploaded. There are 3 layers of green cards. 
The first one has the receiver attached to it. I am planning on getting a 2.4 GHZ nano remote anyways.

<img src="/uploads/db1493/original/3X/8/a/8a9f86fdfb338ed585228c36f366f5cc21d92db2.jpg" width="375" height="500">
```

---
## \#7 Posted by: aigenic Posted at: 2017-04-18T19:19:10.167Z Reads: 105

```
DIY VESC should be OK, you will have to set it up through BLDC (it is not plug and play ESC, you probably know) if you dont want to buy new remote, you can try to separate the reciever and connect it to the vesc (If it can be simply separated/unplugged from the ESC), but if you want to change the remote, I would go this way :) Also I must warn you that the Nano remote controller = Winning remote, which means it has a lot of signal losses, the mini remote is more reliable :) Some guys on this forum upgraded their winnings to make it work, just search if you are interested :)

(sorry for my english, I am not a native speaker)
```

---
## \#8 Posted by: Tomer Posted at: 2017-04-18T19:40:33.648Z Reads: 105

```
It's all good, English is not my native language as well. :)

Separating the receiver from the chip could be done, however I am not sure where is the input of the ACTON's receiver located. I will take a dipper look on it, but I am not going to spend much time to figuring it out, I rather to just buy a new remote.

Thank you for letting me know that the Nano has some issues with it - I didn't know that. 
I don't like the mini remote as it seems to big in my personal opinion.
Can you recommend on another RC with the same sizes of the Winning nano?
I also saw that there are the [nano-x RC by Enertion](http://www.enertionboards.com/categories/wireless-hand-controller.html) and the [mini RC from DIYElectrics](diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/). Are those any better?
```

---
## \#9 Posted by: aigenic Posted at: 2017-04-18T19:54:34.612Z Reads: 103

```
The Nano-x is only on a preorder, but i am not sure, ask enertion support...It should be a better quallity than winning, otherway you can buy winning and make the changes (changing reciever...) and hope it will work properly :D I found some new links on alibaba/aliexpress of a new version of winning which might be better, but I am not sure...Also you can make a GT2B Mod, but that would take too much work...

The last option is buying benchwheel remote...It is not as small and looks a litle ugly, but it has a cruise control and it is reliable :) (this one: https://www.electric-skateboard.builders/t/benchwheel-remote-receiver/14171)
```

---
## \#10 Posted by: yaca Posted at: 2017-04-18T20:31:31.156Z Reads: 99

```
The benchwheel has no cruise control. In the manual they call it cruise mode but it is just a low speed mode. This mode is too weak for adults, maybe it's good for kids. On VESC display it is 10 - 50 - 70 percent (Brake - Neutral - Throttle). The other mode is called sport mode (0 - 50 - 100 on VESC display). I like the benchwheel remote and it feels good in the hand.
```

---
## \#11 Posted by: Tomer Posted at: 2017-04-19T06:13:14.311Z Reads: 93

```
Could you please share with me the new version of Winning remote you found?
Is there any guide on how to use a different receiver for the Winning remote?

GT2B Mod is too big for my preference.

Benchwheel looks like a great alternative for the Nano remote, I'll take it into consideration. Thanks.
```

---
## \#12 Posted by: aigenic Posted at: 2017-04-19T13:46:19.969Z Reads: 84

```
This one: https://www.alibaba.com/product-detail/New-arrival-2-4Ghz-mini-remote_60584821588.html?spm=a2700.7724838.0.0.c6IUES

But it not tested, I haven'tseen anyone using it...they claim it is better then the original Winning...
""There are some upgrade on this remote,according to customer's suggestion:
1.we can customized custom logo onto our remote controller. 
2.increase the throttle range to over 30m 
3.add an extra antenna inside to strengthen the signal;
4.full capacity 3.7v 500Mah battery. ""

But if you buy the original you can buy GT2B reciever and pair it together...many users of this forum did it that way, but I heared it haven't deleted the problems completely...
```

---
## \#13 Posted by: Tomer Posted at: 2017-04-20T10:08:14.104Z Reads: 71

```
This looks interesting. Does anyone plan getting his hands on this remote?

I read someone in the forum who said that even if there is 1% chance of failure
with the remote while riding, this 1% is just too much. I agree with that statement.
In addition, in order to purchase the new released remote you must buy in sets.
That being said, I will stick with the Benchwheel remote as for now.
```

---
## \#14 Posted by: Tomer Posted at: 2017-05-18T16:49:14.740Z Reads: 63

```
UPDATE:

It's working!
Today I received the VESC, after few modifications I managed it to work. I found a new hobby. :slight_smile: 

I'll upload pictures later.
```

---
## \#15 Posted by: Darksyder510 Posted at: 2017-06-16T15:45:57.838Z Reads: 49

```
@Tomer, I know this is kind of old, but would you be able to post some pictures and how you got the VESC working on the Acton board? I am doing a similar project with hub motors for the Acton board and wanted to have a reference on how to get it working.
```

---
## \#16 Posted by: Tomer Posted at: 2017-06-16T16:58:27.408Z Reads: 50

```
You got really nice timing right there, I was able to get it into working state only today. 

Please elaborate more about what would you like to know. I bought my VESC from Maytech as it has a really good price and shipping it to my country is free. My remote of choice is the Benchwheel remote and receiver.
I just received it two days ago and I am still learning on what are the best settings for it in BLDC.

My board is currently in a working state, however it's no perfect just yet. I need to do more research and testing to get there. 

Are you going to use ACTON'S hub motor? If so, are you going for single or dual drive setup?
```

---
## \#17 Posted by: psychotiller Posted at: 2017-06-16T17:03:04.109Z Reads: 52

```
That is the esc that is being sold on ebay in single and dual formats for 6,7 and 10s.

I have one but havent put in in a build yet.
```

---
## \#18 Posted by: Darksyder510 Posted at: 2017-09-14T03:17:59.878Z Reads: 38

```
Hey Tomer,

Sorry for the super duper late reply. I have been in the process of moving to a different city and just finally got all settled back in. I was planning on doing the single motor set up.

It looks like instead of using the Acton ESC you got the Maytech VESC instead. Did you still use the Acton board battery?
```

---
## \#19 Posted by: Tomer Posted at: 2017-09-14T03:39:33.137Z Reads: 36

```
Yes I still use this battery until I'll build a better one. 
I actually upgarded the Acton battery and added 10 more 18650 cells making it 10S1P.
```

---
