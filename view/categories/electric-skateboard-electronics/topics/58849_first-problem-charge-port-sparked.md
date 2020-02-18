# First problem - charge port sparked

### Replies: 24 Views: 862

## \#1 Posted by: Dook Posted at: 2018-06-14T10:03:03.038Z Reads: 222

```
Hey guys. 

Connected up all my electronics (without VESC) went to plug in the charger and had a massive spark. And the light on the charger started flashing red, so quickly disconnected and this was the result. See picture.

So my questions are:
Would that of damaged the BMS?
Based on the charger plug is the charger fried as well?
And, not being an expert but my guess is I had the charge port wired the wrong way round? 

Your help would be appreciated

Cheers
![image|375x500](upload://71YPkdQVqwO6RSzW4XiT3OfxsEk.jpeg)
```

---
## \#2 Posted by: Dook Posted at: 2018-06-14T10:10:23.472Z Reads: 214

```
FYI. I did plug the chargers into the port with the charger already connected to the mains? Should I of plugged into the port first then plug the charger into the mains?
```

---
## \#3 Posted by: rok Posted at: 2018-06-14T10:48:05.522Z Reads: 205

```
[quote="Dook, post:1, topic:58849"]
my guess is I had the charge port wired the wrong way round?
[/quote]

That probably. And no, it doesn't matter which end you plug in first.
```

---
## \#4 Posted by: Dook Posted at: 2018-06-14T11:41:57.034Z Reads: 194

```
So i should be good to go if require polarity on the port?

The charger seems to be untouched. Just have to rewire.
```

---
## \#5 Posted by: Namasaki Posted at: 2018-06-14T11:52:10.855Z Reads: 191

```
Always connect the charger to the charge port before plugging the charger in.
```

---
## \#6 Posted by: rich Posted at: 2018-06-14T14:03:21.371Z Reads: 167

```
Did you check polarity of charger/charge port before connecting to BMS?

[quote="Namasaki, post:5, topic:58849, full:true"]
Always connect the charger to the charge port before plugging the charger in.
[/quote]

When I do it like that it always sparks, when connecting the main power first it never sparks.
```

---
## \#7 Posted by: b264 Posted at: 2018-06-14T14:06:43.102Z Reads: 160

```
[quote="Namasaki, post:5, topic:58849, full:true"]
Always connect the charger to the charge port before plugging the charger in.
[/quote]

What is the reason?
```

---
## \#8 Posted by: Skunk Posted at: 2018-06-14T14:15:40.414Z Reads: 153

```
I too wanna know the answer to this.
```

---
## \#9 Posted by: Namasaki Posted at: 2018-06-14T15:10:17.813Z Reads: 146

```
better to make the connection while the charger is not energized.
```

---
## \#10 Posted by: Namasaki Posted at: 2018-06-14T15:10:57.123Z Reads: 146

```
[quote="rich, post:6, topic:58849"]
When I do it like that it always sparks, when connecting the main power first it never sparks.
[/quote]

I never get sparks connecting the charge port first
```

---
## \#11 Posted by: SORRENTINO Posted at: 2018-06-14T15:14:48.982Z Reads: 141

```
Depends on your BMS....My BMS the charge port is always live so if I plug in my charger to port first I get a big arc. Guess how I found that out :slight_smile:
```

---
## \#12 Posted by: Dook Posted at: 2018-06-14T17:11:30.403Z Reads: 136

```
Hey Rich, yes I did, I posted the results on my build feed (Little Bro Trampa build) Negative on the outside L shaped pin and the positive to the other outside pin with the middle pin unused.

Shall I try again but connect the charger to the mains last?

![image|666x500](upload://ynIl7EyQGjypc8RW1RS2VbLbBFF.jpeg)
```

---
## \#13 Posted by: Dook Posted at: 2018-06-14T17:13:20.965Z Reads: 131

```
Oh and maybe you are on to something as it sparked when plugging into port, and soaked again when unplugging from port whilst charger still plugged into mains
```

---
## \#14 Posted by: mccloed Posted at: 2018-06-14T17:21:12.387Z Reads: 128

```
There's your problem. If you followed the illustration above, it was wired in reverse. The middle tab will need to be positive(+). Unfortunately, you probably fried your charger. :disappointed: We had a couple 8s batteries we accidentally had reversed and the chargers did not work afterwards.
```

---
## \#15 Posted by: SORRENTINO Posted at: 2018-06-14T17:24:01.614Z Reads: 129

```
You always need to verify with your multimeter!!!!!
```

---
## \#16 Posted by: Dook Posted at: 2018-06-14T17:37:09.060Z Reads: 126

```
The red light was still flashing on the charger after I disconnected from the port. Do you think it’s fried? 

Will rewire and see what happens.
```

---
## \#17 Posted by: Dook Posted at: 2018-06-14T17:38:09.988Z Reads: 128

```
Yes I did this and got confirmation from guys on my build feed, so that’s why I was confused as to why it sparked
```

---
## \#18 Posted by: Dook Posted at: 2018-06-14T17:40:20.100Z Reads: 128

```
But the middle tab on the diagram is positive?
```

---
## \#19 Posted by: b264 Posted at: 2018-06-14T17:48:12.541Z Reads: 122

```
Verify with a multimeter...
```

---
## \#20 Posted by: SORRENTINO Posted at: 2018-06-14T17:54:35.470Z Reads: 118

```
If you verified with a multimeter you wouldn't be asking this question. You also should verify the plug on your charger. :thinking:
```

---
## \#21 Posted by: Dook Posted at: 2018-06-14T17:56:11.166Z Reads: 109

```
Oven just bought a charge port with just the 2 pins to be safe. Will get that in a couple of days and try again. Cheers for your advice 👍🏼
```

---
## \#22 Posted by: Namasaki Posted at: 2018-06-14T18:19:53.214Z Reads: 100

```
Good point. 
My bms has on/off switch so both the charger and port are cold when I connect
```

---
## \#23 Posted by: mccloed Posted at: 2018-06-14T18:45:01.342Z Reads: 97

```
I mean the middle portion of the charge port that meets up with the middle of the charger plug. It's is the "L" shaped tab, usually.(see below) The red light would just blink on the the chargers we killed, also.
![recharge-port|390x500](upload://jgPKXea8lzjiIIamjpqSbV92qXm.jpg)
```

---
## \#24 Posted by: buildityourself Posted at: 2018-12-30T02:41:56.917Z Reads: 68

```
Where did you get your 2 pin charge port? How did you wire it and how do you like it?
```

---
