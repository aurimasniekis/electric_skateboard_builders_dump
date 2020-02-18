# VESC Help Please! Motor Judder

### Replies: 139 Views: 3973

## \#1 Posted by: darkkevind Posted at: 2017-05-16T14:31:49.909Z Reads: 218

```
Hi, can anyone tell me what's wrong with the setup of this VESC please?

When it's on the bench it all seems to work OK, but as soon as there's a 'load' on the motor, it just judders. I'm sure it's a setting but I just don't know which one(s).

Setup:
* 2 x 3s 11.1v 25c Li-Po
* Turnigy SK3 5065 236kv
* VESC 4.12 (2.18 Firmware)
* Mini Remote.

https://www.youtube.com/watch?v=s7YP6NxCD-M
```

---
## \#2 Posted by: darkkevind Posted at: 2017-05-16T14:32:27.380Z Reads: 204

```
<img src="/uploads/db1493/original/3X/4/e/4ec0480af1907f4af23e77aa46ae422a32335a79.PNG" width="690" height="405">
```

---
## \#3 Posted by: Namasaki Posted at: 2017-05-16T14:44:24.460Z Reads: 196

```
Try turning you motor max up to 80a
And battery max to 50a
```

---
## \#4 Posted by: darkkevind Posted at: 2017-05-16T14:53:42.688Z Reads: 199

```
Thanks for the advice. Tried that just now but it's still juddering..?
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-16T15:31:18.277Z Reads: 197

```
non sensored motors will stutter when starting up with load from dead stop. You'll have to give it a kick start so it starts up smoother. You can also play around with increasing start up boost and min erpm to help with this.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-16T15:36:59.078Z Reads: 194

```
Can you give more detail on those settings options
```

---
## \#7 Posted by: Jinra Posted at: 2017-05-16T15:40:19.453Z Reads: 195

```
start up boost is the minimum duty cycle when accelerating.  Min erpm is as it states, the minimum erpm your motor will run at lowest duty cycle
```

---
## \#8 Posted by: darkkevind Posted at: 2017-05-16T15:43:37.547Z Reads: 190

```
Can I just be a complete noob here but what does ERPM stand for? I'm assuming 'something' revs per minute?

I'll try playing with those settings. I've tried kicking off as well but that doesn't seem to help...
```

---
## \#9 Posted by: Jinra Posted at: 2017-05-16T15:46:03.740Z Reads: 187

```
electronic RPM. It's the revolutions of pole pairs of the magnets in the motor. Most 50-63mm motors have 7 pole pairs, which means 1 mechanical RPM = 7 eRPM.

You're saying you kick off with your foot on your board and accelerate and it doesnt do anything? You could try adjusting the battery cutoff start, it seems kind of high. You can set it to way below your actual cutoff while you're testing.
```

---
## \#10 Posted by: goldenHusky Posted at: 2017-05-16T15:46:18.995Z Reads: 182

```
[quote="darkkevind, post:8, topic:23208"]
Can I just be a complete noob here but what does ERPM stand for?
[/quote]

electrical revs per minutes, it's mechanical rpm multiplied with the number of pole pairs
```

---
## \#11 Posted by: darkkevind Posted at: 2017-05-16T15:48:01.526Z Reads: 177

```
Thanks for the explanation!

I'll try fiddling. What should the cutoff start/end be during normal use though?
```

---
## \#12 Posted by: Jinra Posted at: 2017-05-16T15:49:16.609Z Reads: 174

```
Depends on your battery, Lipos tend to have higher cutoffs than cylinder cells. I'd probably go with 21~ for you, but it'd be best if you can find a data sheet for your particular pack.
```

---
## \#13 Posted by: darkkevind Posted at: 2017-05-16T15:56:13.913Z Reads: 171

```
OK, I think we're making progress. 

If I kick of now it's working but 'making progress' is slow, much slower than with my old boat ESC anyway, which is good in a way but can I increase it slightly?

Also, the brake doesn't really do much, makes a noise but it's not actually braking me... does it matter how fast I'm going using the brakes?

Any help on the brakes would be very much appreciated? Not sure if this is the right setting but "Max brake current at dir change" is set to 10.
```

---
## \#14 Posted by: Blasto Posted at: 2017-05-16T15:57:55.218Z Reads: 167

```
Just so we can follow your developpement, can you repost your new settings.

Batt min (regen) is your brakes
```

---
## \#15 Posted by: Jinra Posted at: 2017-05-16T15:58:58.820Z Reads: 165

```
You're pretty conservative with your current values (which is good!) but you can afford to up them a bit. Try 60/-60 for motor max/min. Up your battery max higher to about 40A~ as well.
```

---
## \#16 Posted by: darkkevind Posted at: 2017-05-16T16:00:52.137Z Reads: 164

```
Here's my new settings...
<img src="/uploads/db1493/original/3X/2/5/258d6966819bc64b3d11e5708c858f18bd9e00c2.PNG" width="690" height="406">
```

---
## \#17 Posted by: darkkevind Posted at: 2017-05-16T16:02:07.385Z Reads: 155

```
I just loaded the defaults for 2.18 (standard) and the took it from there.

I upped my Motor max/min on @Namasaki 's advice
```

---
## \#18 Posted by: darkkevind Posted at: 2017-05-16T16:03:16.612Z Reads: 156

```
So to make them a bit more aggressive I'd up that value? More minus or more towards a positive figure?
```

---
## \#19 Posted by: Blasto Posted at: 2017-05-16T16:05:07.880Z Reads: 155

```
try what @Jinra is suggesting

motor max: 60
motor min: -60
batt max: 40
batt min: -20
```

---
## \#20 Posted by: Jinra Posted at: 2017-05-16T16:05:10.283Z Reads: 159

```
The lower the stronger (-60 is stronger than -40). I keep my max/min values exact opposites (eg. 60/-60) for the same amount of force when accelerating and braking.
```

---
## \#21 Posted by: darkkevind Posted at: 2017-05-16T16:24:58.127Z Reads: 154

```
OK, so I've taken the settings to this:

Motor max/min 60/-60
Batt max/min 40/-50

I tried the suggested settings and the brakes were still weak. With this setting they seem better but cut off when I get to a certain speed. Would that be something to do with "Max ERPM at full brake"?

Am I right in deducing that the faster you're going the more vigorous the braking power?
```

---
## \#22 Posted by: Blasto Posted at: 2017-05-16T16:28:09.273Z Reads: 151

