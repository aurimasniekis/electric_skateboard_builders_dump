# What does motor MAX actually means?

### Replies: 230 Views: 9637

## \#1 Posted by: joeadams101 Posted at: 2016-08-25T07:11:43.467Z Reads: 716

```
Hey Just I was just reading a thread about someone having problems with a setup. I believe is was a 175kv motor and he had a 16t/36 system. He said he was overheating MOTOR MAX @ 35. He went up to 45 and his problem was fixed. How does the Motor max work? Someone care to explain? Thanks!
```

---
## \#2 Posted by: makevoid Posted at: 2016-08-25T08:06:06.630Z Reads: 721

```
Motor max (A)  is the maximum amount of current the VESC is  supplying to the motor. A value that is too high will overheat the motor if it's over the max rated watts (thus amps) of the motor as the motor can't whitstand that amount of current because of physical  limits (amount of copper etc). 

When setting a too low value instead, especially going up hill and/or with an heavy load, overheating can happen because the motor can't enter/maintain  the "good efficiency zone" (where you have still some throttle left or at least going full throttle your board doesn't decelerate) and it will run at lower RPM and in the end it will need a higher amount of total current to do the same amount of travel, that loss of current used to move the board will be converted to heat. 

If you can get enough speed uphill so that your board maintains it or doesn't decelerate greatly (in fact gaining enough speed before the hill/steep point helps) your board, even if the esc will give max amps, the board will decelerate and even stop. Having a better acceleration (via higher motor max) to use before getting to a steep point will help this too. 

So if you're not light or have a lot of hills you should set a higher motor max, instead if you want to maximize battery performance you can set a low motor amp but it's really battery amps max the value that determines the amount of current the ESC pulls from your battery.
```

---
## \#3 Posted by: devin Posted at: 2016-08-25T16:55:50.468Z Reads: 687

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#4 Posted by: evoheyax Posted at: 2016-08-25T17:35:42.188Z Reads: 634

```
The interesting part I wonder is does anyone know if this is an absolute max or can you still burst higher? I want to burst up to 120 amps (or 30 per motor), but I can't do more than 80 con, I don't want more than 72 personally (which is 18 per motor). But it seems like there's only one setting.
```

---
## \#5 Posted by: devin Posted at: 2016-08-25T17:38:51.275Z Reads: 629

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#6 Posted by: evoheyax Posted at: 2016-08-25T17:45:42.373Z Reads: 596

```
[quote="devin, post:5, topic:8292"]
This should eliminate the unpredictable acceleration / regen braking issues
[/quote]


What issues are these, the sometimes dropping of brakes or acceleration? I definitely feel like I get some slightly weird behavior some times, but I've always associated that to my controller. I want to meet up and do some tests with my 4wd like you did with John. I seem to be getting way better range with 4wd than 2wd, by almost double. I did increase my battery from 3p to 4p, but I can get about 8 miles now instead of 4...
```

---
## \#7 Posted by: devin Posted at: 2016-08-25T17:56:15.353Z Reads: 564

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-08-25T18:25:13.528Z Reads: 553

```
[quote="devin, post:5, topic:8292"]
Set battery amp limit to desired figure. Then set motor amp limit & absolute amp limit at least 12x higher or more.
[/quote]

so.. following that logic... if i have an older space cell, or what i'm now calling a raptor cell to avoid confusion... 

Batt Max: 45
Motor max: 540
Absolute max: 540

That seems odd to me. Usually those settings would look somethig like this:

Batt Max: 45
Motor max: 60
Absolute max: 130


I've seen several of your posts about the AC v DC thing. I'm just trying to straighten this out in my head because i'm not an EE and i get lost easily when you start talking EE stuff.
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-25T18:27:36.189Z Reads: 528

```
I've seen his posts so many times all over forum even when it's not related the topic at hand, and the more I see the less inclined to give his theory any credibility. It also makes no sense to me.
```

---
## \#10 Posted by: devin Posted at: 2016-08-25T18:30:05.167Z Reads: 521

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#11 Posted by: longhairedboy Posted at: 2016-08-25T18:34:37.449Z Reads: 510

```
That explains why raptors haul ass on a 45 amp fuse and why noone will ever need an 80 amp BMS and why Ollin told me i'd be lucky to ever see anything approaching 45 amps, all reasons i switched to 60amp BMSs and felt comfortable with the leftover headroom for cooler running.
```

---
## \#12 Posted by: devin Posted at: 2016-08-25T22:23:35.961Z Reads: 499

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#13 Posted by: devin Posted at: 2016-08-26T02:37:44.219Z Reads: 484

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#14 Posted by: treenutter Posted at: 2016-08-26T04:02:02.845Z Reads: 481

```
@devin like @longhairedboy I've struggled to understand your posts about this issue. It seems like a a compelling argument, but I don't have the knowledge to unpack it. From a more practical perspective, has anyone applied this logic in a build and tested it? What was the result? I'm wary of frying a VESC to test the prediction.
```

---
## \#15 Posted by: devin Posted at: 2016-08-26T08:53:53.579Z Reads: 471

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#16 Posted by: PB1 Posted at: 2016-08-26T11:07:16.416Z Reads: 464

```
@devin, the only thing that your example above proves is that the battery limit didn't have any effect in this case. Could have been set at 50, 60 or 100 Amps. No effect. 

If we approximate the battery voltage to 43v (allowing for some voltage sag) we can conclude that hummies board used 
43V * 44A = 1892 Watts as peak power. 

Why the board didn't use more that this peak power we can only guess. 
Hills not steep enough
hummie not accelerating fast enough because he would have been thrown down
motors too hot
... ?
```

---
## \#17 Posted by: treenutter Posted at: 2016-08-26T14:11:06.249Z Reads: 449

```
thx @devin it helps to know that this approach hasn't been tested "in the wild" just yet. I think your assertion concerns VESC owners because your recommendation asks us to exceed the default values by quite a lot.  

Have you tried sharing this theory with the folks on Vedder's forum for VESC? I think you'll find a lot of people there with the right experience to comment on it. 

@chaka @elkick Do you have thoughts on Devin's theory about batt max / motor max/ absolute max ?
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2016-08-26T14:20:32.533Z Reads: 434

```
Because, it is IMPOSSIBLE.... current is limited by the type of winding use inside the motor, witch can not exceeded maximum power of the motor... Like 500amp at 43v, the motor would need the tolerate the equivalent of P=V*I... 500*43= 21KW of power... EVEN ELECTRIC POWER LINE DOESN'T SUPPORT THIS KIND OF POWER.....
```

---
## \#19 Posted by: devin Posted at: 2016-08-26T14:21:06.339Z Reads: 428

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#20 Posted by: devin Posted at: 2016-08-26T14:24:40.582Z Reads: 421

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2016-08-26T14:40:07.943Z Reads: 408

```
Well, I won't lose anymore time with you, because you don't really want to understand that motor are rated for maximum power and cable can only withstand a certain amount of current.
```

---
## \#22 Posted by: longhairedboy Posted at: 2016-08-26T14:41:44.186Z Reads: 401

```
Like i said i'm not set up to test that yet but i'm looking into finding what i need to do it. I'm already working on one project that will tell me these things, but its a little ways out. I'll see what i can do for the mean time.
```

---
## \#23 Posted by: devin Posted at: 2016-08-26T14:42:41.600Z Reads: 399

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2016-08-26T14:46:44.030Z Reads: 384

```
So are you're motor rate for 6000W.... or else it will burn....
```

---
## \#25 Posted by: devin Posted at: 2016-08-26T14:48:37.331Z Reads: 376

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#26 Posted by: Heavy1 Posted at: 2016-08-26T14:54:27.661Z Reads: 364

```
Is there more to why you think it's should be 10x the battery limit? Why 10x?
```

---
## \#27 Posted by: devin Posted at: 2016-08-26T14:58:44.042Z Reads: 368

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#28 Posted by: Heavy1 Posted at: 2016-08-26T15:09:52.533Z Reads: 344

```
I started reading this and saw how long it is, it's 1am here. Maybe tomorrow
```

---
## \#29 Posted by: PB1 Posted at: 2016-08-26T17:40:36.196Z Reads: 343

