# Build1 &#124; TorqueBoards v2 trucks &#124; sk3-6364-190kv &#124; 10S5P &#124; VESC

### Replies: 14 Views: 2808

## \#1 Posted by: BenL Posted at: 2017-06-21T00:43:26.496Z Reads: 305

```
The core of the build plan is as follows:

sk3-6364-190kv motor
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html

single motor kit from DIY
(trucks, 83mm wheels, 36/16 gear ratio, 12mm belt, etc.)
diy-electric-skateboard-kits-parts/torqueboards-single-motor-mechanical-kit/

VESC
diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/

10S5P - Samsung 25r
https://www.imrbatteries.com/samsung-25r-18650-rechargeable-battery/

I haven't yet chosen a deck, remote, battery enclosure method yet but they aren't my main priorities at the moment.

The esk8 calculator expects a top speed of 25mph/40kmh with 85% efficiency (not sure if 85 is about right or not)
http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":190,"system-efficiency":85,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":83}|

Honestly, that top speed is probably more than adequate. I'm more concerned about hill climbing than top speed. Do you think that this build should be sufficient to get up large/decently steep hills? Also I've seen recommendations to use 15mm belts with single motor builds. Should I be concerned that the belt that comes with this kit is 12mm? I'm only about 130lbs/ 59kg, so I expect that will help.

Does anyone see anything overtly wrong/ any inconsistencies with this build? Otherwise, I'm excited to take the plunge.

Thanks! -Ben

edit: I already noticed that my original build plan (213kv) slightly exceeded the recommended ERPM. I edited this post to swap to a 190kv motor
190*42*7= 55860  - should work
http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#2 Posted by: torqueboards Posted at: 2017-06-21T03:08:32.350Z Reads: 246

```
You'll be fine if you climb steeper hills every now and then but if it's frequent dual drive is better since you have more traction, better braking, better torque.
```

---
## \#3 Posted by: Smorto Posted at: 2017-06-21T13:59:21.669Z Reads: 233

```
Many people have said that the 25r cells are bad in terms of voltage sag. They recommend going with Samsung 30q cells, you will have more range and enough amperage for your build with a 10s5p of Samsung 30q cells. You can also get them from https://ru.nkon.nl for much cheaper and they ship internationally.
```

---
## \#4 Posted by: BenL Posted at: 2017-06-23T02:57:49.543Z Reads: 211

```
@Smorto  Thanks for the advice and the link! I would have never guessed that the 25r cells would have worse voltage sag since the specs list them with a higher amp rating.   

I'm also considering going with the sp3 149kv and moving up to a 12s5 since the presumably lower amp draw should stress the battery/motor less on hills.
```

---
## \#5 Posted by: Smorto Posted at: 2017-06-24T13:25:51.476Z Reads: 202

```
Sounds good be sure to continue your build log once you start building.
```

---
## \#6 Posted by: BenL Posted at: 2017-07-07T23:25:56.824Z Reads: 195

```
I haven't yet received my batteries/ motor, but I did build my spot welder using a 1.5F capacitor. I primarily based it on @whitepony's design (thanks!) from here - https://endless-sphere.com/forums/viewtopic.php?f=35&t=70435&hilit=50km#p1062504

While the spring mechanism may look cool, I'm not sure that I would recommend my version of the design. I was having some pretty inconsistent test welds. I found that I was able to get the most consistent results if I kept my foot on the spring switch and completed the circuit by slowly touching the second electrode to the weld site. Whereas if I took the typical approach of first placing the electrodes before hitting the switch, the weld was typically very weak. I have my theory on why this is, but I don't want to write anything misleading. The .3125'' diameter copper rods that I used seem excessively thick, so I'm currently just using a couple of pieces of bus wire wire at the ends. I may try to file the rods to have thinner ends later.

  <img src="/uploads/db1493/original/3X/d/1/d185fc925956b1218115caa2a64c4ddbbbffdb50.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/0/2/02a884c9506fdf5d1e906cba5c401100038f3436.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/5/1/519679a3826e10a5f7c610ad2ba4fbb3108c5396.jpg" width="666" height="500">
