# The Green Surfer &#124; eMountainBoard MBS Colt90 &#124; 10s Lipo &#124; dual VESC &#124; SK3 192Kv

### Replies: 18 Views: 1912

## \#1 Posted by: jazzcool Posted at: 2017-06-29T02:32:32.489Z Reads: 290

```
Finally I am posting my build thread for my colt90 MBS. I am using the following components:

**Electronics:**

* dual motors Turnigy Aerodrive SK3 - 6374-192kv
* 2 VESC from TorqueBoards connected with Canbus
* remote 2.4ghz HK-GT2B in its original casing
* set of 4 batteries, 5S 5000mah, connected in series and parallel so its 42v, 10ah
* antispark XT90 connectors. wires, bullet connectors, misc. 
* added 5v fan for the VESC colling
* added DROK style voltage meter 

**Board Hardware stuff**
* I am using MBS Colt90 it comes with ATS tracks. 
* I used [this 3Dprint](https://www.thingiverse.com/thing:2236882) to make motor mounts and sprockets adapters out of nylon, hope it's strong to survive the stress otherwise I would CNC in carbon fibre.
* The motors are mounted on 8mm screw rods and 5mm  "gaurds".
* it runs on 25H chains

here are some pictures of the build, it still needs some minor parts (slow orders from aliexpress) so haven't tested it yet. 


<img src="/uploads/db1493/original/3X/2/c/2c4b961a845ff9101c2be496003633a11163216d.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/0/1/010b4e74928540297d77a30aab00f154c2b42d5e.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/8/5/85cd9d131021d73e280e7374216fe25666922b59.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/d/9/d99bf1cb656a5e08ebea11f90d353b418e78a29c.jpg" width="277" height="500">
<img src="/uploads/db1493/original/3X/6/e/6e932bb3134a3f8ff5a85b97d12a54c6732b592f.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/f/2/f2a1190601f92223b449a7eb507944db3dbe9625.jpg" width="690" height="388">

more updates once I get to mount the 25H chains and finally can test ride it.

**edit**
I think we should have a separate E mountain board section for all those building this kind of application. Generally speaking it's hard to find through the various posts specific builds.
```

---
## \#2 Posted by: jazzcool Posted at: 2017-07-02T14:31:40.269Z Reads: 225

```
So I finally got it all built up and tested it. 
Man this is a beast! Had to play around with parameters on the VESC to tame this one. What I am still lacking is a way to lower the throttle response (or throttle curve). I rode it using 25% of throttle and this thing has power.. so I want to put a top limit that I can ride and not be knocked off to my ass and the throttle would gradually reach there. Would limiting the top motor max AMP fix that? 

<img src="/uploads/db1493/original/3X/d/3/d3fb6c52c0eabe241f326ae87b5e6e30f54fd029.jpg" width="690" height="388">
```

---
## \#3 Posted by: bullrider12 Posted at: 2017-07-25T14:26:47.626Z Reads: 205

```
That's a pretty nice build. I'm thinking about buying the same board and using the same motor mount as you do. Can you tell me something about this? Is it holding so far?
```

---
## \#4 Posted by: jazzcool Posted at: 2017-07-25T14:51:49.402Z Reads: 202

```
I am using it mostly on weekend rides (got a scooter for daily commute). So far so good. little maintenance really. Little vibration on the motors but it's all held tight and nice. 
I guess the first thing to go would be the nylon motor mounts. They are heavy duty but I would expect those to fail at some point.

BTW I added vinyl of carbon pattern so those boxes are better looking now. But I finally decided to get some cheap black boxes of Aliexpress. once those are in I would post images of latest iteration.
```

---
## \#5 Posted by: jazzcool Posted at: 2017-07-25T14:56:21.592Z Reads: 201

```
<img src="/uploads/db1493/original/3X/b/b/bb7da239ac144f6d48d372ee7dd0cfaa440c718d.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/7/3/73882dff959fee4600b681c3fe25b313b16d6c25.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/d/b/dbce9042f2b1ef4450d4169e121e9d7a207ec753.jpg" width="690" height="388">

As my friends saw me riding it on the grass while we were all racing our drones (yeah I do that too) they decided to call it the green surfer. I kinda like that name. Hence it shall be known as 
## "The Green Surfer"
```

