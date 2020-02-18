# Please help: Bad FOC Hall Detection Result Received

### Replies: 20 Views: 763

## \#1 Posted by: CrimzonGryphon Posted at: 2018-12-16T12:03:49.411Z Reads: 138

```
Turnigy sk8 6374 149kv

Trying to get hall tables. I click the measure button and it moves back and forth a bit. then I get this error message:

Bad FOC Hall Detection Result Received

I've seen some people having this issue but I don't know how they've fixed it.

I've tried:

Upping the current a bit.

Taking the belt off.

Switching the motor phase wires around.

**I opened up the  motor and checked:**

The sensor wire has continuity.

The hall sensor solder points are properly connected to the sensor wire.

The hall sensors don't seem damaged (can't really tell).

**In terms of the vesc:**

The wiring does match up.

2 Hall sensors give 3.2v and one gives 0v. Ground and 5v are good.

I have tried BLDC mode as well as FOC.

**I have not tried:**

Flashing new firmware, I'm on 3.40.

I'm really at a loss.
```

---
## \#2 Posted by: sayekim Posted at: 2018-12-16T12:59:26.446Z Reads: 125

```
On which values are you doing detection? Up de current more is my initial thought. 

Are you using an phone app or the desktop app?

I would always do it on the desktop app. I got 3.40 too and it works but I think I upped current to 10.
```

---
## \#3 Posted by: CrimzonGryphon Posted at: 2018-12-16T16:07:23.150Z Reads: 118

```
I have a 6374 and I've tried about 12 different currents from 1 to 60A. Thanks for the recommendation though I'm trying anything I can.
```

---
## \#4 Posted by: Friskies Posted at: 2018-12-16T16:14:03.690Z Reads: 114

```
Have you tried running sensorsless? Chances are there is nothing wrong with the motor; you might have a faulty vesc...
```

---
## \#5 Posted by: mikenyc Posted at: 2018-12-16T16:14:44.251Z Reads: 112

```
Check to see that the connector isn’t damaged. Maybe the pin inside doesn’t make good contact when inserted. Do you have another vesc to test the same motor with?
```

---
## \#6 Posted by: Andy87 Posted at: 2018-12-16T16:20:02.898Z Reads: 111

```
Or a other motor to check with the vesc where it’s not working.
Do you have sensor wire extensions? Maybe one of pins don’t have a right contact.
```

---
## \#7 Posted by: CrimzonGryphon Posted at: 2018-12-16T17:40:01.711Z Reads: 107

```
I'll check that. Thanks
```

---
## \#8 Posted by: CrimzonGryphon Posted at: 2018-12-16T17:40:42.903Z Reads: 104

```
I can run it sensorsless
```

---
## \#9 Posted by: Friskies Posted at: 2018-12-17T00:37:56.583Z Reads: 91

```
Something is wrong with the sensors or wiring to the sensors then.
```

---
## \#10 Posted by: b264 Posted at: 2018-12-17T04:47:14.129Z Reads: 85

```
[quote="CrimzonGryphon, post:1, topic:78158"]
2 Hall sensors give 3.2v and one gives 0v.
[/quote]

If you rotate the rotor, do the two which are logic high change, or are they always the same two?
```

---
## \#11 Posted by: ARetardedPillow Posted at: 2018-12-17T04:48:26.832Z Reads: 84

```
What vesc are you using...
```

---
## \#12 Posted by: briman05 Posted at: 2018-12-17T04:56:05.462Z Reads: 82

```
Maybe a bad hall sensor board if you have another vesc you can test it on another and then you could contact hobby king
```

---
## \#13 Posted by: RedBaron Posted at: 2018-12-17T08:29:21.134Z Reads: 76

```
Try this out. I was having the same issues with a maytech, they sent me this video. Make sure to set up bldc through the motor set up wizard first then go to the screen they show and follow along. I haven't tried this yet but I will be tomorrow.

Edit: forgot to post the link, lol

https://m.youtube.com/watch?v=Nre0T85NwsI&feature=youtu.be
```

---
## \#14 Posted by: CrimzonGryphon Posted at: 2018-12-17T11:04:04.603Z Reads: 74

```
I'll take a look. Thanks.
```

---
## \#15 Posted by: CrimzonGryphon Posted at: 2018-12-17T11:04:31.732Z Reads: 71

```
No other vesc unfortunately. I don't mind buying my own hall sensors and soldering them myself tbh.
```

---
## \#16 Posted by: CrimzonGryphon Posted at: 2018-12-17T11:06:34.730Z Reads: 69

```
Actually I'm talking about the voltage on the pins of the vesc. two were high and one was 0 but now all three are high (3.2v). I'm not sure if the vesc is meant to be configured like this. I'll investigate if they change when i rotate the rotor.
```

---
## \#17 Posted by: CrimzonGryphon Posted at: 2018-12-17T11:07:02.057Z Reads: 67

```
The connector is not the problem unfortunately. Just checked that.
```

---
## \#18 Posted by: Friskies Posted at: 2018-12-17T11:35:41.071Z Reads: 66

```
Focboxes are cheap btw ;)
```

---
## \#19 Posted by: CrimzonGryphon Posted at: 2018-12-17T12:20:03.452Z Reads: 59

```
I have a focbox. Unfortunately I bought them a few days before they went on sale.
```

---
## \#20 Posted by: briman05 Posted at: 2018-12-17T13:00:25.566Z Reads: 58

```
I would contact hobbyking about this issue may be a bad sensor board.
```

---
