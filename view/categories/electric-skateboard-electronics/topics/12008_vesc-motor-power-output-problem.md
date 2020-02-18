# VESC Motor Power Output Problem

### Replies: 23 Views: 2105

## \#1 Posted by: Lancer Posted at: 2016-10-27T17:32:34.500Z Reads: 154

```
Hello all,

I recently went and upgraded from a single motor to duel rear motors on my long board.  However in the process when connecting up two VESC's I lost the settings previously set using the BLDC tool.  I tried doing a "Read Configuration" and got back a lot of my settings but when I go to do a motor detection test it fails every time.  

I can pull the trigger on the remote and get power and wheels spin, however i am able to stop it just by grabbing the wheel. 

Lastly:  I know there is a very similar topic called "VESC Motor output power issue"   I have read that post through many times and tried similar solutions.  But might be missing something.  

I am running:
190kv motor (80A)
VESC 4.12
and a 6s battery
BLDC is the latest version.  

I will attach some screen shots of my BLDC tool.  I am thankful for any help or suggestions.
```

---
## \#2 Posted by: Lancer Posted at: 2016-10-27T17:39:04.961Z Reads: 150

```
<img src="/uploads/db1493/original/3X/d/e/de11f4a7666c50b8f37752753e1e4e1c7c408f96.PNG" width="690" height="374"><img src="/uploads/db1493/original/3X/2/6/267e408ed558f5af64f9c4256d553454f2d363c1.PNG" width="690" height="375"><img src="/uploads/db1493/original/3X/c/2/c2b6f6606ee50f35dc723e9698974f7096c19ad9.PNG" width="690" height="374">
```

---
## \#3 Posted by: chinzw Posted at: 2016-10-27T18:58:02.235Z Reads: 124

```
Try setting your battery cutoff start to 12 and end to 10 and do the motor detection again. Most of the time its those values are wrong or your battery is low on voltage.

edit: if it works, set them back to 21 and 19.8
```

---
## \#4 Posted by: zmoney Posted at: 2016-10-27T19:03:23.013Z Reads: 123

```
Try setting your Max voltage at 57V
```

---
## \#5 Posted by: Lancer Posted at: 2016-10-27T21:53:41.834Z Reads: 117

```
I did those changes and the motor detection worded! thanks for that
However I am still able to stop the motor with my hand.  
Any additional recommendations?

I have attached new screen shots of the setting as of now<img src="/uploads/db1493/original/3X/f/9/f96e605d70b84c535e545898adddc89c987a03a2.PNG" width="690" height="368"><img src="/uploads/db1493/original/3X/1/6/164efb4120a768624b8f9d4557c788bae2b3884d.PNG" width="690" height="367">
```

---
## \#6 Posted by: chinzw Posted at: 2016-10-28T00:29:41.379Z Reads: 98

```
try going to terminal and type "faults"
report back what you get
```

---
## \#7 Posted by: Blasto Posted at: 2016-10-28T01:13:54.768Z Reads: 98

```
[quote="Lancer, post:5, topic:12008"]
However I am still able to stop the motor with my hand.
[/quote]

Dude don't do that, you'll hurt yourself. Try it with your remote instead of the keyboard, you'll have plenty of torque
```

---
## \#8 Posted by: TarzanHBK Posted at: 2016-10-28T10:44:14.184Z Reads: 90

```
you´re a bit low on 6s for 190kv. If your motor max is 80A put atleast 70A in. 
Also raise your Battery max.
you´ll have no power with these current settings.

And don´t try to grap in the running wheel.
Jump on your board and try it!
```

---
## \#9 Posted by: chinzw Posted at: 2016-10-28T16:50:01.176Z Reads: 83

```
Im using 40A motor on 6s with 192kv SK3 and at 65kg it carries me just fine.
```

---
## \#10 Posted by: Lancer Posted at: 2016-10-31T19:10:30.453Z Reads: 81

