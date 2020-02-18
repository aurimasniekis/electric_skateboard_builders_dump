# Hardware switch to toggle between legal mode and full power?

### Replies: 15 Views: 422

## \#1 Posted by: Morxy49 Posted at: 2018-06-28T12:34:45.722Z Reads: 130

```
Apparently in Sweden it's only legal to ride electric skateboards with a maximum power output of 250W and max speed of 20 km/h. Is it possible to somehow program a physical switch on the skateboard that limits the skateboard to these specs when flipped on, and when flipped of it just goes full power without any limit?

I'm using FOCBOXes if that makes any difference. 

/Simon
```

---
## \#2 Posted by: Komamtb Posted at: 2018-06-28T12:46:10.590Z Reads: 129

```
Will the police just take and test your board?
```

---
## \#3 Posted by: Morxy49 Posted at: 2018-06-28T12:51:14.604Z Reads: 130

```
No idea how it works with the police actually. I just think it might be a fun little project to make the switch and see it work :stuck_out_tongue:
Plus it never hurts to be cautious.
```

---
## \#4 Posted by: pat.speed Posted at: 2018-06-28T12:54:01.754Z Reads: 129

```
Doubt they would take the board to test, not even really possible for them to test it. As long as you are going less than 20km/h and you’ve got a helmet on I doubt they would have anything wrong with you riding your board
```

---
## \#5 Posted by: Morxy49 Posted at: 2018-06-28T12:55:04.631Z Reads: 126

```
Yeah, I understand you, and I agree. It's probably overkill, but I want to know if it's possible! It may be a fun little project.
```

---
## \#6 Posted by: pat.speed Posted at: 2018-06-28T12:57:59.417Z Reads: 126

```
Well the closest way would be a different mode on your phone that changes the Vesc settings to a max of 250w which is simple all you need is a bt module.
```

---
## \#7 Posted by: rojitor Posted at: 2018-06-28T14:17:30.378Z Reads: 107

```
250w will not let you climb any Hill.
In my country the speed is límited to person pace on pavement only.
The police will not take your board to the testing bench just to fine you.
Just follow the first rule of the esk8r:
"Don't be a jackass" 
I passed the police very often(i'm the only Rider in town) and they never stopped me. I ride according to the rules and the moment.
In the middle of nowhere nobody around= full throttle
In town broad daylight plenty of people walking= as slow as possible and sometimes i get down of the esk8 and walk a few meters if i have to.
Common sense is way more important than rules.
```

---
## \#8 Posted by: banjaxxed Posted at: 2018-06-28T14:27:22.147Z Reads: 94

```
Some remotes have a switch like so, the nano v2 springs to mind
```

---
## \#9 Posted by: linsus Posted at: 2018-06-28T14:30:31.362Z Reads: 93

```
The new VESC app has the possibility to toggle such limits on the fly with a BLE module. 
Not sure if its fully released yet, but works very well on my board. I'm from sweden too and have been stopped twice by the police. Truth is that they dont know the laws that well and if you claim its 250W they wont do shit. If your board only does 20 kmh, it will be legit enough for them.
```

---
## \#10 Posted by: Morxy49 Posted at: 2018-06-28T14:36:16.902Z Reads: 86

```
Yeah, I don't think they'll have some measuring tool to check the wattage exactly, that's a good point. Just limit it to 20kmh and it should be fine probably. Thanks :)
```

---
## \#11 Posted by: Toughook Posted at: 2018-06-28T14:43:10.761Z Reads: 80

```
the slow and fast mode on the Maytech remote only governs acceleration. Will get you top speed, just less angrily !!
```

---
## \#12 Posted by: banjaxxed Posted at: 2018-06-28T15:17:29.120Z Reads: 72

```
Not sure if it has the ability to actually alter acceleration, it just limits ppm, but yeah eventually you should get to around the same speed on a flat

 _a low/high speed mode which basically just cuts PPM signal by 30% in low speed mod_

https://www.electric-skateboard.builders/t/nano-v2-full-review/25159?u=banjaxxed
```

---
## \#13 Posted by: koralle Posted at: 2018-06-28T15:25:59.461Z Reads: 63

```
That switch exists. It's called the on off button. Default mode on slow. Please delete this thread! Cops have Google nowadays :rofl:
```

---
## \#14 Posted by: Morxy49 Posted at: 2018-06-28T17:59:29.398Z Reads: 51

```
:tired_face:
```

---
## \#15 Posted by: karma Posted at: 2018-06-28T18:05:36.586Z Reads: 49

```
You can have profiles in the Ackmanic version of VESC tool, just change profile with 2 clicks and you gotba legal board. :) 
And ofc you can make your own speed regulation.
```

---
