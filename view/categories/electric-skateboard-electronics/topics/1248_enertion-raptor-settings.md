# Enertion raptor settings?

### Replies: 9 Views: 1497

## \#1 Posted by: Nasty Posted at: 2016-02-06T21:59:26.564Z Reads: 125

```
Ok I don't know much, but hopefully someone can help me out. First time I stepped on my raptor softly accelerated, I literally did not move an inch, and the motor vibrated like crazy(I'm sure you've guys have seen this before). So basically 50% of the time, it will actually take off from a stop. So while riding and having the best feeling ever, I had to suddenly brake, which the raptor did do. But the only problem was while braking, it feels like it would skip(not brake) for half a second which is bloody dangerous. All batteries were charged, so I knew it couldn't be that. 

Also does the raptor use foc or bldc? Also what discovery board do you guys recommend? I'm curious if you turn off regen braking, if that would improve my braking.

I hate to say it, but my friends boosted it lightyears ahead of this current set up I have... Help me fall in love with these sensorless motors!
```

---
## \#2 Posted by: Nasty Posted at: 2016-02-06T22:20:38.143Z Reads: 123

```
An option for reverse would be cool too...
```

---
## \#3 Posted by: onloop Posted at: 2016-02-07T02:49:18.913Z Reads: 113

```
Well doesn't sound like you have had a great first experience.. sorry about that.

sorry to ask a very personal question, but how much do you weigh?

There are definitely situations that will make the motors vibrate. Most commonly when trying to start from absolute zero momentum, even worse if there is a slight incline that makes the board roll (or want to roll) backwards. So avoid that.

Also, not getting the timing right with the accelerator, not enough power will cause the motor to semi-stall & vibrate. Too much and you can go flying on your arse.

Maybe you could make a video to better illustrate what it's doing.

The VESC is setup as BLDC, FOC is not quite ready yet for production boards yet.

If you turn off regen you will not have brakes at all. Regen is the only brake method. Making regen current weaker might be better. Once again this is something that rider weight will dictate, if you are heavy & the brake is strong the belt could skip. Applying the brake gradually there will not be any issues. I have the raptor setup for what feels good to me, I'm 95kg.

I don't use a discovery board, I use a USB cable & windows.

My tips for you would be to keep riding the board and learning its characteristics. I suppose this situation could be similar to when you take someone else's manual transmission car for a first time drive and you try to drive it smoothly without stuffing up the braking, accelerating, gear changing etc... but because its new or different you don't do things they way the car wants to have them done so the ride isn't so smooth.


hope this info helps.
```

---
## \#4 Posted by: onloop Posted at: 2016-02-07T02:58:14.132Z Reads: 107

```
is this a dual or mono?
```

---
## \#5 Posted by: cmatson Posted at: 2016-02-07T03:06:40.112Z Reads: 108

```
[quote="Nasty, post:1, topic:1248"]
First time I stepped on my raptor softly accelerated, I literally did not move an inch, and the motor vibrated like crazy
[/quote]

This is what happens when you don't give the VESC enough throttle... The motor will jitter back and forth for a second, and then start moving. If you either give a little push (which I **VERY HIGHLY** recommend doing at all times anyways...) it will start up right away. 

Alo, do you have a mono or dual Raptor? With my single drive board I'll notice that sometimes when I brake hard the single wheel will skid for a second before slowing me down. Graduallly applying the brakes (and not just slamming on them) gets rid of this problem. 

I'm sure once you get used to the Raptor you will be riding circels around that boosted board :wink: 

Similar to @onloop's analogy: driving a high performance car vs your average city sedan. The brakes are way better, but more sensitive as well; same goes for the throttle and paddle shifters...
```

---
## \#6 Posted by: Nasty Posted at: 2016-02-07T21:38:30.439Z Reads: 95

```
I see what you guys mean in terms of having to pretty much deal with it. After really sitting back and absorbing more information on the forum, I would call this a learning experience instead of a bad experience. I have too many hobbys as it is, and the last thing I wanted to do is learn something new(due to lack of time). Good thing is this hobby isn't too much different than my current ones. Eboarding is so much fun that I can't resist. I see what you mean Onloop, after riding I learned to adjust to the board and its characteristics. Cmatson your right, I have the mono, and ever since I broke in the rubber, I haven't slipped or lost grip. Off course It helps to be sensitive with the brakes. I'm excited to jump into bldc tools! I love the freedom of tinkering with specs to my desire. Btw I weigh 203lbs :smile: and this mono definitely does the job up any hill, it's a beast. Definitely happy with my purchase. I can't wait to try and maybe adjust the throttle sensitivity, but most importantly, I want reverse ..that is possible, right guys?
```

---
## \#7 Posted by: onloop Posted at: 2016-02-07T22:27:51.666Z Reads: 91

```
I am glad to hear that you are open minded...

Another analogy; boosted is like a consumer grade production car you buy and drive miss daisy around on. Raptor is raw unfiltered drag car that you need to respect and caress in a certain manner or your hand gets bitten.

Once you have worked out the correct ways you will never look back.. and your mate with boosted will be very jealous. You can ride twice as fast and three times further than him.
```

---
## \#8 Posted by: onloop Posted at: 2016-02-07T22:31:06.436Z Reads: 87

```
Also. Just be careful with BLDC tool. It is possible to kill the vesc by changing wrong settings.
```

---
## \#9 Posted by: Nasty Posted at: 2016-02-07T22:33:09.149Z Reads: 86

```
Yes thanks, I've already read a couple of horror story's. Will be careful for sure.
```

---
