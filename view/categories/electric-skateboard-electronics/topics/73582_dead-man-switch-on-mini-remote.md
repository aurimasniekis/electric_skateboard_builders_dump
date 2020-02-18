# Dead man switch on mini remote

### Replies: 22 Views: 690

## \#1 Posted by: amazingdave Posted at: 2018-11-05T21:48:55.766Z Reads: 187

```
Following my recent fun with tearing knee ligaments I have decided to add a deadman’s switch to my mini remote....  

I’m thinking of a hand grenade style leaf, activating a micro switch, in series with the power switch and reducing my remote timeout to 0.1 seconds. I’ll be adding a Lipo and charging circuit at the same time. 

Before I start on the cad modelling does anyone have any opinions I need to hear?
```

---
## \#2 Posted by: mmaner Posted at: 2018-11-05T22:05:30.264Z Reads: 186

```
I've found that a dead mans switch is actually dangerous for me.  It means I can't switch my hand position or I risk activating the switch (releasing the button/lever).  This causes hand fatigue and if it fails at 30 mphs your screwed.
```

---
## \#3 Posted by: pat.speed Posted at: 2018-11-05T22:19:18.935Z Reads: 180

```
I personally don’t see the need for a dead mans switch unless it’s going to slowly brake. Because if you say dropped the remote, it’s going to stop itself anyway
```

---
## \#4 Posted by: skelstar Posted at: 2018-11-05T23:41:50.093Z Reads: 166

```
I have my deadman switch only operating on acceleration (DIY remote, encoder-style). If switch is released then the throttle goes back to 0.
```

---
## \#5 Posted by: Sn4pz Posted at: 2018-11-06T01:39:38.767Z Reads: 150

```
this is how my firefly works too :slight_smile:

if only I could speed the building process up :laughing:
```

---
## \#6 Posted by: tardyparty7 Posted at: 2018-11-06T02:46:22.936Z Reads: 145

```
It's also if you accidentally accelerate. Say you're holding the remote and try to put the remote down or in your pocket but forget to turn either off. If the wheel (on the remote) is pushed forward, you'll go flying or your board might to into the street.
```

---
## \#7 Posted by: C23 Posted at: 2018-11-06T03:44:45.137Z Reads: 134

```
This is unrelated, but is there a way to know when the torqueboards mini remote is near the end of its battery life?  I would like to avoid it cutting out on me all at once.
```

---
## \#8 Posted by: b264 Posted at: 2018-11-06T04:55:24.861Z Reads: 125

```
Are you in the USA?  You profile does not say
```

---
## \#9 Posted by: Trdolan03 Posted at: 2018-11-06T07:37:45.594Z Reads: 105

```
An easy way would be to just add a momentary switch on the power cable to the battery in the remote
```

---
## \#10 Posted by: amazingdave Posted at: 2018-11-06T08:00:15.729Z Reads: 102

```
I’m in the U.K.  the current behaviour of my vesc is ackmaniak timeout braking which is progressive. When I’ve tested it it works well at not killing me even at high speed. The style of dead man I’m considering would need a full letting go of the remote to deactivate...

@Trdolan03 that’s exactly what I was thinking...

@tardyparty7 and that’s exactly how I’ve destroyed 2 ligaments on the outside of my left knee....
```

---
## \#11 Posted by: Winfly Posted at: 2018-11-06T08:27:58.314Z Reads: 95

```
Only works if your remote magically binds properly in milliseconds.
```

---
## \#12 Posted by: amazingdave Posted at: 2018-11-06T09:32:34.880Z Reads: 87

```
My mini remote does....
```

---
## \#13 Posted by: tardyparty7 Posted at: 2018-11-06T16:19:06.978Z Reads: 76

```
I guess, I just think it's safer. hope  u get better
```

---
## \#14 Posted by: Mich21050 Posted at: 2018-11-06T16:21:37.497Z Reads: 74

```
You could interrupt one potentiometer with a  mini switch :smile:
```

---
## \#15 Posted by: brenternet Posted at: 2018-11-06T16:42:06.064Z Reads: 72

```
The R2 style deadman switch that only activates below a certain speed (2mph?) seems like the way to go from an accidental "launch my board into traffic" perspective.

It won't interfere with your riding but it'll stop stand still activation by bumping the trigger.
```

---
## \#16 Posted by: b264 Posted at: 2018-11-06T19:28:15.983Z Reads: 67

```
[quote="C23, post:7, topic:73582"]
is there a way to know when the torqueboards mini remote is near the end of its battery life? I would like to avoid it cutting out on me all at once.
[/quote]

The Mini Remote:

1) takes so long to die, it's crazy
2) you will feel it cut out very, very briefly a few times and the power light on the remote will flash a bit.  After that happens, you probably only have 5 more rides.  Get a battery and a screwdriver and a pairing key now.
3) if it cuts out completely on you, turn it off for 1 minute.  Then you will probably be able to make it home when you turn it back on.  But you can do this once only.

And finally

BE GENTLE WITH THE POWER SWITCH

That's the first part that will fail due to use.
```

---
## \#17 Posted by: Bataleon Posted at: 2018-11-06T19:31:50.518Z Reads: 65

```
[quote="b264, post:16, topic:7[quote="b264, post:16, topic:73582"]
And finally

BE GENTLE WITH THE POWER SWITCH

That’s the first part that will fail due to use.
[/quote]
It's a bummer the power switch is so weak considering how reliable the rest of the remote is.
```

---
## \#18 Posted by: b264 Posted at: 2018-11-06T19:46:43.472Z Reads: 64

```
[quote="Bataleon, post:17, topic:73582"]
It’s a bummer the power switch is so weak considering how reliable the rest of the remote is.
[/quote]

Understatement of the Year award goes to @Bataleon

:smiley:
```

---
## \#19 Posted by: C23 Posted at: 2018-11-07T17:20:33.211Z Reads: 58

```
Yea that is a real bummer.  Especially considering that I have to turn the power switch on and off more than 5 times per day, because once I ride to school, I ride it between classes.  Haha.  I wonder how long that will last.
```

---
## \#20 Posted by: walleywalker Posted at: 2019-06-14T03:39:58.062Z Reads: 37

```
Sorry to bring this topic back to life but, do dead man switches work the same way on DIY boards as they donon Boosted?

On Boosted if you release the deadman at any point it just kind of goes into 'neutral,' if you will. 

It sounds like on DIY boards that releasing the switch on a diy board will throw you from the board?? Why??
```

---
## \#21 Posted by: amazingdave Posted at: 2019-06-14T06:34:55.593Z Reads: 31

```
It all depends on what vesc firmware you’re running and how you configure the remote timeout behaviour. It’s possible to have it coast, brake gently, brake progressively.... I’m running ackmaniac configured to brake progressively and tested to 20mph it doesn’t throw me on the flat. Up a hill under acceleration, even coasting will throw you unless you’re well braced.
```

---
## \#22 Posted by: walleywalker Posted at: 2019-07-02T03:20:41.493Z Reads: 24

```
Is there a software way like mentioned above that releasing the dead-man switch can make throttle=0 thus putting it into a coast mode? Or does zero throttle on a DIY board still have a lot or braking resistance?
```

---
