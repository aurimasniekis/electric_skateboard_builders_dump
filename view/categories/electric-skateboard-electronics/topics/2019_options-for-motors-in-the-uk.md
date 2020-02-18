# Options for Motors in the UK

### Replies: 18 Views: 2209

## \#1 Posted by: bigben Posted at: 2016-03-28T10:47:59.896Z Reads: 101

```
Hi,
1st post here after the introduction post.. So go easy on me...
I've got an old 8ball carver board which is now up and running with the new turnigy 3c 5000mah batteries.
The huge motor that is attached to this board is very dated and a bit smelly and under performing. I'm looking into trying to replace it with something to get this up and running, Ideally something available in the Uk. After scouring the forums on likely threads I've found a few pointers in amongst the threads but seem to find nowhere to buy what I think i need to buy in the UK. Most of the threads seemed to go off on a tangent of my motor is better than your motor...
All the hobby king motors seem to be on back order and the other motors i looked at seem to have massive shipping costs.
This is merely going to be a get me by until i decide what to build and really spend out so possibly my downfall but for this application we are talking tight budget...
```

---
## \#2 Posted by: akira Posted at: 2016-03-28T10:57:24.097Z Reads: 100

```
Alien power system in UK maybe
 http://alienpowersystem.com/product-category/brushless-motors/63mm/
```

---
## \#3 Posted by: monkey32 Posted at: 2016-03-28T12:11:42.622Z Reads: 95

```
I second alien, also e maxx
```

---
## \#4 Posted by: bigben Posted at: 2016-03-28T15:40:11.895Z Reads: 88

```
Brilliant, thanks for the replies. Any of the alien motors I should particularily look for or avoid or is that too much of a how long is a piece of string question?
```

---
## \#5 Posted by: monkey32 Posted at: 2016-03-28T17:23:54.482Z Reads: 88

```
Size matters- more copper = better or higher power output. Generally 63mm motors are becoming more and more the norm....however two 50mm motors will also serve and I started pushing my 100kg with a single 50mm. Depends on a number of factors including:

Power source
Pulley ratio
Wheel size
ESC
And mount type

I highly recommend that you read read read at this point. Look at what others here have built.....learn the material.....ask questions in their threads.....read the intro guides and then read more threads. Endless sphere also has a butt ton of info about eskates. Whitepony, Okp, Runplayback, longhairboy,  cmadson all have numerous sexy builds most well written up. Onloop- the forum leader and owner of Enertions is also very knowledgeable and put some sticky threads here with tons of info. 
Moral of story best way to do this I think.......dive into the literature....when questions come up search for the answers there first......who knows you may find someone that's already done what you are trying to do

- end rant
```

---
## \#6 Posted by: willpark16 Posted at: 2016-03-28T20:26:04.075Z Reads: 82

```
arent alien motors said to break often or rather the copper comes out
```

---
## \#7 Posted by: dogeatgod Posted at: 2016-03-29T16:33:51.261Z Reads: 73

```
[Converted][1] similar using SK3 192KV for a 10S VESC set up and an SK3 245KV for a 6S set up.

The [192][2] is in stock at European warehouse.

Let me know if you need links to belt and pulley suppliers in UK.

Conversion is easy.


  [1]: http://www.electric-skateboard.builders/t/pink-sector-9-10s-vesc-sk3-192kv-gt2b/1646
  [2]: http://www.hobbyking.co.uk/hobbyking/store/uh_viewitem.asp?idproduct=42024
```

---
## \#8 Posted by: bigben Posted at: 2016-03-29T17:05:06.628Z Reads: 72

```
Thanks,
that sounds like it might be a simple way ahead. The mounting holes on the original motor bracket are 3 hole so I guess that will need changing too? (Doesn't seem like the casting would lend itself to re drilling)
I was planning on using all the original remote and power control system (esc?)but with 3x 3c 5000mah turnigy. Would that make this a 9c setup?
```

---
## \#9 Posted by: dogeatgod Posted at: 2016-03-29T17:14:40.755Z Reads: 70

```
Click the blue converted on earlier post - it's a link - shows how to mount motor.
Not sure the original ESC will work with your battery set up, they run off either a 12 or 24v supply.
```

---
## \#10 Posted by: bigben Posted at: 2016-03-29T17:43:25.531Z Reads: 70

```
That is perfect. Just the info I'm after. 
The original battery set up was 3x 12v lead acid so I went for the 3x 3c turnigys so as to be somewhere near. Seemed to make sense to me at the time! For the motor shaft I guess I'll have to grind a flat and grub screw the new pulley to it. If you had link to a pulley supplier then that'd be great. 
No adjustment with drilling the holes in the plate like you did so was it difficult to get the belt length right?
```

---
## \#11 Posted by: dogeatgod Posted at: 2016-03-29T18:08:01.289Z Reads: 68

```
[Pulleys][1] - Click options for adding keyway, grub screw and getting correct diameter bore.

I needed to adjust belt tension after mounting a 14T pulley this was done by drilling bigger mounting holes and using smaller bolts to grant movement, not had any problems as of yet. 



  [1]: http://www.beltingonline.com/16-tooth-htd5-pulley-16-5m-15f-7774
```

---
## \#12 Posted by: bigben Posted at: 2016-04-05T18:05:46.715Z Reads: 66

```
Heres a really dumb Question but the original motor was a great big heavy brushed thing with just a positive and negative.
The brushless motors have 3 wires, does this mean I'm on a losing streak trying to run the original speed controller?
```

---
## \#13 Posted by: trbt555 Posted at: 2016-04-05T19:58:00.096Z Reads: 65

```
You can't use a brushed controller for a brushless motor.
```

---
## \#14 Posted by: dogeatgod Posted at: 2016-04-05T20:05:06.230Z Reads: 64

```
Brushless motors work differently to brushed - the 3 wires are powered in pairs, creating a magnetic field that turns the rotor part of a revolution the ESC sequences these pairs to create continuous rotation. You will need to replace ESC and RC.
```

---
## \#15 Posted by: bigben Posted at: 2016-04-05T20:46:36.220Z Reads: 61

```
Thanks guys for your replies.
Easy when you know how! Possibly flogging a dead horse then!
Time to look at a proper build.. At least I've got a brushed motor as a starting point now!
```

---
## \#16 Posted by: bigben Posted at: 2016-04-05T22:04:49.105Z Reads: 60

```
So I'm now looking for something like this?

http://www.hobbyking.com/hobbyking/store/__44473__HobbyKing_YEP_150A_2_6S_SBEC_Brushless_Speed_Controller_UK_Warehouse_.html

Looked through the site for other options but this is the only one I came up with.
Coupled with a transmitter.
```

---
## \#17 Posted by: dogeatgod Posted at: 2016-04-06T08:24:10.520Z Reads: 60

```
A cheap controller reliable controller is the GT2B - you plug it into an ESC,

I've been using an EZRUN 150A PRO ESC on a 6S set up and it's been great.

I think you would be better starting from scratch and working out what you are trying for - speed-range-acceleration etc then work out the motor, gearing, battery, ESC needed for your weight and wheel size.

It's easy to just start throwing money at bits and then find out you need to change battery, motor, ESC to get the performance you want.

Where in the UK are you?
```

---
## \#18 Posted by: bigben Posted at: 2016-04-06T12:41:55.494Z Reads: 60

```
Many thanks for the info. 
Like I say I could be flogging a dead horse and could possibly do with starting afresh..
I'm down the south west near Weymouth. Not seen any electric skates here so no comparison really.
```

---