```

---
## \#7 Posted by: whitepony Posted at: 2017-07-08T17:41:23.380Z Reads: 183

```
basically your cap is 75% of mine and not sure what voltage you zse for charging.

also, your switch is too far away - my switch is really close aur gap copper bars, so when my switch closes i got like 100mm^2 of copper contakt area!

<img src="/uploads/db1493/original/3X/c/9/c950d4d8925f7402d1e5ca8c191224df9c70de78.JPG" width="666" height="500">
```

---
## \#8 Posted by: PB1 Posted at: 2017-07-09T07:55:59.368Z Reads: 173

```
FYI I built a similar spot welder and used it to assemble a 10s 5p battery pack. Worked very well. 

Instead of the WP flat bar switch I used a starter relay off an old motorbike. The starter relay is operated by a micro switch. This gave me very consistent welds.
```

---
## \#9 Posted by: BenL Posted at: 2017-08-10T01:02:51.382Z Reads: 154

```
And it's all finished!

<img src="/uploads/db1493/original/3X/3/d/3d48fb3b4f0c96f15b9263a3fc9cecaf9e73e8e5.jpg" width="375" height="500">

Not really, but I became impatient waiting for the cells to arrive so I threw some lipos on there to give it a test run. I ended up going with the 149kv sk3, and even at the current 9S it feels pretty impressively fast to me.

Thanks @whitepony and @PB1 for the feedback! Yeah, I think the capacitor was simply too weak. I have since upgraded to a 3F cap, and I think that one will do the job. The relay idea is pretty cool! Maybe I'll give something like that a try if I still have inconsistent results. 

For the remote/receiver, I ended up choosing the Nyko Kama. However, the fact that it doesn't have a fail safe makes me really nervous. I did the test of pulling the batteries out with full throttle, and the motor just keeps spinning. Even if you set the VESC to send a brake signal on loss of signal, since the receiver apparently keeps sending the last signal that it received to the VESC. So I may looks into a different transmitter with a proper fail safe.

I'm planning to throw on a 12S5P configuration. If they don't all fit in a single row I may stack the last 2 of the 12 packs on top of eachother on the side opposite of the motor.
```

---
## \#10 Posted by: BenL Posted at: 2017-08-14T17:06:09.644Z Reads: 136

```
Cells finally arrived! Looks like I won't be having any space limitations.
<img src="/uploads/db1493/original/3X/5/a/5a9a105800a6d0f1976fe7dc34656c7793d07c53.jpg" width="375" height="500">

I'm having trouble finding a definitive answer. Will it be alright for me to use a 12S configuration with the @torqueboards VESC or would it be smarter to limit it to 10S to avoid frying the VESC  (149kv motor)?

diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
```

---
## \#11 Posted by: torqueboards Posted at: 2017-08-15T02:53:07.049Z Reads: 118

```
I only use 12S on my setups and I have no issue. Just stick to 190KV on 12S.
```

---
## \#12 Posted by: BenL Posted at: 2017-08-24T02:19:47.413Z Reads: 129

```
Today, I finished building the battery. With torqueboards' assurance, I went ahead with the 12S5. This build took a lot longer than expected.

I printed these spacers to separate packs to make myself a bit more comfortable that contiguous packs wouldn't end up shorting out. <img src="/uploads/db1493/original/3X/7/d/7de769bac3083eb11f61e896d4f152289fe90f18.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/2/1/21901f6fddb3135a11c1a055fc9a12bb3be21da7.jpg" width="375" height="500">

I hot-glued the batteries for some initial stability and hot-glued the spaces to the side of one pack.

I spot-welded the inner pack first, but it looks like I forgot to take any pictures of that side. 

On the outside portion, I used bus wire to carry the bulk of the current. I first soldered it the nickel strip before welding. I tried to keep it to the outer edge of the nickel strip so that I would still have enough space for the welds. 

<img src="/uploads/db1493/original/3X/0/2/022c1358117e40b71c16d58b8dc6403cd7010c8c.jpg" width="666" height="499">  <img src="/uploads/db1493/original/3X/d/b/db28c8f9556c2f89324f4e4ff2ce4879b8b153fb.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/b/a/baad6158e7c90be914b7e49d569309e69c78b480.jpg" width="666" height="499">

