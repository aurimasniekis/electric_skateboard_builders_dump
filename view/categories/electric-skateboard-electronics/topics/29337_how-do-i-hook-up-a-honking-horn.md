# How do I hook up a honking horn?

### Replies: 63 Views: 3586

## \#1 Posted by: Sebike Posted at: 2017-08-01T21:10:02.957Z Reads: 356

```
Hi Community!

Can't find any info on how to control a horn from any of the free channels on the GT2B (although I see people mentioning they have added remote controlled horns to their boards). I'm in need of a total noob walk-through if anyone want to share. Parts needed, wiring/diagram and what-not..

I saw a great diagram from @mmaner for controlling lights on/off, but a guess a horn would need a temporary or timed switch maybe, unless you want to run with a constant hooooooonk.

All your thoughts, diagrams, theres-already-a-topic-explaining-this-links are much appreciated.

As mentioned I have the GT2B remote with receiver which will be hooked up to a VESC-X.
```

---
## \#3 Posted by: Jedi Posted at: 2017-08-02T01:03:52.201Z Reads: 334

```
<img src="/uploads/db1493/original/3X/2/6/26abf1ea05def2248688d653c85630cfbe8e18a7.JPG" width="468" height="311">
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-08-02T01:38:14.304Z Reads: 324

```
Unfortunately, most horns that would be loud enough to be heard will all be 12v and quite large.
```

---
## \#5 Posted by: smurf Posted at: 2017-08-02T02:13:11.896Z Reads: 323

```
https://www.instagram.com/p/BNAUg7TjQFX/

36V
```

---
## \#6 Posted by: Nate Posted at: 2017-08-02T02:37:41.443Z Reads: 314

```
@Mikeomania12 has an wireless honking honk. That thing is annoying as fuk but it works!
```

---
## \#7 Posted by: Mikeomania12 Posted at: 2017-08-02T02:39:26.055Z Reads: 313

```
http://www.electric-skateboard.builders/t/unconsiderated-cyclists/6913/21?u=mikeomania12
```

---
## \#8 Posted by: MrHappy Posted at: 2017-08-02T02:42:38.483Z Reads: 315

```
Too much?
https://www.amazon.com/Volt-Electric-Train-Grade-Chrome/dp/B002ITX2RE
```

---
## \#9 Posted by: trancejunkiexxl Posted at: 2017-08-02T07:48:37.546Z Reads: 293

```
 I want to hear it now =)
```

---
## \#10 Posted by: goldenHusky Posted at: 2017-08-02T09:47:39.987Z Reads: 287

```
Something like this? :joy:

