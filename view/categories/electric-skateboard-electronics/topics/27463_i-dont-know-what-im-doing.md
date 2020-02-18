# I don&rsquo;t know what I&rsquo;m doing

### Replies: 23 Views: 1489

## \#1 Posted by: wilkni Posted at: 2017-07-12T21:33:38.443Z Reads: 178

```
I need help finding a new battery for my maverix border x. I want to replace its heavy lead battery with something lighter, I don't know what to look for exactly. I'm hoping to find a decent one on amazon because of 12 month financing that I can do with it. Any help would be appreciated.
```

---
## \#2 Posted by: aigenic Posted at: 2017-07-12T21:50:32.127Z Reads: 170

```
At first you have to give us more information about the board, about voltage, amp ratings, motor, ESC...
```

---
## \#3 Posted by: aigenic Posted at: 2017-07-12T21:51:06.857Z Reads: 161

```
But personally I would not use that board anymore, build a new one, better one :slight_smile:
```

---
## \#4 Posted by: wilkni Posted at: 2017-07-12T22:04:38.318Z Reads: 145

```
Wish I could, but I just got this one and still paying it off. Right now wishing I saved the box to return the thing
```

---
## \#5 Posted by: wilkni Posted at: 2017-07-12T22:11:23.859Z Reads: 141

```
Only things I can tell from the motor is that it's voltage is 36v, rated current is 28.4a and its output is 800w. I don't know a thing about ESC. Motor is a my8919

<img src="/uploads/db1493/original/3X/7/3/73219863239c8dfe25976c9fa7c57450eacc96e6.jpg" width="375" height="500">

If it helps, everything on it is still factory.
```

---
## \#6 Posted by: mwkeefer Posted at: 2017-07-12T22:20:34.285Z Reads: 123

```
What's the voltage of your pack
```

---
## \#7 Posted by: wilkni Posted at: 2017-07-12T22:34:27.105Z Reads: 119

```
Voltage is a 36v 36ah, 3 12v 12 ah batteries in it.
 <img src="/uploads/db1493/original/3X/1/9/19ad6603a0b01b8e5ecde84fc2b7a2311ad5ad93.jpg" width="375" height="500">
```

---
## \#8 Posted by: Jinra Posted at: 2017-07-12T22:36:36.738Z Reads: 115

```
that should be 36v 12ah not 36ah
```

---
## \#9 Posted by: wilkni Posted at: 2017-07-12T22:40:45.174Z Reads: 113

```
Oh dang. 
Sorry when I looked it up on the website 
http://maverixusa.com/products/replacement-sealed-lead-acid-battery-800w-id-8
It said "The Battery itself is capable of generating 3*12 Ampere-hours at 36 Volts."
Thought it meant 3 x 12. So it is 36v and 12ah?
```

---
## \#10 Posted by: Jinra Posted at: 2017-07-12T22:43:07.381Z Reads: 112

```
Yea the batteries are in series for 36v which means the amp hours don't change. Conversely, if they were in parallel it'd be 12v 36ah. You could do something similar with a 10s4p pack of 18650 Li-ion or lipo pouches.
```

---
## \#11 Posted by: wilkni Posted at: 2017-07-12T22:46:45.984Z Reads: 106

```
Awesome, so I'd need to get em to 36v (that much I know) what about the ah, would it be okay to go over 12 or should I stay at 12
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-12T22:47:41.009Z Reads: 102

```
it only affects your range
```

---
## \#13 Posted by: wilkni Posted at: 2017-07-12T22:52:08.550Z Reads: 101

```
Thanks for the help! I'll start working on getting a battery
```

---
## \#14 Posted by: bigben Posted at: 2017-07-12T22:55:01.461Z Reads: 100

```
When I first started on the road to eskates I had bought a malfunctioning board a bit like the one you have.
First I replaced the batteries with lipos. Mine was 24 volts so I went 6s. It was a massive improvement in just weight alone. I made a smaller enclosure too.
Then I smoked the motor so bought a motor from alien power systems. Not realising that the brushless motor I had just bought would need an esc for it and because the esc was integrated with the receiver I would have to replace them too!
Shortly I replaced the trucks, wheels and drive train too.
And so it began....
```

---
## \#15 Posted by: wilkni Posted at: 2017-07-12T23:11:35.794Z Reads: 94

```
Something tells me I'd probably end up in the same boat or end up upgrading it so much that it's not the same board. Now I know, don't buy what you can make yourself. I got so stupidly impatient that I bought it off fingerhut.
```

---
## \#16 Posted by: Michaelinvegas Posted at: 2017-07-13T00:04:15.729Z Reads: 88

```
You can't over volt them?
```

---
## \#17 Posted by: mwkeefer Posted at: 2017-07-13T00:12:34.995Z Reads: 87

```
SLAs rated for 12Ah might be giving you 7 actual AH capacity at the Discharge rate of the board (higher amp Discharge = less capacity and quick sulfation).

 Honestly if you were to do an 8 AM power 10 ass battery using like to fight us 30 5C wiper batteries in series with a little BMS stuck in the board and probably get more arranging a pass anything you do out of your sleds and it would weigh a couple pounds like literally 2 pounds

