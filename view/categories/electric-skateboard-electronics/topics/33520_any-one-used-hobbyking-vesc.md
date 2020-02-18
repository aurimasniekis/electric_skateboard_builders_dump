# Any one used HobbyKing Vesc?

### Replies: 41 Views: 4024

## \#1 Posted by: notepad Posted at: 2017-09-19T20:53:32.837Z Reads: 339

```
Im planning on building my first 4 motor board but I cant really afford multiple Vesc 6's like my current board.

So I was planning on getting the hobbyking ones as they seem nice and cheap.
https://hobbyking.com/en_us/turnigy-skateboard-esc.html

anyone used them, if so,  how are they?
```

---
## \#2 Posted by: BoostedBuilder Posted at: 2017-09-19T21:33:48.751Z Reads: 324

```
How are you planning to get it if it's out of stock?
```

---
## \#4 Posted by: notepad Posted at: 2017-09-19T21:50:12.072Z Reads: 312

```
Waiting untill its back into stock.
```

---
## \#5 Posted by: BoostedBuilder Posted at: 2017-09-19T21:53:51.110Z Reads: 302

```
Do you know when it's coming back into a stock?
```

---
## \#6 Posted by: faithfulpuppy Posted at: 2017-09-19T22:06:36.617Z Reads: 294

```
the hobbyking esc is $90 for 4.10 hardware.  you're probably better off buying a tb vesc for $100 that's in stock, nicer looking, probably better supported, and is 4.12
```

---
## \#7 Posted by: notepad Posted at: 2017-09-19T22:25:47.178Z Reads: 294

```
Originally I was going to be going with either a maytech Vesc,  or the hobbyking 150A ESC.  The problem is Im trying to build the board as cheaply as possible and the HK150A isnt rated for 12S and the maytech is slightly more expensive than the HK4.10
```

---
## \#8 Posted by: GrecoMan Posted at: 2017-09-19T22:35:13.908Z Reads: 288

```
Get the torqueboards vesc. The Hobbyking one is only a good cooker
```

---
## \#9 Posted by: JdogAwesome Posted at: 2017-09-19T22:39:58.660Z Reads: 281

```
So far my Maytech VESC has been great and there only $89 if you email them directly. I personally haven't heard anything good about the HK VESC s so I think the Maytech VESC would probably be a better option. And also I think if your trying to do a 4 wheel drive board you shouldn't be going cheap on components lol.
```

---
## \#10 Posted by: notepad Posted at: 2017-09-19T22:54:11.326Z Reads: 269

```
I think I might have to upgrade to the Maytech.  The only reason I decided not to go with it was its slightly more expensive ( plus id have to pay customs when I import it to the uk )  And some of the bad things I have heard from people about them dying ( The chip not the rider :P ).
```

---
## \#11 Posted by: faithfulpuppy Posted at: 2017-09-19T22:54:59.427Z Reads: 259

```
>some of the bad things I have heard from people about them dying.

still gonna be a lot better than HK.  I'll get really excited when HK starts producing 4.12 hardware though
```

---
## \#12 Posted by: notepad Posted at: 2017-09-19T22:56:26.794Z Reads: 245

```
But do you get a warrenty with Maytech,  If so I dont have any reason not to go with them.  All I know is HK give atleast some form of warrenty ( except batteries )
```

---
## \#13 Posted by: faithfulpuppy Posted at: 2017-09-19T22:56:59.822Z Reads: 236

```
i'm not really sure
```

---
## \#14 Posted by: SilentException Posted at: 2017-09-19T22:57:42.810Z Reads: 235

```
Frankly, you could probably put the missing capacitor yourself if you want 4.12 :)
```

---
## \#15 Posted by: faithfulpuppy Posted at: 2017-09-19T22:59:04.755Z Reads: 222

```
is that the only difference? i'm not aware of the technical differences, only that 4.12 is supposedly way more reliable
```

---
## \#16 Posted by: notepad Posted at: 2017-09-19T22:59:35.390Z Reads: 222

