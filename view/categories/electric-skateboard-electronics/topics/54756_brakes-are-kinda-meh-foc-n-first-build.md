# Brakes are kinda meh&hellip; FOC n first build

### Replies: 16 Views: 771

## \#1 Posted by: accrobrandon Posted at: 2018-05-08T01:47:56.684Z Reads: 201

```
so first build... posting topics as questions arise and reading through past post... so upgraded to FW to 3.x 
6355 matech 190kv
and currently a 10s2p ebay battery with the lg amf cells... (until my cells arrive from nkon for a 4s build)

so these are current settings let me know if you need more info... 

at any rate all i have is a meepo to base my experience on... this is a single drive for now 15mm belt.

braking at low speed and casual cruise is good...but if i try and go into the "fast" realm braking is real slow till it slows down. basically if I REALLLLLY needed to stop once i was going fast it would be bad news...

braking at low speed on a hill was acceptable, however once the board comes to a general stop the motor doesnt lock in place and prevent any further roll...something, once again, i am only familiar with having owned a hub drive.

apples to apples as far as speed is concerned (unmeasured just a feel) my meepo brakes better at what i feel would be a similar speed. Is this what a single belt offers vs dual belt... am i expecting to much because it was a dual hub meepo vs single belt OR?? my weak ass baby battery? =/

i have yet to try bldc mode to what that offers in comparison... but a newbie here trying to work things out

thx!

![25 PM|690x431](upload://wxtbEubaPzi8hZojmLDNaz7co6I.png)
![51 PM|690x431](upload://6m7OxH8t8Bxrfa06erhL95abVy7.png)

![50 PM|690x431](upload://iq87ljqNKBtewpyy9c6wcuqgH8O.png)
```

---
## \#2 Posted by: MysticalDork Posted at: 2018-05-08T02:01:37.085Z Reads: 171

```
The high-speed braking issue is mostly due to your battery regen current (8A currently). If you get a battery that can handle a higher charge current and you set the vesc accordingly, that will improve your high-speed braking.
```

---
## \#3 Posted by: accrobrandon Posted at: 2018-05-09T02:35:33.901Z Reads: 145

```
woudl you say that 8 is an appropriate value for the given battery or could it be a tich higher with out any major issues?
```

---
## \#4 Posted by: myreala Posted at: 2018-05-09T02:42:30.706Z Reads: 144

```
Increase motor current max brake to -70  or -80 if you feel the brakes are too weak, see is that makes a difference. -8A battery regen would be the max i would be comfortable with on a 2p. 
Also on vesc brakes dont lock completely like Meepo.
```

---
## \#5 Posted by: Mikenopolis Posted at: 2018-05-09T03:06:37.239Z Reads: 131

```
Sorry to hijack the thread. But hoping to get some input from @myreala and @MysticalDork 

Any recommendation on my 12s3p 30q dual 6374 bldc uncensored build? I was testing it with the following setting, went maybe 10mph and engaged the brakes, it was smooth slow down then suddenly jolts to a stop and threw me off (I was prepared for it) tried it a few more time and still did the same weird braking. 

Here are my current settings
Motor Max: 60
Motor Min: -60
Batt Max: 30
Batt Min: -12
Start Cutoff: 36
End Cutoff: 33.60
```

---
## \#6 Posted by: myreala Posted at: 2018-05-09T03:25:50.841Z Reads: 118

```
Okay first of all you should not have Bat Min at -12 for a 3p in dual config. Each motor would be putting -12A back in battery, which is double of max recommended. This won't cause throwing you off but it definitely needs to be fixed as this can cause problems with your battery pack. Shorten the life, maybe even cause fire, idk? 

Next for the actual fix try to change your motor min to -30 on both vescs and start testing. Go higher if the braking is too week. I usually stay at -30 each motor for smooth braking.
```

---
## \#7 Posted by: Deckoz Posted at: 2018-05-09T19:57:57.241Z Reads: 96

