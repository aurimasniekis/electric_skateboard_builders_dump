# THE COMEBACK - Need Some Tips

### Replies: 33 Views: 312

## \#1 Posted by: persk8 Posted at: 2019-01-23T14:28:54.786Z Reads: 119

```
Ok, some time ago I built myself an electronic skateboard and Is now coming back to it. 

Are there any upgrades I can do without having to replace anything? Add new batteries to make it go longer or duel motors? 

My build: 

5000 mah 5s x 2 
230 KV 
1x Vesc
Abec 11 - 90mm
```

---
## \#2 Posted by: linsus Posted at: 2019-01-23T14:31:08.148Z Reads: 112

```
That doesn't really say anything.

You can start with what you expect to get from the board and we can give you pointers towards that goal.
```

---
## \#3 Posted by: mynamesmatt Posted at: 2019-01-23T14:31:11.158Z Reads: 108

```
yes
10char
```

---
## \#4 Posted by: persk8 Posted at: 2019-01-23T14:33:16.202Z Reads: 100

```
I would like to get more lenght - Making it able to ride for a longer distance. And I am wondering if its possible to do a duel with 230 KV and what would I need for that? 

I read somewhere that 230 KV from torque was 190 KV.
```

---
## \#5 Posted by: linsus Posted at: 2019-01-23T14:39:36.268Z Reads: 89

```
[quote="persk8, post:4, topic:81822"]
I read somewhere that 230 KV from torque was 190 KV.
[/quote]
I dont even..

To get more range you need to change/add to the battery. Not sure what "5000 mah 5s x2" is but I'm guessing its Lipos. You need another VESC for dual motors. and if you expect to draw some current without voltage sag you're going to need a beefier battery on a dual setup.
```

---
## \#6 Posted by: Riako Posted at: 2019-01-23T14:41:57.513Z Reads: 70

```
You could take 2 new 5s5Ah to your already 10s5Ah (I guess), you make another battery pack and cnnect them in // to get 10s10Ah and you double the C rating ;)
```

---
## \#7 Posted by: persk8 Posted at: 2019-01-23T14:42:22.695Z Reads: 62

```
Would that be safe for the vesc? That would double my distance basically?

I am sorry but i have forgotten everything, researched 5 hours today to try to find out things, but decided to just ask instead
```

---
## \#8 Posted by: Riako Posted at: 2019-01-23T14:43:56.499Z Reads: 57

```
You will don't have to touchc the vesc, same voltage here (just the battery capacity that double)

you could also dual your 230kv if it something like 6354/6355 motor and so add a vesc.

EDIT : yes it should double the range as you will have a better indice of discharge also.
```

---
## \#9 Posted by: persk8 Posted at: 2019-01-23T14:44:57.467Z Reads: 57

```
its a 6374 so I guess its not good for a doble

I think I will go for double the batteries then :slight_smile:
```

---
## \#10 Posted by: Riako Posted at: 2019-01-23T14:45:50.572Z Reads: 58

```
ha yes you could dual diagonal or one motor by truck side (reverse) 
[quote="Riako, post:4, topic:41074"]
It could fit this way …
[ ![|650x500](http://1.bp.blogspot.com/-R0JBT5aV6OM/UXoWzM5U1wI/AAAAAAAAFzQ/GTWZcOzH6r0/s1600/CIM-Motor-Drive.JPG) ](http://1.bp.blogspot.com/-R0JBT5aV6OM/UXoWzM5U1wI/AAAAAAAAFzQ/GTWZcOzH6r0/s1600/CIM-Motor-Drive.JPG)
even 6374 or 63110 :blush:
In any case more than 2 6355 will not fit, plus they’re some who don’t fit the lastest 6355 by Maytech …
Dual 6354 we know it’s possible.
[/quote]
```

---
## \#11 Posted by: linsus Posted at: 2019-01-23T14:46:32.499Z Reads: 52

```
You dont double the C rating... you will have same C rating on 10Ah. thats it.
```

---
## \#12 Posted by: Riako Posted at: 2019-01-23T14:48:33.994Z Reads: 49

```
if you take your initial 10s 5Ah (let say 15c) and add the same one in // so you have : 

10s 10Ah 30c thats all ;)
```

---
## \#13 Posted by: linsus Posted at: 2019-01-23T14:49:09.523Z Reads: 46

```
No, you'll have 10S 10Ah 15C.
```

---
## \#14 Posted by: persk8 Posted at: 2019-01-23T14:50:04.958Z Reads: 46

```
Thanks for the fast reply Riako and linsus. And yes the C rate will be the same. 

I think I will just add new batteries for now, and I will see in the summer how it does uphill. I remember it sucked uphill so haha maybe another engine later
```

---
## \#15 Posted by: linsus Posted at: 2019-01-23T14:53:46.442Z Reads: 50

```
[quote="persk8, post:14, topic:81822"]
engine
[/quote]

Sorry if I sound like an angry EMO but its an electric MOTOR. An ENGINE is something else.

[quote="persk8, post:14, topic:81822"]
I think I will just add new batteries for now, and I will see in the summer how it does uphill. I remember it sucked uphill so haha maybe another engine later
[/quote]

Think you'll notice a big difference with twice the amp(assuming you have something like 6374 size that can handle it), if you still struggle in hills then yes another motor would probably be nice.
```

---
## \#16 Posted by: persk8 Posted at: 2019-01-23T14:58:17.156Z Reads: 44

```
No worries, totally understand. I would be a angry emo if I were asked these questions in a niche I knew a lot in. :) But ohwell, you guys helped me a lot , so thanks. I was thinking about adding batteries, but was worried the vesc would break dont know why ..
```

---
## \#17 Posted by: Riako Posted at: 2019-01-23T14:58:50.938Z Reads: 48

