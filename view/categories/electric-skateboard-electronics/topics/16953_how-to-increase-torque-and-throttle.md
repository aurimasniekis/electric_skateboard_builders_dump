# How to increase Torque and Throttle

### Replies: 65 Views: 3924

## \#1 Posted by: Yoshi14646 Posted at: 2017-01-31T14:43:47.496Z Reads: 270

```
I'm making my own custom electric longboard but I unfortunately bought the Turnigy Aerodrive SK3 - 6364-245kv Brushless Outrunner Motor. At the moment I am using a VESC to control the motor but I can't seem to get my motor to run without kick starting it, furthermore it cant even carry 40kg of load properly.  I have tested my battery and it is not the problem. I'm very new to using the VESC so I can't figure out what to use to increase the torque and throttle. Would be great if someone could help me as soon as possible :smiley:
```

---
## \#2 Posted by: devin Posted at: 2017-01-31T14:46:03.178Z Reads: 260

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#3 Posted by: Yoshi14646 Posted at: 2017-01-31T14:47:40.529Z Reads: 244

```
Thank You :smiley:
```

---
## \#4 Posted by: PXSS Posted at: 2017-01-31T14:53:25.281Z Reads: 236

```
What is your gear ratio and battery voltage?
```

---
## \#5 Posted by: Yoshi14646 Posted at: 2017-01-31T14:59:48.268Z Reads: 232

```
@PXSS The gear ratio is 15T to 60T so 0.25 turns,
```

---
## \#6 Posted by: devin Posted at: 2017-01-31T15:03:58.876Z Reads: 233

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#7 Posted by: Yoshi14646 Posted at: 2017-01-31T15:05:13.314Z Reads: 230

```
Yes, 15 being motor and 60 being Wheel
```

---
## \#8 Posted by: PXSS Posted at: 2017-01-31T15:12:19.135Z Reads: 226

```
Battery voltage?
Also post your esc settings
```

---
## \#9 Posted by: Yoshi14646 Posted at: 2017-01-31T15:24:42.351Z Reads: 230

```
<img src="/uploads/db1493/original/3X/7/6/7627260c181e00cfbd479929daa16e4b54628587.png" width="690" height="403"><img src="/uploads/db1493/original/3X/1/2/122093eaf29e1b41ac05e76d6d97e2a57233fd31.png" width="690" height="400"><img src="/uploads/db1493/original/3X/b/e/bec0e047856b740702ed029c09965ac8ece54fb4.png" width="690" height="399"><img src="/uploads/db1493/original/3X/0/a/0ae94523be191664c8bccdfb53431c7e35d62340.png" width="690" height="403"><img src="/uploads/db1493/original/3X/2/e/2ec74b3bdc6b36650406be0d1ba2818a5864e6ed.png" width="690" height="403"><img src="/uploads/db1493/original/3X/3/5/35d44043d47c8a754165238eb5f87425c660a7e7.png" width="690" height="407"><img src="/uploads/db1493/original/3X/c/f/cf26e7731d9266113dffbb381338023311af4106.png" width="690" height="431"><img src="/uploads/db1493/original/3X/c/2/c2c053667bfd2d9db6a90f87f32a2cb973d49ee0.png" width="690" height="401"><img src="/uploads/db1493/original/3X/f/3/f3f531a0e881e20eb65adc5b711e9b0f76fe9b68.png" width="690" height="401"><img src="/uploads/db1493/original/3X/0/7/07ecba44989d062aa182f3f6caf0297e633aa0ee.png" width="690" height="410">

Screenshots of the BLDC tool with default readings, and the voltage of my battery is 6s
```

---
## \#10 Posted by: devin Posted at: 2017-01-31T15:28:44.857Z Reads: 198

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#11 Posted by: Yoshi14646 Posted at: 2017-01-31T15:36:34.822Z Reads: 193

```
I don't quite understand what you mean by desired battery watts but I would like to draw as much as possible because that would increase torque right?
```

---
## \#12 Posted by: devin Posted at: 2017-01-31T15:37:40.740Z Reads: 189

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#13 Posted by: Yoshi14646 Posted at: 2017-01-31T15:41:59.029Z Reads: 187

```
Around 2000W to 2700W which is the limit for my motor
```

---
## \#14 Posted by: devin Posted at: 2017-01-31T15:43:22.276Z Reads: 185

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#15 Posted by: Yoshi14646 Posted at: 2017-01-31T15:46:50.953Z Reads: 184

