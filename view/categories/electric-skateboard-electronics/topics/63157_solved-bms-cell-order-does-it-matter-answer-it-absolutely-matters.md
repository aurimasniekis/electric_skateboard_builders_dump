# \[ SOLVED \] Bms cell order? does it matter? ANSWER: It absolutely matters

### Replies: 59 Views: 1007

## \#1 Posted by: Jake2k17 Posted at: 2018-07-28T16:29:04.411Z Reads: 175

```
So I’m trying to connect two 5s lipos to a bms from Mboards and I have checked with others and my wiring for the b- and ch- ports on the bms are correct, with a negative lead going to my b- port and my negative charge port wire going to my ch- port. However what is concerning me is my order of balance wires. After reading a long thread about this, I am certain I have it wrong, and I was wondering if someone could tell me the order of the cells, because some color wires repeat. 
@mmaner
@Namasaki
I saw on the other thread that you guys have a lot of knownledge on this topic, maybe you could shed some light on this for me? Thanks
```

---
## \#2 Posted by: mmaner Posted at: 2018-07-28T18:01:08.243Z Reads: 142

```
It definitely matters. Your BMS should have a diagram showing the cell numbers. The battery cell numbers are defined by voltage, the lowest voltage being cell 1 and increasing incrementally to the highest voltage being the last cell.
```

---
## \#3 Posted by: Namasaki Posted at: 2018-07-28T18:28:49.416Z Reads: 133

```
As @mmaner stated, it does matter and if you get it wrong, you will fry the bms. 

I’m at work now but when I get home I will post a couple thoughts that I think will help. 
In the mean time could you post som picks of your Lipos’s wiring and a closeup of the bms balance port top and bottom with the wire connector in place and removed for clarity
```

---
## \#4 Posted by: Jake2k17 Posted at: 2018-07-28T19:34:48.257Z Reads: 122

```
Unfortunately I just left town for the weekend but I have a couple pictures I took before I left.![image|375x500](upload://pE17tBPfFx5zCDIAXzcD61FL1yU.jpeg)![image|375x500](upload://wrZ9fZUH2GftblP6m66VG6vZg87.jpeg) 

The top picture is how I connected the 10 pin connector to the two 6 pin connectors, I stuck the ends of the wires into the 6 pin connectors and hot glued them in place 

My balance wiring starts with the pack that supplies the negative lead, and it goes
10-red
9-black
8-blue
7-white
6-yellow
*Second pack*
5-red
4-Black
3-blue
2-white
1-yellow

I put them in this order because that is what order they connected in on the white plug
```

---
## \#5 Posted by: Namasaki Posted at: 2018-07-28T20:57:06.661Z Reads: 97

```
When you get back we need to start over by first removing the hot glue because you can't just stuff wires in and hot glue them. They need to be soldered or crimped. Or else you will have intermittent connections that will cause a world of problems.
Who ever told you that you could just hot glue the wires in place, Don't take anymore advice from that source.
```

---
## \#6 Posted by: Namasaki Posted at: 2018-07-28T21:01:13.120Z Reads: 98

```
There should be some print on the bms circuit board that identifies the pins of the balance socket.
Can you post a link of the 5s Lipos you are using?

With two 5s packs connected in series.
The pack that supplies the negative main is Batt 1 (Cells 1,2,3,4,5)
The pack that supplies the positive main is Batt 2   (Cells 6,7,8,9,10)

I need to see the balance wires coming from one of your batteries with it's original balance connector to determine the cell order color code.
There is no set standard for balance wire color code except that Red is always the last cell in series for each pack.

So, Batt 1 red balance wire is Cell 5
And, Batt 2 red balance wire is Cell 10

Lipo balance connectors always have an extra balance wire for ground which is always on the opposite end of the Red wire and is usually but not necessarily black.
```

---
## \#7 Posted by: Jake2k17 Posted at: 2018-07-28T21:16:16.432Z Reads: 89

```
Ok starting to make a little more sense

https://www.mboards.co/collections/batteries-1/products/turnigy-5000mah-5s-20c-lipo-pack

This is where I got my batteries from. To see where the balance cables are coming from do I have to take off the shrink wrap?
```