```
don't want to be captain obvious here, are you hitting "write configuration" when you do a change?

also, do you see the full range of your throttle when you go in app configuration-> ppm -> tick display
```

---
## \#23 Posted by: laurnts Posted at: 2017-05-16T16:28:55.076Z Reads: 147

```
I dont think there is a problem within the bat min max and motor min max. Try to redo your BLDC motor detection. You might also be off with wrong firmware - hardware issue.
```

---
## \#24 Posted by: darkkevind Posted at: 2017-05-16T16:30:52.037Z Reads: 145

```
I'm definitely writing the configuration. Most of the time I do a re-boot for good measure too.

On full throttle it's at 91%, full brake is 4% - Sounds wrong to me but maybe that's normal?
```

---
## \#25 Posted by: darkkevind Posted at: 2017-05-16T16:31:44.598Z Reads: 144

```
I've not done any 'detection' other than what it does when it connects. What should I be doing for that please?
```

---
## \#26 Posted by: Blasto Posted at: 2017-05-16T16:34:06.035Z Reads: 138

```
[quote="darkkevind, post:24, topic:23208"]
On full throttle it's at 91%, full brake is 4% - Sounds wrong to me but maybe that's normal?
[/quote]

close enough, should be ok (full throttle could be higher).

 [quote="darkkevind, post:25, topic:23208, full:true"]
I've not done any 'detection' other than what it does when it connects. What should I be doing for that please?
[/quote]

ah forgot my other captain obvious question... yes do a motor detection.

motor configuration -> BLDC -> click start detection -> click apply -> click write config
```

---
## \#27 Posted by: darkkevind Posted at: 2017-05-16T16:35:47.665Z Reads: 130

```
Thanks, how would I get full throttle higher?

OK, what do I need in the Current/minERPM/Low Duty because each time it says detection failed...
```

---
## \#28 Posted by: Blasto Posted at: 2017-05-16T16:37:22.486Z Reads: 132

```
[quote="darkkevind, post:27, topic:23208"]
OK, what do I need in the Current/minERPM/Low Duty because each time it says detection failed...
[/quote]

are your batteries fully charged?
if yes, set your current to 10A (in the detect parameters)
```

---
## \#29 Posted by: darkkevind Posted at: 2017-05-16T16:37:52.622Z Reads: 132

```
Yep, fully charged. Just leave the other settings as is?
```

---
## \#30 Posted by: Blasto Posted at: 2017-05-16T16:39:24.870Z Reads: 128

```
yes the current is the constant current applied, min ERPM is the threshold it need to obtain the low duty is the duty cycle at the end of the detection sequence
```

---
## \#31 Posted by: darkkevind Posted at: 2017-05-16T16:40:16.029Z Reads: 124

```
OK thank you. Done. I'll check it out.
```

---
## \#32 Posted by: Blasto Posted at: 2017-05-16T16:40:40.049Z Reads: 124

```
[quote="darkkevind, post:31, topic:23208, full:true"]
OK thank you. Done. I'll check it out.
[/quote]

it passed the motor detection?
```

---
## \#33 Posted by: darkkevind Posted at: 2017-05-16T16:42:41.309Z Reads: 122

```
Yeah!
<img src="/uploads/db1493/original/3X/b/f/bf8662a49ba70351bf6a61c97276b754ceb28c98.PNG" width="443" height="133">
```

---
## \#34 Posted by: darkkevind Posted at: 2017-05-16T16:43:32.587Z Reads: 122

```
Brakes still aren't great, I wouldn't be confident in them out on the road... Any other setting I should look at?
```

---
## \#35 Posted by: Blasto Posted at: 2017-05-16T16:47:09.705Z Reads: 124

```
motor max: 80
motor min: -80
batt max: 40
batt min: -20

try this?  batt min -20 is pretty much the max you can go with your setup without damaging your cells. (This is debatable, tbh i dont know your cell capacity, this is assuming they are 10 000mah)

If your brakes are still full of weak sauce, i would revise your setup, double check all your connections and such
```

---
## \#36 Posted by: Namasaki Posted at: 2017-05-16T16:50:32.417Z Reads: 125

```
I used to run my motor max at 60a. 
Then I bumped it up to 80a and got a noticeable increase in low speed torque and my motors still run relatively cool. 
That's why I suggested 80a for motor max.
```

---
## \#37 Posted by: darkkevind Posted at: 2017-05-16T16:59:55.806Z Reads: 125

```
It's two 5000mah in series so I think your assumption is correct...

Thanks, I'll try that.
```

---
## \#38 Posted by: darkkevind Posted at: 2017-05-16T17:36:34.564Z Reads: 128

```
That seems a bit better now guys, thank you for your help. I'll try it outside in real use in a little while once I've got the baby to sleep! :unamused:
<img src="/uploads/db1493/original/3X/e/d/ed8d306bea62456accbbee2a052b7621d21aeb7e.PNG" width="690" height="406">
```

---
## \#39 Posted by: Namasaki Posted at: 2017-05-16T17:38:02.238Z Reads: 123

```
With a single drive using a 5065 236kv motor,
Your not gonna have a lot of torque and therefore not a lot a braking power. 
A more suitable choice for a single drive would be a 6374 motor.
```

---
## \#40 Posted by: darkkevind Posted at: 2017-05-16T19:02:51.384Z Reads: 123

```
With all due respect, with my last ESC, a 120A boat ESC I had great torque, could start from a stand-still on a slight hill, no problem, and the brakes were quite good . . . when they worked!
Problem was, I could never tell when they'd actually work so that's why I wanted to get a VESC, also the speed gain was a bit harsh, sometimes if it took me by surprise I could have easily tumbled off the back of the board if I wasn't as quick to react.

I'm sure I just need to play around with some more settings, to get it as good as my old ESC but with less punch and more reliable brakes.

To be fair, I've only tried these settings inside, within a reasonable run, front of my house to the back, so I think outside they'd probably behave a bit differently...
```

---
## \#41 Posted by: monkey32 Posted at: 2017-05-16T19:26:38.025Z Reads: 119

```
Ahem.....I don't know if you heard but it's no longer the VESC......it's now called the FUKYEA
```

---
## \#42 Posted by: monkey32 Posted at: 2017-05-16T19:27:01.860Z Reads: 119

```
Or alternatively SEXMACHINE
```

---
## \#43 Posted by: laurnts Posted at: 2017-05-17T08:50:36.541Z Reads: 114

