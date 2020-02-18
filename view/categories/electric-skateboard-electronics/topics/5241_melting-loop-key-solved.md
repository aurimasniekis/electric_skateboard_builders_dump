# Melting loop key? SOLVED

### Replies: 126 Views: 6601

## \#1 Posted by: barajabali Posted at: 2016-06-28T00:20:32.372Z Reads: 550

```
Magic smoke came from my new xt90 anti spark loop key. 

This is my first time using this so I prob did it wrong lol I plugged it in and my motors were moving very slow and then the male "key" with the resistor started smoking.

What did I do wrong 
Do I have to have the live wire at a particular end of this ? Or can it go on either end 
<img src="/uploads/db1493/original/2X/2/23b22beb2a08aae7b9fc5990a31a9c7c973eb242.jpeg" width="375" height="500"><img src="/uploads/db1493/original/2X/b/bb62765de7ca6064652719a72bbb3bd4ba0a2f1f.jpeg" width="375" height="500">
```

---
## \#2 Posted by: lox897 Posted at: 2016-06-28T00:21:31.987Z Reads: 498

```
It might be a similar problem to @whitepony 
Something about the loop wire being to big.
```

---
## \#3 Posted by: barajabali Posted at: 2016-06-28T00:22:00.980Z Reads: 502

```
I missed that thread let me look for it
```

---
## \#4 Posted by: lox897 Posted at: 2016-06-28T00:22:50.873Z Reads: 500

```
It's on ES somewhere. On one of his build threads I think.
```

---
## \#5 Posted by: lox897 Posted at: 2016-06-28T00:27:12.515Z Reads: 491

```
This is what he said:

about the loop key: I know quite well why my loop exploded and yours worked: my loop was too large! most of you directly bridge the 2 soldering joints of the XT90s plug and then attached something to pull the plug out again. I thought I just use a cable and wind it in a slightly larger loop, so that I can use it to pull the plug out at the same time. the problem is, that the inductance of a single wire loop is increasing with loopsize (~ radius*log(radius)), so the inductance of my loop key was much larger than that of most others.
```

---
## \#6 Posted by: barajabali Posted at: 2016-06-28T00:28:42.213Z Reads: 476

```
Oh no way! So I have to do a direct bridge and it will work? 

Do you know if it matters to which side the live wire is?
```

---
## \#7 Posted by: lox897 Posted at: 2016-06-28T00:30:20.151Z Reads: 464

```
I don't think it matters. Yeah, direct bridge. @whitepony probably knows more about it than me.
```

---
## \#8 Posted by: barajabali Posted at: 2016-06-28T00:33:59.187Z Reads: 455

```
Gonna try it right now made a new key
```

---
## \#9 Posted by: lox897 Posted at: 2016-06-28T00:35:10.704Z Reads: 451

```
Tell me how it goes.
```

---
## \#10 Posted by: barajabali Posted at: 2016-06-28T00:35:59.965Z Reads: 449

```
Didn't work melted again lol I tried a new one
```

---
## \#11 Posted by: barajabali Posted at: 2016-06-28T00:37:21.459Z Reads: 457

```
<img src="/uploads/db1493/original/2X/a/a353a1e4cf9b51971c102e0cba474aa2a520b876.jpeg" width="375" height="500">

I cut the red wire from the old loop key since its toast. I need to order more now hahah
```

---
## \#12 Posted by: lox897 Posted at: 2016-06-28T00:41:10.177Z Reads: 452

```
What about trying the power from the batteries on the other side? Is there a resistor on one side?

This problem only happens with the XT90S. Could it be something to do with the resistor?
```

---
## \#13 Posted by: barajabali Posted at: 2016-06-28T00:47:30.716Z Reads: 451

```
It might be that I need to put the power on the other side but I have no more to test it out. They cost 12 dollars for a pair lol I'll have to order more. 

I went ahead and made me a temp regular xt90 key so I can use the board it works fine <img src="/uploads/db1493/original/2X/8/849eed21b4c773ef66519f868f96877ea602ab58.jpeg" width="375" height="500">
```

---
## \#14 Posted by: lox897 Posted at: 2016-06-28T01:21:05.167Z Reads: 439

```
Could it also be that you are doing it on the positive side maybe?
```

---
## \#15 Posted by: lowGuido Posted at: 2016-06-28T02:16:47.104Z Reads: 439

```
Shouldnt really matter what side.. i have a sneaking suspicion that these XT90s are not up to task. They use only very small smd resistors. I don't think high voltage e skateboards were in mind when they were designed.
I have no proof of this.. just a theory.
```

---
## \#16 Posted by: barajabali Posted at: 2016-06-28T02:21:22.145Z Reads: 440

```
only reason i got them is because ive seen them in a lot of builds I thought they worked pretty well lol. 

@GhettoFab.rictation  I installed one of these in your series connector so let me know if it works or not!
```

---
## \#17 Posted by: cmatson Posted at: 2016-06-28T03:11:00.272Z Reads: 431

```
I had wire about that long on my loop key, and everything worked fine- 

I think it's what @lowGuido said, that the xt90's simply can't handle it.
```

---
## \#18 Posted by: Nowind Posted at: 2016-06-28T03:11:08.768Z Reads: 446

