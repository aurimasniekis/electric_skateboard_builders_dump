# Intermittent Throttle and Brakes

### Replies: 7 Views: 813

## \#1 Posted by: Spencer Posted at: 2017-02-10T14:15:50.341Z Reads: 73

```
Hi all,

I'm a first time builder and I just finished my first board. It works properly after some troubleshooting for the enertion nano-x's binding issue, but one problem still remains.

At times, when I press the throttle, it doesn't immediately go. Sometimes there's delay and then the motor instantly jumps to the highest speed. The brakes have the same problem; sometimes they don't initiate, and then they slam all at once.

This is becoming a major problem, and I'm not sure where to begin troubleshooting. Is it something mechanical, like my belt, or is this something else?
```

---
## \#2 Posted by: psychotiller Posted at: 2017-02-10T15:43:25.422Z Reads: 62

```
I've had that issue before. With my build is was the receiver. You should start by moving the rever away from the other components on your build, Then try a different remote/receiver. Doing that will either confirm/ or rule out the problem. Then move to your Speed controllers and programming.
```

---
## \#3 Posted by: Blasto Posted at: 2017-02-10T17:17:11.630Z Reads: 51

```
[quote="Spencer, post:1, topic:17508"]
Sometimes there's delay and then the motor instantly jumps to the highest speed
[/quote]

Is this while bench testing? with no load the motor will hit maximum speed at a very low throttle input. try it on the ground.

One other thing, did you calibrate the remote in the BLDC tool? (ppm min max and deadband)
```

---
## \#4 Posted by: Spencer Posted at: 2017-02-10T22:25:56.234Z Reads: 40

```
This is with a load attached.

I haven't toyed with VESC settings in regards to the remote--can you direct me to somewhere that can help me with this calibration process?
```

---
## \#5 Posted by: Blasto Posted at: 2017-02-10T22:44:53.907Z Reads: 32

```
Give this a try http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244

What do you mean with a load attached? Are you standing on it?
```

---
## \#6 Posted by: Spencer Posted at: 2017-02-10T22:53:02.202Z Reads: 29

```
Yes, I first noticed the issue when I was standing on the board. I actually had to jump off the board as a result of it, the first time it happened.

I'm checking out the thread now, thank you!
```

---
## \#7 Posted by: SpeedyGornzallez Posted at: 2017-08-07T20:21:44.063Z Reads: 11

```
Hey @Spencer , did you ever find out what the problem was? I'm having the exact same issue as you.
```

---
