# Is there lower than lowest acceleration?

### Replies: 22 Views: 1180

## \#1 Posted by: jbalint1122 Posted at: 2017-06-10T18:50:31.902Z Reads: 159

```
Ok, so I have an 8S setup, with SK3 6374 190 KV, and the esc is an FVT "sleeping lion" 12s esc.

My problem is, that since I am on a penny style board, the torque is way to much. Even on the lowest setting, that is availabe on the programming card.

I guess this is kind of a weird case... People usually have less torque than they need, not more. 

Anyway, I hope there is a solution.
```

---
## \#2 Posted by: Quinlanbrown Posted at: 2017-06-10T19:01:03.919Z Reads: 154

```
What's your top speed because you could change your gearing or get bigger wheels and it would go faster with less tork but at a point it's to weak to make it up his
```

---
## \#3 Posted by: jbalint1122 Posted at: 2017-06-10T19:39:19.947Z Reads: 145

```
Well, I am running 97mm wheels, so I don't want to go higher, also, my speed is 36 km/h, which is scary on a small board like this. (So thanks, but no more speed for me... :slight_smile:)

I am looking for an option with no money spent.
Is there a way to access the settings directly, and instead of selecting "slow", you write in a number?
```

---
## \#4 Posted by: Quinlanbrown Posted at: 2017-06-10T20:28:41.507Z Reads: 132

```
You could probably add something to regulate the exseloration or if it came down to it change escs 
If you did deside to change your gearing you don't have to use all the speed my setup I went 38mph witch is about 61kph but it didn't have enuff tork for hills so I had to down size wheels
```

---
## \#5 Posted by: jbalint1122 Posted at: 2017-06-10T20:40:08.118Z Reads: 121

```
Thanks. But I would really like to solve this without spending any money.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-06-11T02:12:48.964Z Reads: 109

```
The problem is the esc your using. If you where using a vesc, you could fine tune the output.
```

---
## \#7 Posted by: MoeStooge Posted at: 2017-06-11T02:32:22.372Z Reads: 108

```
Yea, drop your voltage . So 33v  @60a=1980w.=2.6hp.       6s  25v@60a=1500w=2hp. A 24% reduction in hp. You can expect  a near same reduction In torque.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-06-11T02:54:20.597Z Reads: 105

```
You can try trimming 2s off the voltage but I'm guessing that your running a couple 4s lipos so going to 6s would mean new batteries and may still not give the results your wanting.
I believe upgrading to a vesc would be the easiest way to achieve smooth controllable power along with smooth controllable and predictable brakes.
Either way your probably not gonna solve this without spending money.
```

---
## \#9 Posted by: MoeStooge Posted at: 2017-06-11T03:00:25.177Z Reads: 98

```
@Namasaki I would re solder my lipos, now that's a cheap bastard.
```

---
## \#10 Posted by: jbalint1122 Posted at: 2017-06-11T07:35:01.484Z Reads: 86

```
Yeah, thanks for the reply, but I can't afford anything at the moment.
```

---
## \#11 Posted by: Iceni Posted at: 2017-06-11T07:36:05.273Z Reads: 85

```
If you're using a controller with adjustable limits on the triggers you could use that to limit the maximum throttle output that way.
```

---
## \#12 Posted by: jbalint1122 Posted at: 2017-06-11T07:37:15.102Z Reads: 79

```
Under resoldering, do you mean that maybe I have bad connections?
Or do you mean that I should make a 6s pack?
@Namasaki is right. I have 2 4s packs in series.
```

---
## \#13 Posted by: jbalint1122 Posted at: 2017-06-11T07:39:09.553Z Reads: 72

```
That is the option I thought about.
The only problem being that I don't want to give up that much speed.
Though this might be my only chance.
```

---
## \#14 Posted by: MoeStooge Posted at: 2017-06-11T13:50:16.725Z Reads: 61

```
Make a parallel 4s and see how it goes. 1/2 speed and torque. Keep the range.  Sounds like you need a control compromise between gear and amp.  I ride a car ESC board making 5600watt, (7.5hp), it has enough torque to rip off a 300lb gorilla. It took some time to get used to the torque. Maby just exercise some throttle control! Good luck with your build
```

---
## \#15 Posted by: jbalint1122 Posted at: 2017-06-11T14:05:13.009Z Reads: 60

```
Thanks!
That seems possibe. I will try it asap, and inform you when possible. :slight_smile:
```

---
## \#16 Posted by: mmaner Posted at: 2017-06-11T16:46:23.798Z Reads: 55

```
I would go to 83mm wheels in a penny, and use a 40 tooth wheel pulley.  There are numerous places you can download wheel pulley models and 3d print them.
```

---
## \#17 Posted by: jbalint1122 Posted at: 2017-06-11T20:37:27.016Z Reads: 48

```
Thanks, but going down in wheel size is not an option for me. 
(Terrible roads, and I don't have the money)
```

---
## \#18 Posted by: Namasaki Posted at: 2017-06-11T21:26:08.852Z Reads: 45

```
I'm interested in seeing how the 4s2p idea works out.
```

---
## \#19 Posted by: jbalint1122 Posted at: 2017-06-12T04:57:22.655Z Reads: 40

```
Me too, I will have a bit of time today, I hope to try that.
```

---
## \#20 Posted by: Namasaki Posted at: 2017-06-12T05:18:27.073Z Reads: 39

```
Please come back and fill us in on the results.
```

---
## \#21 Posted by: jbalint1122 Posted at: 2017-06-12T18:31:21.500Z Reads: 29

```
Ok, this will be interesting:

-----------
So before I went to solder without thinking, I looked at the ESC settings once again. 
The only thing I didn't dig myself into was motor timing. 

I googled it once, but I only found out that it doesn't have much effect on acceleration.

Instead of using google, I used the forum. After a few threads, I found this one:
https://www.electric-skateboard.builders/t/speed-of-acceleration-motor-timing/9464/19

So in that thread @Namasaki suggested not to lower, but to HIGHER acceleration. (Reasons are listed there...)

I was kind of sceptical, but I tried it.

Guess what happened... :grinning: :grinning: :grinning: :grinning: :grinning: :grinning: :grinning:

So thanks a lot @Namasaki ! You gave me the solution, I wanted, (in another thread, but that doesn't matter... :joy:)

Also thanks to everyone else, for suggestions!

I am sorry, but this also means that the 4S board won't happen here...
```

---
## \#22 Posted by: Namasaki Posted at: 2017-06-12T21:04:51.716Z Reads: 21

```
I forgot all about that post and the test I did with those ESC's. 
My Vescs made me forget. 
Yes the timing setting can help. Still nothing like the smoothness of a Vesc.

Of a truth, the Vesc renders the ultimate esk8ing experience...
```

---
