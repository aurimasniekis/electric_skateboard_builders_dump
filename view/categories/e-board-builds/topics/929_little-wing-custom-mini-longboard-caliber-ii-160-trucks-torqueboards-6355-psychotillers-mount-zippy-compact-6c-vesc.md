# Little Wing &#124; Custom Mini Longboard &#124; Caliber II 160 Trucks &#124; Torqueboards 6355 &#124; Psychotiller&rsquo;s Mount &#124; Zippy Compact 6C &#124; VESC

### Replies: 20 Views: 3914

## \#1 Posted by: purplearms Posted at: 2016-01-06T04:44:44.800Z Reads: 261

```
Hi!

I'm new to the scene and stumbled onto this site. I don't know much about skateboarding either, although I can handle a board. There is so much info out there and i'm slowly feeling my way around. Thanks in advance for any guidance & advice!

**About Me:** Proud dad from Toronto who drives a desk from 9 to 5.
Typical jack of all but master of none. Some of my projects:
    [Arcade Coffee Table][1] | [DropCatch][2] | [Optimus Prime][3] [1][4] [2][5] [3][6]

**Goal / Usage**:  To scratch build an ultra portable electric penny longboard. Short range inner city commute to and from subway stations, max 5-6 miles per day, mostly flat. I'd never exceed 15-20 mph due to massive foot/car traffic so i can sacrifice top speed and big range if that saves me weight or space.

**Deck**: 23" custom plywood penny with carry handle cutout, recessed / embedded electronics. I will laser cut and laminate some plywood sheets to do it, steam bend a kick tail.

**Trucks/Mount**:  Maybe a Paris 180mm with 83mm wheels and welded motor mount. Mount for a 63mm motor with 32mm bolt spacing (is this standard?).

**Motor**: Single motor sensorless drivetrain, TBD.

**VESC**: I'd want something very compact that I can directly solder a wiichuck receiver to, and also stack my own custom anti spark pcb. Eliminate whatever wires I possibly can and shove it into a tiny box. VESC seems to fit that bill. Stretch goal to embed ws2812 LEDs into the deck. I hope Ben Vedder put that functionality in to the firmware? 2nd stretch goal is to embed the on/off switch on the inside of the deck carrying handle cutout.

**BATTERY**: 6s - looking into smaller alternatives



Any thoughts / advice?

  [1]: http://www.youtube.com/watch?v=ZpEC-LH5NFY
  [2]: http://www.instagram.com/p/sYeifSTCKx/
  [3]: http://www.instagram.com/p/w-nqGfTCDY/
  [4]: http://www.instagram.com/p/w-nqGfTCDY/
  [5]: https://www.instagram.com/p/w_tRKAzCD-/
  [6]: https://www.instagram.com/p/okPzMrzCJw/
```

---
## \#2 Posted by: chaka Posted at: 2016-01-06T05:23:52.793Z Reads: 243

```
[quote="purplearms, post:1, topic:929"]
Typical jack of all but master of none.
[/quote]

I believe the proper term is renaissance man!

 You will do fine on 6s for the commuting you described. 

70mm wheels might be a little on the small side. Generally 83mm is considered as low as one should go. 

I am a fairly seasoned rider so maybe I don't notice but I have never experienced  any pulling or turning during heavy acceleration.

Welcome to the community!
```

---
## \#3 Posted by: trbt555 Posted at: 2016-01-06T05:59:32.416Z Reads: 227

```
I'm gonna follow this thread with interest. I also had a small & light penny board on my mind as another build.
Looking forward to how you do with the deck.
I think the VESC is excellent, and there is a video somewhere of Vedder using WS2812 leds but I believe it will be a custom application, it certainly doesn't come ready to use.
Good luck !
```

---
## \#4 Posted by: lowGuido Posted at: 2016-01-06T06:18:31.103Z Reads: 234

```
[quote="purplearms, post:1, topic:929"]
Doesnt 1WD cause your board to pull to one side during acceleration/braking,
[/quote]

no it doesnt. that probably one of the most common myths of e-skate. 1WD is fine.
6S is also fine. My daily is a 1WD 6S build and its more than capable of going very fast, It struggles a little on big hills but my area is mostly flat, so I guess this depends where you are riding.
you may want to reconsider the R-spec for something with a bit more kv for 6S though. I Use a 280kv motor.

(not saying an R-spec wont work or isnt good, just will be slower on 6S)
```

---
## \#5 Posted by: onloop Posted at: 2016-01-06T06:44:44.911Z Reads: 233