```
Its mostly because if the Hk one blows I have 6-12 months worth of warrenty to replace / refund.

@SilentException  What diffrences are there between 4.10 and 4.12 exactly.  if its a simple as an extra capacitor, I could always add that myself?
```

---
## \#17 Posted by: SilentException Posted at: 2017-09-19T23:01:00.808Z Reads: 220

```
Well, that and one trace was thickened 4.10->4.11
```

---
## \#18 Posted by: faithfulpuppy Posted at: 2017-09-19T23:02:14.049Z Reads: 214

```
[huh, whaddya know](http://vedder.se/forums/viewtopic.php?t=124)

guess it's a really important trace
```

---
## \#19 Posted by: SilentException Posted at: 2017-09-19T23:03:22.712Z Reads: 215

```
Most important :)
```

---
## \#20 Posted by: onepunchboard Posted at: 2017-09-19T23:05:41.213Z Reads: 211

```
hk and meytech only good for bldc
```

---
## \#21 Posted by: notepad Posted at: 2017-09-19T23:10:07.404Z Reads: 207

```
It seems its alot more complicated than just a single capacitor :confused:
```

---
## \#22 Posted by: faithfulpuppy Posted at: 2017-09-19T23:12:42.219Z Reads: 194

```
[straight from the horse's mouth](http://vedder.se/forums/viewtopic.php?t=124)
```

---
## \#23 Posted by: SilentException Posted at: 2017-09-19T23:13:15.904Z Reads: 197

```
[quote="notepad, post:21, topic:33520"]
It seems its alot more complicated than just a single capacitor :confused:
[/quote]

Hm, what? Differences between 4.10 and 4.12 is thickened trace and one capacitor.

It is clearly written by the man himself in the thread linked:

> 4.10 - 4.12 are very similar and use the same firmware. The difference from 4.10 to 4.11 is that I made a trace thicker, and the difference from 4.11 - 4.12 is that I added a capacitor to GVDD on the DRV8302
```

---
## \#24 Posted by: notepad Posted at: 2017-09-19T23:22:45.292Z Reads: 197

```
The capacitor part is simple, but doesnt the trace part must be important otherwise it wouldnt have been added.  since I would be using 12S,  the chance of arcing and heat generation is higher so wouldnt the thicker trace be a must?
```

---
## \#25 Posted by: SilentException Posted at: 2017-09-19T23:33:25.786Z Reads: 200

```
This is a GitHub commit for the change: https://github.com/vedderb/bldc-hardware/commit/4395c66f4929cf9926a376f03ca1977379c8d233#diff-31c13f47ad87dd7baa2d558a91e0fbb9

> Small update of trace, no significant changes

I don't think it is _that_ important ;)

Here is a nice game, can you spot the difference :slight_smile:

<img src="/uploads/db1493/original/3X/b/a/ba7a7c8669a038e9b04f062cedbd59237fca3c8d.png" width="307" height="456"> 

<img src="/uploads/db1493/original/3X/5/6/56f04d70e49401da595d06d7b464815019810bcf.png" width="294" height="454">
```

---
## \#26 Posted by: notepad Posted at: 2017-09-19T23:35:46.521Z Reads: 180

```
I think I have found it.  is it on the right bridge part?
```

---
## \#27 Posted by: jmasta Posted at: 2017-09-20T03:42:13.884Z Reads: 173

```
When you factor in that it comes with a one year warranty, it's actually a pretty good deal. Often that is an additional $60-70
```

---
## \#28 Posted by: notepad Posted at: 2017-09-20T19:15:47.985Z Reads: 163

```
Thats the only reason I was planning on going for Hk instead of maytech as if I run it into the ground I can just get a refund.
```

---
## \#29 Posted by: Lumaci Posted at: 2017-09-20T19:43:28.962Z Reads: 157

```
Get the torqueboards one instead :-) I just had a talk with an owner of both HK and maytech ones he upgraded to the torqueboards one and he is never going back.

And it's not that much more :-)
```

---
## \#30 Posted by: notepad Posted at: 2017-09-20T20:21:41.348Z Reads: 156

