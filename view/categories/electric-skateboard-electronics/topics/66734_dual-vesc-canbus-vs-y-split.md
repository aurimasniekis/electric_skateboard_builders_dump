# Dual VESC: CANBUS vs Y split

### Replies: 22 Views: 994

## \#1 Posted by: janpom Posted at: 2018-09-01T07:36:51.003Z Reads: 205

```
I'm planing on upgrading to dual drive and I'm researching how things should be connected. As I understand, there are at least two options:

1. Set up the VESCs as master and slave, and use the CANBUS port to connect them.
2. Split the signal from the remote receiver (Y split). Have the same config for both VESCs then.

CANBUS pros:
- Traction control. If one of the wheels looses traction, the interconnected VESCs can figure it out and adjust the spin of the other wheel.
- Realtime data can be read from both VESCs over single USB.

CANBUS cons:
- less reliable
  - If the master VESC dies, the slave VESC has no input signal and can't work. Problem if going downhill since brakes won't work on any of the two motors.
  - Can fry a VESC if not connected correctly. I have seen a few mentions on the forum that you should never connect the CANBUS when only one of the two VESCs is power up since it will fry the VESC.

Does this sound correct? Are there other pros/cons?

Also, what exactly is the issue with having only one of the CANBUS connected VESCs powered up? Does the problem also apply when one of the VESCs dies? I mean, does it mean that if one of the VESCs gets fried, the CANBUS will take the other VESC down with it?

And last question: If the two VESCs are not the same, does that change anything? For example, I have the ESCape. I think I'll just get another one, but I'm also considering the FlipSky 6.6. With the Y split, could it happen that the two different VESCs will interpret the input signal slightly differently and one will spin the wheel faster than the other one? Would that be any better with CANBUS?
```

---
## \#2 Posted by: DeathCookies Posted at: 2018-09-01T08:02:39.881Z Reads: 189

```
Did you already read these topics before you created another one?
https://www.electric-skateboard.builders/t/question-on-can-vs-split-ppm/52443
https://www.electric-skateboard.builders/t/dual-motors-vesc-remote-receiver-ppm-y-splitter-vs-can-bus-via-vescs/65903
https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461
```

---
## \#3 Posted by: dareno Posted at: 2018-09-01T09:01:34.624Z Reads: 167

```
Here we go round again!!   😂
```

---
## \#4 Posted by: DeathCookies Posted at: 2018-09-01T09:30:21.908Z Reads: 164

```
If i had more rights i would have closed this thread 😅
```

---
## \#5 Posted by: janpom Posted at: 2018-09-01T10:00:40.509Z Reads: 163

```
I didn't and I'm sorry. Should have done more searching. Thanks for the links.
```

---
## \#6 Posted by: Wraith Posted at: 2018-09-01T10:06:27.014Z Reads: 157

```
Those are some lengthy back and fourths :sweat_smile: now I’m more unsure than before I started (havent reached the end of the threads yet lol)
```

---
## \#7 Posted by: janpom Posted at: 2018-09-01T10:26:07.596Z Reads: 155

```
Well, I read through those topics now, but I mostly learned what I already knew, i.e.
- CANBUS = more features
- Y-SPLIT = redundancy, less prone to frying (as long as you only split the signal wire)

Unfortunately, I still didn't find the answers to:

[quote="janpom, post:1, topic:66734"]
Also, what exactly is the issue with having only one of the CANBUS connected VESCs powered up? Does the problem also apply when one of the VESCs dies? I mean, does it mean that if one of the VESCs gets fried, the CANBUS will take the other VESC down with it?

And last question: If the two VESCs are not the same, does that change anything? For example, I have the ESCape. I think I’ll just get another one, but I’m also considering the FlipSky 6.6. With the Y split, could it happen that the two different VESCs will interpret the input signal slightly differently and one will spin the wheel faster than the other one? Would that be any better with CANBUS?
[/quote]
```

---
## \#8 Posted by: Andy87 Posted at: 2018-09-01T10:35:11.859Z Reads: 149

```
As far as I know the Flipsky 6.6 don’t have any issues with disconnecting CAN wile operating.
With all the new dual vescs you also don’t get any problems as the CAN bus is hard wired via pcb.
```

---
## \#9 Posted by: Skunk Posted at: 2018-09-01T10:36:38.875Z Reads: 147

```
I've read both those threads like three times and I still don't know if I'm going CAN or split
```

---
## \#10 Posted by: Andy87 Posted at: 2018-09-01T10:39:35.564Z Reads: 146

```
Just go CAN and good. One way no questions 😜
```