```
Hey.
This XT90 work good with 12S, never had any issues with it when directly bridged:

<img src="/uploads/db1493/original/2X/3/37f9524b3ce4d63c5484388134fe29e164fbbe46.JPG" width="666" height="500">

<img src="/uploads/db1493/original/2X/0/0f62287528c5f10f42dd39a1970b4b7627fbfce0.JPG" width="666" height="500">

<img src="/uploads/db1493/original/2X/2/24f76ad24e287f3f0c2ed129912c5fbb14bc0003.JPG" width="666" height="500">

In my Drift Trike with 20S they are reaching there limits :joy:
```

---
## \#19 Posted by: barajabali Posted at: 2016-06-28T03:23:08.800Z Reads: 435

```
Does it have to be connected in a certain way? In terms of the live wire? Maybe live wire to positive? Not sure what I put it on tbh
```

---
## \#20 Posted by: Karmannghiagirl Posted at: 2016-06-28T03:27:14.426Z Reads: 441

```
ok, if i remember correctly it is not a resistor in there, it is a capacitor. resistors dont care about polarity, capacitors do.

swap the wires going into the plug on the board side and you should be good.
```

---
## \#21 Posted by: barajabali Posted at: 2016-06-28T03:28:21.300Z Reads: 422

```
i will try it when i get home.  im gonna try one of the ones that i toasted and see if it works.  its only slightly toasted. just how i like my bread mmmm
```

---
## \#22 Posted by: whitepony Posted at: 2016-06-28T04:07:21.485Z Reads: 431

```
[quote="Karmannghiagirl, post:20, topic:5241"]
ok, if i remember correctly it is not a resistor in there, it is a capacitor. resistors dont care about polarity, capacitors do.
[/quote]

hmm, interesting :no_mouth:

very observant @lox897  is right, i was plagued by the same issues and, while the size of the loop increases inductance, i calculated it in a later post and it looked insignificant. cant remember if loop keys had a +- stamped on them ... or an electron flow direction in the ++ or -- loop key scenario?

fact is: i still havent understood my problem and i left out the loop key ultimately. besides melting keys i had large induced voltages that killed one of my vescs. you could see that in the bench test live monitor: revving up and the battery voltage plummets, stopping the motor and it skyrockets way beyond the battery voltage. my 2nd loop key didnt have that inductance problem, but it also got hot.
```

---
## \#23 Posted by: Mobutusan Posted at: 2016-06-28T04:41:22.101Z Reads: 430

```
Hmm, maybe @Karmannghiagirl is right about the XT90s being directional. Which side of the key is your battery on, positive or negative? I just checked my loop key and I have the battery coming in on the negative side of the connector and the positive side going to the esc. It also looks like there might be some black carbon buildup inside the positive terminal of the key where the green capacitor or resistor is located. I'm only running this on 6s though, so maybe that's why I haven't had it burn up yet? You're running 10s, right?
```

---
## \#24 Posted by: Nowind Posted at: 2016-06-28T05:01:32.113Z Reads: 425

```
I place it in the positive wire.
The battery sits on the negative side:
<img src="/uploads/db1493/original/2X/5/5b136cabe66d0664abe6b5e3d03f898b0fba474f.jpg" width="580" height="486">
```

---
## \#25 Posted by: lox897 Posted at: 2016-06-28T05:15:21.752Z Reads: 413

```
@Karmannghiagirl I just did a bit of research on it. It is a resistor.
```

---
## \#26 Posted by: lowGuido Posted at: 2016-06-28T05:20:28.690Z Reads: 404

```
It has to be a resistor. Putting a cap in makes no sense. It needs to limit the inrush current to stop the spark.
```

---
## \#27 Posted by: lox897 Posted at: 2016-06-28T05:21:12.361Z Reads: 408

```
And now you have a scientific explanation... Jeez your good @lowGuido
:joy:
```

---
## \#28 Posted by: barajabali Posted at: 2016-06-28T05:27:36.412Z Reads: 401

```
Im gonna try this tomorrow thanks for the diagram
```

---
## \#29 Posted by: barajabali Posted at: 2016-06-28T05:28:07.654Z Reads: 385

```
Im not sure and now im flooded with studying so I will let you know tomorrow and ill try to fix it :)
```

---
## \#30 Posted by: barajabali Posted at: 2016-06-28T05:28:17.399Z Reads: 387

```
and yes 10s
```

---
## \#31 Posted by: Karmannghiagirl Posted at: 2016-06-28T06:08:22.811Z Reads: 387

```
thinking about it that does make more sense :sweat_smile:
```

---
## \#32 Posted by: Mobutusan Posted at: 2016-06-28T06:17:47.641Z Reads: 399

```
Ok, I thought it was a resistor. All this talk about melting loop keys and capacitors had me second guessing myself. If I'm not mistaken, once the connector is fully engaged, all the current flows around the resistor. But maybe the main connector isn't engaging/connecting and forcing all or most of the current through the resistor? Not sure what else it could be unless there is massive current draw overloading the connector, but aren't these rated for like 90 amps continuous? 

And fwiw, my setup looks pretty much like @nowind except I'm using XT60s for the battery connections.
```

