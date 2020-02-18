# All bluetooth control system both for mobile &amp; standalone remote

### Replies: 6 Views: 939

## \#1 Posted by: mclightning Posted at: 2017-04-13T19:42:55.543Z Reads: 153

```
Hi Guys,

I have been experimenting with various types of wireless modules to make my own remote control system.

Until now I tried different bluetooth modules, 2.4ghz flysky, 433mhz rf module.

I think now I found the perfect combination. 

I made a remote controller with a bluetooth module in master mode.
I made a receiver with a bluetooth module in slave mode.
I also made an Android app to use when the battery dies out on the remote controller.

Here is the very new demo video:
https://www.instagram.com/p/BS1lCrnAUIB/

------------------
By the way, I started sharing all my materials and progress. I announced it earlier when giving a speech at Arduino Day 2017.
You can find my materials etc. here:
https://github.com/ElectricSkateboard
Some bits from my talk:
https://www.instagram.com/p/BSWfTlagklQ/


Slides:
https://www.slideshare.net/mclightning/electric-skateboard-arduino-day-2017-talk
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-04-14T02:39:36.580Z Reads: 121

```
How does your system compare to an environment with more 2.4ghz interference/noise? Do you get drop outs?
```

---
## \#3 Posted by: mclightning Posted at: 2017-04-14T11:50:11.059Z Reads: 105

```
I have been using bluetooth receiver with my android app for 2 months, had no problem riding my board in the city center anywhere.
```

---
## \#4 Posted by: PI3RR3 Posted at: 2018-11-05T17:03:56.755Z Reads: 39

```
Cool stuff and exactly what I am looking for I think. I plan to do the same kind of stuff using 2 bluefruit feather nRF52 (arduino BLE boards):

One for the remote and one for the receiver.

I have few questions :slight_smile:
* why do you map to 0 - 255 on the remote side? (i guess 8bit data out?)
* on the receiver side, if 0 means ESC.write(90), I suppose full brakes means ESC.write(0) and full speed means ESC.write(180). Am I correct or misunderstanding something?  

My main point of not understanding is how the command ESC.write knows how to scale the bluetooth input integer between full brakes and full speed?

Don't know if I am clear... Thank you in advance for any help or hints =)
```

---
## \#5 Posted by: brenternet Posted at: 2018-11-05T17:08:23.896Z Reads: 32

```
This thread is 2 years old! What's going on at the moment with all these necro posts?
```

---
## \#6 Posted by: PI3RR3 Posted at: 2018-11-05T17:11:29.446Z Reads: 30

```
LoL flooding the search button of the forum ;-)
```

---