```
I don't think I would need that much power just for the build, but a standard motor that many use has 1885W so maybe around 1500W to 1885W?
```

---
## \#16 Posted by: SageTX Posted at: 2017-01-31T15:47:48.682Z Reads: 186

```
What @devin is trying to ask is  
How many "c" is the battery rated for? This determines the amount you can put into the vesc / motor.   
He is trying to show you the math, and not answering you, but challenging you to figure it out.
```

---
## \#17 Posted by: devin Posted at: 2017-01-31T15:48:07.263Z Reads: 184

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#18 Posted by: Yoshi14646 Posted at: 2017-01-31T15:48:43.441Z Reads: 178

```
I'm still only a GCSE student looking to finish his project before the end of February lol, sorry I'm really not that smart
```

---
## \#19 Posted by: Yoshi14646 Posted at: 2017-01-31T15:51:48.667Z Reads: 175

```
Yes If that will push me
```

---
## \#20 Posted by: Ackmaniac Posted at: 2017-01-31T15:52:02.520Z Reads: 173

```
Like a clueless meets a autistic nerd. Nice social experiment. Hopefully nobody get's hurt.
Little hint, You should tell us details about your battery (Li-Ion, Lipo and how many cells in series and in parallel) and how many motors you have.
```

---
## \#21 Posted by: PXSS Posted at: 2017-01-31T15:55:16.842Z Reads: 170

```
Yoshi, what batteries are you using. We can give you some guidance as to how much power you need but we need to answer a few questions. 

What is your battery nominal voltage?
Are you using Lipos or Liions?
What cells are you using(link)?
How much do you weigh?

1500W is a crap load of power for stand still. You dont want that if you dont want to get hurt as Ackmaniac said.
```

---
## \#22 Posted by: devin Posted at: 2017-01-31T16:01:15.259Z Reads: 168

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#27 Posted by: SageTX Posted at: 2017-01-31T16:56:40.311Z Reads: 162

```

@Yoshi14646 you are welcome here and just post away the questions. There are many here to help even with the simplest of tasks.

*Edited to remove "off topic" content.
```

---
## \#29 Posted by: Yoshi14646 Posted at: 2017-01-31T17:05:14.901Z Reads: 160

```
@PXSS 
The batteries I'm using 24 cells of Samsung 30Q 3000mah that are spot welded. 12 in parallel and 2 of the 12 in series. The Rated Max constant current 15A, Calculated max current 37A, Actual constant current 20A+. Each cell has 3.66V rating.

I'll try and answer the question the best I can when I get a reply from the person who sold it to me, who I know but is sleeping at the moment.
```

---
## \#30 Posted by: devin Posted at: 2017-01-31T17:06:24.620Z Reads: 158

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#33 Posted by: PXSS Posted at: 2017-01-31T17:18:07.934Z Reads: 158

```
You really need to figure out what batteries you have. Most likely all of your VESC settings are wrong. 
It cannot be a 2S12P pack. Your vesc doesnt take 7.4V...
```

---
## \#41 Posted by: Hummie Posted at: 2017-01-31T18:34:44.994Z Reads: 154

```
 there's a lot of people annoyed with devin's repeated math but the math isn't wrong!
 telling people it's wrong is not helping.  all those people who think they know what's going on, yet are saying devin's math is wrong..prove it.  I ride 200 motor amps.  I have almost no cogging and super smooth acceleration and exact power output as determined by the math.   the proof is in the pudding.   are we here on the forum to figure out how things work and make things better, because they definitely are for me, or are all you guys going to keep grumbling and flagging the real info while you claim it isn't.  egos abound and they're in the way.  if we're talking about safety this is the way there.  control of what your power output is at all rpms.
```

---
## \#42 Posted by: barajabali Posted at: 2017-01-31T18:36:01.896Z Reads: 146

```

```

---
## \#43 Posted by: barajabali Posted at: 2017-01-31T18:36:44.985Z Reads: 147

```
Ill reopen it once you all stop flagging each other. 

No point in a thread with every post flagged.
```

---
## \#44 Posted by: longhairedboy Posted at: 2017-01-31T19:20:26.096Z Reads: 141

```
thank you. Christ i'm tired of the virtual lynching that's going on here. Devin isn't wrong. He's just vocal, and people are getting board with it. Find something else to get bored with, like alt-facts.
```

---
## \#45 Posted by: barajabali Posted at: 2017-02-01T05:44:58.073Z Reads: 122

```

```