---
## \#33 Posted by: trbt555 Posted at: 2016-06-28T06:20:44.178Z Reads: 406

```
[quote="lox897, post:5, topic:5241, full:true"]
This is what he said:

about the loop key: I know quite well why my loop exploded and yours worked: my loop was too large! most of you directly bridge the 2 soldering joints of the XT90s plug and then attached something to pull the plug out again. I thought I just use a cable and wind it in a slightly larger loop, so that I can use it to pull the plug out at the same time. the problem is, that the inductance of a single wire loop is increasing with loopsize (~ radius*log(radius)), so the inductance of my loop key was much larger than that of most others.
[/quote]

That is way too far fetched.
```

---
## \#34 Posted by: lox897 Posted at: 2016-06-28T06:21:18.294Z Reads: 409

```
That was @whitepony 's theory. He quickly realised that it wasn't correct.
```

---
## \#35 Posted by: DeathCookies Posted at: 2016-06-28T06:22:04.574Z Reads: 414

```
I had the very same problem and everbody told me: "it does not matter how you plug the loop key in"...

Well it did make an difference for me. Here is the [thread](http://www.electric-skateboard.builders/t/xt90-s-loop-key-short-circuit/2383) and to conclude the problem i made the following picture:
<img src="/uploads/db1493/original/2X/d/dc591679dc8878a9e7db87011ae897ed8a9b3c7c.jpg" width="690" height="372">

To put it in a nutshell i made the following diagramm:
<img src="/uploads/db1493/original/2X/e/ecf94ce16a0b380d5f00af81ace48a01e23d64f4.jpg" width="689" height="242">

here you can see that the polarity of the XT-90S needs to be switched. Otherwise it melts like mine or yours.

I hope i could help.

PS: Before someone says that this is not the problem please test both wirings and report back ;)
```

---
## \#36 Posted by: barajabali Posted at: 2016-06-28T06:25:57.823Z Reads: 406

```
Great! So it must be a polarity issue then! Thanks for the shared wisdom. 

I noticed you had yours set up as a break in a serial connection. I have one battery and I am putting my xt90s as a break in the positive lead. Which side in that situation would you believe gets the positive side of the xt90s? The live wire gets the + or the severed wire?
```

---
## \#37 Posted by: DeathCookies Posted at: 2016-06-28T06:36:29.159Z Reads: 393

```
Actually i do not really know. I would guess that you connect the xt-90s positive with the positive battery cable and the xt-90s negative with the esc. Then it is like mine except two batteries and you put it in the positive wire.
But i dont give you guarantee.
```

---
## \#38 Posted by: Mobutusan Posted at: 2016-06-28T06:43:05.110Z Reads: 391

```
So, sounds like it's a combination of incorrect connector configuration and higher voltage, like 10s or 12s?
```

---
## \#39 Posted by: DeathCookies Posted at: 2016-06-28T06:46:16.249Z Reads: 390

```
I dont think the voltage matters... I think it was just the wrong polarity...
EDIT: But i dont think you can use 100S with a XT-90S ;)
```

---
## \#40 Posted by: barajabali Posted at: 2016-06-28T07:09:05.596Z Reads: 380

```
Switched polarity same results.... I might just keep the regular xt90 and let it spark and I'll swap it out ever few months
```

---
## \#41 Posted by: DeathCookies Posted at: 2016-06-28T07:10:49.577Z Reads: 357

```
[quote="barajabali, post:40, topic:5241"]
Switched polarity same results
[/quote]

Did you test it right now? After i switched the polarity of my xt-90s my 12s setup is working flawlessly in FOC :)
```

---
## \#42 Posted by: barajabali Posted at: 2016-06-28T07:12:01.047Z Reads: 350

```
Yes I just did. So I think the issue is that there is no "polarity" this loop key is just an interupt in the positive wire. So there is no negative just a positive wire and a wire that is not connected.
```

---
## \#43 Posted by: Nordle Posted at: 2016-06-28T07:12:10.311Z Reads: 347

```
There is just a resistor in it, and resistors don't have a polarity ;)
```

---
## \#44 Posted by: barajabali Posted at: 2016-06-28T07:13:12.855Z Reads: 343

```
I just don't think it works in the specific way I installed it. As an interupt loop key. It just breaks and closes the circuit
```

---
## \#45 Posted by: barajabali Posted at: 2016-06-28T07:14:02.451Z Reads: 338

```
I noticed you all used it in a manner that had a negative. My situation has no negative so that's got to be why it doesn't work
```

---
## \#46 Posted by: DeathCookies Posted at: 2016-06-28T07:14:49.404Z Reads: 336

```
You mean it should be installed in the negative wire? I cannot test it right now but i would appreciate the result!
```

---
## \#47 Posted by: barajabali Posted at: 2016-06-28T07:15:49.946Z Reads: 336

```
I think it needs to be connected to both the negative and positive wire. So just connecting it as an interupt in one wire it will just melt.

Even tho a regular xt90 will be able to close the curcuit, an xt90s won't it seems in this particular application
```

---
## \#48 Posted by: DeathCookies Posted at: 2016-06-28T07:17:57.004Z Reads: 329