```
Just watch a video tutorial from a youtube how to configure VESC. VESC is if not the same more powerful than then 100A ESC. I have that too. I'm pretty sure you don't have a correct settings (or play around with the settings too much). I Prefer you reset to default setting and do a motor detection and re configure your ppm - current control. It should be more than good.
```

---
## \#44 Posted by: Namasaki Posted at: 2017-05-17T12:30:28.324Z Reads: 108

```
Agree with @laurnts
My Vescs out perform the 12s 120a esc's that I used before with minimal adjustment.
```

---
## \#45 Posted by: zblad Posted at: 2017-05-17T13:01:57.345Z Reads: 112

```
There is a setting on the VESC for dual motors over can make sure those are unchecked I believe there are two spots.  One is under app configuration --> PPM --> multiple ESCs over can. I was having a similar issue with my single drive mountain board.
```

---
## \#46 Posted by: darkkevind Posted at: 2017-05-17T13:07:42.864Z Reads: 109

```
I've used the suggested settings and played around with a few other settings and it seems to be much better now.

Thank you guys.

There's little judder, if i push off (which I pretty much do all the time anyway), then there's no judder at all and the brakes are a lot better.
```

---
## \#47 Posted by: darkkevind Posted at: 2017-05-18T14:58:38.510Z Reads: 101

```
OK! Something's definitely not quite right....

The board seems SO under-powered compared to how it was with the 120A boat ESC! It's struggling to get up any kind of incline, almost struggling to make any sort of progress too, even on a flat. At full throttle it just kind of lists slowly up  to a - slow - speed.

Braking is a bit better, but in all honesty, I'd expect under certain circumstances (maybe in the wet) that the wheel might even skid with the braking force, but with the braking force I have, I'd be lucky to skid it hitting a patch of oil!

I just don't get it. Do I have a dud VESC!?

At this point, and I know it sounds crazy, but I'd love to just get an ESC like my boat one but with much better brakes. I'm quite disappointed in this VESC :frowning:
```

---
## \#48 Posted by: Namasaki Posted at: 2017-05-18T15:11:33.019Z Reads: 99

```
You could try upping your batt max to 50 or 60 amps
Other than that I still think that you need a bigger motor for single drive. 
Something like a Tacon big foot 245kv
```

---
## \#49 Posted by: darkkevind Posted at: 2017-05-18T16:19:33.817Z Reads: 97

```
I'll try that. But how come it was much more powerful with my old ESC?
```

---
## \#50 Posted by: Namasaki Posted at: 2017-05-18T17:46:06.225Z Reads: 95

```
Same Motor and batteries?
```

---
## \#51 Posted by: Jinra Posted at: 2017-05-18T17:47:21.937Z Reads: 95

```
Whatever your old ESC was rated for set your Motor max to match. (If you had a 120A ESC use 120 as motor max). That should help with responsiveness.
```

---
## \#52 Posted by: Namasaki Posted at: 2017-05-18T17:52:17.263Z Reads: 92

```
That's true, as @Jinra said. 
The more you turn up the motor max, the more torque power you get.  
As long as your motor doesn't overheat. 
You can also turn your. Batt max up. 
40a is a bit low. 
Your battery can handle 50 or 60 easily.
```

---
## \#53 Posted by: darkkevind Posted at: 2017-05-18T19:06:02.661Z Reads: 88

```
Yes, same everything, just different ESC.

OK guys, thanks, I'll try that when the rain lets up! :smile:
```

---
## \#54 Posted by: darkkevind Posted at: 2017-05-18T19:32:41.156Z Reads: 94

```
@Namasaki @Jinra @zblad @laurnts

Quick question for you to which I think I know the answer...

Motor min (regen) & Batt min (regen)

Am I right in thinking that the less value you put here the more powerful the brakes will be? So... -80 is more harsh/powerful than -40 ?
```

---
## \#55 Posted by: Jinra Posted at: 2017-05-18T19:35:17.278Z Reads: 93

```
that is correct.
```

---
## \#56 Posted by: Namasaki Posted at: 2017-05-18T19:48:23.946Z Reads: 96

```
Ok, so it's probably settings. 
One difference between hobby Esc's and the Vesc is that hobby ESC's operate in Duty Cycle mode only. 
And Vesc can operate in either Duty Cycle or Current Control modes. 

In Duty Cycle,  Voltage is controlled by the throttle and current is determined by load.  

In Current Control, Voltage stays constant and current is controlled by the throttle. 

Current Control offers smoother operation. 
Duty Cycle control tends to be more snappy and harder to control. Especially at higher voltage. 
I used to run 12s with dual 120a hobby ESC's and dual 145kv hub motors and it was difficult to control. 

If adjusting your current parameters doesn't achieve the results your looking for,  you could try running in Duty Cycle Mode. 
Or you could try downloading @Ackmaniac modified firmware and try running in wattage mode.
```

---
## \#57 Posted by: darkkevind Posted at: 2017-05-19T13:33:43.753Z Reads: 90

```
Thank you. I've upped the current settings and am just waiting for it to stop raining to go test them.

If that fails, I may try your suggestion, however, I do like the fact that the VESC isn't 'snappy', at least it means it's less likely to throw me of my board like the last ESC did a couple of times! lol
```

---
## \#58 Posted by: Namasaki Posted at: 2017-05-19T14:24:37.896Z Reads: 92

```
I also noticed that the Vesc in current mode has more gradual and smooth acceleration than Duty Cycle ESC's. I also found that I attained higher top speed with the Vesc and I believe it's because the Vesc is more efficient. 
I read up a little on the Watt control version of Vesc firmware and what I got is that it is even more gradual than the standard current control version. 
So you might want to stay with the standard version. 
I do know from experience that cranking up the motor max current will give you more acceleration power.
```

---
## \#59 Posted by: darkkevind Posted at: 2017-05-19T14:29:05.754Z Reads: 96

```
OK, something's definitely up!

Here's me testing the VESC just now. I kick off both times, both times it takes an age to get up to any sort of speed and the speed it get's up to is about 1/3 of what it was previously capable of.

Both times I brake with FULL brakes and it barely slows me down any....

https://youtu.be/Ky-7mB5Lnlg

Here are my settings...
<img src="/uploads/db1493/original/3X/d/e/decef7b549d032afbb74cdadbf3da774ea4f9f58.PNG" width="690" height="402"><img src="/uploads/db1493/original/3X/2/4/24f69559e0efd37e39e840736629ed2a97f366a4.PNG" width="690" height="402"><img src="/uploads/db1493/original/3X/c/d/cdc23edd9c62a710785314376a7bef10042ac2cb.PNG" width="689" height="402">
```

