# A Few Questions Before I start Buying Parts

### Replies: 6 Views: 600

## \#1 Posted by: Actungz Posted at: 2017-08-03T01:08:32.419Z Reads: 65

```
Hi guys just found out this forum 2 days ago and I've been doing a lot of research ever since. I've never been much into skateboards in my teenage years (I just walked and commuted for the most part), but recently I've gotten more and more interested in building something myself and learning more about electronics and how they work.

However before I fully commit I'm still confused about the following:

1) Does it matter if you mount the motor in the front or back? I imagine if you make it RWD it would be easier to turn, but wouldn't it be more dangerous if it slips compared to FWD?

2) When I connect 2 4s batteries together, do they become an 8s battery? Does it matter if they are in series or parallel?

3) I see some people say xSxP, does the s mean they connected the batteries in series and p means in parallel?

4) Is there a way to test if the motor is working without an ESC and battery? Or do you need all three together before testing

5) If I want to have a dual motor set up in the future can I run both off one ESC? Assuming I get a high Amp enough one.

6) Does the ESC come with a switch? and if I want to control it  I need to get a new rc receiver, correct?

7) Are you able to control the acceleration like in a car? By that I mean are you able to "half press" the accelerator on your remote.

8) Is it a good idea to make your housing ventilated? I'm scared water might get in and ruin the electronics.

9) Is the consensus that lithium ion batteries are safer than 18650 batteries? In either case would I need a BMS to charge the battery?

10) Btw do you guys wear helmets and gear while riding? Just curious cause 25+mph seems pretty dangerous.

11) Do you guys ride on Rainy days? If so what do you do to prevent water damage.

12) Last question, do you guys ride on sidewalks or on the street?

For my first project I think I'm going to buy most of the parts besides the drive train on aliexpress and other cheaper sources first. If I end up satisfied with my abilities then I would upgrade parts gradually and make the board more unique.

Thanks everyone I must admit I am pretty clueless when it comes to DIY stuff, and I'm really looking forward to learn from this community.
```

---
## \#2 Posted by: DilatedPupils Posted at: 2017-08-03T01:12:55.936Z Reads: 58

```
Welcome to the forum. Everything that you need to know is here. There's a search button on the upper right corner, you should utilize that. I myself didn't buy my stuff for my first build until after like 6 months of reading.
```

---
## \#3 Posted by: Actungz Posted at: 2017-08-03T01:17:58.677Z Reads: 56

```
Thanks!! I've been reading a lot of the beginners guide already :). It's just I find it a bit confusing to navigate the site when I have some specific questions. Like I don't see people asking where to mount the motors or if people wear helmets when they ride. How can I search for topics that are not included in the title?
```

---
## \#4 Posted by: Hummie Posted at: 2017-08-03T01:27:17.463Z Reads: 59

```
1 I like front drive more for reasons but either works similarly. No prob
2 if u make them a chain series or beside each other parallel
3yes
4 u can test w an inductance meter or even spinning by hand while all phases shortedto some degree
5 one esc per motor
6 no switch but xt90s plug is easy. Yes get a trans and received and get a reliable one for safety. 
7 for sure. All programmable
8 depends how hot u get but there's a temp shutdown on vesc so no worry there
9 ion are often in 18650 size. Iron is even safer. U can get away without a BMs if u read up
10 helmet almost always and pants and a couple layers over the elbows
11 never in rain for me
12. Street always.
```

---
## \#5 Posted by: Jinra Posted at: 2017-08-03T01:35:34.770Z Reads: 57

```
[quote="Actungz, post:1, topic:29517"]
1) Does it matter if you mount the motor in the front or back? I imagine if you make it RWD it would be easier to turn, but wouldn't it be more dangerous if it slips compared to FWD?
[/quote]

RWD better traction for acceleration. FWD better traction for braking. I use RWD myself and don't really slip much. If I really try and brake super hard I can get it to skid a tiny bit, not really a problem though. You can use dual diagonal as well.

[quote]
2) When I connect 2 4s batteries together, do they become an 8s battery? Does it matter if they are in series or parallel?
[/quote]

8s if its in series, 4s with twice the mAh if in parallel. Parallel will also double the discharge potential of the pack.

[quote]
3) I see some people say xSxP, does the s mean they connected the batteries in series and p means in parallel?
[/quote]

correct

[quote]
4) Is there a way to test if the motor is working without an ESC and battery? Or do you need all three together before testing
[/quote]

You need an ESC and battery of at least 8v (for the VESC)

[quote]
5) If I want to have a dual motor set up in the future can I run both off one ESC? Assuming I get a high Amp enough one.
[/quote]

No 1 ESC per motor.

[quote]
6) Does the ESC come with a switch? and if I want to control it  I need to get a new rc receiver, correct?
[/quote]

Some do, the only ESC I recommend (the VESC) does not. Vedder anti-spark switch, loop key, or DIYES switch are popular choices. You will need a PPM/UART/ADC compatible receiver/controller

[quote]
7) Are you able to control the acceleration like in a car? By that I mean are you able to "half press" the accelerator on your remote.
[/quote]

Yes, most common control modes are current control (VESC) or duty cycle (most hobby ESCs as well as VESC). Current control mode is superior IMO. In current control, throttle controls acceleration not speed. This means that half throttle does not mean half speed.

[quote]
8) Is it a good idea to make your housing ventilated? I'm scared water might get in and ruin the electronics.
[/quote]

Good idea? sure if you don't mind dust and a non water-proof board. Needed? Nope, I run both my boards without ventilzation. Keep your voltage high (10s or higher) and gearing loose (2.4:1 or higher) and your heat should be low

[quote]
9) Is the consensus that lithium ion batteries are safer than 18650 batteries? In either case would I need a BMS to charge the battery?
[/quote]

18650 batteries ARE lithium ion batteries. Lipo (lithium polymer) as also technically lithium ion batteries. You're probably talking about lipo pouches vs 18650 cells. Cells are safer, but provide less discharge current, and have higher energy density for its weight. Lipos have drastically higher discharge potential, but are less energy dense and can be dangerous if mishandled.

[quote]
10) Btw do you guys wear helmets and gear while riding? Just curious cause 25+mph seems pretty dangerous.
[/quote]

I wear a TSG Pass. I would only recommend full face helmets for esk8 above 20mph.

[quote]
11) Do you guys ride on Rainy days? If so what do you do to prevent water damage.
[/quote]

Foggy and humid, yes. Rainy, no. It has less to due with fear of electronics and more to do with loss of traction and dealing with cleaning the board and making sure the metal parts don't rust.

[quote]
12) Last question, do you guys ride on sidewalks or on the street?
[/quote]

Where-ever a bike would go, mostly streets and bike trails.
```

---
## \#6 Posted by: Actungz Posted at: 2017-08-03T01:51:38.569Z Reads: 38

```
Thank you guys so much!! I'll keep these answers in mind, and hopefully I'll be able to come up with a build plan by the end of this week.
```

---
