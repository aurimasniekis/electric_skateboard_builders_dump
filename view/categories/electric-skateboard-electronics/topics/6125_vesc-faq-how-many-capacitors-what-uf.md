# VESC FAQ &#124; How Many Capacitors &amp; What uF

### Replies: 52 Views: 6823

## \#1 Posted by: onloop Posted at: 2016-07-13T14:52:34.634Z Reads: 508

```
[quote="Nordle, post:317, topic:4672"]
Why they use only two caps then? Cause it's cheaper!
[/quote]

Cheaper & quicker to assemble and most importantly more compact. The various cap configurations that we are delivering are due to what was available from suppliers at the time. When we bought parts for the first 1000 we couldn't secure 3000 caps of the same type. So we had to make some changes otherwise there would be more delays...

Its also worth pointing out that VESC 6.0 is adopting the same configuration of 2 caps.... in my opinion two caps is the best configuration in terms of size, price and assembly time.
```

---
## \#2 Posted by: Hummie Posted at: 2016-07-13T14:55:42.387Z Reads: 488

```

on vedder's site testing has been done by Ren and really there should be more caps than on there.  Without enough caps the inductance of the wires will slowly or quickly destroy the vesc.

The FOC program especially suffers from the inductance of the battery wires
```

---
## \#3 Posted by: onloop Posted at: 2016-07-13T15:25:04.426Z Reads: 491

```
The new upgraded vesc has two caps..

http://www.electric-skateboard.builders/uploads/db1493/original/2X/5/517173b0dd45c7c61695c04b241d5549e6ab5e6a.jpeg

The beauty of DIY is you can add more if you need them. Put on 10 and see if you get better results.
```

---
## \#4 Posted by: quanze Posted at: 2016-07-13T16:07:09.606Z Reads: 470

```
What's a cap :(
```

---
## \#5 Posted by: Hillso Posted at: 2016-07-13T16:08:37.963Z Reads: 462

```
capacitor
10chararar
```

---
## \#6 Posted by: Nordle Posted at: 2016-07-13T17:57:47.265Z Reads: 461

```
..but on the 6.0VESC they are much closer to the power stage..

@onloop just send them, as i said no problem with waiting. But if they come different as shown in the picture you lost 1 customer for the future. Already last time when i bought vesc from you, on your page they were shown with wires+cap soldered but they came without.:sleeping:
When i buy things from other sellers, things arrive like they are shown, or at least there is a decent hint which says something different.
```

---
## \#7 Posted by: furryfrog Posted at: 2016-07-13T18:26:00.719Z Reads: 450

```
Those caps look like they are on the battery power supply side, what do they do? Guessing  they are only for the brake regen charging?
```

---
## \#8 Posted by: Jinra Posted at: 2016-07-13T18:27:04.903Z Reads: 443

```
They "close the gap" for the battery to provide the VESC additional power on demand. Your battery cables may not seem long, but they are for the VESC.
```

---
## \#9 Posted by: Nordle Posted at: 2016-07-13T21:55:26.276Z Reads: 435

```
[quote="onloop, post:318, topic:4672"]
and most importantly more compact.
[/quote]

and please explain this. cause you still use the pcb and skip the middle cap from what ive seen on pictures. takes the same place in my eyes. just curious?
```

---
## \#10 Posted by: shawnh Posted at: 2016-07-13T22:04:34.012Z Reads: 434

```
My VESC's are here!  But they are not identical...
<img src="/uploads/db1493/original/2X/7/7fcf4fc628342732b203cad74b25b1ad32263c7c.jpg" width="500" height="374">
One cap / 2 caps.
I am building the Dual R-spec setup.  Should I be concerned?  or good to go.
```

---
## \#11 Posted by: flatsp0t Posted at: 2016-07-13T22:09:26.431Z Reads: 430

```
Just from the pics I have seen of them, I think they are larger diameter but shorter.
```