---
## \#8 Posted by: Namasaki Posted at: 2018-07-28T21:20:35.251Z Reads: 80

```
[quote="Jake2k17, post:7, topic:63157"]
This is where I got my batteries from. To see where the balance cables are coming from do I have to take off the shrink wrap?
[/quote]


No, don't take off the shrink wrap.
You identify the color code at the connector end.
```

---
## \#9 Posted by: Jake2k17 Posted at: 2018-07-28T21:21:41.954Z Reads: 80

```
![image|648x500](upload://nZEtKBAoXSh0JbBWgGCNeVRR38u.jpeg) 
On the ten pin connector, the red wire on top with the black mark is 10, the top solder is my ch- port, and the bottom left solder is my b- port
```

---
## \#10 Posted by: Namasaki Posted at: 2018-07-28T21:23:19.163Z Reads: 78

```
Are you sure this is a 10s bms and not a 9s?
The original battery was if fact a 10s?
```

---
## \#11 Posted by: Namasaki Posted at: 2018-07-28T21:30:38.394Z Reads: 76

```
Is the black wire on the bms identified as 1 or G
```

---
## \#12 Posted by: Jake2k17 Posted at: 2018-07-28T21:30:55.842Z Reads: 74

```
https://www.mboards.co/products/10s-bms-battery-management-system

This is the bms and I used and 2x 5s lipos in series
```

---
## \#13 Posted by: Jake2k17 Posted at: 2018-07-28T21:31:50.098Z Reads: 67

```
What black wire? There were no labels, just a confusing diagram let me see if I can pull it up
```

---
## \#14 Posted by: Jake2k17 Posted at: 2018-07-28T21:33:29.300Z Reads: 69

```
![image|281x500](upload://mrZZjuyULNSUpIDnY4h5E9vz5N9.png)
```

---
## \#15 Posted by: Namasaki Posted at: 2018-07-28T21:39:14.189Z Reads: 67

```
Ok, no ground wire on the balance connector.
The bms uses the main ground connected to B- as it's ground source for balancing.
So you only use 5 balance wires from each battery. You do not need to connect the balance ground wire from the battery
```

---
## \#16 Posted by: Jake2k17 Posted at: 2018-07-28T21:41:13.274Z Reads: 64

```
The ground wires are connected to the last cells negative side right?
```

---
## \#17 Posted by: Namasaki Posted at: 2018-07-28T21:42:08.256Z Reads: 65

```
You only connect positive wires to the bms balance connector
```

---
## \#18 Posted by: Namasaki Posted at: 2018-07-28T21:42:58.711Z Reads: 64

```
[quote="Jake2k17, post:16, topic:63157, full:true"]
The ground wires are connected to the last cells negative side right?
[/quote]


The balance ground of each pack is connected directly to the pack's main ground wire.
```

---
## \#19 Posted by: Namasaki Posted at: 2018-07-28T21:50:02.920Z Reads: 60

```
I can't find a clear picture of your battery's balance leads to original connector.
There is another option. We can identify them with a volt meter.
```

---
## \#20 Posted by: Jake2k17 Posted at: 2018-07-28T21:52:13.733Z Reads: 59

```
Ok thanks. I think I understand where everything goes, however I just need the order of the balance cells. I’m not a slacker, but I’m really inexperienced with multi meters and I was hoping that you might know which orders the balance wires go in
```

---
## \#21 Posted by: Jake2k17 Posted at: 2018-07-28T21:53:20.717Z Reads: 55

```
I remember which order they were in on the connector

Red 
Black 
Blue
White
Yellow
Black

From left to right
```

---
## \#22 Posted by: Namasaki Posted at: 2018-07-28T21:56:06.690Z Reads: 54

```
What is this?

![27%20PM|375x263](upload://sWI7fuGhk7OPBuvvPdlwxRB7zok.png)

Never mind, I get it, those are the bms wires
```

---
## \#23 Posted by: Jake2k17 Posted at: 2018-07-28T21:58:52.820Z Reads: 52

