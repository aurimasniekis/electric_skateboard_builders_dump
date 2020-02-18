# How does my lipo know when to stop outputting?

### Replies: 13 Views: 495

## \#1 Posted by: Orin635 Posted at: 2017-10-01T19:47:52.300Z Reads: 110

```
I was just watching a video there and it said if lipos discharge too much they will get damaged so I am wondering how do I prevent this or how do you guys prevent it in your builds. Or am I just asking a very stupid question lol?
```

---
## \#2 Posted by: Chewie Posted at: 2017-10-01T19:50:47.806Z Reads: 112

```
They don't they'll just kill themselves.  To prevent that we program cutoff voltages in our speed controls (VESC FOCBox etc)
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-10-01T19:51:34.093Z Reads: 106

```
Use the search function please
```

---
## \#4 Posted by: Orin635 Posted at: 2017-10-01T19:57:10.491Z Reads: 100

```
Do ESC's have that function and what cutoff voltage would you recommend
```

---
## \#5 Posted by: William_Trojel Posted at: 2017-10-01T20:02:17.325Z Reads: 95

```
there are many posts about that already, and there are very different opinions on that some say 3,7 some say 3,3. The higher you set the cutoff voltage, the longer lifespan you will get out of your batteries
```

---
## \#6 Posted by: William_Trojel Posted at: 2017-10-01T20:02:53.639Z Reads: 93

```
but just use the search function :thumbsup:
```

---
## \#7 Posted by: Okami Posted at: 2017-10-02T15:09:16.681Z Reads: 70

```
usually it is not super wise to rely on regular esc cutoff protection, so in my opinion, best would be to manually monitor the voltage using some sort of screen, either in percentage or volts. Individual cell monitoring might work the best not to let the lipo drain too low.
```

---
## \#8 Posted by: Nix Posted at: 2017-10-02T17:58:24.678Z Reads: 62

```
Batteries dont push power into the motor and esc but the esc pulls what is asked of it out. Usually people go 3.3 or so but people who are safe stop using their eboards at 3.7 or so. To stop over discharge, people set their vesc to shut down the system at a specific voltage or use battery indicators or voltage buzzers
```

---
## \#9 Posted by: ShutterShock Posted at: 2017-10-02T18:33:48.011Z Reads: 59

```
I would say 3.3 is way low for lipo, the lowest I go with mine is 3.5 and that is even pushing it.  For max safety and battery preservation go 3.6-3.7

My cutoff start is 3.6/cell and end is 3.5/cell
```

---
## \#10 Posted by: William_Trojel Posted at: 2017-10-02T18:35:32.847Z Reads: 56

```
yea i agree, it is just what some people say
```

---
## \#11 Posted by: Namasaki Posted at: 2017-10-03T01:58:16.946Z Reads: 35

```
[quote="Orin635, post:4, topic:34492, full:true"]
Do ESC's have that function and what cutoff voltage would you recommend
[/quote]


hobby car esc's have a low voltage protection but it is not reliable like it is on the Vesc.
At least not the ones I used back in the day.
```

---
## \#12 Posted by: jmasta Posted at: 2017-10-03T02:01:59.356Z Reads: 33

```
My lipos didn't even last a full season, and I rarely took them past 3.7V.  And they were never above or below storage of 3.85V for more than a few hours.  I only fully charged them to 4.2V a few times (usually to 4.0-4.15V)
```

---
## \#13 Posted by: mmaner Posted at: 2017-10-03T02:07:12.061Z Reads: 33

```
That sucks. I've got a set of 3s 8k mAh that I've been running g for 6 miles the or longer, prolly charged them 50 times.
```

---