```
[quote="myreala, post:6, topic:54756"]
Okay first of all you should not have Bat Min at -12 for a 3p in dual config. Each motor would be putting -12A back in battery, which is double of max recommended
[/quote]

30q is fine to charge at 2c

3ah * 3p * 2c  = -18a or -9/ESC...

Not quite double...

As far as the low speed braking in FOC you need to change the Minimum ERPM before full brake(same for unsensored bldc) Has nothing to do with the current at 1-3mph.. @Mikenopolis but it will still be there barely. In order to get completely smooth you have to adjust min from before full brake and be using sensors.
```

---
## \#8 Posted by: Mikenopolis Posted at: 2018-05-09T20:13:43.803Z Reads: 91

```
I just “finished” the board. Sensor detection failing on one of the motors. Solution TBD. So it’s BLDC Sensorless at the moment. Staying away from FOC with the 12s pack.

I changed the batt min to -8 and took out the dual receivers and did canbus instead. Everything works as it should now. So I think it might have been the dual receivers causing a problem.
```

---
## \#9 Posted by: myreala Posted at: 2018-05-09T20:17:09.588Z Reads: 84

```
Can you give me a source on 2C, I couldn't find anything in a quick search? AFAIK the Fast charge current for 30Q is 4A.
```

---
## \#10 Posted by: Deckoz Posted at: 2018-05-09T20:18:15.333Z Reads: 83

```
Interesting.. 

Anyway one of your sensors is failing detection? If you know your sensor order you can put the reverse sensor readouts into the other motor( I assume they are the same motors just flipped 180 degrees and spinning the opposite driection)

Bldc hall table is very...simple(-6 to +6 values) compared to the scale in FOC(-255 to +255), so it's easy to plug in the numbers in reverse if you are having issues with detection.

Once you plug in the reverse hall numbers you can go-to the real time tab and spin the motor by hand to verify the phases are reading position correctly.
```

---
## \#11 Posted by: accrobrandon Posted at: 2018-05-29T02:56:07.518Z Reads: 67

```
[quote="Mikenopolis, post:8, topic:54756"]
dual receivers
[/quote]

Was this actual dual reciever or split ppm? I'm getting all my dual gear this week.. And was feeling the non-can bus route from what ive been reading... Next stop is to find a good thread on vesc settings for non canbus .... Ideas?
```

---
## \#12 Posted by: ROFEN13 Posted at: 2018-05-29T03:06:13.148Z Reads: 65

```
Just half any max value. I am running split ppm with a 12s4p of 25r and have...
Max motor 40
Min motor-40
Batt max 20
Batt min -8
It works really well for me
```

---
## \#13 Posted by: accrobrandon Posted at: 2018-05-29T03:29:06.163Z Reads: 57

```
good info thanks... so what would be your recommended values for a 10s4p of PF cells?

i think 30-40 will be cool on the motor side... battery max 20 if theyre rated at 10amps each cont. its the regen value that throws me off...

for yours tho...couldnt yur batt max be higher? arent 25r rated at 20amp each?
```

---
## \#14 Posted by: Mikenopolis Posted at: 2018-05-29T03:40:10.149Z Reads: 54

```
The dual receivers was my newest setup that didn’t quite work out. Not sure what it was but going to canbus “solved” my issue. 

I’ve used splitt ppm not my other three builds without a problem. I just didn’t have the necessary cable to do split ppm this time around because Enertion decided to solder on the receiver wire
```

---
## \#15 Posted by: accrobrandon Posted at: 2018-05-29T03:42:31.766Z Reads: 54

```
[quote="Mikenopolis, post:14, topic:54756"]
Enertion decided to solder on the receiver wire
[/quote]

yeah, i got focboxes i was thinking this would work though...no?

https://www.ebay.com/itm/161856282994?_trksid=p2334524.m570.l5999&_trkparms=gh1g%3DI161856282994.N36.S1.R1.TR2
```

---
## \#16 Posted by: Mikenopolis Posted at: 2018-05-29T03:45:21.178Z Reads: 50

```
It was a female vs male issue and I just didn’t have any more servo cables to splice together and had canbus. Never had a problem with either way
```

---