---
## \#46 Posted by: PXSS Posted at: 2017-02-01T09:11:46.852Z Reads: 119

```
I dont disagree with the math. I disagree with presenting very dangerous settings as advice. Think about it this way, your son is thinking about getting his first motorcycle ever, so you get him a beefy one with a computer where you can set limits and what not for safety that he can eventually back off slowly. Now your kid is asking why his bike wont go faster than walking speed, suspects that some of the settings might be wrong. In comes uncle devin, who is tech savvy but has never owned or ridden a motorcycle and removes all safety precautions from the bike so now it has more acceleration than what is safe for an adult that's been riding bikes for years because "thats what your son asked for", but your teenage son is clueless about what he's getting on and could kill himself with the new settings. Do you step in and tell your brother (uncle devin) that he's wrong in doing so or do you just idly watch?
```

---
## \#47 Posted by: devin Posted at: 2017-02-01T09:57:25.522Z Reads: 114

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#48 Posted by: PXSS Posted at: 2017-02-01T10:02:35.766Z Reads: 114

```
You do realize that the OP is a teenager...?
```

---
## \#49 Posted by: devin Posted at: 2017-02-01T10:03:23.260Z Reads: 114

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#50 Posted by: Ackmaniac Posted at: 2017-02-01T10:08:03.522Z Reads: 115

```
[quote="devin, post:47, topic:16953"]
but what I'm talking about is grown adults making choices & riding electric skateboards.
[/quote]

Then why do you talk? :joy::joy::joy::v:
Sorry i couldn't resist.
```

---
## \#51 Posted by: PXSS Posted at: 2017-02-01T10:08:30.969Z Reads: 113

```
There are plenty of teens in this forum. Assuming that only adults ride e-skateboards is ignorant and even then it doesn't excuse you of giving terrible advice you have never PERSONALLY tested or have the means to.
```

---
## \#52 Posted by: devin Posted at: 2017-02-01T10:08:56.511Z Reads: 112

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#53 Posted by: devin Posted at: 2017-02-01T10:09:52.440Z Reads: 111

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#54 Posted by: TarzanHBK Posted at: 2017-02-01T10:10:00.714Z Reads: 110

```
Doesn´t matter if they are old or young, if someone is a noobie and want´s some advice, you can´t tackle them with "how much W do you want?" They don´t know! They never experienced how 1000 W feels on an electrified board.

So much healthier for everyone if someone gives some good standard tips for a good setup and let them read trough the forum and discover experienced things like throttle adjustment, max W possible, start from standstill issues, etc later!

He even does have issues explaining how his battery is aligned! 

So keep it to the standards first!
```

---
## \#55 Posted by: devin Posted at: 2017-02-01T10:11:34.740Z Reads: 104

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#56 Posted by: PXSS Posted at: 2017-02-01T10:15:13.418Z Reads: 104

```
It was brought up in the discussion right around where he mentioned he was still in high school. GCSE particularly pertains to grades 7-10...

So you potentially gave a 7th grader the advice to set his board to accelerate at 1500W based on the fact that "All your friends are not children". Do you see the flaw in that? You need to have more common sense. 

Either way, I just brought it up so @longhairedboy could see where we were coming from and why we advice against your settings

Lets not further derail @Yoshi14646 thread. If you want we can PM
```

---
## \#57 Posted by: devin Posted at: 2017-02-01T10:16:55.018Z Reads: 103

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#58 Posted by: TarzanHBK Posted at: 2017-02-01T10:19:18.223Z Reads: 108

```
[quote="devin, post:55, topic:16953"]
@TarzanHBK there are no standards. standards is an illusion. a fantasy. only values.
[/quote]

And thats your problem! We do have some good, working standards here - tested and proven by lot´s of members here.
If you can optimize something about them - fine! But pls test everything and see if others see that same improvement and THEN! you can help others with a new and good working standard!
```

---
## \#59 Posted by: devin Posted at: 2017-02-01T10:28:10.073Z Reads: 114

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#60 Posted by: TarzanHBK Posted at: 2017-02-01T11:47:51.250Z Reads: 119

```
yah! So ask him about Vesc screenshots and detailed information about the battery and not throwing around with wild numbers, if you don´t know his setup!
```

---
## \#61 Posted by: Ackmaniac Posted at: 2017-02-01T12:12:42.882Z Reads: 119

