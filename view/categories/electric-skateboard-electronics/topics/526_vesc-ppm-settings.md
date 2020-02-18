# VESC PPM settings

### Replies: 42 Views: 9933

## \#1 Posted by: cmatson Posted at: 2015-11-21T19:58:22.483Z Reads: 705

```
So I successfully set up my vesc from @chaka today, and am happy to report I didn't screw anything up! (shrink wrap and pre soldered wires make such a difference, lol)

**The one thing I just couldn't get to work right was the end points of the PPM input** 

I've set it up, and it's working, but I get max speed when I am only pulling the trigger 1/3 of the way.

**What's been done:**
-the PPM display graph has been used to tweak the end point values, and now neutral is perfectly in the middle.
-Going "full reverse" on the remote lines up right at the end of the graph, while going "full forward" also lines up with the opposite end of the graph. 
-neutral range is set to .15 (stock)

but for some reason, once I reach about 1/3 of the way to the end of the PPM display graph, the motor maxes out and the last 2/3 of trigger pull do nothing. I'm sure there is some way to either change the throttle curve or something, I just don't know how to do it and haven't found a way to do it... 

I did watch a couple videos on it, including the one in the vesc brake faq, but didn't have any luck.

Haha it's totally ridable, just deathly sensitive :laughing:
```

---
## \#2 Posted by: jakeyb2525 Posted at: 2015-11-21T20:07:46.356Z Reads: 668

```
Have you tried it when your on the board ?

are you in current no reverse brake? with no load mine did the same

I also asked the same kind of question on ES, my start up acceleration felt a bit slow
```

---
## \#3 Posted by: cmatson Posted at: 2015-11-21T20:25:07.773Z Reads: 630

```
I tried it on the board, but didn't go anywhere near top speed- everything is just ghetto mounted right now for testing. Your point does make sense though; and yes, I am in current with no reverse.

I'll keep that in mind, and try it again with my weight on the board once everything isn't ghetto mounted, Thanks
```

---
## \#4 Posted by: cmatson Posted at: 2015-11-21T22:25:30.469Z Reads: 601

```
I just tested it's real life performance again (but faster this time..) and it seems to still accelerate up to top speed insanely quickly. Before half throttle, I'm already going my max speed... Haha, I was kinda hoping it would be as simple as a performance change once I stood on it, but it doesn't look like that's the answer!
```

---
## \#5 Posted by: chaka Posted at: 2015-11-21T22:27:14.609Z Reads: 559

```
PPM settings can be a little counter intuitive at first. If you are still having trouble dialling it in send me an email and we can do a skype session and get it sorted out.
```

---
## \#6 Posted by: onloop Posted at: 2015-11-21T22:37:33.357Z Reads: 560

```
I don't recall changing any settings like that, is there a reason you are changing the settings?

I just plugged the gt-2b RX in and it was good to go.
```

---
## \#7 Posted by: chaka Posted at: 2015-11-21T23:33:04.067Z Reads: 554

```
Sounds like you need to increase your maximum pulsewidth, You will probably need to decrease your minimum pulsewidth to keep dead stick at 50%

<img src="/uploads/db1493/original/2X/7/7259c00ba07e36e731760f5d7a4336be54b0a87b.png" width="666" height="500">
```

---
## \#8 Posted by: chaka Posted at: 2015-11-22T00:31:23.400Z Reads: 511

```
A simple way to find your min and max values is by monitoring the pulsewidth values in the lower right hand side of the screen while fully depressing the throttle and brake. Those values will give you a good starting point. You will still need to adjust them slightly to find the sweet spot.
```

---
## \#9 Posted by: onloop Posted at: 2015-11-22T01:17:43.433Z Reads: 499

```
check this out:

http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244
```

---
## \#10 Posted by: cmatson Posted at: 2015-11-22T05:30:50.098Z Reads: 473

```
Thanks for the help everyone!

I'll work on it tomorrow, and try to figure it out. Now that I think about it, widening the minimum and maximum endpoints should do the trick, but I'll have to wait and see when I actually test it. 

If I can't seem to get it tomorrow, I might take you up on that offer @chaka

Thanks again!
```

---
## \#11 Posted by: cmatson Posted at: 2015-11-22T23:30:40.279Z Reads: 422

```
didn't get a chance to check it today unfortunately, but Thanksgiving break is in two days. I'll be able to work on it then without school and tennis practice taking up my whole day...
```

---
## \#12 Posted by: NNGG Posted at: 2016-07-24T05:47:53.418Z Reads: 355

```
woah I just realized you play tennis. you compete?
```