```
I can confirm that single motor is really nice (didn't think I'd ever say that) I have been testing single drive, rear mount - heel side, much more lately since I have received the 6374 r-spec. 

The torque output from a single motor better matches that of the human riders movement expectations. Its way more forgiving in the acceleration department... some people really dislike the aggressive nature of a dual drive... if you accidentally move your fingertips 2mm too far you could end up on your arse with a single drive it's less touchy.

Definitely don't use 9mm belts though!. I've been stripping them frequently, mostly when braking aggressivly, which I assume you will doing when riding in a busy city.

This also depends on rider weight too. I'm 95kg so the belt has a big task on its hand when I ask it to stop the momentum. I suppose if you manage braking force with finger control and only slightly apply the brake you might be ok with 9mm... but sometimes you just want to stop NOW.

In any case I would avoid 9mm. 12mm is what I'm running now on all single drive builds.

Get the biggest motor you can afford. Sensors are not needed with the vesc.
```

---
## \#6 Posted by: Chris_KP Posted at: 2016-01-06T08:29:32.715Z Reads: 211

```
is it best to have your motor on toe or heal side @onloop?
```

---
## \#7 Posted by: lowGuido Posted at: 2016-01-06T08:45:46.294Z Reads: 214

```
if you ride regular, heel side.
if you ride goofy.. wait.. its still heel side LOL.. just on the other side of the board.

let me re phrase that. 

Yes heel side mount is best.

edit: also not saying that toe side wont work. (it will) its just that due to the the way you distribute weight when carving you will put more weight on your back heel when carving heel side. 

and yes you can lose drive when carving toe side, but due to the natural tendency to lean your weight a little more forward toeside during the carve its a little less dramatic than if you were carving heelside with a toeside mounted motor. make sense?
kinda the lesser of 2 evils.
```

---
## \#8 Posted by: purplearms Posted at: 2016-01-06T13:37:39.193Z Reads: 212

```
[quote="lowGuido, post:4, topic:929"]
you may want to reconsider the R-spec for something with a bit more kv for 6S though
[/quote]

[quote="onloop, post:5, topic:929"]
Get the biggest motor you can afford. Sensors are not needed with the vesc.
[/quote]

Hmm... I was considering a diyelectricskateboard pre-welded motor mount with their 6355 230KV motor... I am knowledgable with CAD, so I can just as well CNC my own bracket and weld it, but this time might be better put towards other aspects (I have a toddler so time is scarce lol).


[quote="lowGuido, post:7, topic:929"]
heel side mount is best.[/quote]
Awesome I was just wondering which side was best...

[quote="trbt555, post:3, topic:929"]
video somewhere of Vedder using WS2812 leds but I believe it will be a custom application
[/quote]
I see the latest is 4.9 revision of the board and 2.7 firmware. I also see his LED code in Github. I have some PCB design know how, so I'll have to get my hands dirty and make sense of it all. Since this still seems to be in beta, i might just have to leave the VESC programming until the end.

Does everyone here use an anti spark device? I'm fairly confident I can cook one up myself. I'm looking to see what [others have done][1].


  [1]: http://www.rcgroups.com/forums/showthread.php?t=983802
```

---
## \#9 Posted by: Kaly Posted at: 2016-01-06T18:01:51.666Z Reads: 206

```
Hello

This is the one of the best solutions around 

https://endless-sphere.com/forums/viewtopic.php?f=35&t=72687&hilit=Anti+spark+key+loop

I like that can be use as a sort of a key :-)
```

---
## \#10 Posted by: onloop Posted at: 2016-01-07T00:07:31.437Z Reads: 199

```
[quote="purplearms, post:8, topic:929"]
(I have a toddler so time is scarce lol)
[/quote]

i know how you feel brother!
```

---
## \#11 Posted by: purplearms Posted at: 2016-01-07T05:58:52.965Z Reads: 196

```
[quote="Kaly, post:9, topic:929"]
This is the one of the best solutions around
[/quote]
Thanks for that! Now i understand the anti spark. I thought of making my own remote toggled MOSFET, then did a search and found that Ben Vedder already [made this][1] haha. 

It will help eliminate any possibility of melted resistor (and connector) from mechanical factors. I think I will end up making my own flavor of this.. hmm..




  [1]: https://endless-sphere.com/forums/viewtopic.php?f=31&t=73800
```

---
## \#12 Posted by: purplearms Posted at: 2016-02-13T15:56:07.897Z Reads: 187

```
Just a quick update on my project. I nearly have my board outline finished and ready to send to the laser cutters. I've settled on 28" long and about 7.25" at the widest, with a built in carrying handle for subway commuting. Will have more pics when ready to assemble the board... 

I do have one question about gearing ratio i hope someone can answer.. I'm looking at a 3d printed hub for my flywheel clones but its 40t. I'm looking at a 16-40 gear ratio. If i apply bicycle logic to it, smaller chainrings at the crank gives me more torque, larger chainrings at the rear wheel gives me more torque. Does the same apply here? Larger motor pulley would be like larger chainring at the crank?

<img src="/uploads/db1493/original/2X/9/93ce43bd428ede4a891ec2e58a09bf6e986afff9.jpg" width="690" height="214">
```