---
## \#60 Posted by: Namasaki Posted at: 2017-05-19T15:33:34.919Z Reads: 92

```
Please post a screenshot of the page under the Advanced tab

That does look pretty slow.
```

---
## \#61 Posted by: darkkevind Posted at: 2017-05-19T15:46:17.775Z Reads: 97

```
Here you go...
<img src="/uploads/db1493/original/3X/8/6/86e2965fb1a09a16d908a9c6658719c71db9e3c6.PNG" width="690" height="406">
```

---
## \#62 Posted by: Namasaki Posted at: 2017-05-19T17:42:19.826Z Reads: 95

```
I'm gonna compare your settings to mine when I get home from work.
```

---
## \#63 Posted by: Namasaki Posted at: 2017-05-19T20:56:02.199Z Reads: 98

```
Did you do your motor detection with nothing on the motor? I mean not even a pulley on the shaft? and did you apply the results and write configuration?

And did you do the controller setup pulse width setup on the app config page / ppm tab?

Here is a good tutorial for the pulse width setup:
https://youtu.be/OtuofrQr3F8
```

---
## \#64 Posted by: yaca Posted at: 2017-05-19T21:28:39.161Z Reads: 90

```
What is your gearing ratio? Your batteries are in series for sure? For 6s your battery max cutoff start 22,5 V is maybe too high. Set 21V for max and 20V for battery cut off end.
```

---
## \#65 Posted by: darkkevind Posted at: 2017-05-20T11:09:47.776Z Reads: 90

```
No, i did the motor detection etc. with everything connected, pulley, chain, sprocket etc. Are you supposed to do it with nothing on it then?

I did the controller setup, my 'rest' is close to 50% but it all seems to be correct. I already used this video for that :slight_smile:
```

---
## \#66 Posted by: darkkevind Posted at: 2017-05-20T11:11:08.229Z Reads: 93

```
This is my gearing ratio. 10T / 30T
<img src="/uploads/db1493/original/3X/1/c/1c730a584b2989dd1a7584deb2c4dcf70f7df67e.jpg" width="690" height="388">
```

---
## \#67 Posted by: darkkevind Posted at: 2017-05-20T11:11:50.486Z Reads: 91

```
Like i said, it was working great with my old boat ESC, except no brakes! :frowning:
```

---
## \#68 Posted by: Namasaki Posted at: 2017-05-20T13:03:12.082Z Reads: 91

```
You need to redo your motor detection with everything off the motor.
```

---
## \#69 Posted by: darkkevind Posted at: 2017-05-20T20:12:03.461Z Reads: 91

```
OK, I'll do that...
```

---
## \#70 Posted by: darkkevind Posted at: 2017-05-24T10:46:19.564Z Reads: 90

```
Hey guys, I'm back again!

I've re-done my motor detection and changed around the limits. I've taken it up to like 115A for the motor and changed couple of other settings... that seems to have made a bit of a difference. The acceleration is better, and top end is better, however, I'm finding that when I'm full throttle (and it's accelerating slowly but ... nicely), sometimes it will cut out and I just coast... no brakes, no more accelerator, until a few seconds, maybe 10 have passed, then I get control back again... what could that be? Is it getting too hot and it's too much for the mosfets?

After that test I decided to mess around a bit more and I've enabled FOC!!! I just have to say, FOC is amazing! Things got a bit more smooth, MUCH more quiet, a bit more punch in the acceleration and slightly better brakes, however, I'm still getting this cutting out issue? Any ideas?
```

---
## \#71 Posted by: Namasaki Posted at: 2017-05-24T12:31:47.938Z Reads: 85

```
I'm guessing that something is hitting a protection parameter. 
Maybe voltage sag causing low voltage trigger
Or temp trigger.
Your pulling high amps at 6s
```

---
## \#72 Posted by: darkkevind Posted at: 2017-05-24T13:00:47.151Z Reads: 80

```
Hmm ok. Do you suggest any solution?

I'm out on it right now and on some, even just slight inclines it just can't cope! Never had that problem with my old ESC, could drag my fat arse up ALL the inclines in my local park...
```

---
## \#73 Posted by: TarzanHBK Posted at: 2017-05-24T13:36:20.340Z Reads: 77

```
If you´re already going with a vesc, throw in another 3s battery to go to 9s. No problem with your system and will give you a nice boost :slight_smile:
```

---
## \#74 Posted by: darkkevind Posted at: 2017-05-24T13:39:38.645Z Reads: 76

```
Yeah, I don't mind doing that, although I'll have to get a new enclosure etc. but I just don't know why the VESC seems to under-performing a cheap 120A boat ESC? I'm a little disappointed if I'm honest.

The last ESC, the boat one, even got me up this really steep hill near where I live. Although it was only for a short burst, just to the car, it seemed to handle it no problem. With this VESC it wouldn't even get me up the slight hill leading up to this steep hill :frowning:

I really think it must be a dud.
```

---
## \#75 Posted by: TarzanHBK Posted at: 2017-05-24T13:52:54.165Z Reads: 76

```
Calculation:
120A at 6s = 120A x 6 x 3,7V = 2664W max output of your ESC
50A at 6s = 50A x 6 x 3,7V = 1110W max output of your Vesc

Like I said before, Vesc at 6s is not a good idea in my opinion.
You can use it if you´re only cruising slow on flats, but other than that it heats up too fast and I´d go with a ESC at 6s.

9s will be an other league
```

---
## \#76 Posted by: darkkevind Posted at: 2017-05-24T13:58:35.877Z Reads: 78

```
Oh really? It really makes that much difference? I had no idea...

OK, I'll try adding another 3s pack, I do have one somewhere, just need to make up a connector cable... (or buy one)
```

---
## \#77 Posted by: darkkevind Posted at: 2017-05-24T14:00:31.258Z Reads: 78

```
I've also just looked again at the spec of the motor and it's max loading is 60A and I have the VESC set to 115A!!!! :frowning:
Ooops!

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5065-236kv-brushless-outrunner-motor.html?___store=en_us
```

---
## \#78 Posted by: Hummie Posted at: 2017-05-24T14:01:23.218Z Reads: 76