```
[quote="barajabali, post:47, topic:5241"]
I think it needs to be connected to both the negative and positive wire. So just connecting it as an interupt in one wire it will just melt.
[/quote]

Many people use a XT-90S as loop key (= interrupt !?) and have no problems at all. I do run 12S with the wiring i showed above and have no problems....
Maybe some faulty XT-90S??
```

---
## \#49 Posted by: Nordle Posted at: 2016-06-28T07:19:57.926Z Reads: 325

```
Maybe.. can you break one appart and show us whats burned? I really can't immagine what went wrong here.
_double checked all your power and balance wires?_
```

---
## \#50 Posted by: Maxid Posted at: 2016-06-28T07:21:00.784Z Reads: 322

```
An interrupt IS connecting positive and negative wire. Do you know how electricity works?
```

---
## \#51 Posted by: barajabali Posted at: 2016-06-28T07:21:14.347Z Reads: 321

```
I'd be happy to. Tomorrow though it's 2:20 am here this thing is keeping me up! Lol
```

---
## \#52 Posted by: barajabali Posted at: 2016-06-28T07:23:35.654Z Reads: 326

```
Yes I do know how electricity works no need to be rude. 

I will post pictures tomorrow about what I'm doing and maybe you'll get the picture better if I'm not explaining it clearly enough.
```

---
## \#53 Posted by: Maxid Posted at: 2016-06-28T07:25:27.910Z Reads: 318

```
Did not mean to be rude. Just wanted to actually ask. This is a serious topic - you are dealing with high voltages AND high amps, so misinformation can be life threatening. Your statement sounded like you do not know what you are doing there.
```

---
## \#54 Posted by: barajabali Posted at: 2016-06-28T07:26:32.257Z Reads: 310

```
Lol yes... This doesn't concern balance leads or the battery at all in fact.
```

---
## \#55 Posted by: whitepony Posted at: 2016-06-28T07:30:22.133Z Reads: 309

```
just cause you break "++" still means you connect + and - in that moment basically! the battery "+" side of the XT90S will be "+", the other side "-". when Im back home Ill check how I added the loop key into my setup. it would be such a relief to finally understand whats going on with these keys.
```

---
## \#56 Posted by: barajabali Posted at: 2016-06-28T07:30:25.835Z Reads: 309

```
37 volts won't kill me. Not to mention DC volts. 
I'm not new here. I work with these things on a daily basis. This just seems to be something that cannot be done with my present application.
```

---
## \#57 Posted by: barajabali Posted at: 2016-06-28T07:31:14.157Z Reads: 306

```
Agreed. I've done shit many times more complicated than this little thing but it's just throwing me off. So simple yet so annoying.
```

---
## \#58 Posted by: barajabali Posted at: 2016-06-28T07:33:29.439Z Reads: 305

```
As I mentioned before. It the xt90s does work! I get a voltage reading and my wheels spin and all but it moves very slowly and if I exert it too much it melts. I get the same result regardless of polarity because as previously stated is a resistor which doesn't concern polarity.
```

---
## \#59 Posted by: whitepony Posted at: 2016-06-28T07:44:30.914Z Reads: 307

```
can you read live voltage monitor of the vesc when you rev the motor up? check how much the voltage sags, then try to brake the engine from full speed and check how much the voltage jumps up. you might have the exact same symptoms I have experienced.

the funktioning loop keys used smaller loops from one solid thick copper wire whereas we used highly flexible silicone wires with larger loops. maybe there is something to that?
```

---
## \#60 Posted by: Maxid Posted at: 2016-06-28T07:45:13.341Z Reads: 311

```
What does exert too much mean? There is a 5.6Ohm resistor in there - At 42V there will be a current of 7.5A going through that little resistor which will heat up quickly. They are not made to hold that constantly but just for the initial connection. If you exert it too much and the current flows through the resistor constantly it will obviously melt.

Edit: Sorry I thought exert meant to pull the plug - just looked up the word and it means something different.
```

---
## \#61 Posted by: whitepony Posted at: 2016-06-28T07:46:53.117Z Reads: 284

```
the resistor shouldnt be involved once you plug the XT90 in completely. just the tip has Business with a resistor or capacitor or whatever magic device it is. :stuck_out_tongue:
```

---
## \#62 Posted by: barajabali Posted at: 2016-06-28T07:48:39.805Z Reads: 287

```
The resistor isn't bearing any of the load ( or so it shouldn't be after the initial connection)  it maybe it a. Problem of me not plugging the key in far enough maybe...
```

---
## \#63 Posted by: Maxid Posted at: 2016-06-28T07:48:49.533Z Reads: 288

```
yeah mixed up the words - I am sorry
```

---
## \#64 Posted by: Maxid Posted at: 2016-06-28T07:50:56.130Z Reads: 290

```
Maybe you could increase resistor size like someone did on endless:
https://endless-sphere.com/forums/viewtopic.php?f=35&t=63210#p1048110
```

---
## \#65 Posted by: barajabali Posted at: 2016-06-28T07:51:52.808Z Reads: 291

```
Now that we know in theory AND practice that it is not polarity. It must be something else.  

Honestly it might be that I didn't plug it in all the way. LOL it's a tight fit and the last mm or 2 is hard to get all the way in. I totally didn't realize that that actually matters with anti sparks. Whoops. Will try that tomorrow. 

I think the little resister is taking the load which is obviously can't bear much of without melting.
```