---
## \#12 Posted by: Lizardking0069 Posted at: 2016-07-13T22:14:21.042Z Reads: 427

```
Look at the uF values on the two vescs. If the two smaller ones add up to the same as the larger one then they are qeuivalent.
```

---
## \#13 Posted by: Nordle Posted at: 2016-07-13T22:15:32.980Z Reads: 428

```
No they aren't, but should be fine anyways. no guarantee dunno exactly
cause there are other values more important than Farad
```

---
## \#14 Posted by: onloop Posted at: 2016-07-14T00:39:35.005Z Reads: 430

```
This is what the first vesc looked like. One big cap.

http://vedder.se/wp-content/uploads/2015/01/pcb_back-1024x683.jpg
```

---
## \#15 Posted by: Skitzor Posted at: 2016-07-14T08:23:10.926Z Reads: 424

```
You can use the single big 3300µF and put the VESC's in Parallel to save some room in your build.
```

---
## \#16 Posted by: Nordle Posted at: 2016-07-14T08:32:51.731Z Reads: 414

```
But multiple small caps are way better. Cause ESR decreases and thats more important than our Farad number.
```

---
## \#17 Posted by: sismeiro Posted at: 2016-07-14T11:12:30.646Z Reads: 411

```
[quote="Nordle, post:341, topic:4672"]
Cause ESR decreases and thats more important than our Farad number.
[/quote]

Hi, can you explain what is ESR and why it's more important than the capacity? Thank you.
```

---
## \#18 Posted by: Nordle Posted at: 2016-07-14T11:58:48.560Z Reads: 405

```
Sry i can't.. [Equivalent series resistance - Wiki](https://en.wikipedia.org/wiki/Equivalent_series_resistance)
but i read alot trough ES and vedder's forum, and that is what they told me there when i asked about caps. and the guys there normally know what they say..
```

---
## \#19 Posted by: Aleendis Posted at: 2016-07-14T15:45:03.799Z Reads: 389

```
Simply spoken: It's the internal resistance in the capacitor. If you put resistors (with the same value) in parallel the resistance decrease.
If capacitors put in parallel the capacity adds up. 

So it's better to use more caps if a low esr counts.
```

---
## \#20 Posted by: sismeiro Posted at: 2016-07-14T16:06:21.229Z Reads: 393

```
Hi, I did my electrical engineering course some decades ago, so I'm a little rusty regarding some concepts.

I would understand the importance of the ESR if the capacitors were between the ESC and the motor since the current has several different frequencies.

But since the capacitors are between the battery and the ESC their main purpose is to accumulate energy and compensate the lenght of the cables, it shouldn't make any differente the ESR value.

Anybody can prove me wrong about my understanding. I have been proven wrong before and learned something new. :slight_smile:
```

---
## \#21 Posted by: Wolfwoof Posted at: 2016-07-14T16:50:16.746Z Reads: 367

```
Currently finishing up my EE degree and you're pretty much correct. The capacitors are there to prevent voltage droop of the battery when the current being drawn from the battery spikes. Also @Aleendis what you are talking about is actually called impedence and it works pretty much in the same way as resistance, but in reference to energy storage devices and motors (capacitors, inductors, batteries, etc.)
```

---
## \#22 Posted by: onloop Posted at: 2016-07-14T23:54:36.224Z Reads: 324

```
[quote="Nordle, post:343, topic:4672"]
but i read alot trough ES and vedder's forum
[/quote]

Reading is important.... but real world testing is the ultimate.....
```

---
## \#23 Posted by: Nordle Posted at: 2016-07-15T00:15:33.688Z Reads: 311

```
So you say, you testet the 50V caps under very hard circumstances on a 12S setup? Cause i heard caps are very sensitive to overvoltage. Another thing i only read, I believe then. No need to blow up things just because i want to test it. Also i don't have the money for that kind of fun.
But keep going on if that is your way of making buisness :sleepy:
```