```
As Tarzan says, but even still it's surprising as it sounds like you hit an over-temp limit so soon on 6s.

You can forget what's presented as the max amp loading number of the motor and just watch it's temp and that's the real limit
```

---
## \#79 Posted by: TarzanHBK Posted at: 2017-05-24T14:05:03.827Z Reads: 76

```
your combination is just unlucky. Small motor + 6s and Vesc is really heating up everything.
Go with 9s or even 12s if you want. Next upgrade should be a 6374 to keep you going ;)
```

---
## \#80 Posted by: darkkevind Posted at: 2017-05-24T14:06:59.532Z Reads: 84

```
Fair enough. But how come that cheaper ESC performed so well though? Honestly, although I had to be really careful with putting the power down, it was fast and really strong in terms of torque. With that ESC it felt like this smaller motor was more than enough for my needs...
```

---
## \#81 Posted by: darkkevind Posted at: 2017-05-24T14:10:25.825Z Reads: 84

```
I was just messing around with the VESC looking at the real-time data. I gave the wheel some resistance and full throttled it. A fault code came up ABS_OVER_CURRENT. What's ABS?
```

---
## \#82 Posted by: Hummie Posted at: 2017-05-24T14:10:28.198Z Reads: 85

```
If u go 12s with that high kv motor u need to set the erpm limit

The 120 amp esc u had before was giving more amps simply.  U can up the amps like u did but only so far on the vesc. Voltage u have a lot of room though to increase and get that power 
U could try increasing motor amps to 120. That's supposedly the programmed limit anyway.  But the vesc is a voltage hog not amperage and sounds like you'll hit over temp again with amps being hot
```

---
## \#83 Posted by: Norco Posted at: 2017-05-24T14:10:49.245Z Reads: 85

```
How hot did your esc get? I am surprised you haven't burnt up a motor. 

10s on a vesc has been amazing for shifting my chunk!
```

---
## \#84 Posted by: darkkevind Posted at: 2017-05-24T14:12:10.967Z Reads: 79

```
I'm not sure. The real-time data says it's sitting happy at 34 deg, even when I put some resistance on the wheel and put it through it's paces....
```

---
## \#85 Posted by: Norco Posted at: 2017-05-24T14:15:03.190Z Reads: 80

```
very odd. I have no esc to compare too but I was amazed by the torque and top speed I was getting out of mine (6374 though). Doubt I will need a dual drive as there aren't any hills around here at all.
```

---
## \#86 Posted by: Hummie Posted at: 2017-05-24T14:17:05.571Z Reads: 84

```
If u have data can u post it?
```

---
## \#87 Posted by: darkkevind Posted at: 2017-05-24T14:17:52.031Z Reads: 86

```
Sure! How do you save the data though?
```

---
## \#88 Posted by: Namasaki Posted at: 2017-05-24T14:20:04.241Z Reads: 86

```
What brand of Vesc did you say you are using ?
```

---
## \#89 Posted by: darkkevind Posted at: 2017-05-24T14:21:49.738Z Reads: 84

```
I honestly have no idea! :confused:

I got it from Mikee who, when I asked where he got it replied: Freerchobby

I have no idea who or what that is! lol
```

---
## \#90 Posted by: Hummie Posted at: 2017-05-24T14:28:37.906Z Reads: 82

```
Hate to say but it's a suspect vesc.  Do they even say it's ok for foc?
```

---
## \#91 Posted by: Namasaki Posted at: 2017-05-24T14:30:11.319Z Reads: 82

```
Maybe if you could post some close up pics,
Someone could help identify it. 
It could be that you got an inferior rendition.
```

---
## \#92 Posted by: darkkevind Posted at: 2017-05-24T14:35:40.130Z Reads: 82

```
I dunno! :confused:

It was pretty much the same in BLDC mode though...
```

---
## \#93 Posted by: darkkevind Posted at: 2017-05-24T14:48:40.263Z Reads: 81

```
<img src="/uploads/db1493/original/3X/4/8/48fd8b06fec3f6d0effdc26ff52210791ea859a6.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/7/6/7698b037f2cb03449a0bde0f1e76ea0d0945411b.jpg" width="690" height="388">
```

---
## \#94 Posted by: darkkevind Posted at: 2017-05-24T14:49:09.773Z Reads: 82

```
<img src="/uploads/db1493/original/3X/2/a/2a3f80e2c23faf0f508aa623de4a2833c95db948.jpg" width="690" height="388">
```

---
## \#95 Posted by: Blasto Posted at: 2017-05-24T15:06:07.258Z Reads: 80

```
That vesc is missing a bunch of capacitors... mainly the big 15uf 100v
```

---
## \#96 Posted by: darkkevind Posted at: 2017-05-24T15:08:41.933Z Reads: 84

```
Do you mean these?

<img src="/uploads/db1493/original/3X/0/c/0c9aa9011bff0ac5c879cc8aebd53c0022f4a832.jpg" width="690" height="388">
```

---
## \#97 Posted by: Jinra Posted at: 2017-05-24T15:11:41.849Z Reads: 84

```
No, there are some pads on the PCB missing caps.
```

---
## \#98 Posted by: darkkevind Posted at: 2017-05-24T15:14:22.101Z Reads: 84

```
Oh! :frowning:
```

---
## \#99 Posted by: darkkevind Posted at: 2017-05-24T15:22:32.009Z Reads: 91

```
From here?
<img src="/uploads/db1493/original/3X/5/e/5ec7c6afc82faf8bc07995910ad657836ab449c6.PNG" width="690" height="381">
```

---
## \#100 Posted by: darkkevind Posted at: 2017-05-24T18:06:41.812Z Reads: 90

```
Would that contribute towards the issue I'm having then?
```

---
## \#101 Posted by: Namasaki Posted at: 2017-05-24T18:13:48.847Z Reads: 87

```
I'm no electronics engineer but my quess would be yes
```

---
## \#102 Posted by: Namasaki Posted at: 2017-05-24T18:29:33.651Z Reads: 86

```
Think of a capacitor as type of power booster. 
It stores electrons like a battery and then releases them in a burst of power.
And though I'm not an engineer, common sense tells me that omitting these components is likely to have a negative impact on performance.
```

---
## \#103 Posted by: darkkevind Posted at: 2017-05-24T18:52:11.684Z Reads: 84

```
When you explain it like that, indeed it seems it will!

So, have I been sold a dud VESC? Is there anything I can do about it? I'm not electrical engineer either but I'm a dab hand with a soldering iron! Could I just buy the component and solder it on?
```