---
## \#66 Posted by: barajabali Posted at: 2016-06-28T07:52:42.874Z Reads: 280

```
Thanks buddy that will be my plan B :)
```

---
## \#67 Posted by: barajabali Posted at: 2016-06-28T08:01:48.420Z Reads: 283

```
Hahaha I regret to inform you all that it worked all along.... It just needed to be filed down a little to plug 100% in. Those last mm's actually made all the difference.

My dumb ass. Making my mistakes all public and shit. 

Thanks anyway everyone!
```

---
## \#68 Posted by: whitepony Posted at: 2016-06-28T08:03:20.395Z Reads: 281

```
I dont think its a resistor problem, because that shouldnt really play a role after the xt90m is fully plugged in. maybe its really the fine copper strand silicone wire. the high voltage sag/jump I saw in the vesc live Monitor (clearly inductance effect!) made me think it must be a loop size thing, but after I played around with https://www.eeweb.com/toolbox/loop-inductance/ I saw that the inductance of 20cm straight wire is much higher than a 2cm loop.

however, if you decrease the wire thickness the inductivity rises and its proportional to the wire windings, so many many small windings in that loop would actually increase the inductance by a lot!

what I would try next is, using one solid copper wire for the loop and check if the voltage sag/heat thing persists. if thats the case, then there must be something fishy going on with the small strands in the silicone wires.
```

---
## \#69 Posted by: whitepony Posted at: 2016-06-28T08:04:17.040Z Reads: 280

```
[quote="barajabali, post:67, topic:5241"]
Hahaha I regret to inform you all that it worked all along.... It just needed to be filed down a little to plug 100% in. Those last mm's actually made all the difference.
[/quote]

hm, ok :stuck_out_tongue:
```

---
## \#70 Posted by: barajabali Posted at: 2016-06-28T08:05:41.671Z Reads: 269

```
Oh and I tested it with about a 2 inch diameter loop just for shits and giggles and it works fine. And my loops are much smaller than 2 inches in diameter. So that shouldn't be an issue
The wire was made of 10 gauge super worm wire FYI
```

---
## \#71 Posted by: whitepony Posted at: 2016-06-28T08:10:00.349Z Reads: 265

```
im not satisfied with this outcome - I know that my loop key was plugged in :confused:
```

---
## \#72 Posted by: barajabali Posted at: 2016-06-28T08:43:24.404Z Reads: 254

```
Let's keep this thread alive to find a solution because I know you're not the only one with this issue..
```

---
## \#73 Posted by: Mobutusan Posted at: 2016-06-28T08:46:49.019Z Reads: 259

```
Maybe the actual connection inside the connector wasn't fully engaging despite being fully plugged in. What @barajabali experienced seems like the only logical reason why this should happen. 

Path A with resistor connects first, then Path B with ~4mm bullet plug doesn't fully connect sending most or all current through Path A, resulting in poor motor performance and melted loop key. Nothing else left in the equation, right?
```

---
## \#74 Posted by: trbt555 Posted at: 2016-06-28T08:47:15.998Z Reads: 252

```
[quote="whitepony, post:68, topic:5241"]
owever, if you decrease the wire thickness the inductivity rises and its proportional to the wire windings, so many many small windings in that loop would actually increase the inductance by a lot!
[/quote]

I respectfully think you're over-thinking things here.
The only way you can burn an XT90 is by applying more current than it can handle.
If it's not plugged in all the way, the small resistor cannot handle the full current draw for very long.
When it's plugged in all the way, an XT90 can handle over 90 Amps safely.
Inductance of the loop key has nothing at all to do with it.
```

---
## \#75 Posted by: kovjanos Posted at: 2016-06-28T08:51:40.442Z Reads: 285

```
Hi,

If I understood correctly these loop keys are passive components, a single resistor inside. First it looks an easy option but then... 
Easy because they are cheap, small, no polarity to mess up, etc.
...but don't forget the dark side:

1. You must be sure that the key itself can handle the current that will flow through the key and the loop you add. 
E.g. Use a short high-Amp piece of wire, e.g. what was recommended above.

2. You must "operate" it as quick as possible. Don't worry, you won't be faster than electrons, but you must plug the loop key together as fast as possible and properly. 
Why? Because it has two stages. First the contact is made only with the resistor that sucks up the spark. Then on full engagement contact is made directly with the loop moving the stress away from the resistor. So if you not fast enough and let the current flow through the resistor too long or you do not engage the full contact because of poor-quality plastic finish, you can easily burn the resistor.
Yeah, but how fast? Well, let the caps charge through the resistor before the full contact - see next point.

3. Make sure the built-in resistor is powerful enough to handle - even only for a sub-second or a second - the current peak.
If you have a lots of capacitance in your setup - e.g. many and/or large capacitors, like a dual VESC - and you are not pre-charging them, those caps will suck current from your battery when you engage your loop-key. The resistor must be able to handle the current the caps suck out from the battery for long enough the caps are (almost) charged.

@barajabali may had the issue described in #2 - not fully engaged contact stressing the resistor?

R, J.
```

---
## \#76 Posted by: Randyc1 Posted at: 2016-06-28T14:24:26.391Z Reads: 273