---
## \#24 Posted by: onloop Posted at: 2016-07-15T00:18:56.978Z Reads: 308

```
[quote="Nordle, post:350, topic:4672"]
you testet the 50V caps under very hard circumstances on a 12S setup
[/quote]

No becasue I dont recommend 12S. 42v max for me.
```

---
## \#25 Posted by: Jinra Posted at: 2016-07-15T00:30:53.299Z Reads: 305

```
@onloop Is my 50v cap a manufacturing mistake? Would it be possible to get 63v caps as recommended by vedder?
```

---
## \#26 Posted by: Nordle Posted at: 2016-07-15T00:38:19.470Z Reads: 309

```
[quote="onloop, post:24, topic:6125"]
No becasue I dont recommend 12S. 42v max for me.
[/quote]
<img src="/uploads/db1493/original/2X/1/1e96157087fdb2ffd25c44351628daec188921b0.png" width="690" height="388">
you keep going on confusing me
```

---
## \#27 Posted by: Jinra Posted at: 2016-07-15T00:51:54.724Z Reads: 297

```
That's copied from Vedder's info, he didn't write it.
```

---
## \#28 Posted by: Nordle Posted at: 2016-07-15T00:54:05.140Z Reads: 299

```
But it's from his page. And it's written under his VESC description.
..oh and there are also pictures from VESC's with 3 caps..
```

---
## \#29 Posted by: onloop Posted at: 2016-07-15T01:13:58.407Z Reads: 296

```
[quote="Jinra, post:25, topic:6125"]
Is my 50v cap a manufacturing mistake
[/quote]

No mistake, it is a decision made by the engineers at the factory making the VESC, we needed to secure stock quickly to ensure production delays didnt continue to interrupt the schedule. In the end we sourced enough qty using a combination of Single 50v 3300uf & Dual 63v 1000 uf.

What voltage battery will you be running?

We have also designed a new CAP PCB for VESC, this concept is to simplify the setup of dual vesc, it has 4 holes for output wires making it much easier to run twin vesc from single cap board.
<img src="/uploads/db1493/original/2X/9/9f8c8c9044c307901036e749e0099afdc07653b5.png" width="407" height="500">
```

---
## \#30 Posted by: Jinra Posted at: 2016-07-15T01:18:03.399Z Reads: 285

```
This is for my friend's 6s build so I think I'll be okay. Just wondering if it was an error on the manufacturer's end.

Thanks!
```

---
## \#31 Posted by: onloop Posted at: 2016-07-15T01:21:02.603Z Reads: 288

```
[quote="Nordle, post:28, topic:6125, full:true"]
But it's from his page. And it's written under his VESC description...oh and there are also pictures from VESC's with 3 caps..
[/quote]

you have an eye for detail sir! 

this is a snippet from my t&c's http://www.enertionboards.com/pages/enertion-boards-terms-conditions.html

> TYPOGRAPHICAL ERRORS

> _Although Enertion Boards strictly monitors the contents of its website, errors do occur. In the event that Enertion Boards has incorrectly displayed a product's price, Enertion Boards reserves the right to cancel or refuse any orders placed on the product. Enertion Boards attempts to contact any customer where such an error has occurred. Enertion Boards reserves the right to offer solutions on a case by case basis. Enertion Boards does not guarantee the accuracy, correctness, or usefulness of information contained or associated with the site, such as, but not limited to, press releases, industry news, blog updates, or product descriptions and product photos. At the time of publishing such material, Enertion Boards attempts to make every effort to ensure that it is current and correct._
```

---
## \#32 Posted by: Jinra Posted at: 2016-07-15T01:23:58.116Z Reads: 268

```
On that note you have your belts listed as "265T" which I'm sure you meant to say "265mm" 😃
```

---
## \#33 Posted by: Nordle Posted at: 2016-07-15T01:25:17.650Z Reads: 272