```
Back to @Yoshi14646. 
With a 2P setup of those cells you can set the battery max amps to 40 and the max motor to like 60 A for the beginning. You can also try 80 but do 60 first.
Then you should set your Battery cutoff start to 36V and the Battery cutoff end to 33.6V.
You also need to set the Max ERPM to 60000 and the Min ERPM to -60000. And i would disable the "Limit ERPM with negative torgue".
Then you should go in the PPM tab if you use a ppm remote and activate the "soft ERPM limit" and set the ERPM limit start to 58000 and the ERPM limit end to 60000. Because with your 245 kv motor you could easily reach higher ERPMs than the VESC can handle. 
If you use a Nunchuk then set the ERPM limit start and end there.
```

---
## \#62 Posted by: TarzanHBK Posted at: 2017-02-01T12:56:12.737Z Reads: 117

```
@devin there you go! @Ackmaniac with some good, well known and understandable advise for someone who is new.
That´s how it should be :slight_smile:
```

---
## \#63 Posted by: longhairedboy Posted at: 2017-02-01T13:49:46.176Z Reads: 121

```
I understand what you are saying. But It's hard to say in that particular example because my son has been rebuilding 2 stroke engines in his dirt bikes since he was 12, and now, at 15, he's been experimenting with VESC settings in his own boards he built from scratch. Handing him a Ninja with a programmable ECU would be like giving a 3 yo all day with mickey mouse in a cake and ice cream factory. He'd shit his pants and then take off and i wouldn't see him for days. Then he would tell me he did 130 on the interstate and i would yell at him using all manner of imaginative expletives, possibly even offering to throw his face on the street myself and discuss how it would be more efficient than having a $10,000 bike do it. Then we'd go inside and act like nothing happened, as men do. 

So what i would probably do is argue with uncle devin for a minute, see what my son thinks about the dangers involved, then hand him a helmet. If my son was a nitwit he'd be inside playing candy crush and trying to get laid on facebook, not doing his homework first (straight As) and then testing our own bleeding edge prototypes we built in our garage based on the desires of people who have cash to burn on exotic custom electric skateboards while discussing the impact that Mango Mussolini will have on my supply chain. 

But i definitely see your point, and it is well taken. The struggle I have with this is that his facts aren't wrong, he just presents them in a way that makes people want to ignore them or call him a zealot spammer. Honestly if i had the money I'd hire Devin and keep him to myself and mine his intellect until he had nothing left to post here. But the real problem here is that this audience is a mixture of noobs and experts and everything in between, so while conveying information in one way is beneficial to one band of the spectrum, it may irritate others and even raise genuine, legitimate concerns like yours. He is also clearly comfortable with debate, which is something a lot of people aren't and misconstrue as argument. 

So the real question then becomes, to whom does this forum cater? Everyone? The elite? The noobs? When left with such a conflict, most would resolve to stay within their own native tongue so to speak, which is what Devin has done. 

I'm just not a fan of excommunicating people due to failed communication tactics. Especially when they can simply be ignored. 

I apologize for the novel.
```

---
## \#64 Posted by: JohnnyMeduse Posted at: 2017-02-01T14:11:06.582Z Reads: 105

```
[quote="longhairedboy, post:63, topic:16953"]
The struggle I have with this is that his facts aren't wrong, he just presents them in a way that makes people want to ignore them or call him a zealot spammer.
[/quote]


The Math aren't wrong.... but in real world you have to take in consideration the limits of your electronic... witch he doesn't, **and could lead to serious injuries and broken vesc**...

First: Mosfet on the vesc are rated for 239 Amp at 10V for temperature of 100 degree (yes 100 degree, because you have to take heat in cosideration)... So basically at 36V the number of amp the mosfet can endure is way less than 200Amp

Second: there is not enough copper on the Vesc to endure 200amp

Third: Motor can support 200amp, but will likely overheat, isolation will melt and will leave you with a shorted motor under your feet, that is probably gonna to send you farther than all Apollo mission... 

And the list just go and go...

SON IN THEORIE HE MIGHT BE RIGHT.... BUT IN THE REAL WORLD DON'T TRY THIS, YOUR JUST GOING TO BLOW YOUR VESC OR HURT YOURSELF

And since safety should be a important thing on this forum... theories that could lead to any injuries should always come with the proper warning, and if your not able to see the danger behind and keep and pushing your theories as the absolute truth... well you might need a slap in the face IMO.
```

---
## \#66 Posted by: longhairedboy Posted at: 2017-02-01T14:33:21.230Z Reads: 103