```
What ecxactly did you file down to get it to plug in 100% ?

My loopkey is identical to whitepony's when he had it melt  ,...mine is an interupt on the POS of Battery before esc....never had a problem ?<img src="/uploads/db1493/original/2X/2/233a51cc1c177204879d22db1aa09066679eea72.jpg" width="640" height="360">
```

---
## \#77 Posted by: GhettoFab.rictation Posted at: 2016-06-28T14:39:51.210Z Reads: 269

```
I'm still waiting on my cnc shop and some more connectors for the charger, I might get an extra pair of originals just in case hah, xt90 connectors. Or should I just check the connection before the DC is live to make sure they connect 100% ? I wonder if my 44v is too much and 10000mah, it was stated it can only handle 7amps and my connectors are going from the battery to my esc therefore 10 amps is too much right?
```

---
## \#78 Posted by: trbt555 Posted at: 2016-06-28T15:02:16.793Z Reads: 260

```
Somebody needs to launch a poll asking how many people are actually having problems with a XT90s loop key.
Not a lot I expect.
That should kill all this panic.
```

---
## \#79 Posted by: barajabali Posted at: 2016-06-28T15:03:50.098Z Reads: 257

```
You're gonna be fine just make sure to plug it in all the way sorry bout the confusion
```

---
## \#80 Posted by: GhettoFab.rictation Posted at: 2016-06-28T15:08:18.097Z Reads: 255

```
Haha alright, :laughing: not a problem I'd rather hear about it and double check than run into the same issue, I'll check the connectors and all. Should be alright though
```

---
## \#81 Posted by: barajabali Posted at: 2016-06-28T15:11:04.397Z Reads: 243

```
If you noticed my plug goes thru my deck and I wanted a snug fit along with glue so ensure it wouldn't come out. I guess I made it too snug and changed the shape of the connector a bit. So I just had to file down the male connector to match the other one
```

---
## \#82 Posted by: mcfly777 Posted at: 2016-06-28T16:48:45.072Z Reads: 244

```
[quote="Mobutusan, post:73, topic:5241, full:true"]
Maybe the actual connection inside the connector wasn't fully engaging despite being fully plugged in. What @barajabali experienced seems like the only logical reason why this should happen. 

Path A with resistor connects first, then Path B with ~4mm bullet plug doesn't fully connect sending most or all current through Path A, resulting in poor motor performance and melted loop key. Nothing else left in the equation, right?
[/quote]

This. Sounds like all current was passing through the resistor, which would then heat (a lot) and melt the connector. Do the following experiment: measure the resistance when the plug is barely in when it first closes the circuit. then measure it again when you push it all the way in. You'll see that there should be resistance (5.6 ohm) initially, and then no resistance after plugging it fully in.

Leo
```

---
## \#83 Posted by: kovjanos Posted at: 2016-06-28T17:54:09.190Z Reads: 240

```
If it's really 5.6 Ohm only what the XT90S has, then with 12S the peak/spark current will be around 9A in a std. dual-VESC configuration (around 4000 uF; depends on the cap bank + other components like SBEC, etc.) and gets to around 4A only after around 20-30 ms. Probably not a big deal for a wirewound resistor to charge the caps... 
...but I think it can't survive the normal / continuous current even for a single (V)ESC-motor setup.

R, J.
```

---
## \#84 Posted by: Maxid Posted at: 2016-06-28T17:57:12.379Z Reads: 232

```
5.6Ohm is written on the plug but only the initial contact is made by it.
Once the plug is fully inserted basically no current will flow through that resistor.
```

---
## \#85 Posted by: kovjanos Posted at: 2016-06-28T18:10:49.787Z Reads: 239

```
Yep - and for the initial contact don't be faster than around 20ms (or up to 100ms just to be sure) but make sure it's fully inserted before you let your motor spin.

R, J.
```

---
## \#86 Posted by: Okami Posted at: 2016-06-28T20:50:28.228Z Reads: 238

```
Hey there! I recently found this page / calculator:

http://scriptasylum.com/rc_speed/nospark.html

It gives background info, tells 2 ways to connect the no spark switch and there's also a calc for values / wattage.

Although, it recommends quite high resistor (around 2w) for 24v system, IF someone can make use of this, please do so! Would like to understand what ohms/watts would be needed for different systems - 6s, 8s, 10s, 12s.. and so on.
```

---
## \#87 Posted by: GhettoFab.rictation Posted at: 2016-06-29T00:10:01.361Z Reads: 234

```
@barajabali so what's the complete charge time? @chaka what's a uf rating for the esc???
```

---
## \#88 Posted by: barajabali Posted at: 2016-06-29T01:16:33.612Z Reads: 243

```
For your pack?
```

---
## \#89 Posted by: Callum16 Posted at: 2016-06-29T01:33:21.501Z Reads: 245

```
Change your connectors to XT-150's you can get them on Hobbyking and they can take a much larger load...<img src="/uploads/db1493/original/2X/9/9f710b00273fc16ccddd4a13b10aa4ff1e4994de.jpg" width="500" height="500">
```

---
## \#90 Posted by: chaka Posted at: 2016-06-29T03:26:34.478Z Reads: 234

