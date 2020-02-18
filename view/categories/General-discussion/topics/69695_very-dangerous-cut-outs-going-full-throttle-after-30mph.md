# Very dangerous cut outs going full throttle after 30mph+

### Replies: 40 Views: 859

## \#1 Posted by: never4getf150forums Posted at: 2018-10-01T02:55:01.109Z Reads: 276

```
so, this is the second time it has happened, I don't like testing it, but now that I can expect it to happen I know how the board reacts.
    
it happens whenever I try to accelerate.. so if I'm riding from about cruise speed at 20mph, and I go full throttle to pass a car or get across an intersection quickly it happens after i pass 30mph..

i'm guessing something setting related.. atm I don't have a metr module installed to read the faults as it was automatically applying weird settings for some reason, and ever since i got rid of it the board started to work perfectly fine.

here are the files a friend sent me to install them into my focboxes 

"master motor config"
http://s000.tinyupload.com/index.php?file_id=02517771741031456966

"master app config"
http://s000.tinyupload.com/?file_id=83326133372186982274

please help, thx
```

---
## \#2 Posted by: never4getf150forums Posted at: 2018-10-01T02:56:21.417Z Reads: 269

```
running 12s, 5065 200kv 15/36 gearing

if this matters
```

---
## \#3 Posted by: Jake2k17 Posted at: 2018-10-01T02:57:32.572Z Reads: 264

```
Often people have had cutouts with they’re remotes around intersections. Where are you located?
```

---
## \#4 Posted by: never4getf150forums Posted at: 2018-10-01T02:59:30.245Z Reads: 262

```
GT2B, no intersection issues, i'm positive it's 100% based on the power/amps it's pulling.. maybe there is a setting that's too low.. ah, damn just realized i have to open the enclosure and i made it a pain in the ass to do so :confounded:
```

---
## \#5 Posted by: Jake2k17 Posted at: 2018-10-01T03:00:59.493Z Reads: 248

```
If your sure, but I’ve heard about a lot of problems with that remote around intersections...you must be hitting some kind of cut off
```

---
## \#6 Posted by: never4getf150forums Posted at: 2018-10-01T03:03:06.071Z Reads: 240

```
nope, not one problem ever, trust me I tested this in 2 places very far apart from each other, you could be on the moon and it will happen.

no interference, purely cut off..

oh well, guess im gonna have to take off this enclosure and figure out wtf it is doin cuttin me off at those speeds. :sweat_smile:
```

---
## \#7 Posted by: Schulerbible Posted at: 2018-10-01T04:06:51.504Z Reads: 214

```
I got a massive cutout on my Gt2b where it hit full throttle while going slightly up hill, throwing me off the board and almost pushed the board on the street, that was scary af. Still don’t know why.
```

---
## \#8 Posted by: dareno Posted at: 2018-10-01T04:30:41.704Z Reads: 201

```
What wheel size are you you running?  With that set up you are topping out the erpm limits on vesc.  If it only happens on high speed?
```

---
## \#9 Posted by: never4getf150forums Posted at: 2018-10-01T04:51:57.645Z Reads: 203

```
107mm

don't think it's erpm, but i guess i will check settings in a bit, only issue is the enclosure is a complete bitch to remove.. 

can't wait.:confounded:
```

---
## \#10 Posted by: dareno Posted at: 2018-10-01T05:00:56.696Z Reads: 191

```
12s on full charge produces 50.4 volts at this voltage the erpm will be up in the 70000 mark.  Over 30mph will send it over the 60000 and if all your getting is a cut off then consider yourself lucky.  Usually things go poof.  oh and you might want to invest in a pair of these if your enclosure is a bitch to remove.

  ![IMG_1037|375x500](upload://949Zbjw3JBtM2x5fRw9BFv0kNQD.jpeg)
```

---
## \#11 Posted by: never4getf150forums Posted at: 2018-10-01T06:06:02.013Z Reads: 179

```
where can i get those for a m5 bolt.. lol that's awesome.

thank god for that then, it still works great, i just wanna take it over 30mph like i did constantly on 10s
```

---
## \#12 Posted by: dareno Posted at: 2018-10-01T06:11:20.250Z Reads: 175

