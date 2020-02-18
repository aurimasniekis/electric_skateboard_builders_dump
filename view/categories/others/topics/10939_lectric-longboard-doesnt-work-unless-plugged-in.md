# Lectric Longboard doesn&rsquo;t work unless plugged in

### Replies: 13 Views: 2475

## \#1 Posted by: Atimu Posted at: 2016-10-11T03:06:47.520Z Reads: 175

```
This is a "Lectric Longboard" (you can find their site through google), which is one of many of the Chinese clone boards. 
The issue is when not plugged in, the board turns on as usual, makes the turning on noise, ESC fan turns on, but upon pressing the throttle up, the motor spins for 1 second and then the whole board shuts down. It works as normal when plugged in to an outlet. When the charger is removed while the throttle is pressed, it seems to work fine but only until you let go, as demonstrated in the video below. 

I suspect that it is the BMS that is at fault here. The battery works on my brother's board (which is the exact same board). Motor seems fine. In terms of electronics, I haven't tried playing around with anything inside in an effort to avoid warranty issues. 
I have been contacting support but they often take a day or longer to respond so I would be very thankful for any help from anyone really to get this board up and running asap.

https://www.youtube.com/watch?v=29d1Q9lC0Oc
```

---
## \#2 Posted by: VladPomogaev Posted at: 2016-10-11T03:42:32.370Z Reads: 156

```
If you suspect the BMS is the issue, measure the battery voltage after charging the board. If it's not full then the BMS might be at fault.
```

---
## \#3 Posted by: Namasaki Posted at: 2016-10-11T06:07:11.364Z Reads: 133

```
Because of the way it's wired up, you could just have a bad connection. The connectors at the power switch are especially suspect. But check all connections from the battery. Check solder joints by pulling lightly on the wires while wiggling them slightly. If a wire breaks loose, then it was a bad joint. The Bms doesn't look overheated so I would not suspect it right off. More likely to be a bad wire connection.
It looks like the battery wire has to go through the power switch to reach the system. Start there.

Btw, it looks pretty straight forward and easy to work on. Actually a lot like a Diy system.
Your lucky, some production boards are so proprietary, you can't do a thing with them.
Good Luck and please let us know how it turns out.
```

---
## \#4 Posted by: Ethanwind Posted at: 2016-10-11T13:43:54.346Z Reads: 109

```
It's probably the bms or it could be as simple as the esc not having a good connection to the radio receiver. But I would guess the bms
```

---
## \#5 Posted by: Namasaki Posted at: 2016-10-11T15:37:12.948Z Reads: 93

```
[quote="Ethanwind, post:4, topic:10939"]
It's probably the bms or it could be as simple as the esc not having a good connection to the radio receiver
[/quote]
It's probably not the Esc or receiver because it works fine with the charger plugged in. 
Loss of connection to the battery seems more likely to me. 
Anyway, when trouble shooting, rule out the simple stuff first. Like wire connections.
```

---
## \#6 Posted by: Atimu Posted at: 2016-10-12T18:21:55.225Z Reads: 76

```
I didn't think of checking for bad wiring but I tried connecting the battery directly to the esc and it worked perfectly! I was hesitant in trying this earlier because the dean's plug was super tight and it sparked so I thought I was doing something wrong. My bro has the same board and I tried my battery on his and his on mine, both work on his board but neither worked on mine.
So something must be up with my bms, or the wiring between the battery and esc.

I'd rather not pay the $40 shipping and almost a month wait time for the company to replace it under warranty and all, so I'm wondering if I should replace the bms myself or just use the board without it. But if I were to use the board without a bms I could risk over discharging the battery right? Which I should be able to avoid by attaching a battery indicator/voltage meter? My bro and I ordered vescs to replace the esc's so that should probably help.

The bms still somehow charges the battery though. Without it the remote can't indicate the boards remaining battery, which is why I'd like for it to work. But oddly enough the battery is 6s 8ah li ion but the balancing connector only has 6 pins. So my balance charger (which charges all kinds of batteries) doesn't charge it or my bros battery no matter how much I change settings around. I want to get 6s lipos for more range but they have 7 pins and would need a different bms right? I could just settle for an onboard lcd indicator. 
I also don't know if I should settle for 6s batteries if I want to get a faster motor eventually but I could google that. 
Sorry about all the questions haha Im just getting into diy and its so fascinating
```