```
@devin,  don't get stuck on your idea.  Don't think you will find many listeners here. 

Your "theory" only proofs one thing : it does make sense to have two separate amp limits.   
Motor amp limit to protect the motor.  It will mainly be hit accelerating at low speeds. 
Battery amp limit (or fuse)  to protect the battery and overall system.  In a well balanced system it will not be hit.  

Easy,  no conspiracy here ...
```

---
## \#30 Posted by: devin Posted at: 2016-08-26T17:47:19.644Z Reads: 341

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#31 Posted by: PB1 Posted at: 2016-08-26T17:54:59.834Z Reads: 327

```
They are not related.  

If you WANT TO hit battery limit...  Just set it low enough.  Don't know why you want to.  Just set it low.
```

---
## \#32 Posted by: devin Posted at: 2016-08-26T17:56:47.589Z Reads: 321

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#33 Posted by: devin Posted at: 2016-08-26T18:49:49.494Z Reads: 315

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#34 Posted by: longhairedboy Posted at: 2016-08-26T19:12:24.166Z Reads: 312

```
i would never want to hit the absolute batt max limit personally. In fact i set it to something that i know is well within, usually below half, of the stated combined burst rating of the P group. For example, i use Sammy INR18650-25Rs beacuase i'm in love with them, they have a stated continuous current rating of 20A and a burst of 100A which in a 4P group would make it 80A and 400A respectively, so usually my abs max is set to something like 120 or 130. 

I want everything to run cool and use way less power than its rated for. I'm not really interested in bouncing up against hardware limitations in boards i sell to other people.
```

---
## \#35 Posted by: longhairedboy Posted at: 2016-08-26T19:14:27.110Z Reads: 307

```
also i think i agree with what you're saying. It does seem to me like that's how it would play out.
```

---
## \#36 Posted by: devin Posted at: 2016-08-26T19:15:59.041Z Reads: 313

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#37 Posted by: longhairedboy Posted at: 2016-08-26T19:17:41.914Z Reads: 305

```
i can agree with that, yeah. I mean it probably would't climb hills for shit and would have the mushiest brakes ever but yeah.
```

---
## \#38 Posted by: longhairedboy Posted at: 2016-08-26T19:20:14.198Z Reads: 307

```
i sort of wish i had a board i didn't care much about so i could try this, but the reality is i need my scarlet to not be fried accidentally in the name of science. 

How would these setting affect braking? How does the negative regen current play into this?
```

---
## \#39 Posted by: devin Posted at: 2016-08-26T19:24:29.793Z Reads: 315

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#40 Posted by: longhairedboy Posted at: 2016-08-26T19:42:08.237Z Reads: 316

```
usually the sudden bursts of acceleration while already moving are attributed to the motor hitting the "sweet spot." Somepeople call it the secret turbo. That's when the VTEC kicks in as they would have said years ago before literally everyone had variable valve timing. As far as I know, the only issues to have happened relating to sudden accelleration that led to an accident are PWM signal loop or failure issues from the receiver, or from the remote and coming through the receiver. You're suggesting that this could also happen as a result of what your describing, right?

uneven braking is something i've already experienced, but its so minor, even at speed, that its hard to attribute to all of this math and behaves more like its just doing that because you have a lot of momentum going on real world terrain where every little thing affects how the motors gve the VESC feedback and therfore how the VESC controls the motors. Or maybe we're saying the same thing here, because honestly, i'm still having an issue understanding it all. IT makes sense when i read it, but then when i go to think about it, it turns to mush in my head. I probably should have taken engineering classes in school instead of art and psychology before i dropped out and made my career in web development while we were all still fighting our families for dial-up time.
```

---
## \#41 Posted by: furryfrog Posted at: 2016-08-26T20:39:13.278Z Reads: 299

```
I have not looked into this specifically, and I have yet to get my first E skate, but has anyone looked into how power factors can change the relationship between current, volts, and watts? Anyone who understands AC motor theory and inductive loads will be familiar with power factor. It's my assumption that this could play a role in brushless motors, since all motors are an inductive load.
     Though these motors do not use a true 3 phase sine wave per say to operate, I would Imagine the current waveform is still affected by the inductance in the motor, and a lagging power factor is developed between the pulsed waveforms. In otherwords the pulsed current peaks and the pulsed voltake peaks become seperated, described as a lagging power factor. I am assuming this is worse at a lower duty cycle than at a higher duty cycle, so the power factor would be worse at a lower duty cycle, lower loads, or erpm.
     In The AC world we call the relationship between measured current and measured volts VA, or volt amps, also called apparent power. This is not watts, It always measures higher than watts. True watts are the comparison between the instantaneous amount of current to voltage.
     With a lagging power factor the peak of the current lags behind the peak of the volts, so when you multiply them together at there instantaneous position you have less watts.
My assumption is at this point, setting the motor max has to do with the current seen in your motor. Because of power factors, this measurment will be higher than the calculated current from watts.
     Understanding Power Factors and AC motor theory can be tricky. Brushless motors and the accociated hardware to run them, seem even more difficult to understand, being that there are relationships to both DC and AC. I am not pretending to understand brushless motors, this post is an assumption on my part, but I thought I would throw this in this thread. I do understand AC motor theory reasonably well though.
```

---
## \#42 Posted by: devin Posted at: 2016-08-26T21:48:22.187Z Reads: 273

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#43 Posted by: devin Posted at: 2016-08-26T22:19:05.315Z Reads: 259

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#44 Posted by: devin Posted at: 2016-08-27T01:31:10.517Z Reads: 264

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#45 Posted by: PB1 Posted at: 2016-08-27T06:02:14.286Z Reads: 262

```
[quote="devin, post:33, topic:8292"]
if i keep lowering and lowering the battery max setting (keeping motor/absolute the same), each time trying to draw max battery amps during low rpm acceleration full throttle, eventually the battery max limit will be hit during low speed acceleration, and not the motor/absolute max limit? would you agree?
by the same line of logic, by keeping the battery limit at 50, then raising and raising the motor/absolute max settings, eventually the original 50 battery max limit will be hit during full throttle low rpm acceleration? would you agree?
[/quote]

Agree with 1

Not agreeing with point two. 
If you raise the motor limit you get to a point where you don't hit any limit because your motors don't draw enough amps. Perfect.  
Or you burn your motor.  

In a well balanced system you might not hit any limits.  And then your theory is rubbish.
```

---
## \#46 Posted by: devin Posted at: 2016-08-27T09:05:53.818Z Reads: 249

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#47 Posted by: Svenska Posted at: 2016-08-27T09:20:32.190Z Reads: 235

```
One reason the VESC is so good is because it implements very sophisticated Voltage/Current measurements. 
What your little cheap watt meter won't see is spikes. It just doesn't sample fast enough. It is before the big caps too. 
If you want to really see what happens use this:
https://play.google.com/store/apps/details?id=de.solarturtle.vedder_monitor

Here is the thread on ES for the project:
https://endless-sphere.com/forums/viewtopic.php?f=35&t=68975&start=125

Log what the VESC sees and run it through Matlab or any other software of your choice. Then look at the code and see why it reacts the way it does.
```

---
## \#48 Posted by: devin Posted at: 2016-08-27T09:38:51.739Z Reads: 222

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#49 Posted by: devin Posted at: 2016-08-27T10:18:18.748Z Reads: 219

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#50 Posted by: PB1 Posted at: 2016-08-27T10:26:44.268Z Reads: 224

```
[quote="devin, post:46, topic:8292"]
but you're saying if you raise the motor max slightly, you won't hit the motor limit anymore during low rpm full throttle acceleration? and you won't hit any limit? because the motors don't draw enough amps?
[/quote]

Exactly! 

[quote="devin, post:46, topic:8292"]
lets look at what would happen if I hooked a 50V supply directly to 2 of @Hummie 's motor winding leads (no controller - his winding resistance is 0.12566 ohm). this is ohm's law.
[/quote] 

Do you hook up AC or DC? 
If you hook up DC  ohms law will eventually apply and the winding resistance will be the only resistance.  

If you hook up AC you have the inductance fighting quick changes in current and your resistance is far bigger than the pure wire resistance.  
You can calculate all of this.  

So under no circumstances you will have 400 amps.
```

---
## \#51 Posted by: PB1 Posted at: 2016-08-27T10:30:45.720Z Reads: 200

```
I would suspect that in hummies setup of 70amps battery limit and 70amps motor limit none of these limits are hit.
```

