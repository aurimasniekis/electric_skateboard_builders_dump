# Options for connecting dual ESCapes?

### Replies: 17 Views: 538

## \#1 Posted by: ArnhemAnt Posted at: 2018-06-18T22:19:58.998Z Reads: 153

```
I'm nearly at the stage of my first build where I connect the battery, ESCapes and motors together and I can see that there are three main options for connecting dual speed controllers. 
1: CANBUS
2: Split 'Y' cable
3: Dual receivers

Given I'm using the ESCapes and my remote is a Nano-X, and I want to be running in FOC mode, is there an 'ideal' option that I should be going with?

I realise this has been discussed previously, however not with the exact parts I have so I want to make sure I have everything clear before I begin.

Thanks in advance for any advice.
```

---
## \#2 Posted by: mmaner Posted at: 2018-06-18T22:31:02.145Z Reads: 150

```
Can bus is perfect, just don't power up one VESC and not the other when the can bus cable is connected and you will be fine.
```

---
## \#3 Posted by: rich Posted at: 2018-06-18T22:46:48.240Z Reads: 140

```
Exactly what @mmaner said. Furthermore it is important to connect the 2 middle pins only. 

![20180619_004147|690x388](upload://8Z0oy33OjSwEI96N31rtwQwJq5I.jpg)

The canbus cable is a 4pin JST-PH (2mm pitch)
```

---
## \#4 Posted by: ArnhemAnt Posted at: 2018-06-18T22:54:14.318Z Reads: 135

```
Thanks for the quick response. So, obviously, I set each one up on their own initially and then once that is done, then connect Can bus and ensure they both power up together from that time on?

@rich - thanks for the pic - that helps a heap. I'll have to get my hands on that cable.
```

---
## \#5 Posted by: ArnhemAnt Posted at: 2018-08-24T22:53:16.030Z Reads: 106

```
I'm finally back to try and get this build finished. Just relocated interstate, which was a real PITA.

Anyway, from what I can work out (and I'm a dumb ass), I think I have all the necessary connections in place for the dual ESCape.
Would someone with a little more knowledge than me have a quick look over the two images here and let me know if everything looks correct please?

My next hurdle is trying to work out the best way to connect the power leads from the dual ESCapes to the power leads from my battery (12s4p). Any info, or images/links would be much appreciated.![ESCape1|375x500](upload://nk7E6eUShr9Vguon0826Vd3pvtL.jpg)![ESCape2|375x500](upload://sORCwGO6PggDoTqk8cVTgBbLBRA.jpg)
```

---
## \#6 Posted by: ArnhemAnt Posted at: 2018-08-24T23:36:04.278Z Reads: 99

```
Another query. To connect my Tx to the ESCape, I use the PPM connector. I have a servo wire set for my Tx. Can I just use the servo cable plug into the PPM on the ESCape, or do I need to modify this end of the cable?
```

---
## \#7 Posted by: Andy87 Posted at: 2018-08-25T12:24:51.231Z Reads: 95

```
I guess the problem with the ppm plug already solved as you said you found the right jst connector.
Just a quick question, I didn’t understood, you want to use now can bus or split ppm, or both?

To connect the dual escapes to your main battery wires best to use a xt90 parallel plug.
Something like this 
![image|278x500](upload://zzCl120yGDgalnaaTOuBMxkFFEW.jpeg)

As i don’t know any other details of your build one thing that never bad. Include a fuse and a anti spark plug in the wires from your battery to the escapes (if you use a bms or a e-switch than just ignore the last sentence).
```

---
## \#8 Posted by: rich Posted at: 2018-08-25T17:13:38.011Z Reads: 89

