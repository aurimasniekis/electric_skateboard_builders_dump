# Kid Build thoughts and some rambling

### Replies: 40 Views: 1694

## \#1 Posted by: Sender Posted at: 2017-12-04T03:07:09.016Z Reads: 185

```
Hey guys, I just ordered a slew of stuff from all the Black Friday discounts and have a direction question.

One of the boards I am building is for my wee lad, Jackson. He is just a little guy, loves to ride boards, weighs nothing, and I want to build him something  in the 13 MPH range.


I am going to do something on a land yachtz Dinghy (28.5 x 8.5).

This isn't a build post, just a general question.  The board, "Secret Zooma" is going to be built with a FOCBOX, besides setting these parameters,  How should I go about limiting the speed? ,  should I do a smaller battery (6s or 8s), or use a lower kv motor in conjunction with 10s?

Here is why I wonder....  I am also doing some other 10s and 12s builds (no build threads yet... soon 😁), and am also doing this "Kid Build."

I feel like it might be easier to have everything working off 10s (like some other builds I am about to start working on) with a lower (thinking APS 130kv) In order to limit speed.  This way I can use one charger with other 10s builds I want to do instead of also buying an 8s charger.

But then again, if I build an 8s battery with low gearing a d 190kv motor, I could potentially upgrade his board later possibly a bit easier.


Damn you beer, I am rambling!!!

Bottom Line At the End:

10s3p 130 kv 6355 single 14/36 gearing 83mm wheels

or

8s4p 190kv 6355 single 14/36 gearing 83mm wheels

For my 7 year olds board, "Secret Zooma"

Thoughts??

I know it is essentially a high voltage vs higher amp question, but am wondering if anyone has any experience building quality stuff for their little ones.  I want it to be good enough for the random full brown layman "grown up" to hop on as well...
```

---
## \#2 Posted by: MrHappy Posted at: 2017-12-04T03:11:52.823Z Reads: 165

```
You could just limit the ERPM, then as he gets older/skill increases just bump it up a bit until he's at the normal erpm of the setup.
So 10s and 190kv, but limited to 20k erpm (just throwing numbers out there)
```

---
## \#3 Posted by: wafflejock Posted at: 2017-12-04T03:12:34.139Z Reads: 160

```
Using the metr module (or during regular configuration) you can limit the amperage which limits the torque and acceleration but doesn't limit the top-end so you'll have to limit that based on voltage or KV.  Advantage with the module being you can change modes from your phone for more experienced riders.
```

---
## \#4 Posted by: Sender Posted at: 2017-12-04T03:18:37.062Z Reads: 146

```
Not familiar with metr module, I will be sure to search that.   Torque control is the main thing,   He rides the boosted and knows when to back off, but as a bamboo, his dexterity for throttle control isn't quite where ours is... yet.
```

---
## \#5 Posted by: Sender Posted at: 2017-12-04T03:19:16.496Z Reads: 141

```
So will that just limit top end or actual torque curve also?
```

---
## \#6 Posted by: MrHappy Posted at: 2017-12-04T03:25:37.391Z Reads: 131

```
Not sure, i haven't tried it.
```

---
## \#7 Posted by: Sender Posted at: 2017-12-04T03:37:01.670Z Reads: 127

```
Is that just a regular Bluetooth module that is some third party app compatible? Seems like it off my 7 minute inquiry...  I ordered 4  BT modules from @JLabs and I believe I should be able to do some things from there to control torque and top speed, but  I am really wondering what would be best from a design/efficiency perspective I suppose.  I have yet to use a VESC (Sooo excited to get started!) and am still a bit unfamiliar on what my range of control will be... maybe on this sort of build it really won't matter. 

AKA, both batteries and motor config will be so much more than capable of what I am asking them to do, it just won't matter... In that case, I would go 10s39 so I don't need to buy a separate charger.

Am I missing anything here? @longhairedboy what build does your little man ride?
```

---
## \#8 Posted by: wafflejock Posted at: 2017-12-04T03:40:59.206Z Reads: 119

```
Can see the metr app official site here:

https://metr.at/

The app itself is free and basically getting some money back for development through the sale of the module with the connector ready to plug and play from what I gather.  I don't think it's a special bluetooth module really but might be flashed ahead of time with some configuration values that aren't defaults you can maybe check with roman thread here on the module and updates:

http://www.electric-skateboard.builders/t/configuration-and-telemetry-for-vesc-ios-android/13483

Main point of the app and module is for capturing trips/data there's also this site now where you can share results:

http://esk8race.com/

(not affiliated with any of this nor are they related except working together data wise)

Ultimately you can limit the amperage on the motor max amps just using the regular USB connection too the app just adds the convenience of swipe to change config without hooking up USB.
```

---
## \#9 Posted by: JLabs Posted at: 2017-12-04T03:43:55.093Z Reads: 108

```
You can also do the same things @wafflejock mentioned with my module paired with the free android app. It allsow you to change tops speeds, limit amperage, and map the ppm values (Ackmaniac)
```

---
## \#10 Posted by: Sender Posted at: 2017-12-04T03:46:24.034Z Reads: 109