```
Theory vs application. It's something that has kept me on the conservative side of VESC settings all this time for all of the reasons mentioned above. It's easy to get caught up in the theory. It's fascinating stuff.
```

---
## \#67 Posted by: Yoshi14646 Posted at: 2017-02-01T14:44:32.005Z Reads: 104

```
Hi all sorry for the late reply I hit the limit of replies in 24 hours,
Thank you all for contributing to this discussion, and yes I am still a noobie when it comes to the VESC and Electric skateboards so all tips are helpful.

**Just a bit of background:** 
I am still a teenager and currently in Grade 10 in the IGCSE program looking to complete his paper work to get a good grade, I decided to take on this project as seeing all the videos and photos of the projects completed on this forum inspired me to do so. I foolishly thought that assembling and making a motor mount is all I needed to do after purchasing the parts, I have so far burnt out and short circuited a Lipo battery making it unusable and drilled 10 holes into my board which I don't even need :sweat:. 

**Current state:**
At the moment I am buying a motor mount that fits the 63mm and have the battery and motor ready. The only problem remaining is the VESC which is why I opened this discussion. Which many have tentatively replied to and thank you guys for that :smiley:.

@PXSS @devin @Pedrodemio @Ackmaniac
**Information regarding the Battery, Pulley and Motor**
- The battery is the Samsung 30Q 3000mah and are Lithium-ion, 6s4p 24cell rated 22.2 max 25.2v, 11600mah.
- The gear ratio is 15T to 60T so 0.25 turns, 15 being the one attached to the motor and 60 being the one on the wheels.
- The Motor I am using is the Turnigy Aerodrive SK3 - 6364-245kv Brushless Outrunner Motor. (Stats Below)
<img src="/uploads/db1493/original/3X/6/d/6d0eea3bf5ccfefc6cd93d7248c073e05c16c9b1.png" width="231" height="220">

**What I need:**
As many of you have stated I am in fact very clueless as to how all this works despite taking many lessons on electronics :grin:. My problem was that I can't get the right ratings on the VESC to pump enough power to the motor to push me, I am currently 77kg which makes me heavy but shouldn't be much of a problem. I have seen many people use the same setup as me with the 63mm Turnigy motor and the VESC, I wanted to know what ratings they are using. I am aware as @devin said many people have preferences as to how many W they want to pull and how fast they want to go, I am fine with any ratings as long as it will push my 77kg along. 

Thanks all for the help :smiley:.
```

---
## \#69 Posted by: JohnnyMeduse Posted at: 2017-02-01T15:07:18.522Z Reads: 95

```
For what you whant to do.... you won't be able to acheive it with a single setup... belive me, I'm 80kg and I've quite a few motor trying to push them too hard, specialy because at 245kv uour motor is more for speed than torque 😉

So for what you trying to acheive with the motor you have, you need a dual setup or chaging for a single 6374 at around 190kv
```

---
## \#70 Posted by: Yoshi14646 Posted at: 2017-02-01T16:02:28.314Z Reads: 91

```
But I've seen people around the same size being pushed using the same motor, or would I have to spend more money to buy another motor...
```

---
## \#72 Posted by: Okami Posted at: 2017-02-01T16:06:04.042Z Reads: 91

```
@Yoshi14646 On top of that - what wheel size are u using? 60t sprocket is for pneumatics probably
```

---
## \#73 Posted by: Yoshi14646 Posted at: 2017-02-01T16:08:59.857Z Reads: 95

```
I'm currently using the default wheels which are around 75mm but I plan on getting 83mm wheels, I don't know what you mean by pneumatics though
```

---
## \#74 Posted by: PXSS Posted at: 2017-02-01T17:15:45.784Z Reads: 95

```
60T pulleys are usually used on 100mm+ wheels is what he means. But you need them because of your Kv value. 

Can you take some pictures when you get a chance?
That would help some of us here. 

I am still having a hard time fully trusting the battery you have. No offense. Can you measure the voltage across the main leads when fully charged and give me that number. 

The reason I have a hard time believing you have a 6S pack is because your VESC is configured for a 12S pack based on the screenshots above and it should not work at all with those settings unless you have not set it up yet.

The settings @Ackmaniac suggested in post 61 work well if you have a 12S pack. If you have a 6S pack then they wont. 

Not only that but the pack configuration affects your max speed and torque available and 6S to 12S is a pretty substantial difference. 

We can help you tune it but we need accurate info
```