```
[quote="onloop, post:31, topic:6125"]
Enertion Boards does not guarantee the accuracy, correctness, or usefulness of information contained or associated with the site, such as, but not limited to, press releases, industry news, blog updates, or product descriptions and product photos.
[/quote]

And that point will Nordle keep away from Enertionboards in the future. It's too easy to find a more reliable seller. My eye didn't catch this.
Thanks, but somehow pity.
```

---
## \#34 Posted by: onloop Posted at: 2016-07-15T01:26:10.349Z Reads: 263

```
please link to that page so i can check it out, thanks
```

---
## \#36 Posted by: Jinra Posted at: 2016-07-15T01:28:59.522Z Reads: 259

```
Here you go http://www.enertionboards.com/electric-skateboard-parts/pulleys-belts.html
```

---
## \#37 Posted by: Nordle Posted at: 2016-07-15T01:31:09.471Z Reads: 262

```
Can you tell me the capacitance and farad from this belt? :joy: I'm joking..
```

---
## \#38 Posted by: onloop Posted at: 2016-07-15T02:31:27.850Z Reads: 257

```
ok, got it, yeah it should say 256-55t
```

---
## \#39 Posted by: DeathCookies Posted at: 2016-07-15T06:46:38.645Z Reads: 253

```
Probably i could get a VESC with a cap only supporting 50v?
Well, i did not buy such a product and will have a big problem because i just ride on 12S.

Do you have an idea on how to handle my problem if i should get a 50V version of my 3 ordered and shipped ones?
```

---
## \#40 Posted by: sismeiro Posted at: 2016-07-15T08:23:03.162Z Reads: 248

```
Hi, if someone is not confortable with the capacitors delivered with the VESCs and have access to an electronic components store, just buy new ones and substitute them. I don't think is that expensive if someone feels better and thinks is the right thing to have.
```

---
## \#41 Posted by: DeathCookies Posted at: 2016-07-15T08:31:51.692Z Reads: 248

```
Well,
normally i wont complain it that much... but this time i am a bit mad...

One delay hunts the next delay ... ok, the VESC is fairly new and so on but @onloop could have told the costumer that they change something in the product! He did not.

Now i have payed for a product which i dont get as described. That is what i dont like. Now you tell me that i should take responsibility for others faults?

To put it in a netsheel: I am not totally freaking out. i am just a bit mad about the behavior!
```

---
## \#42 Posted by: Nordle Posted at: 2016-07-15T08:45:19.740Z Reads: 227

```
I feel with you! All the waiting, no problem. But this made me freak out! :imp:
```

---
## \#43 Posted by: onloop Posted at: 2016-07-15T15:36:19.118Z Reads: 216

```
[quote="DeathCookies, post:39, topic:6125"]
Do you have an idea on how to handle my problem
[/quote]

buy some 63v or 100v Caps from some nearby online electronics store & send me the bill.
```

---
## \#44 Posted by: Blasto Posted at: 2016-07-15T16:04:31.881Z Reads: 219

```
I really don't know people are getting upset here, @onloop is following his manufacturer's recommendations. I'm pretty dam sure the guy who proposed this recommendation is an electrical engineer. This modification should be trivial for you guys.
```

---
## \#45 Posted by: Radium73 Posted at: 2016-07-23T19:11:41.150Z Reads: 219

```
Got my VESCs yesterday and they've got 63v caps! First thing I checked out of curiosity after reading this, Jason apparently worked it out with the manufacturer very quickly! Or they have run out of 50v caps and now only have 63, so I think everyone should be alright.
```

---
## \#46 Posted by: dinodave Posted at: 2016-08-09T23:02:34.246Z Reads: 208

```
So would it be possible to get confirmation, hopefully from @onloop. If I have 63v capacitors on Enertion VESCs (which I do), am I safe to run 12S? 

Would be a nice bonus if true, as the specs on the Enertion site state 10S max, so I was aiming for 8S, but the motors can handle it, so if I can stick another 4S LiPo on there that would be great.
```