```
[quote="ArnhemAnt, post:6, topic:59329"]
Can I just use the servo cable plug into the PPM on the ESCape, or do I need to modify this end of the cable?
[/quote]

Do you mean the standard servo connector? Because it won't fit. All connectors on the Escape are JST-PH (2mm pitch). If you have cables left (e.g. from canbus) you can easy cut it to make a 3pin ppm cable, this is what I did instead of waiting weeks for new cables.


![210105|690x388](upload://45tUeDYua9nAQVoQljpNxdNceBv.jpg)

![210234|690x388](upload://8g4ASALiYtQQIlewyRkd0iGuVSz.jpg)

[quote="ArnhemAnt, post:5, topic:59329"]
My next hurdle is trying to work out the best way to connect the power leads from the dual ESCapes to the power leads from my battery (12s4p)
[/quote]

You have the enclosure mounted below the deck, right?
The only nice way is to have an antispark switch

**ATTENTION!!!**

Do you know that all your JST-PH connectors on the Escape are mounted wrong by factory? (180 degrees different than normal). This is no problem for canbus connection and I guess you checked the correct pins for the BT-module. The labeling on Escape is correct but as mentioned the male connectors on PCB are rotated 180°.

Did you solder extensions for the sensor wires in reversed order or fixed it differently?
Because if not you most likely kill your hall sensors due to reversed polarity. On the picture you can see the red wire is connected to ground and the black to +5V.

Check if all your cables are connected in the correct order before you power the Escapes! And as mentioned earlier never power 1 Escape only when canbus is connected.
```

---
## \#9 Posted by: ArnhemAnt Posted at: 2018-08-25T20:59:28.988Z Reads: 82

```
[quote="Andy87, post:7, topic:59329"]
Just a quick question, I didn’t understood, you want to use now can bus or split ppm, or both?

To connect the dual escapes to your main battery wires best to use a xt90 parallel plug.
[/quote]


Thanks Andy,
I'm using Can Bus for the dual ESCapes. I don't have any of the parallel XT90 plugs, but I do have some XT60 parallel. If these are only to connect the ESC, will this be fine?
```

---
## \#10 Posted by: ArnhemAnt Posted at: 2018-08-25T21:02:01.151Z Reads: 80

```
[quote="rich, post:8, topic:59329"]
If you have cables left (e.g. from canbus) you can easy cut it to make a 3pin ppm cable, this is what I did instead of waiting weeks for new cables.
[/quote]


Thanks Rich, I never would have thought of that.

I'll also go back over all the connections and ensure the wires are in the correct places. Thank you for mentioning this as I would have thought that it is all correct. Kinda glad I haven't tried to power anything up yet as I sure as heck would have stuffed something.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-08-25T21:59:10.771Z Reads: 74

```
Depends how much amps you plan to get out of your battery. The focboxes come with xt60’s and people say that the xt60 can handle up to 90a as long as it’s not for constant current.
Personally I would go with xt90‘s or xt90 on the battery side and two xt60s on the vesc side.
Just to be safe.
If you don’t have xt90‘s the 60 should do the job also.
Just check from time to time that nothing started to meld 😉
```

---
## \#12 Posted by: ArnhemAnt Posted at: 2018-08-25T22:36:01.863Z Reads: 65

```
Thanks again for the info. 
I've got XT90 plugs from the battery, incl loop key and will only be using the XT60 for the connection to the dual ESCapes so I think everything should be fine.
```

---
## \#13 Posted by: ArnhemAnt Posted at: 2018-08-26T04:03:09.244Z Reads: 63

```
[quote="rich, post:8, topic:59329"]
Did you solder extensions for the sensor wires in reversed order or fixed it differently?
Because if not you most likely kill your hall sensors due to reversed polarity. On the picture you can see the red wire is connected to ground and the black to +5V.
[/quote]


Hey Rich,
Hoping you can help me out here man. I've changed the pins for the gnd and +5 for the motor sensor cables, but what about the other three wires?? I'm running the Dark Matter motors and there is also yellow, green and blue wires but I have no idea what they are for and can 't seem to find any info from the search function on this forum. 
I did read somewhere that the other colours don't matter much, but is this correct? I've come so far and I really don't want to fuck things up when I am so close to finishing this thing.
```

---
## \#14 Posted by: bigben Posted at: 2018-08-26T07:03:19.663Z Reads: 58

```
The other 3 wires are the sensors wires and they are in no particular order. They will be detected when you do the setup so you should be good to go. (make sure you have them on the sensor pins and not the "T" pin.)
```

---
## \#15 Posted by: Andy87 Posted at: 2018-08-26T07:09:32.726Z Reads: 54

```
Yeah, sounds good 👌
```

---
## \#16 Posted by: ArnhemAnt Posted at: 2018-08-26T07:31:36.836Z Reads: 54

```
[quote="bigben, post:14, topic:59329"]
make sure you have them on the sensor pins and not the “T” pin.
[/quote]


When you say, the 'T' pin, I presume you are talking about the temp pin?
```

---
## \#17 Posted by: bigben Posted at: 2018-08-26T07:32:45.319Z Reads: 53

```
Yep, that's the one.
```

---
