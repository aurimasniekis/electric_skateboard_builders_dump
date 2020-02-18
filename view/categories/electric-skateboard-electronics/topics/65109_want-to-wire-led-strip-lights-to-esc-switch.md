# Want to wire LED strip lights to ESC switch

### Replies: 35 Views: 1491

## \#1 Posted by: tkc Posted at: 2018-08-16T20:22:43.847Z Reads: 196

```
Hey there, Can someone photoshop some things on top of this image and tell me what does what? Specifically, I am trying to wire in some LED lights and a better voltage meter. I have a 50v to 5v buck which I had wired after the batteries which worked great, but obviously kept the LED's on all the time! I want to have the LED's come on only after pressing the power button (when the ESC is on). So I know I have to tap into something, just not sure what. I also want to put a voltage meter on top of the board so I need to know how what to tap into for that too. Obviously that ribbon but would like to know the wiring better.

I have a multimeter but not sure what to touch. I have red and black leads on the meter, but what do I ground the black to to test each wire!? Scared to touch anything! HELP!

![IMG_4022|374x500](upload://bP6v9JfduQYsJc95ZMLXOfnuBtO.jpg)

Update: I did test the red and black wires that go to the switch. It appears that when the switch is turned on, I can get voltage (maybe 2V) from those wires. But I need 5V, so what should I do? My guess would be a relay of some sort but I don't know what is small enough to fit into this box.
```

---
## \#2 Posted by: marsrover001 Posted at: 2018-08-16T20:55:26.698Z Reads: 173

```
I would just add a separate switch for LED's I ended up blowing my battery readout eswitch trying to run LED's on a similar ESC. It still worked, but I ended up wiring the battery readout and the led's to a second on/off switch.
```

---
## \#3 Posted by: tkc Posted at: 2018-08-16T20:58:00.092Z Reads: 169

```
That's certainly an option, but I've seen YouTube videos of this ESC and LED's working together nicely. So I just need to know how to wire it up. So I know it's possible.
```

---
## \#4 Posted by: b264 Posted at: 2018-08-16T21:29:24.986Z Reads: 161

```
Multimeter ground (black) goes on this black wire

![IMG_4022|374x500](upload://qeoBJb9ph5hZ8N5H7vMfqezAOTx.jpg)

Then move the red wire around
```

---
## \#5 Posted by: tkc Posted at: 2018-08-16T21:54:42.491Z Reads: 152

```
Cool, that's what I thought. That will help me with poking around! Trying to emulate what this guy did:

https://www.youtube.com/watch?v=XI3oI26uDC4
```

---
## \#6 Posted by: b264 Posted at: 2018-08-16T22:01:14.010Z Reads: 144

```
If reliability is a trait you like your boards to have, might I suggest using a separate battery for that stuff and make it independent of the drivetrain
```

---
## \#7 Posted by: tkc Posted at: 2018-08-16T22:14:03.922Z Reads: 147

```
Forgive me for asking, but wouldn't a relay sourcing power straight from the batteries and getting it's on/off source from the 2v out on the ESC work? therefore the power comes in at 36v and i use a buck to downgrade to 5v, that should work 100%. what is your concern about reliability?
```

---
## \#8 Posted by: b264 Posted at: 2018-08-16T22:40:39.394Z Reads: 136

```
The number one enemy of esk8 is vibration.  Heavy vibration can make stuff fail in ways you never imagined.  

You can envision taking the board after you are done with it, picking it up, and hitting it wheels-first as hard as you can against a concrete wall for 45 minutes.  Because in fact that is exactly what the board feels while you are riding it.
```

---
## \#9 Posted by: b264 Posted at: 2018-08-16T22:44:42.458Z Reads: 139

```
[quote="tkc, post:7, topic:65109, full:true"]
Forgive me for asking, but wouldn’t a relay sourcing power straight from the batteries and getting it’s on/off source from the 2v out on the ESC work? therefore the power comes in at 36v and i use a buck to downgrade to 5v, that should work 100%. what is your concern about reliability?
[/quote]

A relay will fail quickly and waste power while it's working correctly.  A [logic-level MOSFET](https://www.mouser.com/ProductDetail/771-BUK9Y12-100E115) would be a much better choice
```