---
## \#52 Posted by: devin Posted at: 2016-08-27T10:31:51.496Z Reads: 205

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#53 Posted by: devin Posted at: 2016-08-27T10:37:20.821Z Reads: 206

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#54 Posted by: makevoid Posted at: 2016-08-27T10:46:41.485Z Reads: 198

```
Wow that's awesome! is it open source? I'll try it soon (I have an HM-10 lying around even if most of the users use HC-05) ! The UI is in german, I could  translate it if it was open.  I couldn't find a github link of that but  I found another project from that post ( https://github.com/bchiu/Traction/blob/master/README.md  ) that looks good, at least the UI looks very good, it seems a bit complex/advanced (using react and protobufs)  but that can be a good thing if it's complete / stable.
```

---
## \#55 Posted by: PB1 Posted at: 2016-08-27T11:38:01.114Z Reads: 199

```
[quote="devin, post:53, topic:8292"]
@Pb1 that is not true. the motor amp limit (AC) is being hit during low rpm full throttle acceleration. otherwise the peak power would be 20kw x 2 hub motors = 40kw as per ohm's law.
[/quote]

Absolut rubbish! A motor is not just a wire and you can't use ohms law! 

Test it!  Hook up hummies board to a PC and monitor motor amps. I reckon they are below 70 amps.
```

---
## \#56 Posted by: devin Posted at: 2016-08-27T11:43:01.505Z Reads: 197

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#57 Posted by: devin Posted at: 2016-08-27T11:46:40.509Z Reads: 197

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#58 Posted by: makevoid Posted at: 2016-08-27T12:24:38.727Z Reads: 204

```
I think there is, I think the VESC limits the max acceleration you can have and this creates the impression of a hitting a greater acceleration spot for 1/2 seconds. When you are full throttle on a slight hill or on a flat but still not at top speed there's a treshold point, before that point your VESC is  using all amps at/close to you motor max and then the mechanical resistance becomes less thus the VESC will still supply max amps but you'll accelerate more than the VESC limit settings (that's when you'll get more acceleration). Then the VESC will notice that the acceleration is over the limit and it will limit the current to prevent over accelerating even if you are not using max current. I believe it works like this. 


Solution: modify Vedder's code to release that current more softly or check max acceleration more frequently or simply use less throttle ;)


 @devin 
Have you seen Vedder videos with logging overlay like this? We can see the data but not the throttle position unfortunately. Check at 2:40
https://youtu.be/nGb-zt2Jp9k
```

---
## \#59 Posted by: PB1 Posted at: 2016-08-27T13:51:16.224Z Reads: 192

```
[quote="devin, post:56, topic:8292"]
Pb1, so how do you explain why he is not getting 20kw x 2 hub motors = 40kw, as would be the case with ohms law, if current is not being restricted by the programmed motor amp limit (AC)?
[/quote]

BECAUSE ...  A....  MOTOR...  IS...  NOT...  A...  WIRE! 

In your example you would produce 40kw LOSS!
```

---
## \#60 Posted by: devin Posted at: 2016-08-27T14:10:57.389Z Reads: 191

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#61 Posted by: Hummie Posted at: 2016-08-27T14:58:23.407Z Reads: 172

```
Devin if you write a concise question I'll post it on vedders site.
```

---
## \#62 Posted by: devin Posted at: 2016-08-27T15:11:33.816Z Reads: 175

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#63 Posted by: devin Posted at: 2016-08-27T15:43:15.816Z Reads: 174

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#64 Posted by: devin Posted at: 2016-08-27T15:50:08.656Z Reads: 175

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#65 Posted by: devin Posted at: 2016-08-27T16:13:32.058Z Reads: 170

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#66 Posted by: devin Posted at: 2016-08-27T16:33:03.727Z Reads: 158

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#67 Posted by: treenutter Posted at: 2016-08-27T16:42:36.746Z Reads: 162

```
[quote="devin, post:66, topic:8292"]
if no one wants to test this... FINE! at least I'LL have a clear conscience the next time someone is injured or killed when their motor hits the "secret turbo" rpm at the "sweet spot"!!
[/quote]

@devin I think that we all appreciate your efforts to unravel this dilemma. Have you considered testing this with one of your own VESCs? 

Many of us on the forum only have one usable build at a given time, so the risk of damaging a VESC for this exploration is a tough sell.
```

---
## \#68 Posted by: devin Posted at: 2016-08-27T16:43:55.017Z Reads: 161

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#69 Posted by: treenutter Posted at: 2016-08-27T16:47:00.145Z Reads: 160

```
@devin OK message received. Could you please stop tagging me in your posts about this matter? I don't feel that I have any additional input to offer. Good luck sorting it out!
```

---
## \#70 Posted by: Hummie Posted at: 2016-08-27T16:47:54.496Z Reads: 154

```
The throttle response is pretty smooth through the range of speed from 5-30. No hidden sweet spot  . The danger aspect isn't there I really don't think and people on boards and bikes are not being surprise bucked off their vehicle. What is the one single thing I can take from this thread, in terms of bettering my vehicles performance?
```

---
## \#71 Posted by: devin Posted at: 2016-08-27T16:49:04.827Z Reads: 155

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#72 Posted by: Hummie Posted at: 2016-08-27T16:52:16.322Z Reads: 155

```
You need more sleep maybe.  I think the danger you are writing about with the throttle and a sweet spot is just not there in practice.  That's rediculous to me.  But the different amp limits. Three of them.  Battery motor and max. That's what I want to know.
```

---
## \#73 Posted by: devin Posted at: 2016-08-27T16:58:47.331Z Reads: 157

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#74 Posted by: Jinra Posted at: 2016-08-27T17:02:11.880Z Reads: 151

```
my throttle is smooth from 0 to 35. no bursts of speed for me, though I'm using 50mm motors
```

---
## \#75 Posted by: Hummie Posted at: 2016-08-27T17:09:26.637Z Reads: 154

```
Someone just posted this above 

https://play.google.com/store/apps/details?id=de.solarturtle.vedder_monitor

Find the outputs at .005 seconds at full duty cycle and see the increases every small increment of time going forward.  Aren't all the variables represented n holds tool realtime data?  Not max   and then u can see
```

---
## \#76 Posted by: Svenska Posted at: 2016-08-27T17:16:01.825Z Reads: 156

```
@Hummie 

The 3 different limits are really easy.

Motor Max:
Motor current limit. There to protect your motor. Take the max current your motor is able to supply, multiply by 0.6 if it is smaller then 60 enter that in there. If it is bigger then 60, enter 60 in there.

Batt max:
Battery current limit. There to protect your battery. Take the max continuous current your battery is able to supply, multiply by 0.6 and enter that in there.

Absolute max: 
If any of the current samples (There is multiple ones taken on both ends of the VESC) is bigger than this number a fault is generated and the VESC needs a reboot to get back to live. This is pretty much a last ditch effort to keep stuff from going really wrong. This value should never be hit.

The 0.6 is a very conservative setting. Everything from 0.5 - 0.8 should be ok to use. If you know what you do you can go higher, much higher.
```

---
## \#77 Posted by: devin Posted at: 2016-08-27T17:17:16.614Z Reads: 149

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#78 Posted by: Svenska Posted at: 2016-08-27T17:17:58.515Z Reads: 147

```
I posted that. I haven't tried it, don't know if that is any good.
If you should try it, let me know please.
```

---
## \#79 Posted by: Hummie Posted at: 2016-08-27T17:24:20.164Z Reads: 151

```
Yes Devin I see that.  We can agree on that.  What are we trying to figure beyond that. 
Svenska nice find. I want someone to tell me what I need to do next. Get an android phone for starters.  A cheap one.  Someone should do a 3D printed trigger for a cheap android phone! That would be the clincher.
```

---
## \#80 Posted by: devin Posted at: 2016-08-27T17:26:09.780Z Reads: 155

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#81 Posted by: devin Posted at: 2016-08-27T17:35:08.682Z Reads: 148

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#82 Posted by: Hummie Posted at: 2016-08-27T17:59:14.329Z Reads: 148