---
## \#104 Posted by: Hummie Posted at: 2017-05-24T19:38:52.840Z Reads: 79

```
Cheap vescs come like that as they omit the more expensive parts and will sometimes sell it saying u can't use foc
```

---
## \#105 Posted by: Namasaki Posted at: 2017-05-24T20:10:02.955Z Reads: 78

```
[quote="darkkevind, post:103, topic:23208"]
So, have I been sold a dud VESC?
[/quote]

I wouldn't say it's a dud. Just inferior. 
If you can't return it then maybe it would be worth adding the missing parts. 
And you might do well to send it to someone like @JohnnyMeduse for proper inspection and modification.
```

---
## \#106 Posted by: Bataleon Posted at: 2017-05-24T20:41:21.813Z Reads: 75

```
I had a similar issue to yours and it turned out the low voltage cutoff was set too high. This prevented the VESC from delivering full power as the battery's voltage sagged during acceleration. Try lowering your low voltage cutoff temporarily and see if it helps.

Also, what wheels are those? Looks like they handle rough asphalt super well.
```

---
## \#107 Posted by: yaca Posted at: 2017-05-24T21:05:57.782Z Reads: 75

```
I already suggested to lower the battery voltage cut off. Did you try that? On your last screenshot you had 3,75V per cell cut off start and 3,5V per cell cut off end. That's maybe to high.
```

---
## \#108 Posted by: darkkevind Posted at: 2017-05-24T21:26:08.957Z Reads: 78

```
I did lower it a couple of volts, not much though, I'll try lowering it more.

@Bataleon they're 100 or 110mm Yak scooter wheels. They do handle all sorts of dogey terrain ever so well! :slight_smile:
```

---
## \#109 Posted by: darkkevind Posted at: 2017-05-24T21:27:09.649Z Reads: 76

```
Thanks, does anyone know what missing parts I need? Where I can get them from?
Would it be just a normal electrical component supplier?
```

---
## \#110 Posted by: Namasaki Posted at: 2017-05-24T21:50:15.228Z Reads: 80

```
Mouser electronics would be the likely source but I don't know what parts are missing.

Honestly, if I were in this situation, I would send it to @JohnnyMeduse because he's an expert and should be able to tell what parts are missing and have the tools and skills to fix it proper.

If you don't have the right tools and or skills, you could wind up with a mess on your hands and a vesc that won't even turn on.
```

---
## \#111 Posted by: darkkevind Posted at: 2017-05-24T21:57:07.341Z Reads: 77

```
Thanks mate, I've messaged him.
```

---
## \#112 Posted by: racidon Posted at: 2017-05-25T02:34:49.933Z Reads: 77

```
Just to add to this darkkevind, ABS OVER CURRENT is usually a bad connection to the motor somewhere, it can be a loose plug, dodgy soldering or cut wire. Or even burnt out wire. It's that it's having to push too much power to get where you're trying with your remote.
```

---
## \#113 Posted by: TSG_AU Posted at: 2017-05-25T05:43:54.194Z Reads: 75

```
Hey I actually have a setup very similar to yours:

Turnigy 5065 236kv
6S, 5200mAh, 10C
19:34 gearing, 83mm wheels

Works very well, I can go up to ~25mph and go up fairly decent slopes

I'm using FOC as well, but I've got my startup boost set to 0.15, and the board pulls away from standstill without a problem.

Also it shouldn't be a problem since you've got a 4.12 VESC, but with all the missing caps, I hope C26 isn't also missing, as that has been known to cause blown up DRV8302s when running FOC. It should be next to C18 under the wire here

<img src="/uploads/db1493/original/3X/9/9/99ad035f06728df136d86f2363a2918f4916a6dc.jpg" width="690" height="388">
```

---
## \#114 Posted by: darkkevind Posted at: 2017-05-25T14:41:35.779Z Reads: 69

```
Thank you @racidon, I'll check that out to make sure all connections are ok and nothing's burnt out!
```

---
## \#115 Posted by: darkkevind Posted at: 2017-05-25T14:44:14.998Z Reads: 73

```
Thanks @TSG_AU, I'll check that out when I get home to make sure I have it.

I'm a bit annoyed because if i'd have known this was an inferior VESC I'd never have bought it. To be fair it was cheap but with the costs I'm going to have to pay to rectify it, I may as well have got a new more expensive one. :frowning:
```

---
## \#116 Posted by: darkkevind Posted at: 2017-05-25T17:26:17.305Z Reads: 70

```
There's a tiny component there which I can see, but I think the C26 spot is empty! :frowning:

<img src="/uploads/db1493/original/3X/e/3/e323ce68102ea95d40707e350d7a2797fa76b4c0.jpg" width="690" height="388">
```

---
## \#117 Posted by: TSG_AU Posted at: 2017-05-25T18:18:59.751Z Reads: 71

```
Man they really skimped on this VESC

Where are you at, UK?
RS UK sells suitable caps with free next day shipping for a few dollars
http://uk.rs-online.com/web/p/ceramic-multilayer-capacitors/7883048/

The other larger missing caps are on backorder till June though
http://uk.rs-online.com/web/p/ceramic-multilayer-capacitors/9163129/
```

---
## \#118 Posted by: darkkevind Posted at: 2017-05-25T20:14:55.653Z Reads: 70

```
Oh wow! Thanks! Do you think that's it then? Just those two things?

I reckon I could easily solder those on myself....
```

---
## \#119 Posted by: darkkevind Posted at: 2017-05-25T21:30:54.057Z Reads: 75

```
Is this the same as the large one?
http://www.ebay.co.uk/itm/CAP-MLCC-C0G-NP0-15PF-3KV-1808-Part-TDK-C4520C0G3F150K110KA-/351591025576?hash=item51dc754ba8:g:hSMAAOxy7nNTPxhY
```

---
## \#120 Posted by: TSG_AU Posted at: 2017-05-25T21:43:42.521Z Reads: 75

```
Nah that's 15 picofarad, about a millionth of the capacity

This one's 10uF though, compared to the 15uF one in the design
http://uk.rs-online.com/web/p/ceramic-multilayer-capacitors/9155493/
Maybe stack 2 of them on top of each other

Seems like your VESC sorta works right now already, it wouldn't hurt to install these extra caps
```

---
## \#121 Posted by: darkkevind Posted at: 2017-05-25T22:09:45.733Z Reads: 74