[https://www.youtube.com/watch?v=5C2Z7f1e-7Q](https://www.youtube.com/watch?v=5C2Z7f1e-7Q)
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2017-08-02T11:18:38.202Z Reads: 288

```
What's wrong with the old fashioned way? 


https://youtu.be/njIJby7AI8s
```

---
## \#12 Posted by: Sebike Posted at: 2017-08-02T11:49:03.811Z Reads: 276

```
Actually traffic regulations here requires the board to have a bell/horn. If that wasn't the case, old school is the way to go always :smile:
I like the simplicity of the finger bell though. Simpler is better!
```

---
## \#13 Posted by: Sebike Posted at: 2017-08-02T11:56:25.418Z Reads: 265

```
Almost what I had in mind lol. Rather have a ferry horn though
```

---
## \#14 Posted by: themegak Posted at: 2017-08-02T15:03:29.249Z Reads: 248

```
I need this.  Do you know where i can get ?
```

---
## \#15 Posted by: Sebike Posted at: 2017-08-02T15:08:37.459Z Reads: 240

```
@themegak  You'll find those on ebay. Search for bike bell finger ring
```

---
## \#16 Posted by: olgamedt Posted at: 2017-08-02T15:18:27.238Z Reads: 239

```
Hilarious :joy:
```

---
## \#17 Posted by: Jedi Posted at: 2017-08-03T00:35:26.997Z Reads: 231

```
https://run-bell.com
```

---
## \#18 Posted by: lrdesigns Posted at: 2017-08-03T03:38:46.027Z Reads: 233

```
Get one of these receiver controlled switches, then the button on the grip of the GT2B can switch something on and off. 

https://hobbyking.com/en_us/turnigy-receiver-controlled-switch-1.html

Now to figure out what to do about the horn. Easiest may be a 5v buzzer with voltage tapped off the receiver. The sound will be annoying as fuck and maybe not very loud. 

If you want to use a real motorcycle type horn at 12v you will need a DC/DC step down converter to get a 12v line from your battery.  Something like this. 
http://www.ebay.com/itm/LM2596HV-DC-DC-5-60V-Adjustable-Step-Down-Power-Module-/162083468223?hash=item25bced73bf:g:oe4AAOSwa81XRtH6

12v motor cycle horn. 
http://www.ebay.com/itm/BIKINGEAR-UNIVERSAL-MOTORCYCLE-SCOOTER-12v-1-5A-E-MARKED-HORN-70mm-DIAMETER-95DB-/311582806683?epid=1689158345&hash=item488bc8529b:g:1UoAAOSwR5dXRud1&vxp=mtr
```

---
## \#19 Posted by: deucesdown Posted at: 2017-10-31T14:06:34.249Z Reads: 211

```
necropost! I had most of the parts lying around, was gonna do lights.

[dropbox video](https://www.dropbox.com/s/iuyfz69bagits3z/Rc%20horn%20test.mp4?dl=0)

The horn is 12v 1.5A, the green thing is a dual bec, has a 5v and 12v output.

I also bought a 36v horn, and I have some of those cheap buck converters. I figured a smaller voltage drop would be less stress on the converter. Will have to see.

The Turnigy RC switch doesn't seem to have latching behavior, so not good for lights using the steering thing, but good for the horn.

For those not familiar, on the mini remote the trigger goes to CH2 on the receiver, the wheel on the side goes to CH1. In the video, the RC switch thing hooks up to CH1, and switches the 12v line. Need 5v for the receiver (usually from vesc), and 12v 1.5a for the horn.

Gotta mount it up now.
```

---
## \#20 Posted by: Mikeomania12 Posted at: 2017-11-01T19:41:37.824Z Reads: 200

```
I made this wireless air horn that I keep on the outside pocket of knapsack. 
I also use a separate remote to toggle it because at the time i was using a remote with only 1 channel. I just got the 'winning' remote so need to try that second channel now.
The horn is a little too big to mount on the bottom of my board. But its louder than most cars :wink:

https://www.youtube.com/watch?v=kU8rYpDdqXk12
```

---
## \#21 Posted by: danielz Posted at: 2017-11-01T20:19:32.328Z Reads: 197

```
Ive decided to go with a bicycle hand bell. A horn from a vehicle is just too loud and harsh and not at all polite. 99% of the time its pedestrians on cycle-ways and pavements i need to warn. 

If i were using it solely on the road though, then id consider a regular horn.
```

---
## \#22 Posted by: Acido Posted at: 2017-11-01T21:04:49.347Z Reads: 184

```
Why you all so fancy
Just scream beeeeeep as loud as you can and people will react 10times better and faster tested by me almost everyday on my bike
```

---
## \#23 Posted by: b264 Posted at: 2017-11-02T00:18:00.690Z Reads: 177

```
I need a horn that plays the sound of quickly-approaching truck tires with V8 motor noise.  
  
Because nothing else gets people's attention without being rude.
```

---
## \#24 Posted by: Michaelinvegas Posted at: 2017-11-02T03:04:13.664Z Reads: 174

```
https://youtu.be/Khk3_VT2q9g

https://youtu.be/BlrMcENTGY4

https://youtu.be/IhWPf4B1rNc
```

---
## \#25 Posted by: MrHappy Posted at: 2017-11-02T05:48:02.596Z Reads: 160

```
Oh my god, that 3rd video has got to be the worst sound I have heard in a long time. It's not even loud, it's just irritatingly bland.
```

---
## \#26 Posted by: danielz Posted at: 2017-11-02T17:04:03.554Z Reads: 160

```
might try a door bell, lol
```

---
## \#27 Posted by: longhairedboy Posted at: 2017-11-02T17:24:54.612Z Reads: 154

```
i'm watching this thread with interest. I would like some kind of "HEY I'M COMING UP ON YA" sound too, but after a lot of jokes about train and truck horns we're looking for something more car like. But not exactly like a car, there's rules about horns you have to recognize what they are. I don't want to be mistaken for a car. or a train. but something in that vein of sound.
```

---
## \#28 Posted by: mmaner Posted at: 2017-11-02T17:27:41.502Z Reads: 151

```
I cant think of any reason why you couldn't use a turnigy switch connected to an available channel in conjunction with a 12v step down convertor and a really small car horn.  Seems pretty simple, but yeah, being mistaken for a car could be dangerous.
```

---
## \#29 Posted by: longhairedboy Posted at: 2017-11-02T17:30:46.100Z Reads: 152

```
that should work fine an a gt2b style or other remote with a 2nd channel. gt2b has the 3rd channel with the button, perfect.
```

---
## \#30 Posted by: mmaner Posted at: 2017-11-02T17:31:39.187Z Reads: 152

```
yep, or the nano-x or maybe even the remote that @Wajdi is working on if you sub the lights out.
```

---
## \#31 Posted by: Guacamoleface Posted at: 2017-11-02T17:32:51.648Z Reads: 148

```
I mounted one of thoose clown horns on the front of my board. Just put a foot on it and everyone within 50feet will most likely shit themself, including me. Horrendes sound..
```

---
## \#32 Posted by: b264 Posted at: 2017-11-02T17:56:59.093Z Reads: 151

```
[quote="Guacamoleface, post:31, topic:29337"]
I mounted one of thoose clown horns on the front of my board.
[/quote]

Without photos, it didn't happen :stuck_out_tongue:
```

---
## \#33 Posted by: Guacamoleface Posted at: 2017-11-02T18:17:34.736Z Reads: 146

```
Haha video would been even better ;)
```

---
## \#34 Posted by: ninja Posted at: 2017-11-02T18:45:55.379Z Reads: 144

```
Just don't ride in foc. 😃
Use bldc mode. O.k. i have done only 400 km so far. But never had a jell or horn. People just hear my motor sound and always looking back. Of course in bussy and loud environment better horn.
```

---
## \#35 Posted by: Guacamoleface Posted at: 2017-11-02T18:49:02.472Z Reads: 137

```
A bluetooth speaker + phone application with chewbacca sounds works pretty decent att grabbing peoples attention aswell ;)
```

---
## \#36 Posted by: Mikenopolis Posted at: 2017-11-02T19:59:46.557Z Reads: 134

```
[quote="ninja, post:34, topic:29337"]
Just don't ride in foc. :smiley:
Use bldc mode
[/quote]

exactly what I was thinking. FOC is eerie quiet. I went back the BLDC and actually LIKE to have some noise
```

---
## \#37 Posted by: b264 Posted at: 2017-11-03T03:21:53.041Z Reads: 137

```
I found one.  Pop one of these on there with an air compressor and it definitely won't be too big or heavy, and won't make pedestrians mad or cause your way of life to be outlawed.  Definitely in my next build.
  You can just put a valve with a string and just pull on it with your front hand, no need for even a remote.


Nathan K5LA locomotive whistle
https://www.airhornsoftexas.com/collections/train-air-horns/products/nathan-k5la
```

---
## \#38 Posted by: jess.t.moody Posted at: 2017-11-03T03:51:18.831Z Reads: 128

```
You could you use a small PVC air chamber with pressure pump. :smile:
```

---
## \#39 Posted by: b264 Posted at: 2017-11-03T04:09:53.226Z Reads: 128

```
[quote="jess.t.moody, post:38, topic:29337"]
use a small PVC air chamber
[/quote]

I think that runs on 200psi, not sure pvc is up to the task.  You could put an industrial compressor in a trailer though
```

---
## \#40 Posted by: deucesdown Posted at: 2017-11-04T02:45:03.139Z Reads: 123

```
I like the car horn because people know when they hear it they need to move ass or die. Bicycle bells are also good. My scariest moments are from people crossing the road against the light without looking. One lady started crossing with her head down -- I planned a course way in front of her, but without looking up she started running! My one crash was from one of these incidents...

30mph I need something loud that people recognize, I don't have time to fuck around.

[quote="Guacamoleface, post:31, topic:29337"]
clown horns
[/quote]

Fun but I'm close to panic if/when I need the horn, can't be moving my feet around during full power braking lol.
```

---
## \#41 Posted by: Guacamoleface Posted at: 2017-11-04T09:00:57.926Z Reads: 114

```
I feel like Ima need something thats strong enough to shake the ground around me :joy: 
The problem when everyone has noise cancelling headphones is having something strong enough not to be cancelled out by them..
```

---
## \#42 Posted by: MrHappy Posted at: 2017-11-04T19:36:23.520Z Reads: 103

```
you just need pressure rated pvc, you can find some thats 600 psi.
```

---
## \#43 Posted by: deucesdown Posted at: 2017-11-05T03:10:06.833Z Reads: 113

```
EDIT malfunction was due to intermittent mini deans -- swapped out for XT30, all good now.

Got it wired into the board now. A photo and a breakdown for others looking to do something similar.

Couldn't find a proper place for the horn itself (yet), so for now lol it's hanging off the front like a black round unicorn horn. The mounting tab on the horn is some soft metal, it's not gonna survive too long.

https://www.dropbox.com/s/wh54ypo02jgvoqv/ppm%20horn%20wiring.jpg?dl=0

I had crimp contacts that fit the horn tabs. The green thing is being used as a 12v BEC, XT60 taking power from the battery pack at 10s voltage. The green thing also has a 5v output that is unused here.

The little black connectors are mini deans.

The receiver, vesc connects to channel 2, the turnigy switch to channel 1. This switch acts as a momentary when I turn the wheel on the remote to the left.

I'm probably gonna cover the horn in heat shrink to protect from mud and maybe knock it down a few db. And I gotta find a better place to mount it up.

I'll probably heatshrink all the little electrical pieces together so they're in a neat bundle.

BTW this thing is a pain to test, annoys the whole neighborhood. :slight_smile:
```

---
## \#44 Posted by: saul Posted at: 2017-11-05T05:39:34.747Z Reads: 107

```
mm i'm pretty sure i can mod my led circuit to use a horn/speaker.

but honestly I don't why you wouldn't put it on the remote instead of the board?
it simplifies so much!



edit: If this post gets more than a few likes I'll make it ;)
----------
```

---
## \#45 Posted by: b264 Posted at: 2017-11-05T05:44:50.179Z Reads: 105

```
[quote="saul, post:44, topic:29337"]
but honestly I don't why you wouldn't put it on the remote instead of the board?
[/quote]

I agree with wanting a bell or horn like the metroboards have but I also agree it's much simpler to put it on the remote.  And while we are talking remote -- remotes need to run on an 18650 cell already, not sure why none do
```

---
## \#47 Posted by: saul Posted at: 2017-11-05T05:51:13.696Z Reads: 102

```
[quote="WrinklyWink, post:46, topic:29337"]
Having the horn activated by the finger is faster and safer.
[/quote]

I think you missunderstood me. it would still be hand activated, and much more reliable if it was in the remote.

[quote="b264, post:45, topic:29337"]
remotes need to run on an 18650 cell already, not sure why none do
[/quote]

a couple of my custom remotes did, but they get bulky and unless you have high power leds in the remote, charging becomes so rare its actually less convenient because you go months without need to plug in....then forget, then dead on a ride :(
```

---
## \#48 Posted by: b264 Posted at: 2017-11-05T05:52:35.805Z Reads: 101

```
[quote="saul, post:47, topic:29337"]
charging becomes so rare its actually less convenient because you go months without need to plug in....then forget, then dead on a ride
[/quote]

Oh, great point.  I'm converted
```

---
## \#49 Posted by: saul Posted at: 2017-11-05T06:00:49.272Z Reads: 101

```
well i guess i have another project to try..
need some audio samples...

https://youtu.be/zstkw6AEVAE?t=12m30s
```

---
## \#50 Posted by: Idle Posted at: 2017-11-05T06:03:18.280Z Reads: 98

```
Nice job!
Just make sure to loctite the nut on the mounting post. 
Maybe fashion a second tab to affix it to the other truck mounting screw.
```

---
## \#51 Posted by: b264 Posted at: 2017-11-05T06:08:47.502Z Reads: 99

```
[quote="saul, post:49, topic:29337"]
need some audio samples
[/quote]

The first 3 seconds and the last 4 seconds of [this clip](http://www.bbc.com/future/story/20170714-the-brain-hacking-sound-thats-impossible-to-ignore) spliced together is my recommendation.
```

---
## \#52 Posted by: smurf Posted at: 2017-11-05T06:11:19.265Z Reads: 101

```
I would like to have the roadrunner beep if given a choice.

https://i.pinimg.com/736x/6e/5f/60/6e5f6098340c7991b7357ea94ab686e6.jpg
```

---
## \#53 Posted by: b264 Posted at: 2017-11-05T06:12:34.100Z Reads: 100

```
[quote="smurf, post:52, topic:29337"]
roadrunner beep
[/quote]

second this
```

---
## \#54 Posted by: saul Posted at: 2017-11-05T23:37:31.268Z Reads: 97

```
[quote="b264, post:53, topic:29337"]
roadrunner beep

second this
[/quote]

oh yes!!!

https://youtu.be/Jd_41tM6H2Y?t=30s
```

---
## \#55 Posted by: saul Posted at: 2017-11-05T23:38:39.155Z Reads: 96

```
and this for option 2
https://youtu.be/DDZBzvTDhGU?t=7s
```

---
## \#56 Posted by: b264 Posted at: 2017-11-05T23:55:28.877Z Reads: 94

```
[quote="saul, post:54, topic:29337"]
oh yes!!!
[/quote]



Specifically, the one at 742 seconds `https://www.youtube.com/watch?v=Jd_41tM6H2Y&t=742s`
```

---
## \#57 Posted by: deucesdown Posted at: 2017-11-09T16:12:19.749Z Reads: 91

```
Update. The metal bracket broke off in about 4 days. I've got it gaffer taped to the board for now, but as expected the output is greatly attenuated. Will play with various mounting schemes and report back if I find something usable.
```

---
## \#58 Posted by: Loki Posted at: 2017-11-09T17:43:23.594Z Reads: 86

```
Haha!! Is it bad I like this??
```

---
## \#59 Posted by: deucesdown Posted at: 2017-11-10T04:50:14.897Z Reads: 89

```
So this morning some guy walked into the crosswalk against the light without looking. I had room but thought I'd test the horn. This is with all the tape so it's pretty quiet. Beep, and the guy looks up, gets a really pissed expression on his face and starts cursing at me. Hmmm, not the reaction I was expecting...

I cut some of the tape off, the decibels are up near usable levels now. I'll see how long the gaffer's tape lasts...
```

---
## \#60 Posted by: krloz Posted at: 2017-11-16T08:54:13.697Z Reads: 87

```
BIKIGHT Bicycle Electric Horn USB Charge Loud horn 110-120db 22.2-31.8 Bars IP65 Waterproof Safety Cycling Bells 40g
https://banggood.app.link/At7V9gMg7H
```

---
## \#61 Posted by: longhairedboy Posted at: 2017-11-16T13:09:57.237Z Reads: 87

```
[quote="b264, post:45, topic:29337"]
remotes need to run on an 18650 cell already, not sure why none do
[/quote]

The new maytech remotes don't have room for it. Iopened one up last night hoping for the same thing. There is room for a larger pouch though.
```

---
## \#62 Posted by: deucesdown Posted at: 2017-11-17T03:55:55.425Z Reads: 85

```
I'm probably ordering this and attaching to remote.

The car horn with gaffer tape is holding up lol. Was very helpful today. This time an Asian lady suddenly starts running across the road without looking. BEEP! She took a full second to react, but fast enough to save our asses.

I've had this happen to me a few times, I don't understand this behavior. It's very scary because if they look up and see me they'll stop or slow down, so I have to find room to go in front of them or waaay behind them.

I'm gonna see if the tape holds on until the 3d printer comes in...
```

---
## \#63 Posted by: krloz Posted at: 2017-11-17T09:17:38.279Z Reads: 81

```
If you buy it comment how the switch is connected to the board and if it can be swapped for something remote
```

---
## \#64 Posted by: krloz Posted at: 2017-12-10T12:57:26.827Z Reads: 72

```
ROCKBROS Cycling Alarm Bells 90 dB Electric Horn Waterproof Bicycle Handlebars Silica Gel Bike Bells
https://banggood.app.link/Fs38tgSnLI
```

---
## \#65 Posted by: Spacecase418 Posted at: 2019-07-01T14:15:44.546Z Reads: 20

```
It’s been two years since this post started. How’s the motorcycle horn holding up?
```

---