```
 I'm assuming that a motor's heat to torque ratio is going to be the same regardless of how the 3amp limits are set.  
I do want to know what the max power I can put through the esc to the motor is.  They could easily be messed with ( unfortunately ud have to go back onto a real computer with the linked phone thing) none the less going through different settings and ...it only relates to heat right?  That's the one limitation on things and there is that temp sensor and the over-heat cut-off on the vesc so really there shouldn't be a danger in increasing the motor amp limit a lot right? 

  Could almost have been all figured out from youre phone. 

  I'm really happy with the performance on 70/70 but would love more power always.
```

---
## \#83 Posted by: Svenska Posted at: 2016-08-27T18:04:49.701Z Reads: 137

```
@Hummie

You're forgetting about spikes. I'm not knowledgeable enough to understand where they are coming from. But I ensure you they are there and they fuck your shit right up. 
That is why the MOSFETs can take 250A but you want to stay way below that.
```

---
## \#84 Posted by: Hummie Posted at: 2016-08-27T18:11:17.489Z Reads: 127

```
I've heard of voltage spikes with the vesc but never heard of amp spikes.  What is their danger?  Only heat right?
```

---
## \#85 Posted by: Svenska Posted at: 2016-08-27T18:20:18.919Z Reads: 126

```
You need to think of it in terms of power. 

If you go and lightly stroke the cheek of your special other you transmit a certain amount of power over time, aka work.
If you punch them in the face, you transmit the same amount of power but in a much shorter time.

One of these two scenarios has a good outcome.
```

---
## \#86 Posted by: devin Posted at: 2016-08-27T18:31:49.857Z Reads: 127

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#87 Posted by: devin Posted at: 2016-08-27T18:33:26.692Z Reads: 128

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#88 Posted by: devin Posted at: 2016-08-27T18:34:39.736Z Reads: 126

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#89 Posted by: Svenska Posted at: 2016-08-27T18:49:09.024Z Reads: 126

```
Have a look at fig 10.
```

---
## \#90 Posted by: devin Posted at: 2016-08-27T19:36:47.256Z Reads: 125

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#91 Posted by: Hummie Posted at: 2016-08-27T20:41:41.683Z Reads: 121

```
What does fig 10 say?
```

---
## \#92 Posted by: Hummie Posted at: 2016-08-27T22:25:25.860Z Reads: 127

```
The temp sensor is singular and off the side from the mosfets a bit so maybe you could burn up before it was sensed.  But there's wiggle room and bumping it up, motor amps,  or maybe amp max, u could see what the temp was doing and get an idea of what to expect. 
My board is down right now unfortunately.  Hope to be riding in a day or two max and then I'd be interested in testing a bit but only after reading up some more on other's max settings with success.  I think I've seen 150 done!
```

---
## \#93 Posted by: devin Posted at: 2016-08-27T22:33:14.345Z Reads: 125

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#94 Posted by: Hummie Posted at: 2016-08-27T23:44:37.619Z Reads: 120

```
But with volts being converted to amps wonder what motor amps are possible. Maybe you can still only have 40amps drawn from the battery yet still have a huge amount of amps
```

---
## \#95 Posted by: devin Posted at: 2016-08-28T00:33:56.520Z Reads: 119

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#96 Posted by: devin Posted at: 2016-08-28T00:45:32.895Z Reads: 127

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#97 Posted by: devin Posted at: 2016-08-28T00:47:54.101Z Reads: 131

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#98 Posted by: devin Posted at: 2016-08-29T17:12:03.446Z Reads: 143

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#99 Posted by: devin Posted at: 2016-08-29T17:16:33.532Z Reads: 143

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#100 Posted by: devin Posted at: 2016-08-29T17:33:43.617Z Reads: 138

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#101 Posted by: PB1 Posted at: 2016-08-29T18:43:49.521Z Reads: 135

```
@devin,  I  mentioned several times that I don't like it when you quote me out of context.  
Now you did it again,  single statements out of a private conversation... 

Good luck
```

---
## \#102 Posted by: devin Posted at: 2016-08-29T21:43:33.045Z Reads: 143

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#103 Posted by: makevoid Posted at: 2016-08-29T22:11:45.248Z Reads: 145

```
I am slowly working on a video logging solution even if at the moment it's all in alpha stage and requires multiple apps/steps.

I recorded a video holding an ipad with an [ios logging app](https://github.com/gpxlBen/VESC_Logger) that is actually working and uses the adafruit [bluefruit](https://www.adafruit.com/product/2479) bluetooth chip thing. here's the video:

https://www.youtube.com/watch?v=IBh3x0yLSbo

I [integrated](https://github.com/makevoid/VESC_Logger) the logging to .json file on that app, and that file needs to be manually imported in a [animation generator script/app](https://github.com/makevoid/sdl2-text-video-example) that right now needs to be screen-recorded (example [here](https://www.youtube.com/watch?v=IKrXR40SMpc)) and manually overlayed onto a video through a video editing software (a very manual and cumbersome process) - hopefully I will have time to make it easier and build a full-fledged app/solution to do that.
There is an android app as well that does logging in excel format but I couldn't try yet. I will do in a week or so when I get back home.
```

---
## \#104 Posted by: devin Posted at: 2016-08-29T22:21:32.844Z Reads: 138

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#105 Posted by: makevoid Posted at: 2016-08-29T22:30:04.851Z Reads: 144

```
Well I don't know the winding resistance of the [enertion rspec 6372](http://www.electric-skateboard.builders/t/new-enertion-r-spec-2-0-190kv-6374/358) (also they're not showing up on the site anymore) but I can tell you that the voltage the vesc was showing when the battery was almost fully charge is 32V as you can see in the video, and that on my current [board/build](http://www.electric-skateboard.builders/t/the-mkv2-vesc-8s5p-li-ion-drop-down-deck-97mm-60a-bms/6930) I have only 1 vesc / 1 motor and these are the vesc settings:

    ----------------------------------------------------
    Motor max                                 : 60 A
    ----------------------------------------------------
    Motor min (regen)                         : -50 A
    ----------------------------------------------------
    Batt max                                  : 50 A
    ----------------------------------------------------
    Batt min (regen)                          : -25 A
    ----------------------------------------------------
```

---
## \#106 Posted by: devin Posted at: 2016-08-29T22:31:32.750Z Reads: 141

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#107 Posted by: makevoid Posted at: 2016-08-29T22:33:16.938Z Reads: 135

```
Oh ok, I'll let you know in about a week when I'll be back home, I didn't do FOC detection so I don't have it in the XML file I exported from bldc tool
```

---
## \#108 Posted by: devin Posted at: 2016-08-29T22:34:40.802Z Reads: 136

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#109 Posted by: makevoid Posted at: 2016-08-29T22:36:29.040Z Reads: 135

```
I have another rspec 6372 motor with me and a vesc but only a 12V 1.2A power supply that I brought with me to continue developing the logger app, I can do a FOC detection on that but I don't know if it will output a different result...
```

---
## \#110 Posted by: devin Posted at: 2016-08-29T22:37:11.093Z Reads: 138

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#111 Posted by: makevoid Posted at: 2016-08-29T22:49:18.545Z Reads: 145

```
<img src="/uploads/db1493/original/2X/d/d38062a0cac94f5897ea924f19a7402cf09d91c6.png" width="690" height="68">
```

---
## \#112 Posted by: Hummie Posted at: 2016-08-29T23:39:10.483Z Reads: 147

```
But I didn't say there's  uneven acceleration.  I think ur looking for a false danger. From 0-2mph I can get "cogging". This is common with an extremely slow moving brushless motor.  It's not dangerous.

I would like to know what the limits could be though
```

---
## \#113 Posted by: devin Posted at: 2016-08-30T01:14:44.439Z Reads: 143

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#114 Posted by: Hummie Posted at: 2016-08-30T01:27:00.748Z Reads: 137

```
Cogging is the term people use to describe what is happening when the motor is going very slowly and it doesn't know it's exact position.  This is why if you're not using sensors u need to give it a push.  This is common.  Cogging also is the meaning u gave. 
This isn't a dangerous thing

Data logging has just been figured and available.  I linked u to it in this thread above. Solartutle
```

---
## \#115 Posted by: devin Posted at: 2016-08-30T01:31:42.136Z Reads: 135

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#116 Posted by: devin Posted at: 2016-08-30T01:34:29.999Z Reads: 129

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#117 Posted by: Hummie Posted at: 2016-08-30T01:39:53.476Z Reads: 126

