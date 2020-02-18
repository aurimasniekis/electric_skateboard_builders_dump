# Need help with Nano-X tx/rx

### Replies: 49 Views: 1713

## \#1 Posted by: Pr0dy Posted at: 2017-02-22T18:30:20.276Z Reads: 106

```
Alright, I received all the parts I needed for my first build. Now what pissed me off a bit at first was not to receive a bind key with my receiver (Nano-X), but I figured I could just connect two of the pins together to get the same result. I tried to find on the internet how to bind the nano-x transmitter to the receiver, and in every video there is a red blinking light on the receiver, which I don't have. There is no red blinking light and the transmitter won't bind.
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-02-22T18:36:11.311Z Reads: 105

```
Do you have any picture of your connection, so we can help you double check them... alao the nano-x have a auto-bind fonction wich do not require a binding tool.
```

---
## \#3 Posted by: Pr0dy Posted at: 2017-02-22T18:38:45.863Z Reads: 101

```
<img src="/uploads/db1493/original/3X/1/0/108ed7b7c7bc503bc1fc8e4ab6855ae0ea2ea0c5.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/f/d/fdf61b7f8c17c1c627b35713a06811fafb1ede83.jpg" width="281" height="500">
```

---
## \#4 Posted by: Pr0dy Posted at: 2017-02-22T18:40:42.897Z Reads: 90

```
note : VESC lights are on while the receiver's light isn't
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-02-22T18:44:31.121Z Reads: 90

```
Have you try to just plug one vesc at the time... just to see if the problem is from the connection or the receiver
```

---
## \#6 Posted by: Pr0dy Posted at: 2017-02-22T18:47:00.238Z Reads: 90

```
<img src="/uploads/db1493/original/3X/c/4/c42e38e6c8ef30adf7f6ccf372228bf41d9e0834.jpg" width="281" height="500">

Light doesn't turn on on the reveiver, tried with both or only one VESC at a time. No change, no red light.
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2017-02-22T18:56:27.891Z Reads: 84

```
Your cable are inverted inside your connector... it should be brown, red, yellow (same order as on the vesc) 