```
680uf x 3 ... 2040uf 63v
```

---
## \#91 Posted by: GhettoFab.rictation Posted at: 2016-06-29T04:22:01.566Z Reads: 231

```
Yeah I'm going to try and use the calculator for knowledge :stuck_out_tongue: thank you @chaka
```

---
## \#92 Posted by: Nordle Posted at: 2016-06-29T04:25:35.938Z Reads: 232

```
I always doubt these connectors are made to make life easy:D now we have almost 100replys here. personally i would go the next step;)
<img src="/uploads/db1493/original/2X/7/77aa195f601ca505f3459b91c62b22415971772b.jpg" width="690" height="207">
```

---
## \#93 Posted by: GhettoFab.rictation Posted at: 2016-06-29T04:55:38.873Z Reads: 226

```
I couldn't understand your diagram unless I saw the components. Lol I'm a little rusty with all that. I see the diode but your resisters confuse me
```

---
## \#94 Posted by: Nordle Posted at: 2016-06-29T05:09:31.778Z Reads: 222

```
I'm not 100% sure, i think the resistors are just current dividers. The 1uF is bipolar!
I'm not sure cause i used anotger design before i switched to this. This is just coppied from fechter/vedder.
```

---
## \#95 Posted by: lowGuido Posted at: 2016-06-29T05:21:27.933Z Reads: 222

```
hahaha I would have thought that the next step would be to simplify things not complicate.. 
remove all resistors and just deal with a little spark, replace the connectors if they get eroded to the point that their performance is affected.
```

---
## \#96 Posted by: GhettoFab.rictation Posted at: 2016-06-29T06:10:29.362Z Reads: 225

```
Yeah I thought of that in the beginning but doesn't that mess up the vesc if there's no switch or fuse between the battery and vesc?
```

---
## \#97 Posted by: lowGuido Posted at: 2016-06-29T06:12:18.392Z Reads: 221

```
@GhettoFab.rictation you know its the caps on the VESC that causes the spark right?
```

---
## \#98 Posted by: GhettoFab.rictation Posted at: 2016-06-29T06:20:13.550Z Reads: 223

```
Right so install fuse between connector and vesc then connect the plugs that spark. Or go with these connectors on this thread. That's what I figured, if you really wanted to take care of a hundred dollar investment O.o
```

---
## \#99 Posted by: kovjanos Posted at: 2016-06-29T06:34:26.505Z Reads: 226

```
[quote="chaka, post:90, topic:5241, full:true"]
680uf x 3 ... 2040uf 63v
[/quote]

On 12S (~50V) with the XT90S the peak charging current would be ~9A.  
The first ~10ms and already ~half, full charge ~40-50ms.

R, J.
```

---
## \#100 Posted by: GhettoFab.rictation Posted at: 2016-06-29T06:43:59.756Z Reads: 224

```
Ok so with chaka's vesc and 190kv motor two 6s batteries 5,000 mah it may be smarter to run a bigger connecter on the end of the two batteries if they are connected in series
```

---
## \#101 Posted by: kovjanos Posted at: 2016-06-29T06:48:14.008Z Reads: 208

```
Fuse is a good idea - at least it helps when things go wrong like a faulty component or accidentally shorting things. 
...but problems come from wrong assumptions: don't expect that the fuse would secure anything from the spark from the initial connection. The fuse you would use for the ESC/Motor probably will have higher limit and slower break than the spark. 
Knowing the characteristics of the resistor would help to state YES or NO - but based on experience, XT90S should do the job.

R, J.
```

---
## \#102 Posted by: kovjanos Posted at: 2016-06-29T07:36:01.367Z Reads: 216

```
[quote="GhettoFab.rictation, post:100, topic:5241, full:true"]
may be smarter to run a bigger connecter[/quote]

What are your batteries' C-rates? 
This tells you what the max current you should expect (and secure with a fuse).
Even if your battery setup would be powerful, good to think about the other components - e.g. VESC's current limits. If this is less, your fuse could go down and would not be necessary to use high-current rated connectors. For a single VESC an XT90 should be enough (even if you have heatsink and active cooling).

R, J.
```

---
## \#103 Posted by: GhettoFab.rictation Posted at: 2016-06-29T22:51:23.545Z Reads: 215

```
18650's, and vedder's vesc rated 240amps burst and 50a continuous, input voltage rates 60v max. Yeah I figured it would be safe, but wondered if I could make it bullet proof and protect all of the investments haha :laughing:
```

---
## \#104 Posted by: GhettoFab.rictation Posted at: 2016-06-29T22:52:32.494Z Reads: 216

```
I'll have single 190 kv with a 110mm wheel and geared 15t 30t
```

---
## \#105 Posted by: Jinra Posted at: 2016-06-29T22:53:27.215Z Reads: 218

```
Sounds like you're going to have a ton of amp draw, and perhaps less than average acceleration.
```

---
## \#106 Posted by: GhettoFab.rictation Posted at: 2016-06-29T22:54:16.150Z Reads: 222

```
Yes more of a cruiser not a racer, but the high torque motor will make up for it,top speed wanted I hit 35mph here in AZ on south mountain np
```

---
## \#107 Posted by: Jinra Posted at: 2016-06-29T22:56:16.446Z Reads: 220