```
There's cogging.  It cogs to maybe up to 2.5mph.  No cogging beyond.   His program is really smooth, smoother than other escs, but it still will cog a bit at that speed.
```

---
## \#118 Posted by: devin Posted at: 2016-08-30T01:43:23.998Z Reads: 124

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#119 Posted by: devin Posted at: 2016-08-30T01:57:31.377Z Reads: 124

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#120 Posted by: devin Posted at: 2016-08-30T02:01:43.990Z Reads: 120

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#121 Posted by: devin Posted at: 2016-08-30T02:06:09.259Z Reads: 115

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#122 Posted by: devin Posted at: 2016-08-30T03:52:04.583Z Reads: 129

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#123 Posted by: devin Posted at: 2016-08-30T04:03:24.679Z Reads: 130

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#124 Posted by: makevoid Posted at: 2016-08-30T06:49:47.710Z Reads: 126

```
You could try increasing the Startup Boost Duty (Advanced tab, bldc current control) value a little bit, what's your current value? Anything up to 0.01 should be ok. That will give more power when starting from still. Jacob suggests a value from 0.07 to 0.09 for his hubs. Hope this helps
```

---
## \#125 Posted by: devin Posted at: 2016-08-30T18:54:18.300Z Reads: 124

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#126 Posted by: makevoid Posted at: 2016-08-30T19:20:46.546Z Reads: 127

```
I wasn't able to finish the external logging data feature on the iOS app before, also I fried the arduino so I couldn't use that as well (logs to SD card). I won't have any real logging data for another week because I am on holiday, can't wait to get back to try it now that I have also the video overlay part done :) . I will let you know.
```

---
## \#127 Posted by: devin Posted at: 2016-08-31T01:35:51.569Z Reads: 134

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#128 Posted by: Heavy1 Posted at: 2016-08-31T04:22:00.340Z Reads: 132

```
@devin So your basic assumption is battery amp/motor amp = duty cycle?
```

---
## \#129 Posted by: devin Posted at: 2016-08-31T13:32:22.380Z Reads: 140

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#130 Posted by: devin Posted at: 2016-08-31T16:27:06.177Z Reads: 136

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#131 Posted by: Heavy1 Posted at: 2016-08-31T17:43:14.557Z Reads: 137

```
@devin 
Just watching vedders logging video, it would appear at any throttle application when you take battery amp/motor amp x100 it is almost always within .5%
```

---
## \#132 Posted by: devin Posted at: 2016-08-31T18:08:53.386Z Reads: 132

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#133 Posted by: Heavy1 Posted at: 2016-08-31T18:24:22.450Z Reads: 121

```
Help me out here, so how is the buck down ratio determined? What determines how many amps are required at 0rpm.
```

---
## \#134 Posted by: devin Posted at: 2016-08-31T18:28:13.001Z Reads: 124

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#135 Posted by: devin Posted at: 2016-08-31T18:44:59.487Z Reads: 126

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#136 Posted by: Heavy1 Posted at: 2016-08-31T19:12:08.763Z Reads: 121

```
So how do these figures play out when you consider the motors are all rated to a max of around 70A, do minimum motor voltages need to be taken into account?
```

---
## \#137 Posted by: devin Posted at: 2016-08-31T19:16:44.137Z Reads: 119

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#138 Posted by: devin Posted at: 2016-08-31T22:40:03.991Z Reads: 119

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#139 Posted by: devin Posted at: 2016-08-31T23:35:45.873Z Reads: 116

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#141 Posted by: Hummie Posted at: 2016-09-01T02:58:02.150Z Reads: 112

```
are you saying space travel is possible with the right vesc settings?  when did this turn into show and tell about anything related to anything you might be interested in.  this is the dance of the winner in the Super Bowl.  i want some of those beers and he said I could have some.
```

---
## \#143 Posted by: Skitzor Posted at: 2016-09-01T14:17:14.054Z Reads: 109

```
As a Belgian it's a shame they put our country on those aweful beers :angel:
```

---
## \#144 Posted by: devin Posted at: 2016-09-01T15:09:04.809Z Reads: 112

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#145 Posted by: devin Posted at: 2016-09-02T17:24:57.633Z Reads: 112

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#146 Posted by: Hummie Posted at: 2016-09-02T20:10:49.636Z Reads: 118

```
i think you rubbed it in too much.  reminds me i should be rubbing it in about volts being converted to amps.
```

---
## \#147 Posted by: devin Posted at: 2016-09-02T20:20:30.384Z Reads: 126

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#148 Posted by: PB1 Posted at: 2016-09-02T20:39:56.537Z Reads: 122

```
@devin, you don't like my statements. 
I'm not agreeing with your figures nor you theories. The video above proves nothing. 

Let's just agree that we don't agree.

I could search this forum and find some statements where your posted rubbish. But what's the point, 
1) nobody cares
2) I I have neither the time nor the energy to do that because I rather spend time with the family, work on my boards, ride my boards or go mountain biking. 

And I never agreed to your wager. 

So instead of nagging me, please do something else.
```

---
## \#149 Posted by: kaziupir Posted at: 2016-09-02T22:06:15.399Z Reads: 115

```
What is goin on here :smiley:
<img src="/uploads/db1493/original/2X/b/b231e43a7aa446636f5cbb75450c68cd50628974.jpg" width="603" height="315">
```

---
## \#151 Posted by: devin Posted at: 2016-09-05T04:37:32.324Z Reads: 102

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#153 Posted by: PB1 Posted at: 2016-09-05T11:57:22.327Z Reads: 91

```
Withdrew my last post as I shouldn't feed the troll. 

Devin, stop nagging me.
```

---
## \#154 Posted by: devin Posted at: 2016-09-08T15:14:11.471Z Reads: 91

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#155 Posted by: devin Posted at: 2016-09-08T15:27:47.511Z Reads: 93

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#156 Posted by: devin Posted at: 2016-09-08T15:48:22.692Z Reads: 87

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#157 Posted by: devin Posted at: 2016-09-08T15:54:57.869Z Reads: 87

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#158 Posted by: devin Posted at: 2016-09-08T16:00:46.833Z Reads: 86

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#159 Posted by: PB1 Posted at: 2016-09-08T16:04:21.835Z Reads: 87

```
That is actually your first sensible idea.  Exactly what I will do.  :slight_smile:
```

---
## \#160 Posted by: devin Posted at: 2016-09-08T16:06:37.035Z Reads: 88

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#161 Posted by: PB1 Posted at: 2016-09-08T16:18:38.989Z Reads: 84

```
I'm sure the whole community can see the difference between our two statements.  

You quoted my statements out of context.  I said those two LIMITS are not a function of each other.  

I've always said that motor and battery currents ARE related. 

So yes,  I'm going to ignore you.
```

---
## \#162 Posted by: devin Posted at: 2016-09-08T16:21:22.582Z Reads: 87

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#163 Posted by: devin Posted at: 2016-09-08T16:36:11.287Z Reads: 86

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#164 Posted by: PB1 Posted at: 2016-09-08T16:38:19.973Z Reads: 88

```
/ignore off 

[quote="devin, post:162, topic:8292"]
So now you agree: "motor and battery currents ARE related."
[/quote]

It was ME who explained this concept in a post to YOU on July 29..  

/ignore on
```

---
## \#165 Posted by: devin Posted at: 2016-09-08T16:39:54.865Z Reads: 88

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#166 Posted by: devin Posted at: 2016-09-08T16:56:45.505Z Reads: 89

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#167 Posted by: devin Posted at: 2016-09-08T17:13:07.523Z Reads: 83

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#168 Posted by: chinzw Posted at: 2016-09-08T17:13:53.942Z Reads: 88

```
[quote="devin, post:102, topic:8292"]
my goal is to save folks from potential serious injury caused by the "secret turbo" "sweet spot accleration" "dangerous acceleration curve" reported by @longhairedboy  & @Luke and the uneven acceleration under load from .001mph-5mph reported by @Hummie
[/quote]

That's just newbies going full throttle and not being prepared for the instant acceleration. You're looking at this from an electrical perspective when you should be looking at it from a physics perspective.
```

---
## \#169 Posted by: devin Posted at: 2016-09-08T17:30:11.769Z Reads: 87

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#170 Posted by: Hummie Posted at: 2016-09-08T17:34:18.495Z Reads: 89