```
Thats why 10s is spot on for 200kv  12s you need to go down a bit or adjust the gearing to suit.  I run 12s with 15/36 and 192kv's  I'm close to the limit but no issues so far.  

[quote="never4getf150forums, post:11, topic:69695"]
where can i get those for a m5 bolt… lol that’s awesome.
[/quote]
this I'm not sure what you mean and I probably should have been more clear they are usb ports so you don't have to remove your enclosure for settings
```

---
## \#13 Posted by: Aeroquiv Posted at: 2018-10-01T07:06:07.481Z Reads: 168

```
What % was your battery pack at? And are you bypassing discharge?
```

---
## \#14 Posted by: Aeroquiv Posted at: 2018-10-01T07:12:00.834Z Reads: 169

```
But the thing is your battery will sag well below eRPM even _assuming_ motor kV's are 100% accurate, which they are not, especially for racerstar motors. It only happens during acceleration as well, where battery current requirements are highest. I highly doubt eRPM is the problem.
```

---
## \#15 Posted by: Sebike Posted at: 2018-10-01T08:07:41.977Z Reads: 158

```
...or if you have a BT module you can fully configure all settings via the ackmaniac app and a pc. no usb needed.
```

---
## \#16 Posted by: dareno Posted at: 2018-10-01T08:09:03.962Z Reads: 156

```
motor detection?
```

---
## \#17 Posted by: Sebike Posted at: 2018-10-01T08:14:44.217Z Reads: 157

```
Yes

5000 charz
```

---
## \#18 Posted by: Sebike Posted at: 2018-10-01T08:19:15.047Z Reads: 155

```
However, I experienced the connection not being stable last time I tried when monitoring RT app data, so I actually ended up opening up the enclosure. 

Didn't have this problem before, so probably a bug in a newer version. @Ackmaniac
```

---
## \#19 Posted by: dareno Posted at: 2018-10-01T09:09:32.039Z Reads: 152

```
[quote="Aeroquiv, post:14, topic:69695"]
I highly doubt eRPM is the problem.
[/quote]
I'm just going to leave you in these capable hands.  My work here is done.  
@Sebike :sunglasses:
```

---
## \#20 Posted by: never4getf150forums Posted at: 2018-10-01T09:26:20.650Z Reads: 147

```
new motors, gotcha, figured it was this.. thanks for your help, and i was tricked into thinking you use some hand tightened nuts to hold enclosure down.. that would be.. nice. :sweat_smile:
```

---
## \#21 Posted by: never4getf150forums Posted at: 2018-10-01T09:28:04.291Z Reads: 140

```
i have the metr pro, but for some reason.. it keeps making my settings change and the board act weird. like every time it's in it makes one motor stop working and the other act crazy, one time it was making a very loud 
 humming sound and i thought i messed them up.. thankfully they didn't.
```

---
## \#22 Posted by: Sebike Posted at: 2018-10-01T10:23:13.837Z Reads: 128

```
@rpasichnyk maybe?
```

---
## \#23 Posted by: rpasichnyk Posted at: 2018-10-01T10:36:13.970Z Reads: 133

```
More details please
Configs before change
Configs after change
Logs
```

---
## \#24 Posted by: pat.speed Posted at: 2018-10-01T11:13:06.284Z Reads: 127

```
Is it possible you are pulling too many amps?
```

---
## \#25 Posted by: Kug3lis Posted at: 2018-10-01T11:18:56.789Z Reads: 124

```
Did you checked if you not reach ERPM limit? I have same issue that at high speed sometimes I get ERPM cutouts :)
```

---
## \#26 Posted by: never4getf150forums Posted at: 2018-10-01T11:19:19.181Z Reads: 122

```
how would i check this exactly? it doesn't happen at low speeds, only higher speeds when acceleration is super hard
```

---
## \#27 Posted by: never4getf150forums Posted at: 2018-10-01T11:19:50.545Z Reads: 123

```
im pretty sure that's what it is, already bought a set of new motors.. can't wait to get them switched out :grin:
```

---
## \#28 Posted by: Kug3lis Posted at: 2018-10-01T11:20:41.018Z Reads: 124

