# Why do private messages have max. limit of 500 replies?

### Replies: 16 Views: 591

## \#1 Posted by: Cobber Posted at: 2018-05-11T15:10:09.390Z Reads: 159

```
That said I am afraid to ask a mod why as when they normally play with stuff sometimes it gets deleted...

anyone?
```

---
## \#2 Posted by: Deckoz Posted at: 2018-05-11T15:14:12.672Z Reads: 157

```
Think 500 is the max standard for Discourse forum software. :)
```

---
## \#3 Posted by: Cobber Posted at: 2018-05-11T15:49:52.887Z Reads: 149

```
meh... foiled by the man
```

---
## \#4 Posted by: Kug3lis Posted at: 2018-05-11T15:56:36.321Z Reads: 141

```
I am interested in your discussions happening in those 500 messages :D
```

---
## \#5 Posted by: Cobber Posted at: 2018-05-11T16:06:13.390Z Reads: 127

```
There is some cray cray in there and mind blowing brilliance! :exploding_head:
```

---
## \#6 Posted by: anorak234 Posted at: 2018-05-11T16:11:29.486Z Reads: 121

```
Deleting stuff? What? We’d *neeeeeeeever* do that

In all seriousness though, it’s just the software
```

---
## \#7 Posted by: b264 Posted at: 2018-05-11T18:28:00.580Z Reads: 100

```
Discourse is [open-source](https://github.com/discourse/discourse) and you are more than welcome to submit a code patch to fix that.  Then once this forum get upgraded to the new version containing your fix, the 500 message limit would be raised.
```

---
## \#8 Posted by: Blitz Posted at: 2018-05-11T18:28:42.307Z Reads: 98

```
Can someone patch the Open/Live chat?
```

---
## \#9 Posted by: b264 Posted at: 2018-05-11T18:29:17.427Z Reads: 95

```
Yes; you can.  That's a separate plugin called [Babble](https://meta.discourse.org/t/babble-a-chat-plugin/31753).  It's open-source as well.  Go forth and fix it!
```

---
## \#10 Posted by: ATLesk8 Posted at: 2018-05-11T22:38:37.647Z Reads: 55

```
Better question is "Why do you know this?"
```

---
## \#11 Posted by: banjaxxed Posted at: 2018-05-12T07:27:16.841Z Reads: 39

```
Performance reason seemingly 
https://meta.discourse.org/t/using-private-personal-messages-as-long-term-chat/41356/21
```

---
## \#12 Posted by: b264 Posted at: 2018-05-12T07:46:40.393Z Reads: 40

```
Oh, there you go.  The answer is in there.

[quote]
OK! This change is in 1.6 beta 1, with the following default limits:

500 max replies in a PM topic
10000 max replies in a topic

These can be changed (or disabled, by setting to 0) via auto close messages post count and auto close topics post count in Admin, Site Settings.
[/quote]

So @moderators can adjust this by typing in 0 there or changing it to the more sensible 10,000.
```

---
## \#13 Posted by: b264 Posted at: 2018-05-12T07:47:04.854Z Reads: 34

```
For the record, I have also hit this limit numerous times...
```

---
## \#14 Posted by: pixelsilva Posted at: 2018-05-12T08:34:36.290Z Reads: 31

```
Why I got this feeling all our private messages are completely the opposite, and one person can read them all ? :thinking:
```

---
## \#15 Posted by: b264 Posted at: 2018-05-12T09:17:06.929Z Reads: 28

```
The owner of the forum (enertion) does have full database access.
```

---
## \#16 Posted by: banjaxxed Posted at: 2018-05-12T09:44:52.744Z Reads: 26

```
It's a config file but same thing probably
```

---
