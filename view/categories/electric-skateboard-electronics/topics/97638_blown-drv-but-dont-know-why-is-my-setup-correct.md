# Blown DRV but don&rsquo;t know why, is my setup correct?

### Replies: 5 Views: 171

## \#1 Posted by: Anditheblacksmith Posted at: 2019-07-01T14:46:28.296Z Reads: 67

```
After years of saying but no doing I finally got my build done 2 weeks ago. Had a few test runs then about 2 miles of riding before heading off to work at Glastonbury festival where I had planned to use it to get around site on. First day out and it rode lovely at 20mph (first build so didn't want to set it to go too fast!) or so on everything I came across, after twenty minutes or so I stopped to see friends for an hour but when I went to leave one wheel didn't move and the other just rotated a little and stopped. Looked in the box and one of the vescs was flashing red three times, the other was fine. Already knew that it meant the drv was probably fried so walked back to my rig and plugged it in to confirm and yes, it was gone :-( 
I know they can just go, but can anyone see any reason for the sudden failure?
I'm running : 
2x Zippy Flightmax 30c series 8mAh 5s packs in series
2x Turnigy sk8 vesc4.12
2x Turnigy sk8 6374 192Kv
13:55 gearing on 6mm chains
Scrub Psycho with 200mm tyres
I'm about 68kg
![Screenshot%20(5)|690x387](upload://859CQTn9oOLDcCNoKKOXU6CLYJP.png) 
![Screenshot%20(4)|690x387](upload://nZYht6QHV4kUCP9sAE0qTGUiLbV.png) 
![Screenshot%20(6)|690x387](upload://vzjrcFuLIIY8jH93mdjn6LhRWEN.png) 
![Screenshot%20(7)|690x387](upload://mgKzBlwKxEwKuAqNkWnu3rEMsQw.png)
![Screenshot%20(8)|690x387](upload://i27cxkc3Esm0XgKeanECOLBdOzB.png) 
![Screenshot%20(9)|690x387](upload://el4ej7QulQdVRPj7FDU8cWRFvHK.png) ![Screenshot%20(10)|690x387](upload://hzgiC71HIbVQZweBl3pJzZK3IW7.png) 
![Screenshot%20(11)|690x387](upload://xEYQSqfMYdqRE6oAoPLkfMiB6Jl.png) ![Screenshot%20(12)|690x387](upload://txeSFsSmZuGyaOdpuxlUfxdyVRG.png) 
![Screenshot%20(13)|690x387](upload://qUbZfW6eBKKCGf2B8rOJ4pDgvAX.png) 
![Screenshot%20(14)|690x387](upload://5iXeBsgEdzV0fjdM7eSumqYiBYM.png) 
![Screenshot%20(15)|690x387](upload://6QzjJtJEG5Y0yDgNOdt4UnSGwLp.png) 
![Screenshot%20(16)|690x387](upload://wMr1irKs1beHMZENHTnzKErrykp.png) 
![Screenshot%20(17)|690x387](upload://e5cW5yl6XQg2CKBxoUaVCe2udvx.png) 
![Screenshot%20(18)|690x387](upload://x0lqp0WaVEzLcC1c6HyGu7bOoFt.png) ![Screenshot%20(19)|690x387](upload://1CuDcDC7PimCgbmCpJaBMlMiHni.png) 

As I say, it's my first build, so I'd appreciate any help anyone can give me. I knew it wasn't going to be cheap to do a build, but I didn't expect to be having to replace stuff already!!
```

---
## \#2 Posted by: Michaelppainter Posted at: 2019-07-01T17:00:27.706Z Reads: 50

```
Motor max and battery max look high for those 4.12 vescs. Can't they only handle 50a continuous?
```

---
## \#3 Posted by: Anditheblacksmith Posted at: 2019-07-14T09:54:50.688Z Reads: 33

```
Yeah, they are 50A max. I set it to higher amps because I was thinking it would limit the surge current. Not paying proper attention was I, too keen to ride!
```

---
## \#4 Posted by: b264 Posted at: 2019-07-14T11:10:29.539Z Reads: 32

```
-4A battery min is going to be pretty light brakes at high speed.  You could even double that if you wanted.

90A battery max is waaaay too high.  Try 25A battery max to start with (per ESC) and bump up from there if stuff stays cool.
```

---
## \#5 Posted by: Anditheblacksmith Posted at: 2019-07-21T16:10:24.698Z Reads: 19

```
Sorry for slow reply, been away working at festivals. Thanks for that, it's my first build so I didn't want to risk blowing the batteries with too much regen. What would you consider the maximum regen? I've replaced both vescs with Flipsky fsesc 4.12s now, if I were to set the motors to 45A and -45A and the batteries to 35A and -8A do you think I'd be safe?
Bloody expensive learning curve innit?!
```

---