---
## \#10 Posted by: tkc Posted at: 2018-08-16T22:50:06.080Z Reads: 129

```
Oh man. This is above my pay grade! I know about relays from dealing with 12v vehicles and stuff, it's pretty standard to use them. I don't know how to wire up this MOSFET you mention, leaving me basically at a stand still like when I created this post.
```

---
## \#11 Posted by: b264 Posted at: 2018-08-16T22:51:26.547Z Reads: 128

```
![N-channel-enhancement-type-MOSFET-setup|460x399](upload://xsr60KeZZAjc0PJ67pOwpRNUpyw.png)
```

---
## \#12 Posted by: tkc Posted at: 2018-08-16T22:53:34.760Z Reads: 115

```
Looks like a foreign language to me... No idea what I would need to purchase, where I would connect things, etc...
```

---
## \#13 Posted by: b264 Posted at: 2018-08-16T23:00:06.371Z Reads: 111

```
Ahh, nevermind that specific MOSFET turns on at 3V anyway.  My bad
```

---
## \#14 Posted by: Brdchris Posted at: 2018-08-16T23:23:40.963Z Reads: 113

```
Look up solid state automotive relay. I’m not sure how much voltage they handle but it would wire up like a relay and function like a relay but uses much less space, power, and are more reliable. I’ve used them on motorcycles before with good success
```

---
## \#15 Posted by: dareno Posted at: 2018-08-17T21:39:19.437Z Reads: 102

```
do you want the lights to come on when you switch on?
```

---
## \#16 Posted by: b264 Posted at: 2018-08-17T21:54:48.878Z Reads: 96

```
[quote="Brdchris, post:14, topic:65109"]
solid state automotive relay
[/quote]

Those won't be rated for 60V probably.  They will contain MOSFETs inside though, wired similarly
```

---
## \#17 Posted by: tkc Posted at: 2018-08-17T22:02:41.571Z Reads: 95

```
YES!!! I had it wired into the battery before but I hated turning the lights on/off. I want it to be like the video I linked to above.
```

---
## \#18 Posted by: dareno Posted at: 2018-08-17T22:18:05.743Z Reads: 94

```
I was thinking of doing this on my sons meepo and was going to try splicing into the led wiring to the switch. 
@b264 any reason why this wouldn't work?
I do have a vedder type switch which has all the wiring identified clearly so if I get time I'll wire up an old strip light to it and see later. The only problem with that esc I can see is identifying the wiring but a multi meter should tell you
```

---
## \#19 Posted by: b264 Posted at: 2018-08-17T23:01:33.026Z Reads: 93

```
You can engineer a solution that will work, sure :slight_smile:
```

---
## \#20 Posted by: dareno Posted at: 2018-08-17T23:06:00.032Z Reads: 94

```
Yeah I mean all you really need is a 5v output from the esc and that's what the led on the switch requires so should work in theory.  
@tkc check back with you in a few hours after i've been your guinea pig :grinning:
```

---
## \#21 Posted by: b264 Posted at: 2018-08-17T23:09:28.997Z Reads: 83

```
[quote="dareno, post:20, topic:65109"]
5v output from the esc
[/quote]

So now the ESC has another failure method that can streetface you
```

---
## \#22 Posted by: tkc Posted at: 2018-08-17T23:11:17.143Z Reads: 82

```
You get 2 volts from the switch (if you bother reading what I wrote above)
```

---
## \#23 Posted by: dareno Posted at: 2018-08-17T23:27:59.402Z Reads: 83

```
yeah mine is giving out 3v according to the meter but its a separate switch so that won't work at all lol   Never mind it was worth a try and there is absolutely no need to get all snippy because I'm only trying to help.:stuck_out_tongue_winking_eye:
```

---
## \#24 Posted by: tkc Posted at: 2018-08-17T23:51:49.799Z Reads: 79

```
All good. Just trying to get to the end result. I know it’s possible to accomplish (that video is proof) so we’ll make it happen.
```

---
## \#25 Posted by: dareno Posted at: 2018-08-18T00:24:32.894Z Reads: 73