```
No he didn't say that. 
Didn't we already have this warning in bold many times.  I think, and I think most others feel, there are other bigger dangers.   Sure u could have an uneven acceleration curve based on settings.  You can also have it based on the terrain with the amp control program.    We get what you're saying but I don't think it's the danger your making it out to be over and over .
```

---
## \#171 Posted by: devin Posted at: 2016-09-08T17:39:00.510Z Reads: 90

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#172 Posted by: Hummie Posted at: 2016-09-08T17:43:37.728Z Reads: 91

```
Maybe we don't want to blow our stuff up as I've never heard of anyone going over 150 motor amps successfully.   Have u bothered to ask on vedders site or look at the threads there about the limits recommended?
```

---
## \#173 Posted by: devin Posted at: 2016-09-08T17:45:45.207Z Reads: 91

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#174 Posted by: Hummie Posted at: 2016-09-08T17:46:16.398Z Reads: 93

```
I agree to a point.  There could be more power at slow speeds but so you've said.  I don't think the risks you mention are real other than possibly blowing ur stuff up...no matter how cool u think you look with pics of women.
```

---
## \#175 Posted by: devin Posted at: 2016-09-08T17:48:09.424Z Reads: 93

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#176 Posted by: devin Posted at: 2016-09-08T17:55:34.379Z Reads: 91

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#177 Posted by: longhairedboy Posted at: 2016-09-08T18:04:46.148Z Reads: 93

```
Just for the record, 

I never once disagreed with you. I just don't completely understand it yet. My "sweet spot" comment was based on other people's observations as well as my own. That's just what it has been referred to.
```

---
## \#178 Posted by: chinzw Posted at: 2016-09-08T18:06:07.404Z Reads: 102

```
[quote="devin, post:169, topic:8292, full:true"]
[quote="chinzw, post:168, topic:8292"]
That's just newbies going full throttle and not being prepared for the instant acceleration. You're looking at this from an electrical perspective when you should be looking at it from a physics perspective.
[/quote]


@chinzw ok so in your opinion, changing the ratio between motor amp limit and battery amp limit doesn't affect acceleration curve? i strongly disagree.

seems to me everyone is just in mass denial that there's a problem because it is embarassing for everyone to think they've been blindly entering the wrong settings, without having a clue what they mean, and everyone has just grown to accept whatever performance is the result. because that's what's normal.

i'll bet 99% of the people on this forum either thought until this thread, or still think that motor amps and battery amps are the same thing, and that there were 2 limits for no good reason.
[/quote]

I definitely did not say that. But what you're ignoring is a a simple physical principle that the board accelerating under from rest. Why do you think once you're moving this effect doesn't seem so drastic?

Try standing on the roof of a car (lets make it an automatic car so that the acceleration is constant) you will have the same effect! Lets call the car companies and tell them that they have a problem, this can't be happening!

Or grab a 2 stroke dirt bike, give it to a newbie and you'll see him flip it in about 2 seconds.

Or give a ferrari to a guy that drives a pruis... i guarantee he will have problems with the acceleration.

See where im going with this?

Limit the power output for newbies until they're comfortable riding.
```

---
## \#179 Posted by: longhairedboy Posted at: 2016-09-08T18:55:30.119Z Reads: 88

```
motor max is exactly how you limit throttle response and shape the acceleration curve. I don't think there's really any debate about that. If you want a smoother launch that doesn't street your ass at 12S or even 10S then you would set it around 40 or 50, and if you want raptor like acceleration then set it to 60 or higher. 

I personally prefer it set around 40-45 on a 15/36 ratio on 83mm wheels because it still climbs hills like a wild animal and doesn't feel like its constantly trying to shoot out from under me. And it still gets ridiculous top end at well over 30mph.
```

---
## \#180 Posted by: devin Posted at: 2016-09-08T19:01:16.989Z Reads: 90

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#181 Posted by: devin Posted at: 2016-09-08T19:14:06.036Z Reads: 90

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#182 Posted by: chinzw Posted at: 2016-09-08T21:09:12.240Z Reads: 108

```
I'[quote="devin, post:180, topic:8292, full:true"]
[quote="chinzw, post:178, topic:8292"]
I definitely did not say that. But what you're ignoring is a a simple physical principle that the board accelerating under from rest. **Why do you think once you're moving this effect doesn't seem so drastic?**

**Try standing on the roof of a car (lets make it an automatic car so that the acceleration is constant) you will have the same effect!** Lets call the car companies and tell them that they have a problem, this can't be happening!

Or grab a 2 stroke dirt bike, give it to a newbie and you'll see him flip it in about 2 seconds.

Or give a ferrari to a guy that drives a pruis... i guarantee he will have problems with the acceleration.

See where im going with this?

Limit the power output for newbies until they're comfortable riding.
[/quote]

@chinzw **That is not what I am saying is happening when I say "uneven acceleration."**

What I am saying is the effect in some circumstances could be analogous to this:

Let's say you're driving a honda civic through a school zone, there's a police officer who will give you a ticket over 25mph, and you just drove off the mechanic's lot, and **the mechanic has programmed your gas pedal to behave in this manner (though you are unaware of this as the driver)**:

at or **below 20mph, with 10% depression of gas pedal, motor revs to 10% Red Line RPM**

**above 20mph, with 10% depression of gas pedal, motor revs to 50% Red line RPM**

so you're driving through the school zone, trying to stay just under 25mph, and you have no idea the mechanic has programmed your throttle to jump to 50% red line rpm with 10% throttle depression above 20 mph.

so you decide to drive just under 25mph (about 23mph). so you're accelerating smoothly up till you hit to 20mph, when suddenly your engine RPM jumps to 50% Red Line RPM, causing your car to suddenly accelerate well above 25mph in a matter of a second or 2.

the officer witnesses you going above 25 mph and pulls you over and writes you a ticket for speeding in a school zone.

THIS is what I mean by uneven acceleration caused by improperly determined battery max and motor max limits.

This is from my very first post in this topic (Post #3):
[quote="devin, post:3, topic:8292"]
At higher rpms, full throttle, when the ratio between motor amps and battery amps becomes much closer, it actually means you can draw more battery amps suddenly then you could at slower speeds, because now the ratio between the 2 values is much closer than at very low rpms.
[/quote]

PS... this dangerous uneven acceleration effect applies to REGEN Braking batt/motor amp limits as well.
[/quote]

m sorry, have you measured this? Other from some quotes (some of them even misinterpreted) i have not seen any empirical evidence to support your theory. You clearly stated you don't have a VESC, and the only measurement you have is a cheapo amp gauge showing that the peak amps don't hit the limit (which still proves nothing except that the motor wasn't taxed enough).

Also, not sure if you've used any of the remotes we use, but to keep the throttle "light" the manufacturers of the potentiometers use thinner retainer washers, which make the pots more prone to resistance variations (i do actually have proof of this) which on a 5k pot can generate quite a change.

Show us evidence of VESC connected to a controlled and stable pwm that shows this "problems" you want to prove.
```

---
## \#183 Posted by: devin Posted at: 2016-09-08T21:15:56.665Z Reads: 111

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#184 Posted by: chinzw Posted at: 2016-09-08T22:26:36.125Z Reads: 106

```
I'm sorry, but that still doesn't prove your theory. I can think of a few ways to test it, in a controlled environment. But having someone ride a board on the street has relatively 0 value. You want to prove to you're right, you'll need to do it in a controlled environment. Why do you think people don't just go on the street, accelerate their cars 0 to 100, time and plug in the cars Cx value and get that HP number everyone wants to see for free? That's right, TOO many variables.
```

---
## \#185 Posted by: devin Posted at: 2016-09-09T01:10:10.267Z Reads: 104

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#186 Posted by: longhairedboy Posted at: 2016-09-09T13:50:06.150Z Reads: 104

```
[quote="devin, post:181, topic:8292"]
@longhairedboy the dangerous effect I perceive from your methodology is the numbers involved change drastically depending on winding resistance of the motor and voltage of the battery. so if you are used to using certain settings, and then you switch to for example a hub motor with more or less winding resistance, or you swtich to a different voltage battery, the acceleration profile you have become accustomed to based on your batt max / motor max settings will suddenly be drastically different, and in unexpected ways unless you thoroughly understand the maths involved. this is the very real danger I am trying my best to make folks aware of.
[/quote]

You seem to be really good at math. Are you decent at scripting? Would you be willing to build a javascript calculator to help us get the right settings into the VESC based on these attributes you describe?

Also i street test everything i build, so the only danger is to myself as far as this particular things goes.
```