```
Uhhh
Well I though it would be easier than soldering so I stuck all of the wires from the ten pin into the male connector of the 6 pins
```

---
## \#24 Posted by: Jake2k17 Posted at: 2018-07-28T21:59:16.762Z Reads: 52

```
Yeah exactly
```

---
## \#25 Posted by: Namasaki Posted at: 2018-07-28T22:01:34.869Z Reads: 52

```
**Battery 1**
Red---------Cell 5
Black-------Cell 4
Blue--------Cell 3
White------Cell 2
Yellow-----Cell 1

**Battery 2**
Red---------Cell 10
Black-------Cell 9
Blue--------Cell 8
White------Cell 7
Yellow-----Cell 6
```

---
## \#26 Posted by: Jake2k17 Posted at: 2018-07-28T22:02:26.011Z Reads: 51

```
So if I connect the balance wires in that order it will charge?
```

---
## \#27 Posted by: Namasaki Posted at: 2018-07-28T22:03:54.621Z Reads: 51

```
I would connect the balance wires from the batteries directly to the wires from the bms balance connector.
You can solder them together and insulate them with shrink tube or use small crimp connectors.
I've done it both ways and soldering them makes the least bulky harness 
You will need to use a volt meter to make sure which black wires are ground and which are cells 4 and 9
```

---
## \#28 Posted by: Jake2k17 Posted at: 2018-07-28T22:06:01.765Z Reads: 51

```
Damn it 

Well if it helps I already pulled apart and old turnigy 5s battery and the black wire on the right is soldered onto the negative wire
```

---
## \#29 Posted by: Namasaki Posted at: 2018-07-28T22:07:18.897Z Reads: 51

```
did you already remove the original battery balance connectors?
```

---
## \#30 Posted by: Jake2k17 Posted at: 2018-07-28T22:08:04.551Z Reads: 50

```
No I pulled off the shrink wrap and yellow tape to look for the black wires
```

---
## \#31 Posted by: Namasaki Posted at: 2018-07-28T22:13:23.937Z Reads: 49

```
If you have a hobby charger, you should fully balance charge the packs before putting them together in series and connecting them to the bms.
Otherwise, if they are not closely balanced, the bms will struggle to fully charge them.
```

---
## \#32 Posted by: Jake2k17 Posted at: 2018-07-28T22:14:22.113Z Reads: 48

```
Yeah I already did that stuff. They are both at 18.80 volts right now
```

---
## \#33 Posted by: Jake2k17 Posted at: 2018-07-28T22:18:59.430Z Reads: 50

```
Here is what hobby king customer support told me
![image|666x500](upload://174HSZK0HqSD2Y07WadRTz0PL6A.jpeg)
```

---
## \#34 Posted by: Namasaki Posted at: 2018-07-28T22:21:03.745Z Reads: 49

```
I thought that you had removed the original battery balance connector.
the ground balance wire is always on the opposite edge from the Red wire.
That is a standard.
```

---
## \#35 Posted by: pat.speed Posted at: 2018-07-28T22:21:28.715Z Reads: 49

```
I think that diagram that is supplied is actually wrong, I’m 99% sure that the b1 lead goes on the left hand side of the bms balance connector. It says the order on the bottom of the bms. I could be wrong but that’s how I remember seeing it. I can open up my board to show you guys if needed
```

---
## \#36 Posted by: Namasaki Posted at: 2018-07-28T22:23:51.709Z Reads: 47

```
You have an MBoard bms?
```

---
## \#37 Posted by: Jake2k17 Posted at: 2018-07-28T22:23:52.616Z Reads: 47

```
right that is what the guy from hobby king said. I never removed the original connector, I just stuck the wires coming from the ten pin connector into the other side.
```

---
## \#38 Posted by: pat.speed Posted at: 2018-07-28T22:25:31.034Z Reads: 46

```
Nope, but the identical one from eBay, it works fine just has a low balancing current. 

And that diagram seems to be correct I found some images of the back side. Damn it...stupid memory getting shit wrong
```

---
## \#39 Posted by: Jake2k17 Posted at: 2018-07-28T22:26:48.292Z Reads: 47