```
That was my plan (and why I snagged 4 at the redonkulous Black Friday price) 💪💪💪


BTW, where the hell is my Spud, dick! 🤣🤣 

JK
```

---
## \#11 Posted by: JLabs Posted at: 2017-12-04T03:50:55.329Z Reads: 102

```
Did you order one? Once I have a tracking number (this week) they will be back on my site if you haven’t all ready.
```

---
## \#12 Posted by: Sender Posted at: 2017-12-04T03:52:26.045Z Reads: 97

```
oh yeah, grabbed 4 brohawn, you already shipped them out!
```

---
## \#13 Posted by: JLabs Posted at: 2017-12-04T03:52:59.603Z Reads: 101

```
[quote="Sender, post:10, topic:40065"]
BTW, where the hell is my Spud, dick! 🤣🤣
[/quote]

Wait a minute... am I missing something?
```

---
## \#14 Posted by: Sender Posted at: 2017-12-04T03:53:24.116Z Reads: 98

```
Nope, just a joke...
```

---
## \#16 Posted by: JLabs Posted at: 2017-12-04T03:54:53.170Z Reads: 99

```
Ohhh haha.. I’m slow :laughing:
```

---
## \#17 Posted by: CamBo Posted at: 2017-12-04T05:11:32.276Z Reads: 110

```
I use the eSkate VESC app on iOS.  You can change the eRpm limits from your phone through the hm10 Bluetooth module really easily.  Kids run on 10s3p limited to 15 mph. It works great <img src="/uploads/db1493/original/3X/f/5/f5e676aa267f23084d55d621233af113469bb22b.jpeg" width="375" height="500">
```

---
## \#18 Posted by: longhairedboy Posted at: 2017-12-04T15:09:38.090Z Reads: 106

```
[quote="Sender, post:7, topic:40065"]
@longhairedboy what build does your little man ride?
[/quote]

He's still in training, only 3 years old. So he rides on my board with me up front and i'm teaching him how to stance. 

HE'll be on a tuned down ArcBoards mod with a popscicle deck within 6 months in full pads and helmets at the basketball court learning to control his throttle and carve. More than likely this exact board with far more conservative VESC settings and a new maytech remote in slow mode. 
https://www.instagram.com/p/BXT8Gmuli2P/?taken-by=longhairedboy

After the basics comes trail riding, then the larger more powerful boards to graduate to. Alsthough its a lot more amusing to see him with this board, because its just not fucking practical, or even ridable, at all. 
https://www.instagram.com/p/BXNt0OYFaVS/?taken-by=longhairedboy
```

---
## \#19 Posted by: Sender Posted at: 2017-12-04T15:19:26.903Z Reads: 101

```
Awesome! I kbow that penny build is a hellcat, but couldnt you tone it down in the VESC, like a lot, and make it workish for him? Or would that be to far out of operating parameters to get it to a reasonable state?
```

---
## \#20 Posted by: longhairedboy Posted at: 2017-12-04T15:24:47.959Z Reads: 101

```
when i say its unridable, i mean it makes me want to order a solid gold abec clone pulley from Shapeways and award it to anyone who can stay on it for more than 10 minutes in my neighborhood. I was seriously joking about making that board some kind of give-a-way contest obstacle. 

its not only meme worthy, its probably deadly. The deck is flexible plastic, the wheels are too big, and its a single drive with almost no wheel base to speak of. The wheels are shit from amazon in a durometer that just bounces all over the street and never gets traction. 

Arcboards did a very proper penny that is ridable and kind of amazing. This is so far from that... i mean damn. But it looks so cute with Simon.
```

---
## \#21 Posted by: egzplicit Posted at: 2017-12-04T16:09:08.908Z Reads: 89

```
[quote="MrHappy, post:2, topic:40065"]
You could just limit the ERPM, then as he gets older/skill increases just bump it up a bit until he's at the normal erpm of the setup
[/quote]

This or limit PPM values so that full throttle acceleration is not 100% duty cycle.
```

---
## \#22 Posted by: Sender Posted at: 2017-12-04T16:11:32.847Z Reads: 89

```
Love it.  Epic build.  Here is my little maniac<img src="/uploads/db1493/original/3X/0/1/01f5b88b5a7027ce561abe085df014d3d0f0d443.jpg" width="243" height="500">
```

---
## \#23 Posted by: Sender Posted at: 2017-12-04T16:12:51.803Z Reads: 87

```
ok that makes sense, I was worried about torque being to high even with a reduced erpm
```

---
## \#24 Posted by: koralle Posted at: 2017-12-04T16:18:19.575Z Reads: 88

```
OK please be gentle if this plan is crap but what about obstructing the upper end of the throttle leaver travel on the remote with some epoxy? Each Christmas you carve a little bigger piece out again with a box cutter.

My godchild just turned 3 and much to the parents dismay, I'll have to introduce her to eskating at some stage.
```

---
## \#25 Posted by: MrHappy Posted at: 2017-12-04T16:25:38.240Z Reads: 87

```
Don't do this, it will just put all of the acceleration at the bottom of the throttle.
```

