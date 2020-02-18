# Gear ratio belt length

### Replies: 27 Views: 3427

## \#1 Posted by: curtis Posted at: 2017-11-10T17:48:59.506Z Reads: 323

```
How is the length of the belt determined? The Gear Reduction Ratio?  Is it just that bigger gears need longer belts?
https://www.bbman.com/belt-length-calculator/ How do I use this?
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-11-10T17:52:42.681Z Reads: 316

```
You have to know the diameter of both pulleys (or the teeth number and size) and the distance between the two pulleys. Changing either the diameter or the distance will change the belt length.
```

---
## \#3 Posted by: Idle Posted at: 2017-11-10T18:09:08.534Z Reads: 292

```
I had no problem using that calculator. 
Just click all the clickys that you know and it will spit out the length you need. 
Center to center also.
On a side note, does anyone have any 280mm belts in the US..?

<img src="/uploads/db1493/original/3X/d/a/da9712dc496abc1cb4ab7b89abdfe6b2e010d3d2.PNG" width="690" height="388"><img src="/uploads/db1493/original/3X/a/9/a991d6574cb00518f5860709f480ab24d4a8724a.PNG" width="281" height="500">
```

---
## \#4 Posted by: MrHappy Posted at: 2017-11-10T18:17:25.585Z Reads: 230

```
http://www.vbeltsupply.com/280-5m-15-synchronous-timing-belt.html
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-11-10T18:36:04.936Z Reads: 215

```
VBS is my go-to. They even have weird ones like 390mm.
```

---
## \#6 Posted by: curtis Posted at: 2017-11-10T23:38:32.412Z Reads: 203

```
So I am correct in saying a larger gear rato means that their is a bigger belt. A smaller gear ratio wouldn't have to have a as big of a belt.
```

---
## \#7 Posted by: akhlut Posted at: 2017-11-10T23:41:02.220Z Reads: 193

```
[Center Distance Designer](https://sdp-si.com/eStore/CenterDistanceDesigner)
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-11-10T23:43:44.676Z Reads: 192

```
Not always. The key word is **ratio**. You could have a 20t and 40t gear, and that would be a smaller ratio than a 10t and a 30t, but the belt would be longer. 

If you only change ONE pulley, and you make the pulley bigger, then the belt will be bigger.
```

---
## \#9 Posted by: curtis Posted at: 2017-11-10T23:44:39.612Z Reads: 184

```
I did that and I only got this
Attribute	Value
Speed Ratio	0.39
Pitch Diameter - Large Pulley (A) (in)	5.730
Pitch Diameter - Small Pulley (B) (in)	2.228
Desired Belt Pitch Length (in)	 ?
Next Available Belt Pitch Length (in)	 ?
Next Available Number of Teeth - Belt	 ?
Center Distance Using Next Available Belt (in)????	 
Teeth in Mesh
```

---
## \#10 Posted by: curtis Posted at: 2017-11-10T23:46:55.886Z Reads: 166

```
The question I need answering is Desired Center Distance (in)/ how do you figure that?
```

---
## \#11 Posted by: Idle Posted at: 2017-11-11T00:59:45.456Z Reads: 152

```
You need to input the center to center distance.

Use mm not inches as the belts are metric.

Do you have a mount to measure?
```

---
## \#12 Posted by: curtis Posted at: 2017-11-11T01:39:54.496Z Reads: 144

```
No.I don't have a motor mount to measure. I know what it's asking but the problem I have is I don't know what center distance to use. That is the last thing I think I need.
```

---
## \#13 Posted by: MysticalDork Posted at: 2017-11-11T02:08:15.117Z Reads: 134

```
What mount do you plan to use? Most mount sellers can tell you the belt length that works with their mount. Also, those diameters seem really large for esk8. Are you sure you picked the correct belt pitch?
```

---
## \#14 Posted by: curtis Posted at: 2017-11-11T02:16:03.022Z Reads: 124

```
?[quote="MysticalDork, post:13, topic:37943, full:true"]
What mount do you plan to use? Most mount sellers can tell you the belt length that works with their mount. Also, those diameters seem really large for esk8. Are you sure you picked the correct belt pitch?
[/quote]
I am going to build my own so this is why I need to figure this out.  I know my gear ration 14/36, a .75 belt width and the pitch is L don't quite understand the pitch thing.
```

---
## \#15 Posted by: MysticalDork Posted at: 2017-11-11T03:44:57.292Z Reads: 118

```
Ahh, right. You need to pick a different belt type. The standard one most of us use is HTD 5mm. It's under the metric selection.
```

---
## \#16 Posted by: curtis Posted at: 2017-11-11T03:48:47.821Z Reads: 115

```
[quote="MysticalDork, post:15, topic:37943, full:true"]
Ahh, right. You need to pick a different belt type. The standard one most of us use is HTD 5mm. It's under the metric selection.
[/quote]