```
There is one other way you could do it.  You have a buck converter right?  So get an anti spark switch like a vedder or similar and wire that in between your battery and esc.  Leave the existing switch on  and tucked in the enclosure and use the new switch as your power on that way you can wire the buck converter after the new switch and control everything from there.
Or you could just have both switches on the enclosure as it won't matter because the meepo switch is auto on anyway.  All you're doing is creating a master switch with an anti spark which will keep @b264 happy because hes a safety kind of guy
```

---
## \#26 Posted by: TowerCrisis Posted at: 2018-08-18T03:18:08.120Z Reads: 76

```
I would not hook up anything to the switch power. For all we know it could be ONLY a logic level switch intended for very low current. You could seriously mess things up while it's connected, or permanently if you fry something.

EDIT: the fact that it is 2V makes me think it's logic more so, most of our diy switches are full votage if I remember correctly.
```

---
## \#27 Posted by: tkc Posted at: 2018-08-20T06:12:46.208Z Reads: 68

```
I bought this switch so I could put the buck after the switch and have it turn on the Meepo ESC too (I guess I’ll short the wires the old switch flipped on).

https://www.amazon.com/dp/B07CMYPZ6Z/ref=cm_sw_r_cp_api_sTLEBb980GHC4

This won’t give me auto-on ESC but at least the buck won’t be running the entire time and the lights turn on when the board does.
```

---
## \#28 Posted by: dareno Posted at: 2018-08-21T09:44:59.792Z Reads: 60

```
Don't short the wires.   Mine is running fine with both switches right now and so will yours.  One is just acting as a battery Isolator.  The esc switch will automatically turn off and on as normal but only turn on after you have switched on the main and then when you roll it the esc will power up.  This is how I have mine running after our first conversation and it works.  The only down side I can see is when the auto stops working (and they do fail) so keep the original switch on the enclosure so you can manually use it.
Also you have another thread asking the same questions so be patient and let people help in their own time.
```

---
## \#29 Posted by: tkc Posted at: 2018-08-21T13:15:05.135Z Reads: 60

```
Actually one question was how to wire LED lights to my skateboard which I was able to do using a buck. They just didn’t turn on/off. The other question was how to do it when the ESC turns on and off. So two different questions with two different answers. One I was successful doing and the other I’m still on path to accomplish.

Why are you saying not to short the wires? I put a jumper on that switch and it seemed to work great turning the ESC on/off from another power source. Are you saying it’ll randomly shut off maybe?
```

---
## \#30 Posted by: tkc Posted at: 2018-08-26T01:06:30.247Z Reads: 55

```
Ok! I was finally successful in wiring everything together. So the Meepo switch is different than a normal switch, it turns the ESC on by shorting two contacts. So I put a jumper in there and wired in another switch. That way, I could be sure what was on the outgoing side of the switch had 40v ONLY when turned on. I used my 50v to 5v beck to wire up the lights. So now, everything works great. Was going to upload a video but I can't, oh well!
```

---
## \#31 Posted by: andyspeed Posted at: 2019-04-18T20:59:26.882Z Reads: 40

```
Great so you ended up connecting everything and now you wont share more in depth of how you did it or how it looks? You couldn't upload a video?? You seemed to upload a video just fine when you needed help though.... I had an easier solution the entire time that i've been using on my board for over a year now that turns on and off with my cell phone if want to use that feature. BUT after hearing the way you talk disrespectful to others who are taking the time out of their day to try to HELP you, the last thing I want to do is HELP YOU. Oh well! Good luck with that janky setup you got going on though rookie! lolol
```

---
## \#32 Posted by: Kingdom421 Posted at: 2019-04-18T21:08:45.392Z Reads: 38

```
Use as many separate systems and batteries for each thing in the board as you want.... Great!!! So how about a multi channel compact remote to turn each on individually.
```

---
## \#33 Posted by: drone001 Posted at: 2019-04-23T17:59:25.412Z Reads: 29

```
any pics as to how you wire a buck converter to your battery? how can something that small not burn up when you connect it to such a large battery.
```

---
## \#34 Posted by: tkc Posted at: 2019-04-23T18:10:27.376Z Reads: 25

```
Put an anti-spark switch between battery and buck
```

---
## \#35 Posted by: drone001 Posted at: 2019-04-23T20:15:54.046Z Reads: 21

```
thx.....where can i find info on how to wire a buck inside an electric skateboard. want to use it to power lights and possibly an Arduino
```

---