As a newbie you're probably better off to go with a prebuilt tennis for pizza and a power pack , Make sure that you get Samsung 25 or or equivalent cells so they can handle this and discharge those cells are rated for 20 A continuous discharge rate so in a 4P configuration you have idiots continuous discharge capability although I wouldn't go that far with it

Do you have any idea how much  current your bored uses how many amps the controller drawers there's a question what's the rated power how much do they advertise it as wattage ?

-Mike

PS excuse Siri for being completely stupid
```

---
## \#18 Posted by: detroitwheelin Posted at: 2017-07-13T00:25:55.837Z Reads: 84

```
i have an Altered M4 800 - single 800w motor ,  looks very similar ,  and i'm working to convert it over as well.  One thing to note if you decide to upgrade the ESC is that these motors are Brushed DC (not Brushless).  You can tell because the motor has 2 phase wires,  rather than 3.   you should be able to use VESC set to DC mode (instead than BLDC or FOC).   i'll be testing this soon on mine and will let you know how it goes.
```

---
## \#19 Posted by: wafflejock Posted at: 2017-07-13T00:27:04.377Z Reads: 78

```
[quote="mwkeefer, post:17, topic:27463"]
prebuilt tennis for pizza
[/quote]

You should fire Siri she's a terrible assistant... let her go lightly.  Unless.... you were talking about playing a game of tennis with factory rackets (as opposed to DIY tennis) for a pizza, in which case carry on.
```

---
## \#20 Posted by: wilkni Posted at: 2017-07-13T02:45:03.251Z Reads: 75

```
Only thing that it tells me about power is that the engine is 800w and it's recommended 28.4a. Probably another reason to start building a board instead of buying
```

---
## \#21 Posted by: mwkeefer Posted at: 2017-07-13T07:27:08.329Z Reads: 64

```
Wow, I should have asked you if it was 2 or 3 wires to the motor too :slight_smile:

So 800w @ 12v and somewhere ill assume you see the 28.4Amps so lets check it out 800 / 12 = 66.6 Amps so not at 28.4 Amps and I guarantee your not pulling 66 Amps (or likely even 28.4 A ) from SLA batteries :slight_smile:

Lets check, 28.4 * 12 = 340.8 watts so more likely this :slight_smile:

Im thinking its time to build a whole new board brother, if you want to get just a better battery seek out a LifePo4 4S 10AH or better pack capacity and it should be plug and play with the 12v SLA system in that board.

Hope that helps some!

Regards,
Mike
```

---
## \#22 Posted by: wilkni Posted at: 2017-07-20T11:45:34.081Z Reads: 47

```
Thanks for all the help guys, my computer had issues ... but I fixed it and I wanted to wait a bit before telling anyone. I saw a 36v battery a friend of mine used for an ebike. I put the plug wire adapter for my board and bolted it on and it works so far. Since Monday, been riding it at least 2 hours straight and no problem. Oddly enough it feels like it goes faster, just guessing its cause the board is 30lbs lighter. 
<img src="/uploads/db1493/original/3X/b/a/baa49004da0d42ea856ebf34a5ea73bae6da4a33.jpg" width="281" height="500">
Just in case anyone is wondering what the battery was
```

---
## \#23 Posted by: wilkni Posted at: 2017-07-23T05:53:45.534Z Reads: 30

```
Just road my board a bit, was having fun and it suddenly stopped and won't turn back on. Best guess is, it's probably like other users, the ESC burned out. Best advice to anyone who is looking at this chat looking to customize their maverix is to replace the board or don't buy one. Replacing the battery would be a start, then you'd replace the ESC because it'd fry over. Then you'd consider replacing it's trucks or motor but the trucks are attached to the motor mount or cover. By the time you're done, you'd probably have built a new board.
```

---