---
## \#6 Posted by: bullrider12 Posted at: 2017-07-25T15:13:51.932Z Reads: 178

```
That's good to hear, what material are you using for the mounts right now? 
Another question: is there enough space between the wheels and the outer side of the mounts to put pulleys in? I see you are using chains and I want to know why :slight_smile:
```

---
## \#7 Posted by: jazzcool Posted at: 2017-07-25T15:22:53.782Z Reads: 172

```
as mentioned I printed it in nylon. It's quite strong. You can use a pulley but the design I had was made for chains. Chain is noisy while pulley generally smoother. However pulley system can slip (unless you use a wide belt). It seemed to me like chain is the way to go over belts. You need to make sure to have as many teeth in the chain/belt as possible to reduce chances of that happening. I got 6 on the motor sprocket.
```

---
## \#8 Posted by: bullrider12 Posted at: 2017-08-06T17:51:06.926Z Reads: 155

```
@jazzcool can you measure something for me? How much is the distance between the outer side of the motor plate and the inner side of the wheel rim? :slight_smile:
```

---
## \#9 Posted by: jazzcool Posted at: 2017-08-07T11:09:05.869Z Reads: 145

```
I'd say about 2.5 to 3 centimetres <img src="/uploads/db1493/original/3X/a/b/ab8d85e10393a1700e1a166dc03426fe945f3324.JPG" width="375" height="500">
```

---
## \#10 Posted by: bullrider12 Posted at: 2017-08-07T12:44:49.558Z Reads: 140

```
Nice, thank you :slight_smile:
```

---
## \#11 Posted by: jazzcool Posted at: 2017-08-09T11:57:25.969Z Reads: 131

```
Found really cheap 'mean' looking boxes so had to do an upgrade. 
Latest iteration here. 
Futur upgrade - adding Arduino connection to my mobile. 
<img src="/uploads/db1493/original/3X/e/c/ecc67169d1a5b7020e3bd11f829c0d5e57f2e7af.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/b/b/bb49f257492247ac698e314374249b550bbff6eb.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/a/2/a2c3b5604e7d54d2c1639cc429dfb19a6d319ffc.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/0/a/0af445258e4a8de2580cb4a3aa6aac2634ca736d.jpg" width="690" height="387">
```

---
## \#12 Posted by: jazzcool Posted at: 2017-09-02T00:45:20.030Z Reads: 120

```
Added Bluetooth to the mix with almamiac Android app. It's a bit prone to crash however you get all the telemetry data you need.
Here's a short video
https://youtu.be/BBzoDL6kP3s
```

---
## \#13 Posted by: jazzcool Posted at: 2017-09-02T00:52:06.454Z Reads: 119

```
And here's a ride I had last week. Lots of fun 😁
https://youtu.be/ftM45TGvjlk
```

---
## \#14 Posted by: Twinsen Posted at: 2017-09-20T09:34:07.554Z Reads: 109

```
How has it been holding up? Did the 3D printed parts break or did the threaded rods bend? Seems like a lot of torque being held by 2 tiny rods screwed in a bit of aluminium.

I plan on building an almost identical one since the design is so simple and cheap.
```

---
## \#15 Posted by: danieloath Posted at: 2017-09-20T09:50:44.420Z Reads: 104

```
Nice build. I, too, am wondering how the 3D printed components are holding up! I'm liking the idea of the foot straps. I plan to try for something similar with my upcoming build.
```

---
## \#16 Posted by: bullrider12 Posted at: 2017-09-20T10:10:49.954Z Reads: 101

```
I have pretty much the same build, but printed the components with petg. It's holding pretty good. Nothing bent or broke so far after some rough rides through the forest.  :slight_smile:
```

---
## \#17 Posted by: jazzcool Posted at: 2017-09-20T10:44:28.411Z Reads: 98

```
It's pretty awesome so far. No bents or nothing breaking. Nylon print holds up really good.
```

---
## \#18 Posted by: Twinsen Posted at: 2017-12-24T08:57:35.165Z Reads: 79

```
I made a similar one. I used smaller motors and some steel plates to reinforce the mounting I used.

<img src="/uploads/db1493/original/3X/c/5/c56406a9ac9b550012674ea86fd006d17967d576.jpg" width="690" height="388">
```

---