---
## \#7 Posted by: Namasaki Posted at: 2016-10-12T19:03:35.212Z Reads: 64

```
The problem is most likely in the wiring. 
Try bypassing the switch and connect the battery directly to the BMS and Esc. and see if it works. 
Usually the battery's black wire goes to the BMS and the battery's red wire goes to the Esc. 
Lipos always have an extra ground wire on the balance harness. 
BMS Boards don't. That's why it only has 6 pins. 
To connect Lipos to a BMS you would need to know the specs of the BMS and if it is compatible with Lipos. The you just connect the 6 color wires and omit the black ground wire from the Lipo.
```

---
## \#8 Posted by: Ethanwind Posted at: 2016-10-13T12:30:07.953Z Reads: 63

```
I would say if you have the money build your own board... I have a lectric board and based off what I can tell so far is that it's pretty hard to upgrade especially if your new with diy. Putting in a vesc would help, and if the bms isn't blow and still works you could take it out and use it as a off board charger it might be a pain. But it will keep it from blowing in the future. It makes the board especially hard to upgrade because it's hard to find the specs of the motor, battery, ect... if you have the specs can you pleas share. I would build a new board. Get a space 4 or 3 battery from enertion it has a built in bms and indicator (kind of expensive but worth it) then get a vesc and a enertion motor (in my opinion they have one of the best motors) and then a 2.4 gh transmitter should work and you will have a professional grade board for around 500 to 800$
```

---
## \#9 Posted by: Atimu Posted at: 2016-10-17T05:32:50.754Z Reads: 56

```
Currently I'm using the board by manually opening the cover every time I need to go out to connect the battery straight to the esc and its working great. I'm rewiring things inside soon and probably am gonna use hinges to make a quick release flap so that I can still connect the bms inside to be able to charge the board on the go and without having to remove the battery. I'll also be putting my vesc in soon. 

I happen to have two 3s 5500mah lipo's that i could connect in series to get extended range. Which means adding an encasing to hold the batteries.

Oh right so the battery it comes with is a 6S1P 21.6V 8,000mah li ion. However, my battery is 320*135*10mm. It does not fill up the entire battery compartment, there's about 2.5 inches of extra space (which i plan on cutting and fitting in the extra lipo's), which my brother's board does not have. His battery fits the entire casing but is not labeled with any information like mine was. But the range, speed, and charging time of both boards seem about the same. 

Email lectriclongboardsco@gmail.com about the motor specs and whatnot. They seem to respond to questions. I'm sure you could buy a different motor mount and fit whatever belts and motors necessary on this board since the existing mount doesnt seem to have much in terms of making belt length adjustments.
```

---
## \#11 Posted by: irlandaise Posted at: 2018-01-11T16:02:29.677Z Reads: 31

```
This company sold a defective board (just like what you’re describing) to my nephew. Can you tell me how you found out that the boards they sell are “clones” from China? We are still trying to get our money back from them. Any info would be helpful, thanks!
```

---
## \#12 Posted by: Mikenopolis Posted at: 2018-01-11T16:16:28.955Z Reads: 27

```
We call them clones because Chinese manufacturer makes these cheap boards and if you can pay and order a large amount they will print your company name and logo on the grip tape, deck and wheels.
```

---
## \#13 Posted by: irlandaise Posted at: 2018-01-11T16:24:59.002Z Reads: 26

```
Thanks thats good to know! This company advertises as though their boards are all custom / hand made, its ridiculous.
```

---
## \#14 Posted by: Mikenopolis Posted at: 2018-01-11T17:19:25.986Z Reads: 21

```
The recent board are Chinese parts shipped to them in Arizona. Then assembled by two guys.
```

---