```
Good luck with your build! Just be careful of the huge current you'll be pulling.
```

---
## \#108 Posted by: barajabali Posted at: 2016-06-29T22:58:21.966Z Reads: 216

```
What do you mean he's running 12s with a 15 30 ratio he's gonna go fast as fuck. 

Acceleration not sure depends on your weight
```

---
## \#109 Posted by: GhettoFab.rictation Posted at: 2016-06-29T22:58:27.821Z Reads: 218

```
Thanks dude, yeah I'm getting mechanics done first and basic electronics before anything that requires tedious work this thread caught my eye. I will study more for sure!
```

---
## \#110 Posted by: GhettoFab.rictation Posted at: 2016-06-29T22:58:54.906Z Reads: 213

```
Weight is 170, 6ft 3 in. Fit 170* lol
```

---
## \#111 Posted by: Jinra Posted at: 2016-06-29T22:59:42.005Z Reads: 215

```
For sure he'll be fast. Like 45+mph at full effiency, but the reduction is pretty minimal, and it's a single motor, so I imagine (but definitely can't say for sure) that acceleration will suffer.
```

---
## \#112 Posted by: barajabali Posted at: 2016-06-29T23:00:06.368Z Reads: 215

```
Acceleration will be fine I think. Those motors Are tough
```

---
## \#113 Posted by: GhettoFab.rictation Posted at: 2016-06-29T23:00:50.086Z Reads: 215

```
Yeah that's what I read after reading rpm per volt!  :smile:
```

---
## \#114 Posted by: Jinra Posted at: 2016-06-29T23:03:02.176Z Reads: 216

```
Please do a review and build log, when you get to it, I'd love to know how it turns out.
```

---
## \#115 Posted by: GhettoFab.rictation Posted at: 2016-06-29T23:09:53.025Z Reads: 235

```
I will brotha I have chaka bara and psychotiller to thank I'll include parts pictures and prices along with everything I've learned and finishing video, and a fellow in Poland for the 3d printed 30t and trial 36t for cheap
```

---
## \#116 Posted by: mason Posted at: 2016-09-09T23:13:13.554Z Reads: 221

```
<img src="/uploads/db1493/original/3X/1/e/1ee538183628ad914834c14ea547ca6af77ad5ac.jpg" width="281" height="500">
ugh. ruined my weekend plans.

I've had issues recently where I can ride for ~1 minute without abnormal behavior, and then randomly power will be reduced drastically. I can still brake, and the motor still runs but only if I get off. I make sure to plug in my XT90s quick and all the way every time. I had a direct bridge using solder wick. I have it setup to bridge the positive to the battery. 

Not too sure what the issue is here.
```

---
## \#117 Posted by: lox897 Posted at: 2016-09-10T00:35:18.136Z Reads: 211

```
Have you made sure the resistor in the connector is the right way around?
```

---
## \#118 Posted by: mason Posted at: 2016-09-10T01:07:26.422Z Reads: 206

```
I'm not at home to check but I'm 99% sure it's correct.
```

---
## \#119 Posted by: psychotiller Posted at: 2016-09-10T01:48:15.812Z Reads: 214

```
Why not just put the loop key on the negative side? Or the positive side...Either way polarity wouldn't even be a concern. The only reason this was ever an issue is because wiring it like a plug instead of an interupt created the polarity issue. 

Just cut one wire. Negative or positive. Doesnt matter which. Then solder both negative ends to the plug. Or both positives. Doesn't matter.
```

---
## \#120 Posted by: mason Posted at: 2016-09-10T01:59:42.617Z Reads: 218

```
That's what 90% of us are doing
```

---
## \#121 Posted by: psychotiller Posted at: 2016-09-10T02:14:41.771Z Reads: 223

```
 Do the same 90% run 12s? Maybe it's the voltage if that's the case.
```

---
## \#122 Posted by: CaptainMerricka Posted at: 2016-11-11T09:14:09.933Z Reads: 183

```
I don't know if anyone has mentioned this, but it is convention that the "hot" connection is the female connector so that you can't short the connection by touching the prongs. So, for the loop key,  it be better to use the female plug as the one on the board and the male connector as your key.
```

---
## \#123 Posted by: Maxid Posted at: 2016-11-11T09:43:42.016Z Reads: 189

```
First: Polarity is not an issue - how many times do we have to talk about this?
Second: The XT90 "male" plug has actually female prongs whiel the female version has male prongs. So you should use the female as your key - however this would also mean that you have the male plug sticking out of your board and is not hidden as nicely as when you mount it the other way around.
```

---
## \#124 Posted by: SORRENTINO Posted at: 2016-11-11T14:47:06.827Z Reads: 183

```
Actually to be totally clear the casing on the plugs does not determine if its a male or female plug. The actual prongs in the plug determines that. ;)
```

---
## \#125 Posted by: Stas74 Posted at: 2019-01-11T06:36:01.423Z Reads: 71

```
What is the thiccnes of this copper rod? What thiccnes should i do i have 10s
```

---
## \#126 Posted by: b264 Posted at: 2019-01-11T07:45:41.169Z Reads: 70

```
10AWG

You could get by with 12AWG if you only have one motor.
```

---