```
The only problem with that is its atleast £40 more expensive than the HK and doesnt include shipping or a wanntey unless I shellout another £60.  PLus it doest tell me how much shipping actually is and I would still need to pay import tax.  The niceity of the Hk is its shipped within Eu and is much cheaper with a warrenty.

If I had more money to spend on this project I would definitely get 4 more vesc 6's as I already have 1 and its amazing. but I am trying to keep the cost of the board down to a minium  without sacrificing quality ( or spending extra after a vesc blows )
```

---
## \#31 Posted by: Lumaci Posted at: 2017-09-20T20:24:05.806Z Reads: 156

```
The torqueboards wont really blow unless you really do something bad, also i ordered mine outside of US / In EU and i dont expect to pay anything high in import duty at all since they label the price at 35 USD When shipping :-)
```

---
## \#32 Posted by: notepad Posted at: 2017-09-20T20:26:35.362Z Reads: 153

```
[quote="Lumaci, post:31, topic:33520"]
since they label the price at 35 USD When shipping
[/quote]

Thoes cheeky buggers.

Problem still is its quite a price hike for a cheap project. the jump from £62 to £100 isnt as drastic for one chip. but thats a £120 jump over 4.  Would you say its really worth the extra cash for marginal performance gain?
```

---
## \#33 Posted by: jmasta Posted at: 2017-09-20T20:27:44.375Z Reads: 151

```
Yeah that's not true. I did everything by the book. Conservative limits. Never even considered FOC.  Even powered it for the first time with a certified lab power supply.  Yet my VESC from Torqueboards still failed
```

---
## \#34 Posted by: bigben Posted at: 2017-09-20T20:29:12.810Z Reads: 151

```
I have a brand new torque and a used maytech for sale here.
http://www.electric-skateboard.builders/t/vescs-for-sale-uk-eu-price-drop/32248
```

---
## \#35 Posted by: notepad Posted at: 2017-09-20T20:32:06.046Z Reads: 148

```
OOO very interesting.  I might have to pop you a pm!
```

---
## \#36 Posted by: BoostedBuilder Posted at: 2017-09-20T20:50:14.791Z Reads: 144

```
I'm considering getting 4 for myself, if I add 4 for you we could get the price down to perhaps $90. Would you be interested?
```

---
## \#37 Posted by: notepad Posted at: 2017-09-20T20:58:37.658Z Reads: 149

```
Unfortunatly thats still quite a high price when you factor in shipping to the uk and what not.   to be honnest I was planning on getting a single one to start with to check quality.   So I am going to have to politely decline :/   

(that and the reason I was asking about the vescs isnt because of a 4wd board Like I mentioned.  its actually for a super cool project that will be posted up in the next month or two using multiple motors onto a single wheel to create a super quick racer )
```

---
## \#38 Posted by: BoostedBuilder Posted at: 2017-09-20T21:14:51.307Z Reads: 143

```
I'm not insisting or whatever, but 90 including shipping. You would have them in the U.K. for $360 total.
```

---
## \#39 Posted by: notepad Posted at: 2017-09-20T21:16:49.349Z Reads: 143

```
Thats actually an amzing deal. If I had the cash right now I would say yes to that.. unfortuantly I dont, so this post was mostly intended as research into which ones to get.
```

---
## \#40 Posted by: Lumaci Posted at: 2017-09-20T21:36:33.085Z Reads: 146

```
When did it happen? I've seen them been running with Foc no problem if it's a little while ago it's the older versions before they upgraded caps and bootloader and more.
```

---
## \#41 Posted by: Pedrodemio Posted at: 2017-09-20T22:00:36.643Z Reads: 139

```
Same for me, DRV error in the detection, never managed to spin the motor, is has warranty, but if you are from outside the states you have to return it at your own cost, not worth
```

---
## \#42 Posted by: UKRider Posted at: 2018-08-26T10:42:20.191Z Reads: 45

```
I have been using the Hobby king VESC 4.12 and it's works fine. I run a 6S setup with 270KV motor and 90mm wheels. Good cheaper option it's my first build and I'm very satisfied
```

---