---
## \#13 Posted by: Pablo_702 Posted at: 2016-08-11T23:46:43.144Z Reads: 333

```
u ever got your ppm setting right? im having the same issue and on top of that as soon as i get to my destination if i turn my remote of with out turning the board off before the motor star spinning at full speed i almos had to ran behing my board hahahaha, good thing i had one foot on it still, any ideas????
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-11T23:47:49.108Z Reads: 325

```
What remote do you have? Sounds like you need to set your throttle mid on your receiver.
```

---
## \#15 Posted by: Pablo_702 Posted at: 2016-08-11T23:48:51.895Z Reads: 320

```
i have a mastercho mod (gt2b) do u mean on the transmitter?
```

---
## \#16 Posted by: Jinra Posted at: 2016-08-11T23:49:24.277Z Reads: 317

```
The receiver. Try re-binding the remote doing the whole rebind process.
```

---
## \#17 Posted by: Pablo_702 Posted at: 2016-08-11T23:52:51.554Z Reads: 313

```
ill try it tonight when i get home, before switching to ppm last nigh i was riding the non ppm mode i guess idk whats called, and also the throttle was already max at 1/3,
i thougth the binding procces is just to sync remote with speed controller dou think that by rebinding ill actually change anything??
```

---
## \#18 Posted by: Jinra Posted at: 2016-08-11T23:53:41.374Z Reads: 294

```
Rebind also sets the throttle mid value on the receiver, at least on my remote.
```

---
## \#19 Posted by: Pablo_702 Posted at: 2016-08-11T23:54:22.936Z Reads: 294

```
u have a gt2b?
```

---
## \#20 Posted by: Jinra Posted at: 2016-08-11T23:54:55.029Z Reads: 291

```
Winning remote. Pretty similar receivers though. They work with each other.
```

---
## \#21 Posted by: Pablo_702 Posted at: 2016-08-11T23:57:38.165Z Reads: 281

```
aight ill try it when i get home tonight, thank you man i hope thats it what bothers me the most is the board taking out when i turn transmitter off, the throttle im kind of use to already since i been riding like that since i put it together a month ago, and ya know first build u just want to wrap it up asap and go skate
```

---
## \#22 Posted by: Jinra Posted at: 2016-08-11T23:58:48.578Z Reads: 277

```
If you adjust the PWM on the remote you have to rebind to set neutral on the receiver. I had similar result when I adjusted without rebinding. Turning off remote = throttle forward.
```

---
## \#23 Posted by: Pablo_702 Posted at: 2016-08-12T00:03:54.355Z Reads: 267

```
i hope u are online tonight just in case i need help!
```

---
## \#24 Posted by: Jinra Posted at: 2016-08-12T00:07:36.565Z Reads: 263

```
i'm on this forum almost 24/7
```

---
## \#25 Posted by: Pablo_702 Posted at: 2016-08-12T00:17:01.368Z Reads: 255

```
hahahahahahaha i know theres a few like us @Michaelinvegas is one of them
```

---
## \#26 Posted by: Hummie Posted at: 2016-08-12T00:25:46.815Z Reads: 238

```
I'm thinking my steez remote might be able to benefit from a ppm setting but not sure if anything more can be done. Anyone experience bad brakes wi the steez?  I don't mean weak brakes, what happens is there's no modulation possible, as soon as I put on half brakes there's no going back to quarter brakes I have to release the brakes and then put them back on to get to quarter brakes. I've already adjusted them in Ppm and it's seeming a steez flaw
```

---
## \#27 Posted by: Jinra Posted at: 2016-08-12T00:27:37.278Z Reads: 236

```
You've adjust the min/max PWM signal?
```

---
## \#28 Posted by: Titoxd10001 Posted at: 2016-08-12T00:37:11.215Z Reads: 238

```
The gt2b has the fail safe on the receiver it's a button. You can check in bldc tool by turning off your remote and make sure it goes to 50%. Also make sure that your remote doesn't go below the minimum ppm or you'll lose brakes when you need it the most I superglued a plastic to stop the trigger where it goes to 0%.
```

---
## \#29 Posted by: Pablo_702 Posted at: 2016-08-12T00:41:33.033Z Reads: 230

```
mmmmm trying to visualize what ur saying here
```

---
## \#30 Posted by: Hummie Posted at: 2016-08-12T00:53:37.487Z Reads: 232

```
Yea I adjusted myself and had evoheyax do it also.  He said its just how the steez works unfortunately and he has the same problem.  Wondering if anything can be done or if anyone else has this prob
```

---
## \#31 Posted by: Titoxd10001 Posted at: 2016-08-12T00:57:25.936Z Reads: 226

```
Adjust throttle trim on the remote till you get 50% in bldc tool. Then hold the fail safe button on the receiver. Now when you turn off the remote it should remain at 50%.
```

---
## \#32 Posted by: cmatson Posted at: 2016-08-12T02:05:00.256Z Reads: 224

```
Ya of course @NNGG,