```
Hmmm, will that work then?
```

---
## \#122 Posted by: TSG_AU Posted at: 2017-05-25T23:09:29.934Z Reads: 74

```
Should do, it's just either a decoupling or bypass cap between Vdd and GND, so it'll be close enough, and much better than no cap.
```

---
## \#123 Posted by: darkkevind Posted at: 2017-05-26T16:25:52.037Z Reads: 75

```
[quote="TSG_AU, post:117, topic:23208"]
http://uk.rs-online.com/web/p/ceramic-multilayer-capacitors/9163129/
[/quote]

Do you know of an EU supplier that might have one of these?

http://uk.rs-online.com/web/p/ceramic-multilayer-capacitors/9163129/1
```

---
## \#124 Posted by: TSG_AU Posted at: 2017-05-26T17:41:13.988Z Reads: 71

```
Mouser/Farnell/Digikey will get one of those to you, but also charge you $10-$15 for shipping

There appears to be a few Arrow electronics centres in the UK though, in which case shipping may be cheaper from there.
This part will do
https://www.arrow.com/en/products/ckg57kx7s2a156m335jh/tdk
```

---
## \#125 Posted by: darkkevind Posted at: 2017-05-26T21:30:45.902Z Reads: 65

```
Thanks man! I've ordered the little one from RS and the big one from Arrow.

Hopefully once I get them soldered on it'll be a fully functioning bad ass VESC!
```

---
## \#126 Posted by: TSG_AU Posted at: 2017-05-26T23:49:10.267Z Reads: 65

```
Great, good luck!
```

---
## \#128 Posted by: darkkevind Posted at: 2017-05-31T19:01:27.859Z Reads: 62

```
This is the box the large cap came in!! lol
<img src="/uploads/db1493/original/3X/9/d/9dbfaccd76df887fc560e5bff484cd2954a0d3fa.jpg" width="690" height="388">
```

---
## \#129 Posted by: TSG_AU Posted at: 2017-06-01T02:57:30.169Z Reads: 59

```
Man that's a big box. How much was shipping?
```

---
## \#130 Posted by: darkkevind Posted at: 2017-06-01T07:16:16.167Z Reads: 58

```
It was free!! lol

Bear in mind that's a bread bin behind it, and this thing is like 5mm square, if that! lol
```

---
## \#131 Posted by: darkkevind Posted at: 2017-06-02T14:28:17.980Z Reads: 63

```
OK, I'm seriously thinking about just giving up with this now and save up a bit to buy a new VESC!

I soldered on both caps...
<img src="/uploads/db1493/original/3X/3/8/384511c35b97d55fd81bff48c5b6ae649118e764.jpg" width="690" height="388">

Hasn't made a blind bit of difference unfortunately! :frowning:

Here's a screen cap of the data for when I'm going full throttle, then braking full, a few times in a row... from what I've read on some other posts, that's not good right?<img src="/uploads/db1493/original/3X/1/2/1224e048ea2c41fa7e44807c566fab0f9bc17c51.PNG" width="690" height="431"><img src="/uploads/db1493/original/3X/5/9/59b347b00bc6012296be31972205bbf8591ef225.PNG" width="690" height="334"><img src="/uploads/db1493/original/3X/4/7/4736f5566d36d39cd1b6d05bcc791f015d08c8ef.PNG" width="690" height="332">
```

---
## \#132 Posted by: TSG_AU Posted at: 2017-06-02T20:45:45.105Z Reads: 58

```
Yeah I'm outta ideas too at this point. I can see more missing caps from that view though
If you have some leftover of the small caps, you could try soldering them into the blank spots of C31 and C14-  those are for the STM32 MCU, and are the same value (2.2uF)
The C4 cap shouldn't matter as that's just for an external temp input

I'll also see if I can find my BLDC-tool settings for you to try since we have the same setup
```

---
## \#133 Posted by: darkkevind Posted at: 2017-06-02T20:49:30.618Z Reads: 68

```
Hmm no worries. I might try those caps...

FYI, I just tried out 9s instead of 6s and although I got an eventual higher top speed, the pick-up was exactly the same, just weak and pathetic and cut out if I floored it, even whilst already in motion...

I think it's just a dud! That's what I get for buying second hand I guess :frowning2:

You make anything of the graph?
```

---
## \#134 Posted by: TSG_AU Posted at: 2017-06-02T20:56:44.236Z Reads: 70