```
![Capture_pp|690x384](upload://hu36n0OWtJQ2HMOdirVFBMOivqk.jpeg)
```

---
## \#18 Posted by: linsus Posted at: 2019-01-23T15:01:47.671Z Reads: 46

```
As you can see from the picture you posted, Its not twice the C rating from doing a two 15C parallel. 10Ah x15 = 150A (cont) and 10Ah x30 = 300A (peak).
```

---
## \#19 Posted by: persk8 Posted at: 2019-01-23T15:03:30.882Z Reads: 44

```
On the calc it says 30 KM , thats far :D
```

---
## \#20 Posted by: Riako Posted at: 2019-01-23T15:08:14.282Z Reads: 40

```
Finally !!! Thanks a lot for highlighting the solution I had in front of me !! I wanted to understand  why I'm thinking this since the beggin and nobody correct me during the last 6 years :D :+1:
```

---
## \#21 Posted by: b264 Posted at: 2019-01-23T15:09:10.865Z Reads: 34

```
Scrap the 230kv all together.  Go for 190 kv or lower.
```

---
## \#22 Posted by: persk8 Posted at: 2019-01-23T15:09:37.612Z Reads: 31

```
any reason why?
```

---
## \#23 Posted by: persk8 Posted at: 2019-01-23T15:20:09.771Z Reads: 32

```
What is 10s5p (what the heck is the P for)
```

---
## \#24 Posted by: Andy87 Posted at: 2019-01-23T15:22:44.239Z Reads: 32

```
How much cells in parallel
```

---
## \#25 Posted by: Andy87 Posted at: 2019-01-23T15:23:21.510Z Reads: 33

```
More torque
```

---
## \#26 Posted by: persk8 Posted at: 2019-01-23T15:25:06.862Z Reads: 32

```
ah ok, so in theory I could connect 10 x 5000 mah 5s battieris in parallel without damading the vesc or engine?
```

---
## \#27 Posted by: persk8 Posted at: 2019-01-23T15:26:30.885Z Reads: 34

```
and why would I need to drop the 230KV all together I didnt understand that one. Whats so bad with 230KV?
```

---
## \#28 Posted by: Andy87 Posted at: 2019-01-23T15:27:19.388Z Reads: 32

```
10 is the serial count, 5 is the parallel count in this case.
You would have 10packs with each 5 cells in parallel and those wired up in series
```

---
## \#29 Posted by: Andy87 Posted at: 2019-01-23T15:29:25.856Z Reads: 30

```
[quote="persk8, post:26, topic:81822"]
10 x 5000 mah 5s
[/quote]

About which cells you speak?
5000mAh is probably lipo. With lipos you don’t need a 5p configuration (Usually).
```

---
## \#30 Posted by: wafflejock Posted at: 2019-01-23T15:35:06.150Z Reads: 32

```
@persk8 yeah to try and summarize the above when you have a 5S LiPo pack, you have 5 cells in series in that one pack.  If you chain one of those packs in series with another one then you have 10S (10 cells in series, 5S + 5S in serial configuration).  If you want to increase the Ah (capacity) and max Amps you can draw from a given "battery" (set of cells) then you want more cells in parallel (1S 2Ah cell + 1S 2Ah cell in parallel equals 1S 4Ah battery, if you do the same two cells in series you have a 2S 2Ah battery, voltage doubles in series capacity stays same, with parallel connections between cells it's the opposite so capacity doubles voltage stays the same).

With LiPo packs the way the packs are designed (number of layers surface area etc. etc.) can effect the C rating or max current draw so you can have cells that have much higher discharge ratings than a 18650 style solid cylinder cell.  You'll see lots of 10S4P or 10S5P if using 18650 form-factor cells because of the need to get the discharge amperage higher and avoid voltage sag (pulling too many amps from the cells makes them heat up from internal resistance and creates heat loss and lowers voltage delivered to other components).
```

---
## \#31 Posted by: persk8 Posted at: 2019-01-23T16:01:50.465Z Reads: 26

```
Waow, that made everything "click". I am currently using 30C batteries from hobbyking. I am not sure if i have the budget to switch batteries atm. 

What do you think about the motor @wafflenock ? Is 230KV fine or what would you say would be a ideal set up if i have the 5s 5000 mah x 2 from before?
```

---
## \#32 Posted by: wafflejock Posted at: 2019-01-23T16:36:03.572Z Reads: 28

```
Agree with others here it's all trade offs but if you go single drive then a 190kv (or so) seems to be the sweet spot between enough torque and speed for most people (heavier riders and/or hilly areas need more torque less kv/speed typically, also I'm assuming 'standard' pulley sizes that will change your speed/torque trade off as well, more teeth on wheel vs motor means wheel turns less per turn of motor so less speed but more torque).

Personally have a 149kv 6374 (unsensored Turnigy SK3) with 10S LiPo cells, 2x5S in series, makes charging easier for me.  But if I'm honest I didn't do enough research when I jumped into this and at the time there seemed to be a lot more mixed opinion on the best option (also this is what Benjamin Vedder, original guy behind the VESC and main developer, had been using and suggesting at the time due in part I think to issues with the DRV chip blowing out at higher RPMs).

All that said given my current understanding of things and seeing others experiences here 190kv or so and 10S seems about the "best" for most people (assuming not attempting to achieve speed records or climb mount Everest).  If you need more torque or want more stable high speed braking then I think dual motor is probably worth it (no experience just imagining), but more components is more chance for things to fail, but mixed bag since you are also splitting the electrical load and other forces across two belts motors mounts etc instead of one, so again all trade offs.
```

---
## \#33 Posted by: persk8 Posted at: 2019-01-23T16:48:54.334Z Reads: 24

```
Ok will look into 190kv then :)
```

---