I don't do any USTA tournaments anymore, but play year round, and enjoy my school season the most by far-

Haha the only reason I built an eboard was to get to where I play tennis after school (about 2.5 miles away) and be able to get there and back with zero effort. It sucks biking home after not being able to feel your legs.. Lol.
```

---
## \#33 Posted by: NNGG Posted at: 2016-08-12T02:07:44.036Z Reads: 209

```
I was in your exact same position when I was in high school, except I loved to mountain bike to school and tennis through my backyard canyon that eventually lead to my high school. I didnt build an esk8 back then because I was having so much fun with building rc airplanes :grin:
```

---
## \#34 Posted by: cmatson Posted at: 2016-08-12T02:08:58.492Z Reads: 200

```
Rc cars -> eboards 

This was me
```

---
## \#35 Posted by: NNGG Posted at: 2016-08-12T02:10:09.834Z Reads: 206

```
Rc airplanes were always king for me. Back when Ni-cad was supreme
```

---
## \#36 Posted by: Titoxd10001 Posted at: 2016-08-12T02:18:16.787Z Reads: 215

```
I have to many rc cars that I don't use anymore because e board took over
```

---
## \#37 Posted by: rasmukri Posted at: 2017-04-04T00:00:18.811Z Reads: 152

```
Holy resurrected threads Batman!!
I have some PPM issues. When I change the min and max pulswidth then the resting position is nowhere near 50% it usually sits around 63% or so. If I adjust the knob on the remote to change it down to about 50% then full throttle goes to about 85% when its at full. I have the GT2B transmitter with dual VESC. Is there a way to adjust the actual transmitter for it to sit at proper 50% neutral? Also when i test the remote connect failure by turning off my remote the motors go to like 3/4 power. At first I thought it was because i was still plugged into the computer but after the VESC were unplugged from there it still goes to full speed. I tried changing the brake setting for the timeout but that did nothing.
 I hope this makes sense and thanks if anyone can help me out.`
Edit: I just opened my transmitter and tried messing with the 2 white potentiometers and that didn't do anything different that the knob i already tried messing with. if i adjust to 50% then full throttle is less than 100%.

<img src="/uploads/db1493/original/3X/3/9/3930acddd774d68f4590936acc7361d476b061c6.jpg" width="690" height="406">
<img src="/uploads/db1493/original/3X/c/c/ccd15a09a254fa9159dd2ce4a92f047045f5933b.jpg" width="690" height="407">
<img src="/uploads/db1493/original/3X/b/7/b7c70477a8a221ac4942b01efbdf86ee4e785916.jpg" width="690" height="408">
```

---
## \#38 Posted by: Titoxd10001 Posted at: 2017-04-04T00:22:04.903Z Reads: 136

```
If you're using a modded case you need to limit trigger brake travel physically. Your min an max pulsewidth values need to be close to 1 and 2. Then you be able to set failsafe properly
```

---
## \#39 Posted by: rasmukri Posted at: 2017-04-04T01:14:31.774Z Reads: 143

```
Any recommendations for doing that? Pictures?
All I can think of is filling in the opening a little with JB Weld and then filing it down to make it the right sizes.
```

---
## \#40 Posted by: Titoxd10001 Posted at: 2017-04-04T01:31:43.537Z Reads: 154

```
That's pretty much what I did, I used steelstik jb weld then just black marker. A little sloppy but you can't really tell. You pretty much want it even with the case. Also it will be more comfortable because your finger doesn't have to bend as much to get to the max brakes.
<img src="/uploads/db1493/original/3X/2/0/20287f3830347af7fb54bd066bd1a0fa76a4a95c.jpg" width="375" height="500">
```

---
## \#41 Posted by: kornum Posted at: 2017-07-18T18:41:56.881Z Reads: 109

```
Mine is not at 50% In the graph In the bottom.... guessing i only have Breaking on/off? I have this controler https://www.proto-boards.com/product-page/wireless-remote-controller can i change that?
```

---
## \#42 Posted by: Jinra Posted at: 2017-07-18T18:54:55.949Z Reads: 111

```
Use Ackmaniac's firmware so you can set center PPM position.

http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