---
## \#11 Posted by: hoeksame1 Posted at: 2018-09-01T13:08:37.620Z Reads: 145

```
I have canbus with dual 192kv 10s. A beast! 
Its super! No problem with canbus. I connected splitter but one motor was more delayed.. ( maybe i did something wrong xD) also when i go offroad,  trsction controle is super Nice in the dunes! :slight_smile:
```

---
## \#12 Posted by: longhairedboy Posted at: 2018-09-01T13:26:17.786Z Reads: 139

```
CAN bus all the way. Split ppm exibits annoying behavior on the street in my opinion. 

also if you do things in the right order you don't have to worry about it. 

1) connect CAN bus leads, 
2) connect both VESCs to power supply while it is still off
3) power on 
4) configure 
5) enjoy

@blasto correct me if i'm wrong but didn't Enertion already fix the "only one CANBUS device powered on so let's blow the other CAN controller" issue in the focboxes? It seems like i would have accidentally blown more focboxes by now if they hadn't.
```

---
## \#13 Posted by: linsus Posted at: 2018-09-01T13:29:03.722Z Reads: 134

```
Indd, CAN all the way.
Last time I had this discussion, we concluded that there can be ground loops present in the splitt ppm scenario. Which isnt good.

I'm not sure how you fry a vesc thru CAN if you're only using the data lines between them :sweat_smile:
```

---
## \#14 Posted by: Wraith Posted at: 2018-09-01T13:30:43.574Z Reads: 128

```
And that’s that. Please mark this as solved so I can just decide already on can bus :laughing:
```

---
## \#15 Posted by: 12meterkuk Posted at: 2018-09-01T15:19:52.819Z Reads: 115

```
I’ve blown 2 focboxes like that already, issue is definitely not fixed. Had to desolder the campus chips and run split ppm
```

---
## \#16 Posted by: kuphjr Posted at: 2018-09-01T17:38:29.001Z Reads: 111

```
I just blew a FOCBox using canbus and it was a FOCBox purchased less than 3 months ago. You have to consider the situation in which the canbus cable comes loose while riding.

Also, I have never experienced a single issue with split ppm and I have noticed no difference with or without traction control.  That's my 2 cents, but really if you go with canbus just put a dot of hot glue on each connection and don't screw with it unless all power is disconnected.
```

---
## \#17 Posted by: Trdolan03 Posted at: 2018-09-01T18:00:06.097Z Reads: 109

```
[quote="hoeksame1, post:11, topic:66734"]
also when i go offroad, trsction controle is super Nice in the dunes!
[/quote]

I want to see this board
```

---
## \#18 Posted by: skatardude10 Posted at: 2018-09-01T18:23:58.364Z Reads: 105

```
Hot glue on the connections so they don't come out... Good advice.
```

---
## \#19 Posted by: kuphjr Posted at: 2018-09-01T18:28:02.969Z Reads: 106

```
Maybe, I only ride street so I guess I should have mentioned that.
```

---
## \#20 Posted by: Taliesin Posted at: 2018-09-03T17:35:48.947Z Reads: 87

```
All due respect @DeathCookies

Yes I did see those threads.

And 

I bet you a year from now someone else will be googling and searching for similar questions and answers and will stumble upon this thread and find some info that will help them solve their problem.

I see this all the time on other forums where someone gets upset that someone else made a post asking a question that’s similar to a thread that has been made in the past but yet that ends up being the thread with the most helpful answer for someone in the future. And I roll my eyes.

There’s a difference between invasive spam posting and people actually just trying to learn and ask questions.

By saying you want to close the thread because your upset that there is another similar thread make sure me think you should just leave the forum. No offense.
```

---
## \#21 Posted by: DeathCookies Posted at: 2018-09-03T19:36:54.948Z Reads: 77

```
Maybe the people should just ask these questions in one thread instead of making multiple threads and spreading the Information on the forum.

The Best approach would be that people are searching first and if they cannot find the answers they are looking for to ask in the Best matching thread.

Just my opinion. No offense taken

Edit : I suggested to closed this thread. Well, it would be better to merge it. My fault
```

---
## \#22 Posted by: Taliesin Posted at: 2018-09-03T19:45:11.685Z Reads: 75

```
I can agree with merging. 

I felt I didn’t see a specific enough answer for my question in the other threads and there’s a lot of back and forth on what the right thing is to do, as well as being older threads, there may be more up to date knowledge by re hashing an older topic with newer knowledge.

But I agree, mods could totally merge threads and just mark them with a date showing the most recent activity and that could be really helpful.
```

---