---
## \#48 Posted by: FredSaberhagen Posted at: 2017-04-27T22:16:52.625Z Reads: 144

```
incorrect... the impedance of a cap or inductor refers to resistance but also reactance "X" - the time-varying phase shift of the current or voltage it's resisting... that doesn't get "spent" in the form of heat.

The ESR or _Resistance_ is the actual resistive component of the inductance (think total Z = 1/jwC + ESR) or X + ESR

The ESR being high means, when you try to pull a lot of current, V=IR will be your voltage drop from the cap internals out the wire, to your VESC.  So if there was 0.1 ohm ESR and you tried to pull 10A out of a 40V cap, you would only "see" about 40V - 0.1(10) = 39V.  Imagine an instantaneous inrush of 100A and you lose 10V!

If you start combining a bunch of caps into one package or picking cheaper, larger values you typically have an increase in ESR which not only heats up your cap (shortening the life) but is less "real" - the capacitance isn't really at the voltage you want after it is burnt across the ESR.  The cap heating effect is why your capacitor has a **"ripple current" rating** meaning how much watts it can passively dissipate as it is constantly burning back and forth as current moves across it.  I doubt builders like Jason are measuring these values in their design.  Note that for every 10 deg C you increase the temp of aluminum electrolytic caps the lifetime is cut in HALF!

Definitely study up on reactance vs impedance vs resistance as you finish your EE degree as people love to ask this sort of shit in technical interviews ;-)
```

---
## \#49 Posted by: jaysoncena Posted at: 2017-04-28T09:51:17.478Z Reads: 133

```
Does that mean that multiple capacitor might be less preferred than a single, big capacitor because its will combine the ESR, increase the resistance between positive and negative and means an increase in voltage drop?

Sorry if its a stupid quesion.
```

---
## \#50 Posted by: FredSaberhagen Posted at: 2017-04-28T18:10:33.816Z Reads: 124

```
Multiple capacitor do "combine the ESR" as you say, but they combine in parallel meaning overall resistance goes down.

Imagine 1 guy with a pile of 100 snowballs VS 10 guys with a pile of 10 snowballs each.  Which would you rather get in a snowball fight with ;-)
```

---
## \#51 Posted by: jaysoncena Posted at: 2017-04-28T20:44:29.253Z Reads: 123

```
My bad, I'm not sure why I typed "increased" :) what I have in mind is reduced

So does that mean that bigger capacitor is better since its just a single capacitor or the ESR is relative to farad?

Sorry I have no idea about this. I only know the basics of resistors. Parallel is subtraction and series is addition :)
```

---
## \#52 Posted by: FredSaberhagen Posted at: 2017-04-29T01:57:49.684Z Reads: 121

```
Series may be addition but parallel is hell no subtraction (If I start with 1 ohm and put two more 1 ohm in parallel do I get negative resistance?  ;-) )

Bigger cap is better from an energy standpoint -  And you can always pay more money to get lower ESR for any given size cap - but if you could choose 1x660uF or 2x330uF , the 2x will probably deliver it more effectively (inductance is also a factor with long package leads and high di/dt).  The only reason to go single big package is cost.
```

---
## \#53 Posted by: jaysoncena Posted at: 2017-04-29T02:20:52.401Z Reads: 119

```
Ok, my bad again. Heh. But 2x1ohm in parallel is 0.5ohm. Is that right?

I should start reading more :)

But I appreciate your insight :thumbsup:
```

---
## \#54 Posted by: Marksmoura Posted at: 2019-04-27T23:03:05.665Z Reads: 33

```
Hello guys,

I've read many posts about caps as my vescs are the ones with a big cap instead of 3 smaller ones.

At the moment I would like to change my caps but I am wondering what is the typical Vue for a low esr for the vesc.

0.1ohm is what we should aim for? Lower? I'm trying to figure out what values I should be looking for.
```

---