```
Because motors are not always exactly kv they specified :) you can find out your kv after motor detection writing something in console don't remember now, but at 200kv 4.2V * 12S its already over 60k
```

---
## \#29 Posted by: pat.speed Posted at: 2018-10-01T12:15:02.976Z Reads: 121

```
Well hard acceleration and high speeds definitely pull a lot of amps. A bt module is the easiest way but you probably could plug the vesc into your computer after it happens. I don’t really know how to do this though as I never have needed to
```

---
## \#30 Posted by: Kug3lis Posted at: 2018-10-01T12:59:28.409Z Reads: 114

```
One thing is that bluetooth apps has to inquire current reading and based on update rate you can not see some nasty current spikes coming up. It would be nice if vesc itself would log highest and lowest values of current voltage and etc values and would report it via same status command.

@trampa if you could forward this to Benjamin :)
```

---
## \#31 Posted by: trampa Posted at: 2018-10-01T14:15:17.070Z Reads: 107

```
Thought of already....

Frank
```

---
## \#32 Posted by: lrdesigns Posted at: 2018-10-04T04:50:14.245Z Reads: 90

```
What is the behavior on the bench with wheels in the air? This way can see if its load related or RPM related.
```

---
## \#33 Posted by: never4getf150forums Posted at: 2018-10-05T01:31:00.785Z Reads: 80

```
works perfectly fine, no issues what so ever.. it's only load related, and happened again this time accelerating full throttle from 15mph.. it triggered and cut off..

how do I figure out if it's erpm related or load related?
```

---
## \#34 Posted by: lrdesigns Posted at: 2018-10-05T01:51:30.839Z Reads: 80

```
I think you just did. Its load / amp related. If it cuts out and you plug into pc after without turning the board off there is no errors recorded?

If no then I would say its not the vesc causing the issue, some other component is at play. Battery / BMS / receiver.  Sometimes a receiver can be swamped by magnetic interference under load if its in a bad location.
```

---
## \#35 Posted by: never4getf150forums Posted at: 2018-10-05T01:54:03.442Z Reads: 79

```
No errors recorded at all last I checked, I'll admit I'm very new to vesc and the software in general so I have not a clue what I'm doing most of the time but looking in the ESC Terminal or bug console, there is no fault that pops up. I'm gonna try checking right now.

as for it being the BMS, the BMS is currently bypassed, so shouldn't be that. I have a strong feeling it's only happening under semi-hard accelerations to pass a car or get up to speed for example.. rarely does it ever happen going slow or just cruising, but it is a bit frustrating that I have to ride it like it's a boosted board in eco mode otherwise it may just cut out mid-acceleration and the momentum throws me off. I've gotten used to cut offs and I can recover from them if the road ahead is nice and empty, but with obstacles which are common in my area it's only luck that I recover, most of the times there isn't enough space to do so.
```

---
## \#36 Posted by: never4getf150forums Posted at: 2018-10-14T16:42:10.657Z Reads: 62

```
solved by a simple 10$ receiver replacement..

I recall also getting cut outs after putting my hand in a different position, and overall the connection was fluky at best. So, I figured all along it was this damn antenna / receiver.

Now it works great, 80 miles on it so far in 3 days and not a single issue...

so dang happy :grin:
```

---
## \#37 Posted by: legend27 Posted at: 2018-10-14T16:53:21.076Z Reads: 61

```
Do you have some pictures of the board?
```

---
## \#38 Posted by: never4getf150forums Posted at: 2018-10-14T18:14:02.695Z Reads: 59

```
this is it when it was brand new 

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/5940


this is it after using it for a few weeks and realizing it's too damn low, so i restored it some.

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/6169

and now i have to take updated pics, it's rougher looking now, but it works better now.
```

---
## \#39 Posted by: legend27 Posted at: 2018-10-14T18:38:42.330Z Reads: 57

```
Sweet!

10cha
```

---
## \#40 Posted by: lrdesigns Posted at: 2018-10-15T04:53:28.443Z Reads: 47

```
[quote="never4getf150forums, post:36, topic:69695"]
solved by a simple 10$ receiver replacement…
[/quote]

I was on the right track! Glad you fixed it and that I could help. :+1: :sunglasses:
```

---
