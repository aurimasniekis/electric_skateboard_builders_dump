# Would a 12s3p result in more range compared to a 10s3p?

### Replies: 10 Views: 288

## \#1 Posted by: Ultimiant Posted at: 2019-07-25T20:26:56.548Z Reads: 117

```
Currently I'm deciding between 2 batteries. Im almost certain my enclosure can fit a 12s3p and it can guaranteed fit a 10s3p, but sadly not a 10s4p :frowning:. I'm not going to be doing any uphill runs or going at super high speed as its a board for carving but I want to get as much range as possible out of my board and stuff as many batteries in it as possible. I've read a lot that 12s batteries can stress the components of a VESC (Im using the Flipsky 6.6 dual) and I was wondering if I could have a 12s3p but still program my VESC to pull the same amount of power as if it were a 10s battery. I assume that I would be pulling less current from each cell and therefor would get more range out of the pack while reducing voltage sag at the same time. 

Basically can I use a 12s setup to get an extra 6 cells in my setup and increase my range but not power.

Is my thinking right on this?
```

---
## \#2 Posted by: Chaki Posted at: 2019-07-25T20:41:20.548Z Reads: 110

```
Let's say Samsung 30Q 

12s- 388 wh
10s- 324 wh

Flipsky 6.6 can Handel 12s 
And u can cut the power to 20A IF u want.
```

---
## \#3 Posted by: Ultimiant Posted at: 2019-07-25T20:44:48.391Z Reads: 108

```
Yeah that was my thinking and yes I am using 30Q's, ultimately I have more cells in the pack and therefor more wh meaning I should get more range if I limit my power to a lower amperage.
```

---
## \#4 Posted by: a13xr3 Posted at: 2019-07-25T22:33:10.743Z Reads: 100

```
With a 12S setup you could lower the amperage you would have to push to the motors for the same acceleration feeling, you would get better range based of that ability alone. How much this would increase is hard to say.

You could also look at a different form factor. A 10S3P sanyo 20700B would be a whole lot of range, relatively equal to a 10S4P 30Q pack in Ah rating (lower max drain rate, 45A vs 60A)
```

---
## \#5 Posted by: sayekim Posted at: 2019-07-26T09:00:15.110Z Reads: 66

```
In short yes. More cells equals more range with identical batteries. 
However since you are now capable of more power should you use it you would actually use that more often and then I suppose the range would be pretty similar.
```

---
## \#6 Posted by: Winfly Posted at: 2019-07-26T09:10:39.978Z Reads: 62

```
[quote="Ultimiant, post:1, topic:99119"]
I was wondering if I could have a 12s3p but still program my VESC to pull the same amount of power as if it were a 10s battery.
[/quote]
you can do that by lowering battery current and motor current settings. 

ideally if you ride the same way, you will have increase range by adding those 6 cells. but 12s allows you to have more power so idk if you can resist to untapped power in a long run. I would generally recommend ppl to go 12s3p rather than 10s4p just because 12s gives you a much better acceleration and speed even at low battery. IMO low battery on 10s is unridable.
```

---
## \#7 Posted by: Ultimiant Posted at: 2019-07-26T15:59:51.400Z Reads: 42

```
[quote="a13xr3, post:4, topic:99119"]
With a 12S setup you could lower the amperage you would have to push to the motors for the same acceleration feeling
[/quote]

Sorry I got a little lost there, I know I can lower the amperage from the battery but what do you mean I would have to push the motors more, you mean when I'm riding I'd have to gun it a bit more to get a punch?
```

---
## \#8 Posted by: Ultimiant Posted at: 2019-07-26T16:00:52.816Z Reads: 37

```
[quote="Winfly, post:6, topic:99119"]
you can do that by lowering battery current and motor current settings
[/quote]

Yeah, I'm assuming this is all done through programming my VESC, or does any of this have to be done with resistors?
```

---
## \#9 Posted by: a13xr3 Posted at: 2019-07-26T16:41:56.752Z Reads: 34

```
It's common, I think, to refer to battery amps as pull and motor amps as push due to the direction of current relative to the VESC, but I'll try to explain better.

Lets say you configured the VESC to be 40A per motor while using a 10S battery. If you were to adjust none of the amperage's and move up to a 12S battery the board would fell torquer and you would have a higher top speed just due to the voltage increase. 

Therefor, you can lower the battery and motor amps on a 12S and still have a very similar ride experience to 10S, with a higher top speed and lower power consumption.
```

---
## \#10 Posted by: Ultimiant Posted at: 2019-07-26T18:26:50.967Z Reads: 23

```
Thanks for the detailed response, that makes much more sense now.
```

---
