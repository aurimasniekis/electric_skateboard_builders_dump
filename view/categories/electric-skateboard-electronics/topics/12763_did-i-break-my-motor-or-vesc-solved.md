# Did I break my motor or vesc? (SOLVED)

### Replies: 9 Views: 1578

## \#1 Posted by: mikey Posted at: 2016-11-09T17:29:10.695Z Reads: 203

```
Can anyone familiar with Carvon hubs help me identify my problem?

**Setup:**
I'm using Dual Carvon 2.5 hub motors with 2 Ollin 4.12 Vescs using a y splitter servo cable to connect to the receiver (not using canbus cable). I'm also in FOC mode.

**Issue:**
One of the hubs spins sometimes. When it doesn't it just makes a high pitch squeaking grinding noise.

**What I did (I'm dumb I know)**
Everything was great but I thought the trigger on my Gt2b was a little too sensitive.
I was messing with PPM app configuration to get more range. 
In doing so I must have accidentally hit "read default configuration". 

I found out something was wrong when one motor was significantly louder. I road one block and turned around and I lost brakes. 

When I checked the setting on the vesc I noticed it was set back to default motor configuration with BLDC.

I reloaded the firmware and loaded the settings when it worked. 
Motor detection for FOC works every now and then.
Now I get the noise on one motor and it just vibrates and squeals. No Fault code.

I also noticed the servo wire was loose on one of the vescs. Since I have been opening and closing my incredibly tight enclosure. I think the servo wire may have broke. So I re soldered a fresh y split servo wire. There also may be a slight possibility I connected the servo wire backwards, but really don't think so.

**What did I do? Did I...**
1. Break or stripped something in the hub motor
2. Blow something in the Vesc
3. Getting interference from motor wires.

I will try post a video tonight.
```

---
## \#2 Posted by: treenutter Posted at: 2016-11-09T17:35:43.601Z Reads: 180

```
[quote="mikey, post:1, topic:12763"]
Motor detection for FOC works every now and then
[/quote]


Check the length of your battery and ESC wires; VESC is sensitive to the length of battery wire.

[quote="mikey, post:1, topic:12763"]
also noticed the servo wire was loose on one of the vescs.
[/quote]

Soldering these once you know how you want everything wired up is a good step that many folks here recommend. At the very least, hit the connection with hot glue to keep it stable.
```

---
## \#3 Posted by: mikey Posted at: 2016-11-10T03:05:47.714Z Reads: 150

```
So narrowed it down to one vesc. 

https://youtu.be/zbAOcjrWIsU
Heres a video
```

---
## \#4 Posted by: mikey Posted at: 2016-11-10T05:41:10.479Z Reads: 135

```
The issue was one vesc and the BLDC tool!


For some reason after I did motor detection, hit apply and then write configuration I noticed the bottom right corner of the app never said it was writing. So I rebooted then hit write again. Now its working!

YAY
```

---
## \#5 Posted by: caustin Posted at: 2017-01-30T20:48:54.887Z Reads: 97

```
Would you mind PM or posting your vesc settings, or screenshot?  I am configuring dual Carvon v2.5 now, on dual ollin vesc, but on 12s2p.  Having some issues, trying to figure out if it is the config or the remote.  I basically used @RunPlayBack settings but sticking with BLDC until I get it stable as hear FOC on 12s is not as EZ as 10s!  If I have your BLDC or FOC settings, I can probably figure out what I am doing wrong, and if a VESC or remote issue.  THanks for any help!
```

---
## \#6 Posted by: RunPlayBack Posted at: 2017-01-30T21:05:52.178Z Reads: 94

```
Yeah sure..this is for my 12s1p though so results may vary.

RIK A2ESK8 12S1P LIFEPO4 MINI CRUISER SETTINGS 7/22

FOC enabled
Motor Max: 60.00 A
Motor Min: -60.00 A
Bat Max: 40.00 A
Batt Min: -12.00 A
Absolute Max: 130.00 A
Max ERPM: 60000.00
Min input voltage: 8.00 V
Max input voltage: 57.00 V
Battery cut off start: 33.00 V
Battery cut off end: 30.00 V
```

---
## \#7 Posted by: caustin Posted at: 2017-01-30T21:28:50.727Z Reads: 85

```
Thanks!  Also, I think I have the startup boost setting wrong, it is ramping really slowly even on bench test which a first!

Anyway, I know that setting is for BLDC only and you are FOC, but I defaulted to 0.04...does that sound really low, what do people tyrpically use between 0.1 and 0.01?  If that is not it, need to look elsewhere for the problem.
```

---
## \#8 Posted by: RunPlayBack Posted at: 2017-01-30T21:39:19.617Z Reads: 76

```
yeah 0.040 is what I use on BLDC
```

---
## \#9 Posted by: caustin Posted at: 2017-01-30T21:55:28.149Z Reads: 69

```
Thanks, will try a few of these tomorrow, maybe it warms up!  Maybe just pitch over to FOC and try that instead, sounds like 12s1p worked ok.
```

---