```
Here are my settings for a 6S setup: Copy and paste them to a text file and name it "something.xml" and then use the load xml feature of the BLDC-tool to read them:

    <?xml version="1.0" encoding="UTF-8"?>
    <MCConfiguration>
        <pwm_mode>1</pwm_mode>
        <comm_mode>0</comm_mode>
        <motor_type>2</motor_type>
        <sensor_mode>0</sensor_mode>
        <l_current_max>60</l_current_max>
        <l_current_min>-60</l_current_min>
        <l_in_current_max>50</l_in_current_max>
        <l_in_current_min>-30</l_in_current_min>
        <l_abs_current_max>100</l_abs_current_max>
        <l_min_erpm>-100000</l_min_erpm>
        <l_max_erpm>100000</l_max_erpm>
        <l_max_erpm_fbrake>300</l_max_erpm_fbrake>
        <l_max_erpm_fbrake_cc>1500</l_max_erpm_fbrake_cc>
        <l_min_vin>19</l_min_vin>
        <l_max_vin>25.4</l_max_vin>
        <l_battery_cut_start>19.5</l_battery_cut_start>
        <l_battery_cut_end>19.25</l_battery_cut_end>
        <l_slow_abs_current>1</l_slow_abs_current>
        <l_rpm_lim_neg_torque>1</l_rpm_lim_neg_torque>
        <l_temp_fet_start>80</l_temp_fet_start>
        <l_temp_fet_end>100</l_temp_fet_end>
        <l_temp_motor_start>80</l_temp_motor_start>
        <l_temp_motor_end>100</l_temp_motor_end>
        <l_min_duty>0.005</l_min_duty>
        <l_max_duty>0.95</l_max_duty>
        <sl_min_erpm>500</sl_min_erpm>
        <sl_min_erpm_cycle_int_limit>1100</sl_min_erpm_cycle_int_limit>
        <sl_max_fullbreak_current_dir_change>10</sl_max_fullbreak_current_dir_change>
        <sl_cycle_int_limit>80</sl_cycle_int_limit>
        <sl_cycle_int_limit_high_fac>0.8</sl_cycle_int_limit_high_fac>
        <sl_cycle_int_rpm_br>80000</sl_cycle_int_rpm_br>
        <sl_bemf_coupling_k>600</sl_bemf_coupling_k>
        <hall_table_0>-1</hall_table_0>
        <hall_table_1>1</hall_table_1>
        <hall_table_2>3</hall_table_2>
        <hall_table_3>2</hall_table_3>
        <hall_table_4>5</hall_table_4>
        <hall_table_5>6</hall_table_5>
        <hall_table_6>4</hall_table_6>
        <hall_table_7>-1</hall_table_7>
        <hall_sl_erpm>2000</hall_sl_erpm>
        <foc_current_kp>0.0138</foc_current_kp>
        <foc_current_ki>18.1</foc_current_ki>
        <foc_f_sw>20000</foc_f_sw>
        <foc_dt_us>0.08</foc_dt_us>
        <foc_encoder_inverted>0</foc_encoder_inverted>
        <foc_encoder_offset>180</foc_encoder_offset>
        <foc_encoder_ratio>7</foc_encoder_ratio>
        <foc_sensor_mode>0</foc_sensor_mode>
        <foc_pll_kp>2000</foc_pll_kp>
        <foc_pll_ki>20000</foc_pll_ki>
        <foc_motor_l>1.385e-5</foc_motor_l>
        <foc_motor_r>0.0181</foc_motor_r>
        <foc_motor_flux_linkage>0.00341</foc_motor_flux_linkage>
        <foc_observer_gain>7.22e+7</foc_observer_gain>
        <foc_duty_dowmramp_kp>10</foc_duty_dowmramp_kp>
        <foc_duty_dowmramp_ki>200</foc_duty_dowmramp_ki>
        <foc_openloop_rpm>400</foc_openloop_rpm>
        <foc_sl_openloop_hyst>0.1</foc_sl_openloop_hyst>
        <foc_sl_openloop_time>0.5</foc_sl_openloop_time>
        <foc_sl_d_current_duty>0.05</foc_sl_d_current_duty>
        <foc_sl_d_current_factor>0.05</foc_sl_d_current_factor>
        <foc_hall_table_0>255</foc_hall_table_0>
        <foc_hall_table_1>255</foc_hall_table_1>
        <foc_hall_table_2>255</foc_hall_table_2>
        <foc_hall_table_3>255</foc_hall_table_3>
        <foc_hall_table_4>255</foc_hall_table_4>
        <foc_hall_table_5>255</foc_hall_table_5>
        <foc_hall_table_6>255</foc_hall_table_6>
        <foc_hall_table_7>255</foc_hall_table_7>
        <foc_sl_erpm>2500</foc_sl_erpm>
        <s_pid_kp>0.0001</s_pid_kp>
        <s_pid_ki>0.015</s_pid_ki>
        <s_pid_kd>0</s_pid_kd>
        <s_pid_min_rpm>900</s_pid_min_rpm>
        <p_pid_kp>0.03</p_pid_kp>
        <p_pid_ki>0</p_pid_ki>
        <p_pid_kd>0.0004</p_pid_kd>
        <p_pid_ang_div>1</p_pid_ang_div>
        <cc_startup_boost_duty>0.15</cc_startup_boost_duty>
        <cc_min_current>1</cc_min_current>
        <cc_gain>0.0046</cc_gain>
        <cc_ramp_step_max>0.04</cc_ramp_step_max>
        <m_fault_stop_time_ms>3000</m_fault_stop_time_ms>
        <m_duty_ramp_step>0.02</m_duty_ramp_step>
        <m_duty_ramp_step_rpm_lim>0.0005</m_duty_ramp_step_rpm_lim>
        <m_current_backoff_gain>0.5</m_current_backoff_gain>
        <m_encoder_counts>8192</m_encoder_counts>
        <m_sensor_port_mode>0</m_sensor_port_mode>
        <meta_description>&lt;!DOCTYPE HTML PUBLIC &quot;-//W3C//DTD HTML 4.0//EN&quot; &quot;http://www.w3.org/TR/REC-html40/strict.dtd&quot;&gt;
    &lt;html&gt;&lt;head&gt;&lt;meta name=&quot;qrichtext&quot; content=&quot;1&quot; /&gt;&lt;style type=&quot;text/css&quot;&gt;
    p, li { white-space: pre-wrap; }
    &lt;/style&gt;&lt;/head&gt;&lt;body style=&quot; font-family:'Cantarell'; font-size:11pt; font-weight:400; font-style:normal;&quot;&gt;
    &lt;p style=&quot; margin-top:0px; margin-bottom:0px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;&quot;&gt;Configuration loaded from the motor controller.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</meta_description>
    </MCConfiguration>
```

---
## \#135 Posted by: TSG_AU Posted at: 2017-06-02T20:57:21.418Z Reads: 68

```
I'm not really sure what to make of the graph, you're not getting any faults in the terminal?
```

---
## \#136 Posted by: darkkevind Posted at: 2017-06-02T20:59:21.017Z Reads: 70

```
Thanks, I'll do that. Are you running FOC?
```

---
## \#137 Posted by: darkkevind Posted at: 2017-06-02T21:01:00.644Z Reads: 71

```
Only the ABS_CURRENT.... one now and again...

What's also weird is that when I hit a large bump, 9/10 times I lose all control for a few seconds...? All connectors are secure etc.
```

---
## \#138 Posted by: TSG_AU Posted at: 2017-06-02T21:09:28.111Z Reads: 70

```
I am running FOC, and actually I do also get the same fault occasionally. Happens when I hit a bump while at max throttle (I use current control btw)
Only things I haven't tried are increasing the Absolute max current, or unchecking the "Limit ERPM with negative torque" option, but I haven't had time to try.
```

---
## \#139 Posted by: darkkevind Posted at: 2017-06-02T22:50:46.765Z Reads: 66

```
Well that's weird, how come we're getting the same issue with bumping? 

Is anyone else getting that with their VESC?
```

---
## \#140 Posted by: darkkevind Posted at: 2017-06-13T11:16:45.396Z Reads: 56

```
Guys, long time no post!

I got a new VESC! It arrived today and all I gotta say is . . . . Wow! This is how I expected a VESC to be, great response, good punch and great brakes! I'm so happy to be boarding properly again! and silently (FOC) too!! :smile: 

Going to try it over my local park shortly and see how it fares with the inclines...
```

---