```
Yeah Mboards gets his from that eBay China seller
```

---
## \#40 Posted by: Namasaki Posted at: 2018-07-28T22:27:48.700Z Reads: 49

```
What I did on my builds that worked well and would work well in your case is to get 2 balance wire extensions that you plug into the battery balance connector and then cut the connector on the other end of the extension off and connect the wires directly to the balance wires from the bms either by soldering them or with crimp connectors.
That setup makes it easy to maintenance or replace your packs if need be.
Make sure that the extensions are not connected to the batteries when you cut them and connect them to the bms harness. It's very easy to short your battery if it's connected.
```

---
## \#41 Posted by: Jake2k17 Posted at: 2018-07-28T22:29:40.345Z Reads: 44

```
ok i have two of those that i used for balance charging
```

---
## \#42 Posted by: Jake2k17 Posted at: 2018-07-28T22:33:23.965Z Reads: 44

```
@pat.speed
I'm positive that b10 is on the left side

Also do you use lipos or li ions?
```

---
## \#43 Posted by: pat.speed Posted at: 2018-07-28T22:45:07.180Z Reads: 46

```
If this helps this is how I connect my batteries.

1. connect them in series (red of one to black of other)

2. Work out which balance lead is the first one (the lead also connected to the main black wire of the battery)

3. Cut the bms wires to desired length

4. One bms wire should be black that is the first one

5. Plug that black wire into the first wire of the battery (in your case skip the first one and plug it into the second lead)

6. Sequentially connect all of the next wires to the bms wires making sure to skip the first wire of the second plug (as that is already connected to the last wire of the first plug)

7. Once all leads are connected, start from the first wire and check that all cell voltages increase by about 3.6-4.2v each time you move the second multimeter lead over a cell/ hole.

8. Once verified that all cells are in the correct spots, solder the b- lead to the bms and c- or p- too if need. (It is very important to connect these first before the balance wires or it can fry the bms)

9. Once it’s all connected and not smoking, charge the battery to full voltage while measuring each cell periodically though the charge, especially near the end to make sure they aren’t over charged. (I have noticed my cells being charged to 4.23v before but are then balance back to 4.2 shortly after)

10. Go rip around your town and have some made fun on your new eboard that has a one plug charge system

Hope it helps a bit, and sorry if there’s any errors. @Namasaki could you plz just verify that sounds correct, I wouldn’t want to cause damage to anyone else property based on bad advise
```

---
## \#44 Posted by: pat.speed Posted at: 2018-07-28T22:46:36.118Z Reads: 43

```
Lipos, 10s5000mah in 5x 2s and a 12s5000mah with 4s3s. Each pack gets me about 20km at 20km/h cruising speed, much more if I walk the dog, since I go about 10km/h
```

---
## \#45 Posted by: Jake2k17 Posted at: 2018-07-28T22:52:38.982Z Reads: 44

```
that all seems pretty accurate, it would be:

*first pack (supplies negative lead to Vesc)*
b1-yellow
b2-white
b3-blue
b4-black
b5-red
*second pack (supplies positive lead to Vesc)*
b6-yellow
b7-white
b8-blue
b9-black
b10-red

negative lead to b-
charge port negative to ch-
charge port positive to positive lead

@Namasaki could you verify
```

---
## \#46 Posted by: pat.speed Posted at: 2018-07-28T22:57:33.306Z Reads: 42

```
Seems right except for that the red and black wire shouldn’t be next to each other, they should be at opposite ends of the plug
```

---
## \#47 Posted by: Namasaki Posted at: 2018-07-28T22:58:26.619Z Reads: 41

```
First pack supplies negative main to B- on bms

Second pack supplies Positive main to Vesc and positive lead to charge port
```

---
## \#48 Posted by: Namasaki Posted at: 2018-07-28T22:59:17.660Z Reads: 40

```
[quote="pat.speed, post:46, topic:63157, full:true"]
Seems right except for that the red and black wire shouldn’t be next to each other, they should be at opposite ends of the plug
[/quote]


Abnormal color coding on these batteries.
They have two black balance wires
```

