# Almost done Connectors right?

### Replies: 21 Views: 808

## \#1 Posted by: Blitz Posted at: 2018-01-05T14:09:59.884Z Reads: 179

```
Almost done biggest worry is Wrong li-po connectors 


Motor KEDA 63-64 190KV
https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html

Battrey 3x in series https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html

series Connectors 2x  https://www.ebay.ie/itm/HXT-4-0mm-1-Jack-to-2-Male-Series-Harness-Battery-Adapter-12AWG-for-RC-Car-Plane/222191569363?hash=item33bba649d3:g:k1UAAOSwIgNXjdlT

and series connector to xt60 https://hobbyking.com/en_us/hxt-4mm-to-xt-60-battery-adapter-2pcs-bag.html

and entertion Focbox
Anything wrong i can solder but not without clear instructions
```

---
## \#2 Posted by: SimosMCmuffin Posted at: 2018-01-05T14:23:36.753Z Reads: 159

```
I would have not made a new topic about this, but rather continued on your "Li-po help topic".

I suppose you're going to change the 5,5 mm bullet connectors coming with the battery to the 4 mm HXT ones? Otherwise you can't use the connectors you listed. You should then add the needed HXT connectors to change the battery wire connectors.
```

---
## \#3 Posted by: Blitz Posted at: 2018-01-05T14:24:50.392Z Reads: 152

```
So just change the5,5 bullet connection to 4mm and i'm good to go?
```

---
## \#4 Posted by: SimosMCmuffin Posted at: 2018-01-05T14:28:28.065Z Reads: 143

```
Yes, assuming that the load side connector has a male XT60, then you this should work, but I recommend getting one more persons opinion first. Just in case I missed anything.

By the way, seeing that you're seem to be in a big hurry. How do you plan to charge the Li-po packs? Do you plan to disassemble the pack for charging?
```

---
## \#5 Posted by: Blitz Posted at: 2018-01-05T14:29:18.283Z Reads: 127

```
NO preferance but most likly 1 by 1
```

---
## \#6 Posted by: Blitz Posted at: 2018-01-05T14:30:20.412Z Reads: 117

```
IF you could just tell me what to get, and i would check with everyone id be done today
```

---
## \#7 Posted by: SimosMCmuffin Posted at: 2018-01-05T14:33:26.191Z Reads: 110

```
Sorry, but I don't know what your setup is, what kind of charging equipment you have, what kind of performance you want, what's your budget, what's your building skill...

This is your build. I recommend trying to learn on your own with available material and via google. Asking about something specific that you're not sure about or don't know is okay, but don't shove your own project into someone elses hands and ask them to make it for you.
```

---
## \#8 Posted by: Blitz Posted at: 2018-01-05T14:34:34.464Z Reads: 102

```
This is like a copy of https://www.youtube.com/watch?v=_G0e4_WeKzw

But my battery has bigger C rating

Also forgot to include i will use focbox

and i want series

and i would balance charge
```

---
## \#9 Posted by: SimosMCmuffin Posted at: 2018-01-05T14:42:19.751Z Reads: 99

```
Can't help, but notice this in the video description
<img src="/uploads/db1493/original/3X/c/b/cb6ad33f11819f9d427efba9b5056afd74b1ba3e.png" width="690" height="314">

And you can also see in the picture that the Batteries have the 4 mm HXT -connector on them, most likely because they are lower C-rated so they don't need the 5,5 mm beefier connectors. You might save yourself some work if you find other similiar sized batteries with the 4 mm HXT connectors already on them. Then everything should just plug straight together, at least on the battery pack side.
```

---
## \#10 Posted by: Blitz Posted at: 2018-01-05T14:44:03.696Z Reads: 90

```
his wires are 12awg so 14 will be good right?
```

---
## \#11 Posted by: JonathanLau1983 Posted at: 2018-01-05T15:26:29.432Z Reads: 87

```
With AWG lower means thicker and therefore higher current rating. So going from 12 to 14 would mean it'll handle less amps, you really should be using lower AWG rating as well as changing the connectors as has been mentioned.

Most people use a minimum of 10AWG, it's what I use for my 6S Lipo setup.
```

---
## \#12 Posted by: Blitz Posted at: 2018-01-05T15:29:12.779Z Reads: 75

```
Ok so i need to find 7-9 AWG cable
```

---
## \#13 Posted by: JonathanLau1983 Posted at: 2018-01-05T15:51:21.555Z Reads: 75

```
You should use 10AWG, any thicker and you'll start running into soldering issues unless you have a decent soldering iron.
```

---
## \#14 Posted by: Blitz Posted at: 2018-01-05T16:27:55.606Z Reads: 75

```
@Kug3lis Said 

You need just buy connectors Like xt90 

Replace on batteries

 Replace on vesc 

Replace on charger, Then buy series adapter 2 of them



SO i just need to solder this on batteries bullet wire, vesc and charger  

https://hobbyking.com/en_us/nylon-xt90-connectors-male-5pcs-bag.html

and then use this Series connector 

https://hobbyking.com/en_us/xt90-harness-for-2-packs-in-parallel-2pcs-bag.html
```

---
## \#15 Posted by: JonathanLau1983 Posted at: 2018-01-05T17:05:58.460Z Reads: 72

```
[quote="Blitz, post:14, topic:42846"]
SO i just need to solder this on batteries bullet wire, vesc and charger
[/quote]

Those connects are male when you want Female for the batteries. The connector you linked is parallel.

You could stick with XT60, they should suffice for what you're doing. It's what the Vesc comes with I think.
```

---
## \#16 Posted by: Blitz Posted at: 2018-01-06T14:22:28.645Z Reads: 62

```
Are you Sure That XT60, would work because it is a lot cheaper for me,
```

---
## \#17 Posted by: GrecoMan Posted at: 2018-01-06T14:24:33.658Z Reads: 61

```
that’s not a fucking series connector

it says “parallel connector” in the name...
```

---
## \#18 Posted by: Blitz Posted at: 2018-01-06T14:26:03.226Z Reads: 59

```
That was a typo you know, Now chill
```

---
## \#19 Posted by: Deckoz Posted at: 2018-01-06T14:27:14.567Z Reads: 60

```
Series
<img src="/uploads/db1493/original/3X/2/7/27263dde0714d68218180cc219c1cef23a2c7c19.jpg" width="565" height="414">

Parallel
<img src="/uploads/db1493/original/3X/3/c/3c08a4d81f4eb65238ffdcba3f7f16cafcba543d.jpg" width="690" height="471"><img src="/uploads/db1493/original/3X/3/e/3e0ee140901dfd5c4f98690d914ffc285de92eb7.jpg" width="450" height="299">
```

---
## \#20 Posted by: GrecoMan Posted at: 2018-01-06T14:29:11.646Z Reads: 56

```
i’ve told you atleast 3 times that that connector isn’t for series. it obliviously wasn’t a typo dude, stop trying to play it off

man i hate liars...
```

---
## \#21 Posted by: Blitz Posted at: 2018-01-06T14:32:23.852Z Reads: 55

```
I know that series is taking the positive from one wire bring it to the negative and then the last positive and negative done,
```

---