---
## \#13 Posted by: lowGuido Posted at: 2016-02-13T17:05:40.005Z Reads: 184

```
[quote="purplearms, post:12, topic:929"]
I do have one question about gearing ratio i hope someone can answer.. I'm looking at a 3d printed hub for my flywheel clones but its 40t. I'm looking at a 16-40 gear ratio. If i apply bicycle logic to it, smaller chainrings at the crank gives me more torque, larger chainrings at the rear wheel gives me more torque. Does the same apply here? Larger motor pulley would be like larger chainring at the crank?
[/quote]

 true.


---------------
```

---
## \#14 Posted by: JT_Clemente Posted at: 2016-02-13T19:08:52.802Z Reads: 173

```
That's an awesome shape! Can't wait to see it!
```

---
## \#15 Posted by: lowGuido Posted at: 2016-02-13T19:15:13.658Z Reads: 178

```
here is a question for you.
why have you put the handle in the nose? wouldn't it be better in the side?
carrying it from the nose at that point wouldn't be too different from just carrying from the front truck.
```

---
## \#16 Posted by: purplearms Posted at: 2016-02-13T19:45:40.433Z Reads: 193

```
Oh i'm still debating the handle. Its purely for hanging up on the wall on a hook, and maybe a more ergonomic way to carry it around on public transport. If I held it by the handle and let my arm down, the board will have a few inches of clearance to the ground lol.. I truly do want to design it to be a public transport companion. I could integrate headlights there if i removed the handle though...

I'm splitting up my 6 cell lipo battery into three stacks of 2 cells, which will reduce the component height to 15mm. But since my board is quite small, it eats a bit of space on the "wings" and I can't put a handle in there. I'm thinking about how i would do the enclosure if i bent the wings upwards a little... Maybe i should do two stacks of 3 cells which will make the components ~22mm high

Mulling over the layout of the electronics right now. You'll see i'm planning some internally routed wires, red LEDs in the kicktail, some other color for the shoulders... any feedback? lol



Its all a work in progress...

<img src="/uploads/db1493/original/2X/6/6ba3a442ccc61063b7ea2429daa548d1438c2083.jpg" width="690" height="311">
<img src="/uploads/db1493/original/2X/e/e1376b100b7fff339d29e291d6d21dc6048ce17f.jpg" width="690" height="316">
<img src="/uploads/db1493/original/2X/3/32ee44cb64f4a392670e057ab45785fc690f1f3b.jpg" width="281" height="500">
```

---
## \#17 Posted by: purplearms Posted at: 2016-02-26T23:25:30.886Z Reads: 169

```
Plywood is back from the laser cutters!

<img src="/uploads/db1493/original/2X/b/b34db09d2cf24605350c1becf2a63f518af5e6f5.jpg" width="606" height="500">
```

---
## \#18 Posted by: torqueboards Posted at: 2016-02-26T23:36:12.901Z Reads: 167

```
sweet photos... boards look nice.. can't wait to see the final.
```

---
## \#19 Posted by: purplearms Posted at: 2016-04-28T04:51:05.024Z Reads: 151

```
Hey everyone. I've been away fighting pneumonia for the past few months, but i'm back on the mend and the project continues!

I found a local company ([Roarockit.ca](http://www.roarockit.ca/)) that sells diy thin air press skateboard kits. So i bought a vacuum bag to use with my custom laser cut wood. In the first pic I am preparing to carved the foam mold in order to create a slight gas pedal (the board is very narrow). I originally wanted a kick, but opted for longer wheelbase.

<img src="/uploads/db1493/original/2X/c/cc8d9ae12ce4bf967fb564c42700975e5dcf5111.jpg" width="690" height="388">




In the following pic, i've got the air pimped out of the bag, and using clamps to add extra pressure. As you can see the board is mounted the opposite way. That's because this is my second attempt. My first attempt resulted in [too much curvature](http://www.instagram.com/p/BDXJ_X1zCHn/) for such a narrow board.

<img src="/uploads/db1493/original/2X/9/9f5efcb5eefa8421430b5ef6045ebcae3e79d8ad.jpg" width="690" height="388">



And now the board is out of the mold, routed, sanded and ready for a few modifications. More good stuff to come :grin:

<img src="/uploads/db1493/original/2X/8/8a9bb75609522c57efb8e16ab691be9c8cac6337.jpg" width="500" height="500">
```

---
## \#20 Posted by: psychotiller Posted at: 2016-04-29T00:52:28.239Z Reads: 139

```
Welcome back from the dead!
```

---