```
Here is the screen shot from the terminal.<img src="/uploads/db1493/original/3X/d/d/dd12ee04ec11fdb775934ddd2b0ca2481e97d994.PNG" width="690" height="367">
```

---
## \#11 Posted by: Lancer Posted at: 2016-10-31T19:11:15.559Z Reads: 74

```
I have been doing that.  (using the remote) I can still stop it easily
```

---
## \#12 Posted by: Lancer Posted at: 2016-10-31T19:25:11.829Z Reads: 73

```
Here is the new specs.  
I just went and tried and tested the board,  I can walk faster then it goes at full throttle.  Also the motor sounds like its not running right.  But its brand new.  I also tried the old one and it has the same effect.  

Let me know if you guys have any more ideas to try!<img src="/uploads/db1493/original/3X/9/e/9e67d6f7dc3f08a418e593b59275a561be64c468.PNG" width="690" height="368">
```

---
## \#13 Posted by: Blasto Posted at: 2016-10-31T20:30:03.650Z Reads: 72

```
[quote="Lancer, post:1, topic:12008"]
a 6s battery
[/quote]

What is this battery? is it able to output the current you are asking for?

You can also look at your remote configurations, under ''app configuration'' -> ''ppm settings'' to see if your remote is within the working window of your settings. (tick the display box)
```

---
## \#14 Posted by: Lancer Posted at: 2016-10-31T21:23:32.033Z Reads: 72

```
My battery is this:
 http://www.ebay.com/itm/2X-6S2P-22-2V-13000mAh-35C-Li-Po-Battery-Pack-For-RC-Helicopter-Hobby-Denas-Plug-/311614676170?hash=item488dae9cca:g:VhgAAOSwB9xXO9Le
Should be plenty of power

As for the Remote settings,  I haven't changed those since last time. I ran it.  But here is a screen shot of the setting there

<img src="/uploads/db1493/original/3X/5/8/5874eccf0a00ca23e2748d2bdb3faddc14665c9e.PNG" width="690" height="367">
```

---
## \#15 Posted by: Blasto Posted at: 2016-10-31T21:31:44.555Z Reads: 67

```
Another stupid question, your batteries are charged?

Do you see the full swing of your remote in the display?
```

---
## \#16 Posted by: Lancer Posted at: 2016-10-31T21:57:07.640Z Reads: 69

```
Never a stupid question,  but yes they are fully charged.  

And yes the remote gives full authority and swing on the display
```

---
## \#17 Posted by: Lancer Posted at: 2016-11-04T23:04:17.332Z Reads: 66

```
I have updated my current settings. (see attachments below) Any further ideas?
```

---
## \#18 Posted by: Blasto Posted at: 2016-11-05T04:00:09.398Z Reads: 67

```
just noticed in one of your screen shots you have a "motor detection fail". are you able to perform a successful motor detection?
```

---
## \#19 Posted by: Lancer Posted at: 2016-11-05T04:21:33.060Z Reads: 68

```
yes, i have fixed that, and can run a successful motor detection.  However the board can not move its self.
```

---
## \#20 Posted by: elkick Posted at: 2016-11-05T09:03:37.004Z Reads: 62

```
In the BLDC Tool: check in the real time tab (mark the checkbox at the bottom of the screen) if the batteries are providing the voltage you need.
```

---
## \#21 Posted by: Lancer Posted at: 2016-11-07T22:51:06.916Z Reads: 51

```
Is this what your talking about?  
It looks like the amps are low.  Im not sure what to make of this graph<img src="/uploads/db1493/original/3X/8/7/87ea6bb7b660359bcbf0c75897c7a16bd4294461.PNG" width="690" height="366">
```

---
## \#22 Posted by: Rollbrett Posted at: 2017-01-14T21:35:57.574Z Reads: 41

```
were you able to solve your problem? i'm experiencing similar issues
```

---
## \#23 Posted by: Ollie Posted at: 2018-12-03T17:50:30.983Z Reads: 19

```
Same. I'm having the same issue with Flipsky FESC4.20 and any help would be greatly appreciated.
```

---