That's not the prettiest connection for the ground wire, but I don't think it should be a problem. You can't realIy see what's going on with all the solder on top, but the bus wire is bent at 180 degrees and the ground wire is wrapped around it.   

Below is after adding balance wires and folding the battery. I wasn't expecting such a large gap in the middle. Maybe it doesn't look very large in the image.

<img src="/uploads/db1493/original/3X/b/1/b144bd0d05f7e685a16e30e4805c46fb718f4761.jpg" width="666" height="500">

To finish it, I used shrink wrap. However, I don't think that I like how the pressure of the shrink wrap is making it bow in the middle. I may end up cutting it off. 

<img src="/uploads/db1493/original/3X/c/7/c7561e279f8b4bf93b51c367d18f34206b52d4da.jpg" width="375" height="500">
```

---
## \#13 Posted by: BenL Posted at: 2017-08-28T23:23:27.686Z Reads: 115

```
I 3d printed a temporary enclosure in PLA. I plan to re-print in ABS once I come up with a nicer design. 
  
<img src="/uploads/db1493/original/3X/9/f/9f4caee1756f3177fc9a20c5f3afc982ebd3fb23.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/5/a59ea2eddbe214db5c85e3f89520136451c191e5.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/4/e/4e6165730d180923e10d945c53a98a294214c117.jpg" width="375" height="500">

I did end up cutting the shrink wrap to relieve some pressure that was bowing the batteries. I think it ended up looking cooler this way.

<img src="/uploads/db1493/original/3X/7/d/7d49cfbbcb4b6e9bf5dd12ab45d01343de1f8c67.jpg" width="666" height="500">


Routing a path for the motor wires. I kind of made a mess with the wood glue and some liquid electrical tape.
<img src="/uploads/db1493/original/3X/d/1/d195080c5a229c9c1a1931ea737e4b0de9299476.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/b/5/b54ced6607fa06c15b98a8bab9991619c688a34b.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/c/a/ca000dc81102eefa2f70c7f97beba2622f4ccb77.jpg" width="375" height="500">
Pretty tight fit. I was getting worried the enclosure wasn't going to be big enough.
<img src="/uploads/db1493/original/3X/e/9/e930c6667e3f5a00909400bc7b3d8ce946b9bf7e.jpg" width="375" height="500">


What? Who put this there?
<img src="/uploads/db1493/original/3X/6/6/661e425e5fa0d39a4a77386431150762709597a7.jpg" width="666" height="500">
Yeah, I wasn't too concerned with aesthetics since I know I'm going to be replacing this enclosure
<img src="/uploads/db1493/original/3X/f/6/f6b77ab2db39dd4347de89f4e36f4e8c96757091.jpg" width="375" height="500">
I really like this voltage indicator though.
<img src="/uploads/db1493/original/3X/4/3/431efc1cde8be9d55a809f8f28452e815014e064.jpg" width="666" height="500">
Charging swiftly at 1.6A
<img src="/uploads/db1493/original/3X/8/6/864743e1f452484dacf41201a8b1498223be8c3d.jpg" width="375" height="500">
Went with clear grip tape
<img src="/uploads/db1493/original/3X/9/2/92f18857f5c821f4f78df19d3bc192cc11200afc.jpg" width="375" height="500">

I went for a couple short test rides today, and it feels great, but still definitely still needs some work. I'm having some issues keeping the motor mount tight, hopefully some more loctite will do the trick. Also, I discovered bullet connectors on the outside of the board to connect to the motors probably isn't a great idea. I was having some cutouts that I thought were from a loss of connection with the receiver, but it turned out one of the bullet connectors was just barely hanging on. I got thrown off the board a couple times, but fortunately that was at low speed and I landed on my feet. So I suppose I'll solder those into place. 

<img src="/uploads/db1493/original/3X/d/4/d471eec87e528bb6a3e537520f91841b332a5531.jpg" width="375" height="500">
```

---
## \#14 Posted by: torqueboards Posted at: 2017-08-29T02:28:07.716Z Reads: 96

```
Nice LHB inspired! :)
```

---