---
## \#75 Posted by: Okami Posted at: 2017-02-01T19:00:57.004Z Reads: 88

```
Yes i meant the ratio of 1:4 does not sound right.. especially with not pneumatic (5+ in) wheels..

So the question is - what pulley tooth does @Yoshi14646  really have.. the biggest ive seen is 40T for the lonboard urethane wheel..

Plus, i could agree, that settings for vesc could be messed up.

---

Sidenote - 190kv motor with 230mm (9in) 6s (li-ion), car esc and 1:4.33 ratio can start slowly from standstill if rider weight is below 70kg or so.

Not sure what ratio, wheels and weight + motor kv needed for longboard to start from standstill

--

Im 90kg and can also start from standstill with a bit of jerking. Not sure does vesc would be doing much differently but i thought to share whats (at what setup) is working for easy startup
```

---
## \#76 Posted by: Pedrodemio Posted at: 2017-02-01T20:12:44.772Z Reads: 85

```
He probably is using HTD 3M, a 60mm pulley

Looking again on the vesc screens, the voltages cut off are completely wrong, you can set up cut off start to 20V and cut off end to 18V
```

---
## \#77 Posted by: Okami Posted at: 2017-02-01T20:17:17.224Z Reads: 84

```
I totally forgot to mentioned the option that perhaps he is having htd3 toothing.. Thanks for pointing this out, as this might explain the high tooth count he has..
```

---
## \#78 Posted by: PXSS Posted at: 2017-02-01T21:52:58.222Z Reads: 85

```
@Pedrodemio, @Okami, @Yoshi14646 
I think there is too much conflicting information right now for us to make a suggestion. 

Yoshi,
If you can provide pictures and a little more info it would be great. What belts are you using? Also what width? If your belts are not wide enough and the right series even with the right settings you might not have enough torque transfer.
```

---
## \#79 Posted by: mmaner Posted at: 2017-02-02T00:47:54.117Z Reads: 84

```
This may not be what your looking for, but...

The shaft shim on my 260kv motor, running on 6s, broke so I've been running a single 190kv.  I felt like a little old lady.  I just added another VESC and 190kv motor and holy bad guano Batman, I can't reign it in its so powerful, so much torque and I haven't hit the end of the throttle yet and I'm doing 22mph..  Cant wait to see it when my 10s battery gets here.
```

---
## \#80 Posted by: Yoshi14646 Posted at: 2017-02-02T04:01:11.889Z Reads: 88

```
I move with Singapore time so my replies will probably be late sorry :grin: 
the belt I am using is [HTD Timing Belt 3M 3mm Pitch 9mm Wide CNC-Drives](http://www.ebay.co.uk/itm/HTD-Timing-Belt-3M-3mm-Pitch-9mm-Wide-CNC-Drives-Choose-Size-150mm-to-501mm-/131713051095?var=431089914162&hash=item1eaab5a9d7:m:mZPTRNF6YGTNye_Q73jkhxA)
The pulley is [HTD Timing Belt Pulley](http://www.ebay.co.uk/itm/HTD-Timing-Belt-Pulley-Pilot-Bore-3M-3mm-Pitch-9mm-Wide-CNC-ROBOTICS-/200958049830?var=&hash=item0)
The only photo I only have is this one <img src="/uploads/db1493/original/3X/a/9/a9fbbce4e388185af88539779f47b3f98da14e50.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/3/a/3a3aa4661d3fb36b618965a8e4c96577efc19fe0.JPG" width="375" height="500">
Im planning on getting the 83mm wheels and a chain drive that will fit onto the wheels.
```

---
## \#81 Posted by: Tampaesk8er Posted at: 2017-02-04T15:23:38.568Z Reads: 78

```
Well spoken, I'm currently building my first eboard and my son is the one that will be using it the most. I've found this forum and I've been reading so much in the last 2 wks, so much experience here on eboards and im so greatfull for this forum and the people. I've come here to try to learn how to program my first build, etc. It would be very dangerous if i would program my board incorrectly and have my son really hurt himself because of someone posting wrong info. I am amazed of how big the eboard community is and please post true settings info when helping someone like me, thank you., Keep up the good work.
```

---
## \#82 Posted by: Yoshi14646 Posted at: 2017-02-05T16:19:54.024Z Reads: 71

```
<img src="/uploads/db1493/original/3X/e/6/e6e23dc61628b728ebe7011993d93c126647e8a6.png" width="690" height="431">
Forgot to upload this but i think this will help in telling what the problem is.
```

---