That still doesn't get the center distance.
```

---
## \#17 Posted by: MysticalDork Posted at: 2017-11-11T03:52:21.720Z Reads: 109

```
Nope. But it gets you more realistic pulley diameters. Then you can make up your own center distance, since you're making your own mount. Rule of thumb, shorter mount is better because stiffness. Go as short as you can and still be able to tighten the motor screws without taking the wheel off.
```

---
## \#18 Posted by: MysticalDork Posted at: 2017-11-11T03:53:35.592Z Reads: 100

```
I designed my own mounts in a cad program so I could visualize the dimensions better.
```

---
## \#19 Posted by: Idle Posted at: 2017-11-11T03:53:52.206Z Reads: 103

```
First of all, change everything to metric, as all your components are metric.

And use the esk8 calculator to decide on your gearing if you haven't already.


http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":240,"system-efficiency":95,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":97}|

Then on the belt calculator page
Pick a number (in mm) for your ctc (center to center) distance.

Try 75

Look at what the belt length is. 

Adjust the ctc distance untill it's right at the specific belt length you need. 


Make your mount with same ctc distance and your golden.
```

---
## \#20 Posted by: curtis Posted at: 2017-11-11T03:58:40.459Z Reads: 96

```
http://www.electric-skateboard.builders/t/gear-ratio-belt-length/37943/15
Why are you so opposed to 14t/36t? isn't like 16t/36t like pretty mainstream?
```

---
## \#21 Posted by: Idle Posted at: 2017-11-11T04:20:21.935Z Reads: 84

```
Omg, please finish talking untill you're actually ready for some help.

Nobody knows what you are trying to do, we are simply guessing, and/or assuming with the VERY limited info you've provided. 


You haven't stated any facts about your build except for:

Randall trucks. 

Deck
Motor/s
Battery
Trucks
Wheels
Esc
Top speed you desire
Range

*yes it matters very much

*without all the info, there's no way we can possibly hijack this thread and argue about bearings, rogue axles and red circles.


That is all.
```

---
## \#22 Posted by: MysticalDork Posted at: 2017-11-11T04:37:14.735Z Reads: 76

```
I didn't say anything at all about 14t/36t.  I was mentioning https://www.electric-skateboard.builders/t/gear-ratio-belt-length/37943/9?u=mysticaldork where you have some very large values for pitch diameter. 2.228 and 5.7 inches, for a 14/36 doesn't add up for a HTD5 pulley.

14t is a little on the small side just because there won't be many teeth engaged in the belt at any time, and more teeth allow more torque without slipping. Should still work though.
```

---
## \#24 Posted by: curtis Posted at: 2017-11-11T17:42:03.916Z Reads: 74

```
The gear ratio I plugged into the calculator was 14/36.
```

---
## \#25 Posted by: curtis Posted at: 2017-11-11T17:45:25.172Z Reads: 76

```
First off I tried to reply yesterday and was unable to since I am a new member.  Only so many amount of post I can make. 
As you requested.The center distance. That's what I need to figure out.
I don't think this changes much 
I have randles trucks 
balute orangatang wheels that are 73mm, a gear ratio
The only recognizable thing on my deck is that it's from db long boards. It is top mount.
Top speed 20-35 mph 
bones reds with some spacers
Probably the Vesc
and a range of 20 miles
motor 190 kv
Battery 1860 10s 4p
```

---
## \#26 Posted by: Idle Posted at: 2017-11-11T17:51:36.202Z Reads: 74

```

Edit your last post please.
Battery is not stated
```

---
## \#27 Posted by: DevinG Posted at: 2018-01-28T03:03:31.270Z Reads: 68

```
i couldnt find a belt using this.... 
this is what im working with...
 
|Attribute|Value|
|---|---|
|Speed Ratio|0.33|
|Pitch Diameter - Large Pulley (A) (mm)|95.5|
|Pitch Diameter - Small Pulley (B) (mm)|31.8|
|Desired Belt Pitch Length (mm)|372.8|
|Next Available Belt Pitch Length (mm)|375|
|Next Available Number of Teeth - Belt|75|
|Center Distance Using Next Available Belt (mm)|81.3|
|Teeth in Mesh  |7|
```

---
## \#28 Posted by: drangboards Posted at: 2018-12-01T00:17:00.317Z Reads: 34

```
So people say no no to using v1 boosted belts on a v2, however they fit just fine.  What could go wrong?  Hold my beer.

Also, not sure if this has been shared yet, but I found this cool calculator for this very topic. 
https://www.blocklayer.com/pulley-belteng.aspx
```

---
