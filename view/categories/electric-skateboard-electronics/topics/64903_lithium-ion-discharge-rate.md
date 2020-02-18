# Lithium ion discharge rate

### Replies: 16 Views: 698

## \#1 Posted by: SquidKingRabbit Posted at: 2018-08-15T01:03:36.843Z Reads: 170

```
Hi so I have been reading and looking around for lithium ion battries discharge rate and found it to be 1c. 

So am I right to say that a 7s4p 8.8mah lithium ion battery pack is able to discharge 61.6amps (7 x 8.8) continuous?
```

---
## \#2 Posted by: Michael319 Posted at: 2018-08-15T01:56:15.129Z Reads: 166

```
All lithium ion batteries have a designated discharge. (I'm no expert so please correct me if I'm wrong.)

Lets say each cell is rated for 15A continuous. I believe Samsung 30Q 18650s are this. They can't actually output anything near that. The most I've seen out of mine is ~9A per cell peak. Most of the time it seems to be sitting around 3-6A. So take that into consideration.

Using that knowledge you can multiply those numbers by the parallel number in your battery config. Let's say a 7s4p like you said. That would be about ~20A continuous with ~36A peak.
```

---
## \#3 Posted by: SquidKingRabbit Posted at: 2018-08-15T05:42:42.809Z Reads: 138

```
Thanks for your reply, I am not sure of the cells I am using. They are Chinese battery packs. Is there a way to find out?
```

---
## \#4 Posted by: Acido Posted at: 2018-08-15T06:07:31.185Z Reads: 128

```
Thats total crap how many amps did you pull?
What are your esc specs or vesc setting

@SquidKingRabbit each cell has its own discharge rate, the higher the capacity the lower the discharge rate usually
The best choice with li ion is Samsung 30q for smaller packs and 35e for larger (5p+)
```

---
## \#5 Posted by: Acido Posted at: 2018-08-15T06:11:27.434Z Reads: 118

```
You can rip apart the shrink wrap and see usually theres the brand and model written on the cells
```

---
## \#6 Posted by: Andy87 Posted at: 2018-08-15T06:45:52.962Z Reads: 111

```
You made a wrong calculation here.
Of you have a 4p 8.8ah pack one cell will be 2.2ah. If your cells can handle 1c than it is 2.2ah*1c= 2.2a per cell or with 4p 8.8a in total.
The more parallel groups or capacity the more current your batteries can handle as the current split between the parallel groups (not between serial connections like you calculate).
Like @Michael319 and @Acido said, Samsung q30 are good cells for esk8. They have a discharge rate around 20a so in your case with 4p up to 80a continues which is very good for a dual setup
```

---
## \#7 Posted by: SquidKingRabbit Posted at: 2018-08-15T16:57:35.996Z Reads: 91

```
Pulled about max 35amps from my 7s2p with LGEAMF11865 cells.

Pulled about max 31amps from my other 7s2p with FST 18650-2000mah cells.

My VESC is set to battery max 50a and motor max 70a. I have always ran the board with just a 7s2p but recently have decided to just put the 2 packs in parallel. But it seems that the cells are different and that would pose to be a problem, right? 

Anyway I am still not sure of the discharge rate of the individual cells. 

For the LG, the specs are as follows for the discharge rate: 430mA Standard 10000mA Maximum, which translates to what C rating?

For the FST, the specs are as follows for the discharge rate: Max. continuous discharge current: 3000mA, which translate to what C rating?
```

---
## \#8 Posted by: SquidKingRabbit Posted at: 2018-08-15T17:00:56.052Z Reads: 76

```
![photo_2018-08-16_00-59-46|666x500](upload://b8rn8ybqngv2lGvrOvh322CrO7E.jpg)![photo_2018-08-16_00-59-48|666x500](upload://bLIDITw8Vspyh2vIxxaHf1xv4gV.jpg)
```

---
## \#9 Posted by: SquidKingRabbit Posted at: 2018-08-15T17:03:52.882Z Reads: 74

```
Oh I see. Thanks for clearing it up! Maybe I will look into getting some Samsung q30 in the future. But for now, I will just stick with what I have and make the best out of it
```

---
## \#10 Posted by: bartroosen12 Posted at: 2018-08-15T17:19:25.247Z Reads: 74

```
Your pack uses the LG MF1 which can handle like max 15A continues but they will have a huge voltage sag. 5A - 10A should be fine
I should say for your 7S4P like max 50A.
```

---
## \#11 Posted by: SquidKingRabbit Posted at: 2018-08-15T17:59:31.530Z Reads: 70

```
Hey thanks man! So I am able to connect the 2 packs in parallel even with different cells?
```

---
## \#12 Posted by: bartroosen12 Posted at: 2018-08-15T18:04:32.839Z Reads: 65

```
Oow I didn't red your previous message.
I shouldn't connect 2 different kind of batteries in parallel but you can try.
```

---
## \#13 Posted by: SquidKingRabbit Posted at: 2018-08-15T18:06:41.986Z Reads: 60

```
I will take a look when I have more time. Thanks a bunch though!
```

---
## \#14 Posted by: bartroosen12 Posted at: 2018-08-15T18:09:38.084Z Reads: 60

```
The FST cells have a max discharge rate of 8A so it's not pretty good to mix batteries.
```

---
## \#15 Posted by: Michael319 Posted at: 2018-08-15T18:30:12.114Z Reads: 52

```
I have a 12s2p 30Q pack. I've never seen more than 20A in my data.

Although that was when it was discharging through the bms. I just recently bypassed it but my Bluetooth module died so I don't have any data.
```

---
## \#16 Posted by: pat.speed Posted at: 2018-08-16T11:10:20.559Z Reads: 41

```
Just because you only pull 9a max doesn’t mean you can’t pull more. I think either your settings limit the discharge to this rate or you just don’t ride hard enough to pull any more. 

The 30q is tested to 20a max cont. This means it can discharge at any rate in this range. The cell doesn’t dictate how much current it puts out, the Vesc and motor do
```

---