---
## \#49 Posted by: Jake2k17 Posted at: 2018-07-28T22:59:56.408Z Reads: 40

```
there are two black wires, the one next to red is a positive cable, the one on the end is the ground wire
```

---
## \#50 Posted by: pat.speed Posted at: 2018-07-28T23:00:03.858Z Reads: 39

```
Ahh all g then
```

---
## \#51 Posted by: Namasaki Posted at: 2018-07-28T23:05:54.408Z Reads: 38

```
Looks like you have it all figured out now.
Follow @pat.speed advice and test voltages at the bms connector after you have it all wired and before you plug it into the bms.
Volt meter negative probe on the main negative wire from battery 1
Then check pins 1 through 10. voltage should increase by apx 4.2v at each pin in succession.
```

---
## \#52 Posted by: Jake2k17 Posted at: 2018-07-28T23:10:20.326Z Reads: 38

```
Ok. 
@Namasaki Thank you so much for taking time out of your day to help a noob. I hope this thread can also help other people with bms and lipos. 

Getting back from vacation on monday, will fix problem and post pictures when done.
```

---
## \#53 Posted by: Jake2k17 Posted at: 2018-07-29T03:37:17.899Z Reads: 35

```
Wait
@Namasaki
Sorry to bug you, two small questions:

1) since the bms/ charger is connected to my power leads, does my board need to be powered on for it to charge?

2) my 42 volt Mboards charger has an led that is green when charge full or disconnect, and red is charging, will this work with lipos if all my wiring is correct?
```

---
## \#54 Posted by: mmaner Posted at: 2018-07-29T03:50:31.600Z Reads: 35

```
Yes, the BMs needs to be in to charge. If the charger is the correct voltage and the +/- match you should be good.
```

---
## \#55 Posted by: Jake2k17 Posted at: 2018-07-29T04:11:23.905Z Reads: 33

```
thank you guys for all the help
```

---
## \#56 Posted by: Namasaki Posted at: 2018-07-29T22:29:14.862Z Reads: 31

```
[quote="Jake2k17, post:53, topic:63157"]
1. since the bms/ charger is connected to my power leads, does my board need to be powered on for it to charge?

2. my 42 volt Mboards charger has an led that is green when charge full or disconnect, and red is charging, will this work with lipos if all my wiring is correct?
[/quote]


1. Your board does not need to be powered on to charge the battery with that bms.
2. Your 42v Mboards charger will work because lithium ion and Lipos both have the same voltage at full charge.

Connect the charge port positive directly to the positive main of your battery.
The charge port negative goes through the bms to the battery.

![59%20PM|656x500](upload://eI3Jfpcd57kDf7qV11KtR7OwTKb.png)
```

---
## \#57 Posted by: Vinny1 Posted at: 2018-12-15T04:43:31.497Z Reads: 22

```
So is the post marked solution correct if I follow this?
```

---
## \#58 Posted by: J_Dizzle Posted at: 2018-12-15T18:24:03.859Z Reads: 19

```
Yes, that is correct
```

---
## \#60 Posted by: janjan Posted at: 2019-07-27T01:03:15.635Z Reads: 6

```
First off I would like to say thank you to the main contributors on this discussion as it cleared a lot of stress in my mind. I am however still running into charging problems with my diy build and I’m using the exact same setup and and I just followed your wiring guide. My brick still shows green when plugged in when the batteries are discharged. My balance wires are in the correct order from B10-B1 and so are the Ch- and B- ports. 
I would really like some help as this is the the very LAST problem I have to fix which is preventing me from enjoying my full diy build

![image|375x500](upload://nhqeVQkUR7f6KBhDKV0g9FcLHcx.jpeg) 
![image|375x500](upload://dJEnGQfwiVt5vrr0CEZYyKVRyES.jpeg) 

I would love to know if anything seems wrong with my BMS or the wires (too thin or something)
I am still wondering if that extra black balance at the end of the first pack(negative main to VESC) port is still supposed to be connected to the B- port along with the negative main lead. I have tried both with and without to no luck.
```

---