---
## \#187 Posted by: Hummie Posted at: 2016-09-09T15:12:06.269Z Reads: 91

```
Devin I posted ur theory on vedder's site.  Curious if a circuitry bit would blow with a 10000 motor amp limit or will the battery limit supersede
```

---
## \#188 Posted by: Sharkface Posted at: 2016-09-09T17:18:29.137Z Reads: 87

```
O ME ME ME ME ME

I can totally script the heck out of this, I am just gonna need somebody to send up a feature list, or I am going to have to read this thread from top to bottom to see what is going on. We can get this programmed up in Angular and it would be secks.

BTW, this thread, is pretty epic. Thanks for continuing to hash it out boys!
```

---
## \#189 Posted by: devin Posted at: 2016-09-09T18:31:04.115Z Reads: 89

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#190 Posted by: longhairedboy Posted at: 2016-09-09T18:39:05.783Z Reads: 89

```
What's the best/easiest way to determine winding resistance? A multimeter on the phase leads?
```

---
## \#191 Posted by: devin Posted at: 2016-09-09T18:40:30.757Z Reads: 93

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#192 Posted by: Sharkface Posted at: 2016-09-09T21:36:14.127Z Reads: 90

```
epic, thanks bruh!!!!


now go back to hashing this out with @Hummie and @chinzw  lolololol
```

---
## \#193 Posted by: chinzw Posted at: 2016-09-09T21:37:10.086Z Reads: 90

```
hey hey! we came to an agreement! :slight_smile:
```

---
## \#194 Posted by: Sharkface Posted at: 2016-09-09T21:38:40.933Z Reads: 92

```
[quote="chinzw, post:193, topic:8292, full:true"]
hey hey! we came to an agreement!
[/quote]

but but but.... i just got some popcorn after reading you guys going back and forth so productively! lol
```

---
## \#195 Posted by: kampfhahn Posted at: 2016-09-09T22:50:50.913Z Reads: 88

```
I have to admit that i stopped reading this really interesting topic after about 50 posts because it got way to nerdy for me :smile:

So is there a working way to get rid of the unpredictable acceleration bursts in the the area close to max rpm without damaging the components in low rpm / full throttle situations?

My Setup:
- VESC
- 2,2 kW 6355 190 KV (description says 80A max)
- 5000 mAh 10S 20C (100A continuous / 150A 10-second burst)
- Hardware car fuse 40A continuous / 60A 10-second burst
```

---
## \#196 Posted by: Hummie Posted at: 2016-09-10T02:47:11.192Z Reads: 88

```
This is where it gets not nerdy and I say as a rider there's no danger of unpredictable acceleration bursts.  When u drive It often is a not perfectly smooth acceleration curve especially if ur driving a stick!  U get used to it and id rather call it an acceleration profile. 
Getting more torque at low speeds is what this is about I believe.  The possibility to increase the battery amp limit
```

---
## \#197 Posted by: Bender Posted at: 2016-09-10T18:23:49.319Z Reads: 93

```
[quote="longhairedboy, post:179, topic:8292, full:true"]
motor max is exactly how you limit throttle response and shape the acceleration curve. I don't think there's really any debate about that. If you want a smoother launch that doesn't street your ass at 12S or even 10S then you would set it around 40 or 50, and if you want raptor like acceleration then set it to 60 or higher. 

I personally prefer it set around 40-45 on a 15/36 ratio on 83mm wheels because it still climbs hills like a wild animal and doesn't feel like its constantly trying to shoot out from under me. And it still gets ridiculous top end at well over 30mph.
[/quote]

The needle in the haystack! Some useful real world info in this thread.
Thanks @longhairedboy
```

---
## \#198 Posted by: Hummie Posted at: 2016-09-10T21:00:02.199Z Reads: 88

```
With hub motors I've it set to 70 and would like more.  I notice the difference coming from the default 60. If u can set ur battery max to whatever the max u want to pull from the battery that's fine and makes sense but it's possible to set the motor max to 200, just because that's all the bldc program allows.   then I'll bet 200 rocks.  Who's going to do it. ?
```

---
## \#199 Posted by: Ackmaniac Posted at: 2016-09-10T21:14:19.396Z Reads: 98

```
Actually i am developing a new mode to control the power. And for that i needed to calculate how the actual power is calculated. So to answer your question how it would feel like with motor current set to 200 you can see it in the second picture. First picture is for 70 A motor current. 
Both pictures show how how much watt would be produced at 70 % throttle.

**70 A Max Motor Current at 70% throttle**
<img src="/uploads/db1493/original/3X/6/0/60bc8f9091458e33f48794adc084b8d049960f1d.png" width="446" height="500">

**200 A Max Motor Current at 70% throttle**
<img src="/uploads/db1493/original/3X/8/d/8d4a955de1db42cb5cf135feb4512372fcd0c893.png" width="448" height="500">

So you see that you would reach max power at 0,85 Duty Cycle with 70 A Motor current and with 200 A you would reach it already at  0,3 duty cycle. So the board would feel more powerful but you have less control with the throttle.

So to summarize it.
With Max batterie Current you define the max power.
And with Max Motor Current you define how much power will be created by the throttle. This counts the most at low speeds an also defines how much control you have at higher speeds.
```

---
## \#200 Posted by: Ackmaniac Posted at: 2016-09-11T11:10:00.596Z Reads: 103

```
I made a interesting video to show the issues i see with current control.

My settings are:
Motor Max 80 A
Batt max 35 A

So it is 1400 Watts max in theory (35 A * 40 Volts = 1400 Watt).

For the video i added a stoper to my throttle so that the throttle will always give 50%.
As you can see it nearly reaches max power even at 50% throttle position.

[Live recording of Vesc](http://sendvid.com/tgpwi02g)

And here are the calculated numbers
<img src="/uploads/db1493/original/3X/1/a/1a9982b8dea25b1eb872a36717e6aacdca5ec86c.png" width="364" height="500">

So the faster you go the more you loose the ability to fine adjust the power.
```

---
## \#201 Posted by: devin Posted at: 2016-09-11T13:38:51.579Z Reads: 96

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#202 Posted by: Ackmaniac Posted at: 2016-09-11T14:02:36.548Z Reads: 101

```
I created another power control mode which lets you control the Watts by the throttle and not the current that goes to the motor. That means i can control the power in % at any speed.
See this video and have a look at the Watts. It is the same rack and the same throttle setting (50 %from start on) as in the previous video. 
At duty cycles below 0.50 i use curent. otherwise the power would come in too hard. So don't be confused that it doesn't give 700 Watts from start on. 

[Live recording of VESC in costum Watt control mode](http://sendvid.com/5f3zshzx)
Remark. max motor current changed from 80 to 70 to give a softer acceleration.

<img src="/uploads/db1493/original/3X/9/2/92b1a6a28b0cf56b55c8e626ff8cb514ed82143e.png" width="690" height="432">

So you see in the graph the way i power the Motor with this new mode. You see the calculations of curent control and watt control and in the last colum on the right the watts it will use. 
I know it is a bit hard to understand but it feels great. Gives you much more control at higher speeds.
```

---
## \#203 Posted by: devin Posted at: 2016-09-11T14:08:07.628Z Reads: 98

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#204 Posted by: SimosMCmuffin Posted at: 2016-09-11T14:10:08.797Z Reads: 96

```
The motor max limit and battery max limit should be IMO thought in this way:

**Motor max** is used to protect motor from excessive I^2*R losses.

**Battery max** limits the max input electric power, but should not necessarily be set as the max amount the batteries can supply, as this can be a pretty darn high amount of power at higher RPMs, as @Ackmaniac shows in his test table.

http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/1/a/1a9982b8dea25b1eb872a36717e6aacdca5ec86c_1_364x500.png

So even though we operate at constant current, because the AC voltage rises, and the current stays the same the overall power also increases and therefore provides uneven acceleration.

My controller doesn't exhibit this problem as it is speed (duty cycle) controlled compared to the VESC's torque control. All my controller does is ramping up of the duty cycle to the accelerators linear trigger movement. AKA RC car remote, neutral position 0% duty, halfway pulled 50% duty and all the way pulled 100% duty.
```