---
## \#26 Posted by: Sender Posted at: 2017-12-04T16:57:33.994Z Reads: 85

```
hmmm so ERPM for top speed, but what would be the best way to mellow out torque in settings?
```

---
## \#27 Posted by: MrHappy Posted at: 2017-12-04T17:27:38.286Z Reads: 81

```
Lower the Amps, it should make it accelerate slower. If you lower the torque, but leave the erpm, it will still get up to higher speeds, it will just take longer for the torque of the motor to slowly build up speed. So, limit both, and i think it will be perfect.
```

---
## \#28 Posted by: wafflejock Posted at: 2017-12-04T18:30:41.002Z Reads: 79

```
The metr app comes with 3 default settings (motor max amps) 10A for beginner/slow mode 30A for intermediate and 50A for fast mode.  10A is really a crawl but depending on his weight the ride experience will change since it's less torque to accelerate a smaller mass but I'd probably guess 15A or maybe even 30A is good (I'm most comfortable personally at 30A for regular cruising)
```

---
## \#29 Posted by: longhairedboy Posted at: 2017-12-04T18:49:22.834Z Reads: 77

```
lot of good advice here. 

Definitely the best thing to do is drop the motor amps waaaay down then work them back up. That's pretty much all it would take ona VESC build. Even something like Ru could be configured for a small child in that way. 

This is Ru. 

https://www.instagram.com/p/BaxYjVSl6Jx/?taken-by=longhairedboy

not exactly kid friendly with a top end somewhere around 37-38mph. But if i dropped those motor amps to like 10 i'll bet simon could handle the throttle for a few minutes in slow mode. and not fall too hard. May even have to drop the startup boost but likely not by much.
```

---
## \#30 Posted by: GrecoMan Posted at: 2017-12-04T22:35:35.978Z Reads: 67

```
rockin the same maytech remotes you use (love the thumb throttle) but have only been able to ride on slow mode. every time I put it on fast mode if I accelerate or brake decently hard the remote loses connection momentarily then reconnects. doesn’t happen on slow mode
```

---
## \#31 Posted by: longhairedboy Posted at: 2017-12-05T03:58:15.743Z Reads: 60

```
that sounds like it has more to do with something tripping in your motor controllers. Whatever it is, it sounds irritating.
```

---
## \#32 Posted by: koralle Posted at: 2017-12-05T12:19:27.920Z Reads: 58

```
So this made me actually think of something else: Is there any way I can **quickly** and **kind of secretly** make my board only go 6kph max?

This might save my ass, riding around GER and being caught by cops...

like through an app or by pulling a plug that only leaves it with 2s1p or something?
```

---
## \#33 Posted by: TarzanHBK Posted at: 2017-12-05T12:34:42.431Z Reads: 56

```
thats exactly whats @Ackmaniac s app is able to do
```

---
## \#34 Posted by: GrecoMan Posted at: 2017-12-05T12:40:46.391Z Reads: 55

```
it’s annoying as fuck. Especially when I manage to accelerate but hit the brakes and they instantly cut out...

my settings aren’t even crazy, not conservative but not insane. I’ll post some screenshots later but these are what I can remember:
60a Motor Max
-60a Motor Min
35a Batt Max.
-12a Batt. Min
i’m fuckin confused
```

---
## \#35 Posted by: longhairedboy Posted at: 2017-12-05T12:50:32.786Z Reads: 53

```
how big is your pack? Try these settings and see what happens:

50a Motor Max
-40a Motor Min
45a Batt Max.
-8a Batt. Min
```

---
## \#36 Posted by: GrecoMan Posted at: 2017-12-05T13:20:30.229Z Reads: 51

```
i’ve got a 10s6p that should capable of 80a cont. Bypassed for discharge. i’ll try those a bit later when i’m not in school
```

---
## \#37 Posted by: longhairedboy Posted at: 2017-12-05T13:37:47.731Z Reads: 49

```
IT sounds to me like the ESC is faulting a bit on hard acceleration (which goes both ways), so this may help mitigate that. It's actually kind of rare for a receiver to just start acting stupid like that. ITs more likely a conflict between settings and power draw.
```

---
## \#38 Posted by: GrecoMan Posted at: 2017-12-05T13:48:08.827Z Reads: 49

```
yea that’s what i’m thinking too. I really gotta grab a micro usb extension so i don’t have to keep taking my enclosure off... whatever, I gotta fill it with some more foam before I ride again anyway
```

---
## \#39 Posted by: GrecoMan Posted at: 2017-12-05T22:30:39.597Z Reads: 46

```
I think im officially an idiot. I did the PPM detection in low-power mode...

Means when I switch to high-power, the ppm signal is waaaaaay over the max pulsewidth it's set to. Its  currently dark and about 22 degrees out but ill try it out when I get a chance (probably tomorrow)
```

---
## \#40 Posted by: longhairedboy Posted at: 2017-12-06T00:04:32.356Z Reads: 42

```
don't drink too heavy man i've done worse lol
```

---
## \#41 Posted by: GrecoMan Posted at: 2017-12-06T01:18:35.241Z Reads: 39

```
I feel like I have sinned. On my 8th root beer now 😤
```

---