Edit: can you double check (still not 100% sure, since I'm on mobile 🙂)
```

---
## \#8 Posted by: Pr0dy Posted at: 2017-02-22T18:57:52.683Z Reads: 86

```
Doesn't light up on both sides anyways. Tried brown, red, yellow and yellow, red, brown. No red light on both sides... :/
```

---
## \#9 Posted by: Montiey Posted at: 2017-02-22T19:00:40.210Z Reads: 86

```
Do you have an Arduino? You can make a simple script to power the receiver, and also listen for the 1-2 millisecond pulses. Or, use any 5v power source, and a small hobby servo to test it.
```

---
## \#10 Posted by: Pr0dy Posted at: 2017-02-22T19:01:20.663Z Reads: 85

```
I don't have an Arduino, no idea what it is either
```

---
## \#11 Posted by: Montiey Posted at: 2017-02-22T19:01:47.480Z Reads: 84

```
https://www.google.com/#safe=strict&q=arduino

You can use a servo, also. I was just going to recommend a micro controller because some people don't have servos.
```

---
## \#12 Posted by: Pr0dy Posted at: 2017-02-22T19:02:26.312Z Reads: 79

```
I don't have that lol
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-02-22T19:03:06.409Z Reads: 80

```
No.... the cable inside the connector.... they had swap some cable when soldering them on the vesc... brow (gnd), should be on the outside side of the receiver, red(5v) should be in the middle and yellow (signal) sould be on the interior side of the receiver, same order on the vesc...

But if you look at your the red and brown are not in the same order on your vesc and on the connector.
```

---
## \#14 Posted by: Pr0dy Posted at: 2017-02-22T19:03:07.344Z Reads: 77

```
I start thinking the receiver is just dead... First build big problems lol
```

---
## \#15 Posted by: Pr0dy Posted at: 2017-02-22T19:03:43.059Z Reads: 76

```
Not sure I'm following you here
```

---
## \#16 Posted by: Montiey Posted at: 2017-02-22T19:03:56.718Z Reads: 76

```
I wonder if the Nano-X has a light regardless of connection?
Maybe you need to rebind the controller and receiver.

Edit: JohnnyMeduse may be right. Just make sure the ORDER matches on both ends, and then turn the cable around to get it to work.
```

---
## \#17 Posted by: Pr0dy Posted at: 2017-02-22T19:05:13.863Z Reads: 82

```
[quote="JohnnyMeduse, post:13, topic:18099"]
order on
[/quote]

Just checked, I think the camera took the wrong color. Red is in the middle, orange to the right and brown to the left, same on VESC
```

---
## \#18 Posted by: Montiey Posted at: 2017-02-22T19:06:13.678Z Reads: 80

```
Then it should work- if not, flip the connector on the receiver side.
It's good form to make sure that it's right-way-round, but if you need to you can use it backwards if you've already soldered one end.
```

---
## \#19 Posted by: Pr0dy Posted at: 2017-02-22T19:07:13.655Z Reads: 79

```
As I said, doesn't work on either sides...
Tried flipping and flipping, nothing works. No red light receiver looks dead
```

---
## \#20 Posted by: Montiey Posted at: 2017-02-22T19:07:37.982Z Reads: 77

```
Oh. What about trying the other ports on the receiver? Is it in the wrong one?
```

---
## \#21 Posted by: Pr0dy Posted at: 2017-02-22T19:08:01.352Z Reads: 73

```
Doesn't work on channel 1 or channel 2
```

---
## \#22 Posted by: Montiey Posted at: 2017-02-22T19:08:59.269Z Reads: 70

```
Ok. Try rebinding. unplug the power to the VESC, then insert a bind plug. Power it up, then turn on the remote with the button held down. See what happens?
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2017-02-22T19:11:10.578Z Reads: 67

```
Ok... just make sure that your connection are the same as those (I had make a nice drawing that I don't want to loose 😅), and if you have acces to a multimer make sure that you have 5v on the 5v pin... and if not try to contact enertion support 😉

<img src="/uploads/db1493/original/3X/1/c/1c058e2ee7850ba5f68c37f150d2fd36c3c4eb53.JPG" width="666" height="500">
```

---
## \#24 Posted by: Pr0dy Posted at: 2017-02-22T19:12:29.609Z Reads: 63

```
Couldn't post a video but I tried binding it. Still no red light, green light on receiver keeps on switching on/off as it should on binding process. VESC lights are on too.
```

---
## \#25 Posted by: Pr0dy Posted at: 2017-02-22T19:13:33.524Z Reads: 62

```
Checked the connections. Red in middle, black/brown to the left, yellow/orange to the right. No switch between VESC and Rx
```

---
## \#26 Posted by: Montiey Posted at: 2017-02-22T19:13:40.111Z Reads: 58

```
;)

I would test the power lines, too. But be CAREFUL. I don't think the VESC has short protection, so don't let the multimeter probes slip and short out the pins…

If there are no lights on the receiver, then it is most likely faulty. Will they void warranty if you open the case and have a look at the soldering job? That'd be my first move, anyways.
```

---
## \#27 Posted by: Pr0dy Posted at: 2017-02-22T19:15:15.662Z Reads: 58

```
<img src="/uploads/db1493/original/3X/3/e/3e2671bd5f4f649f348b8690433f37ef27229ccb.jpg" width="281" height="500">
I am no expert in electronics tbh. Whatever, if it voids warranty I'll just buy from another company -_-
```

---
## \#28 Posted by: Pr0dy Posted at: 2017-02-22T19:16:12.594Z Reads: 57

```
<img src="/uploads/db1493/original/3X/b/d/bd285277b912939152c7ba7cf81b0bc1e54b9af7.jpg" width="690" height="388">
```

---
## \#29 Posted by: Montiey Posted at: 2017-02-22T19:19:55.407Z Reads: 57

```
Looks alright, to be honest. How are the voltages from the VESC? You may have a cold joint at the servo lead on the VESC.
```

---
## \#30 Posted by: Pr0dy Posted at: 2017-02-22T19:20:15.918Z Reads: 55

```
How do I  check voltages ?
```

---
## \#31 Posted by: Montiey Posted at: 2017-02-22T19:20:33.389Z Reads: 54

```
Do you have a multimeter?
```

---
## \#32 Posted by: Pr0dy Posted at: 2017-02-22T19:20:57.765Z Reads: 54

```
sadly, nope
```

---
## \#33 Posted by: Montiey Posted at: 2017-02-22T19:22:26.464Z Reads: 53

```
Hmm.. That would be a priority in my case. I have 2, but some people have entire collections.

Does it seem like the receiver is connecting to the remote during binding at all? There might be an RF problem.
```

---
## \#34 Posted by: Pr0dy Posted at: 2017-02-22T19:23:04.995Z Reads: 55

```
[quote="Montiey, post:33, topic:18099"]
g to the remote du
[/quote]
 
Definitely not binding, as I said, there is no red light and the green light on the transmitter keeps beeping
```

---
## \#35 Posted by: Pr0dy Posted at: 2017-02-22T19:27:46.656Z Reads: 54

```
Alright, I'll just give up at this point. Anybody knows where I can find a good remote (under like 100$) That will ship to Canada-East in under a week?
```

---
## \#36 Posted by: JohnnyMeduse Posted at: 2017-02-22T19:28:06.677Z Reads: 53

```
Where are you located
```

---
## \#37 Posted by: Pr0dy Posted at: 2017-02-22T19:28:19.298Z Reads: 56

```
Quebec city
```

---
## \#38 Posted by: Pr0dy Posted at: 2017-02-24T14:41:56.755Z Reads: 49

```
Just found out that I actually own a multimeter, how do I test it now?
```

---
## \#39 Posted by: Blasto Posted at: 2017-02-24T14:48:00.432Z Reads: 49

```
Unplug the connector from the receiver,  put your multimeter on the 20V DC scale

<img src="/uploads/db1493/original/3X/8/1/818775678ce71ce2e83a77f817f877ce6f6a0167.jpg" width="380" height="388">

with the vesc powered on, red probe on the middle pin of the connector and black probe on the ground. (red on red, black on brown cable)
```

---
## \#40 Posted by: Montiey Posted at: 2017-02-24T19:17:07.464Z Reads: 46

```
You should be getting 4.8-5v, but since the receiver's lights already work that's probably the case.
```

---
## \#41 Posted by: Pr0dy Posted at: 2017-02-24T21:37:11.836Z Reads: 43

```
Got 5.15V 
Guess my VESCs are not dead haha
```

---
## \#42 Posted by: Montiey Posted at: 2017-02-25T01:57:51.609Z Reads: 44

```
Yeah, so your receiver / vesc probably isn't the problem after all- Either the remote has a problem, or it's magic. Can you open the remote and take some good pictures? :D
```

---
## \#43 Posted by: Pr0dy Posted at: 2017-02-25T02:15:54.407Z Reads: 44

```
As I wrote earlier, receiver normally has a red light flashing on it when it's trying to bind, this light is not lighting up on my receiver. However, my transmitter do have a green blinking light, which is normal. Next week I'll go to Enertion's repair facility and they told me they could help me out with my board and repair the receiver. I'm just glad it's not the VESCs lol
```

---
## \#44 Posted by: Montiey Posted at: 2017-02-25T02:28:17.320Z Reads: 44

```
I know the feeling. I'd be fine if my batteries were bent in half- just protect my VESC!! I got mine for around $120 before Ollin had to raise prices, so now I basically have a board designed around a $150 piece of electronics. I get real scared sometimes that i've broken it, but it's working O.K so far :) Good luck with the repair center, and maybe they'll let you keep the old one for parts.
```

---
## \#45 Posted by: Pr0dy Posted at: 2017-02-25T02:40:41.585Z Reads: 43

```
Oh they just said they would repair de receiver, not replace it :stuck_out_tongue: . That's my first build and hope it's going to be worth it
```

---
## \#46 Posted by: DuskisNigh Posted at: 2017-02-25T14:07:17.342Z Reads: 40

```
someone else on here posted they were also having receiver binding problems, so they opened up the receiver and the sticky foam tape holding the board down was conductive enough that it was causing a problem, so they switched it to the side that didn't have any connections and it worked fine.  maybe check that out.
```

---
## \#47 Posted by: Montiey Posted at: 2017-02-25T15:26:08.451Z Reads: 36

```
Interesting. Never thought of foam tape being too conductive, but if someone didn't do their research, I guess it's possible to end up using conductive material by accident.
```

---
## \#48 Posted by: Pr0dy Posted at: 2017-02-25T19:24:16.354Z Reads: 35

```
Alright, I tried removing the PCB from the case and the foam, plugged everything in, receiver still doesn't work. I checked with the multimeter and it's still displaying 5.15v
```

---
## \#49 Posted by: Lsalt Posted at: 2017-02-26T02:44:00.822Z Reads: 34

```
Maybe the red led doesn't work and you also have the same issue I have....try removing the signal wire only and leave the power lines. Then see if your remote stops blinking and is solid green. If you plug the signal line back in after and it works then you have the same issue I have. Mine only binds with the signal line disconnected and then reconnected. I am sending mine in for repair.
```

---