---
## \#205 Posted by: devin Posted at: 2016-09-11T14:20:28.669Z Reads: 86

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#206 Posted by: Ackmaniac Posted at: 2016-09-11T14:21:15.432Z Reads: 88

```
@devin my resistance is R: 0.01923
SK3 6374 - 192kv
But i don't run it in FOC mode because i have the HV 4.10 which doesn't have the right capacitor. But i get my new 4.12 versions tomorrow where i can test in FOC mode.

And i know that the calculation is not 100% correct. Till a duty cycle of 0.85 it is 5% off from reality (compare the video with the table) and above that the efficiency reduces the power. But i did not want to make it too complicated.
```

---
## \#207 Posted by: devin Posted at: 2016-09-11T14:33:35.553Z Reads: 88

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#208 Posted by: devin Posted at: 2016-09-11T14:50:37.520Z Reads: 89

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#209 Posted by: devin Posted at: 2016-09-11T14:53:19.587Z Reads: 84

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#210 Posted by: Ackmaniac Posted at: 2016-09-11T15:04:08.964Z Reads: 85

```
I set the duty cycle to 3,846% and i come to the same value of 123,07 watts. but my new mode uses at such low duty clycle the current calculation instead of the watt calculation. Otherwise it would mostly give full throttle at low duty cycles which i don't want. At 45 % duty cycle it switches to watt control.
At 100% throttle it would use those 123 watts but at 50% throttle is use the 62 watts of the current calculation.

<img src="/uploads/db1493/original/3X/4/8/48fb49770a259f8c68f9dab18bf7f131c64b1ed1.png" width="690" height="432">
```

---
## \#211 Posted by: makevoid Posted at: 2016-09-11T15:06:59.490Z Reads: 80

```
Very interesting overall. Which app are you using to get the data out of the vesc? Is it open source? Right now I am using an ios app made by gpxlBen but I am searching for an android app so I don't have to carry my ipad with me lol. I would like to implement a log-to-file functionality and maybe add GPS coordinates to it. I stumbled upon an app called Traction that is using cordova and it seems to work but I need to double check if it's getting all the data correctly (I can see only mosfet temp atm). it would be great to have an open source vesc logging solution for android as well .
```

---
## \#212 Posted by: devin Posted at: 2016-09-11T15:11:26.283Z Reads: 81

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#213 Posted by: devin Posted at: 2016-09-11T15:16:36.763Z Reads: 78

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#214 Posted by: Ackmaniac Posted at: 2016-09-11T15:17:55.008Z Reads: 91

```
@devin, i don't want that. I want it smooth and controlable.

@makevoid
That is my own app that i am currently developing. It also provides to setup the number of the Magnets, Wheelsize, and pulleys to calculate the speed. And you can precisely define at which volts you have how many percent of capacity left. And you can switch between 4 different speed modes that you can adjust durcing driving. But i am using a ESP8266 with wifi connection and not a bluetooth module. So it can only support that. 
Of course it would also be adjustable for bluetooth but i wait for the ESP32 which provides both and could do it's own calculations. 

But all of that is something for another topic at another time.
And the mode switches work curently only with my modified firmware.
```

---
## \#215 Posted by: devin Posted at: 2016-09-11T15:19:25.106Z Reads: 93

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#216 Posted by: SimosMCmuffin Posted at: 2016-09-11T15:21:09.595Z Reads: 93

```
[quote="devin, post:215, topic:8292"]
@Ackmaniac one critique of your logging app is the duty cycle % value needs to be multiplied by 100 to be accurate. But overall great job! Very useful...
[/quote]

This can be argued, as the column on the table just says "duty cycle" not "duty cycle %", besides it is just a ratio and can therefore be presented between 0 and 1.
```

---
## \#217 Posted by: Ackmaniac Posted at: 2016-09-11T15:21:34.445Z Reads: 86

```
i showed it the same way as Vedder does in the BLDC-Tool. Only wanted that people can read the graphs as they are used to in BLDC-Tool.
```

---
## \#218 Posted by: devin Posted at: 2016-09-11T15:22:00.144Z Reads: 84

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#219 Posted by: devin Posted at: 2016-09-11T15:24:31.413Z Reads: 87

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#220 Posted by: devin Posted at: 2016-09-11T15:31:49.982Z Reads: 90

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#221 Posted by: devin Posted at: 2016-09-11T15:34:22.152Z Reads: 91

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#222 Posted by: SimosMCmuffin Posted at: 2016-09-11T15:39:01.099Z Reads: 86

```
I understand this and I believe that @Ackmaniac does too, but we don't want to push that high current through the motor at low rpm, so we don't burn our windings , just so we can have that constant power ALL the way through the RPM range, but we would rather start at lower power and then stabilize to a constant power somewhere 30 - 50 % of our RPM range.
```

---
## \#223 Posted by: devin Posted at: 2016-09-11T15:41:19.307Z Reads: 92

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#224 Posted by: devin Posted at: 2016-09-11T15:50:21.423Z Reads: 94

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#225 Posted by: SimosMCmuffin Posted at: 2016-09-11T16:27:32.299Z Reads: 91

```
Well if you want predictability, you should really then run in speed control mode, not power.

Besides, running in constant power mode doesn't give you steady acceleration.
Why?
Because kinetic energy increases in velocity's square. So:
if at power X, it takes you 1 second to accelerate to 10 km/h
Your acceleration is 2,78 m/s^2 on average
but it takes 4 times the energy to achieve 20 km/h
it will take you 3 more seconds to achieve that speed
so then your acceleration is only 0,69 m/s^2 on average

so your acceleration is not steady.
```

---
## \#226 Posted by: devin Posted at: 2016-09-11T16:31:36.712Z Reads: 99

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#227 Posted by: chinzw Posted at: 2016-09-14T16:48:15.567Z Reads: 99

```
I just read this on vedder's forum, from Vedder himself:

[quote]
The power burst that you are feeling is caused by the current measurement problem that I have tried to solve recently. What happens is that at a certain duty cycle (around 80%) one of the shunts will get noise coupled which causes an offset so that too hich current is measured for one commutation cycle and the current backoff kicks in. After this noise disappears the backoff will go back and you feel the kick that you described. With the recent firmwares I have been working on the sample synchronization and some other things to make it better in software, but a hardware solution would be better (by the way, this would not be a problem using three shunts, but using two is more tricky).
[/quote]

So it doesn't seem to be related to motor max/batt max settings.
```

---
## \#228 Posted by: devin Posted at: 2016-09-14T17:03:58.054Z Reads: 106

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#229 Posted by: zmoney Posted at: 2016-09-14T17:23:50.949Z Reads: 109

```
Someone should print every post on this thread and turn it into a book.
```

---
## \#230 Posted by: elkick Posted at: 2016-09-14T19:33:59.038Z Reads: 109

```
That was not on Vedders forum, it was on ES. If you copy/paste my stuff please do it right.

Edit: just saw that ackmaniac copied my answer to him into  Vedders forum and you copied it again from there. We are living in a copy/paste world. 😂
```

---
## \#231 Posted by: Ackmaniac Posted at: 2016-09-14T19:56:05.392Z Reads: 113

```
I am a programmer. So copy paste is 90% of my job. Sory for that.
```

---
## \#232 Posted by: elkick Posted at: 2016-09-14T20:06:26.612Z Reads: 119

```
No worries, I'm a programmer too - just another generation. :slight_smile:
```

---
## \#233 Posted by: chinzw Posted at: 2016-09-14T20:39:51.082Z Reads: 120

```
Yep!

10CHARS (THIS ONES I DID NOT COPY PASTE)
```

---
## \#234 Posted by: PDXroses Posted at: 2017-07-08T23:44:50.599Z Reads: 77

```
LHB, would you mind helping me uncover this mystery?

My board experiences an acceleration burst at ~13 to 15mph on occasion.  It's dangerous because doesn't happen all the time, just half the time at that speed range.

My config is:
10S3p, Dual Vesc.  Two 6533 motors.
Motor max 60A.  Min -30A.
Bat max 25A.  Min -20A.
PPM Current, no reverse with brake.
Soft RPM limit start 30K.  End 40K.
Starup boost 0.05

Thanks for any info you can provide!
```

---
