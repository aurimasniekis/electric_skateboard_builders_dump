# 25R 10S6P Vanguard. Does this battery layout look ok?

### Replies: 22 Views: 1924

## \#1 Posted by: michaelcpg Posted at: 2017-07-22T03:38:47.370Z Reads: 226

```
Hey all, getting close to finishing a new build. Thought it might be a good idea to have you guys look over my wiring design before I start connecting things up. 

I'm using a standard LCD (the same one as Enertion uses in their space cells which just shows a percentage value based on battery voltage) and an XT90S loop key for a switch. Would there be any issues with having these half way through the battery circuit as opposed to at the other end of the board with the VESC's?

I forgot to include the wiring for the charging circuit in the diagram but I'm going to be using a basic 10A BMS just for charging which will be connected down at the same point as the VESC's.

<img src="/uploads/db1493/original/3X/4/b/4b0e92ab375d1808f53547931f89a51755bde621.jpg" width="165" height="500">

Looking forward to hearing your thoughts :)
```

---
## \#2 Posted by: Vlu Posted at: 2017-07-22T04:09:48.249Z Reads: 215

```
If I understand your wiring diagram correctly, your lcd would have no voltage going through it since the  electricity would just run through the wire it is parallel to. The lcd would need to be wired with the entire battery for it to work properly. The xt90 would do its job of breaking the circuit though, so that would turn the board on/off.
```

---
## \#3 Posted by: michaelcpg Posted at: 2017-07-22T04:17:33.146Z Reads: 205

```
My understanding is that you need to run the LCD in parallel like this as if it was in series on the main circuit it would just blow due to not being designed to handle the current that our boards pull?
```

---
## \#4 Posted by: Vlu Posted at: 2017-07-22T04:23:33.458Z Reads: 203

```
<img src="/uploads/db1493/original/3X/e/9/e99c0e7490c7b7c896eb0b80b6d82ce7a7fc36f5.png" width="690" height="154">

You are correct about using parallel. But the way you have it the power would not run correctly through the lcd. This diagram would work (excuse the mspaint). This way the lcd gets the full voltage of the battery and wont need to handle the high current as you mentioned. Hope this helps.
```

---
## \#5 Posted by: longjohn Posted at: 2017-07-22T05:36:41.796Z Reads: 187

```
battery packs are not easy.

There is a good diagram here showing how current flows in the tabs.

Instead of linking P-packs at an end or another, you want to make multiple links in between cells.

You can find more info on optimal packs from endless sphere and endless sphere only.

Here the rate of engineers to amateur is not optimal for the construction of battery packs...
```

---
## \#6 Posted by: michaelcpg Posted at: 2017-07-22T05:48:38.963Z Reads: 176

```
The battery packs themselves are already complete. Might do a build log later on once the board itself is finished. This is also my second board with a custom battery so I've done most of this stuff before. 

My main concern with this build is really the placement of the LCD and loop key (I haven't used a loop key before) as obviously normally these components are at the other end of the board along with the VESC's and BMS etc so I was just curious if having them at the other end may possibly make any difference :) 

<img src="/uploads/db1493/original/3X/a/3/a34336f22f5637f3f20d4faf95533fda97194545.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/c/6/c6862039e6a332e7cbb9d553d4fce2d8f2fd6ac4.jpg" width="690" height="388">
```

---
## \#7 Posted by: willpark16 Posted at: 2017-07-22T06:14:36.926Z Reads: 168

```
LED should touch positive and negative lead of battery
```

---
## \#8 Posted by: Eboosted Posted at: 2017-07-22T06:25:38.601Z Reads: 164

```
Why not use Samsung 30Q if you are going with such a big battery?
```

---
## \#9 Posted by: michaelcpg Posted at: 2017-07-22T06:49:08.254Z Reads: 161

```
Technically it is :p
```

---
## \#10 Posted by: michaelcpg Posted at: 2017-07-22T06:50:52.128Z Reads: 161

```
I bought the cells ages ago around the time when not that people on these forum were using 30Q's so decided to stick with 25R's at the time. Had I bought the cells more recently I likely would have gone with 30Q's.
```

---
## \#11 Posted by: darkkevind Posted at: 2017-07-22T08:59:32.599Z Reads: 152

```
Doing your batteries in this way you're using up a lot of space on your board. You may want to think about dismantling them and creating one big pack, spot welded together...
```

---
## \#12 Posted by: michaelcpg Posted at: 2017-07-22T09:28:36.263Z Reads: 157

```
That was the original plan. Unfortunately that would mean the board would no longer be rated for taking on a plane. These packs also use Tesla style cell level fuses so are safer than spot welded packs.
 
Tbh, the final design I've gone with probably only adds an extra 1-2cm of length to the whole battery which is pretty much only taken up by the small amount of padding that I have around each battery pack. 

The other advantage with this approach is that separate packs means the battery handles the flex of the Vanguard much better.
```

---
## \#13 Posted by: Eboosted Posted at: 2017-07-22T14:20:39.366Z Reads: 149

```
What enclosure are you planning to use? 

I'd suggest two of my battery enclosures:

http://i.imgur.com/1Vue0hk.jpg

http://www.electric-skateboard.builders/t/loaded-vanguard-and-never-summer-reaper-enclosures-for-sale/17137
```

---
## \#14 Posted by: michaelcpg Posted at: 2017-07-22T14:38:06.391Z Reads: 142

```
Vacuum forming my own. A big concern for me is that the enclosures are as waterproof as possible. I live in the middle of NZ, so it's kind of a necessity if you want to be able to ride your board most days.
```

---
## \#15 Posted by: willpark16 Posted at: 2017-07-22T18:50:35.791Z Reads: 133

```
I can recommend rubber sealant that u can get from Home Depot
```

---
## \#16 Posted by: michaelcpg Posted at: 2017-07-22T22:13:52.684Z Reads: 117

```
I've got a 2 part design that I'm working on with a silicone seal
```

---
## \#17 Posted by: Jebe Posted at: 2017-07-22T22:17:22.955Z Reads: 117

```
New zealand. Where even the moss has moss on it 😂
```

---
## \#18 Posted by: willpark16 Posted at: 2017-07-22T22:22:06.816Z Reads: 113

```
Niceee my friend
```

---
## \#19 Posted by: michaelcpg Posted at: 2017-07-22T22:40:25.706Z Reads: 111

```
I'm not sure I understand the difference of having the LCD in parallel at that end of the battery as opposed to the other end?
```

---
## \#20 Posted by: Vlu Posted at: 2017-07-22T23:21:11.048Z Reads: 119

```
The reason the lcd would not work as intended on the side you drew it on is because the LCD needs a potential (voltage) difference between its two leads. Having it on the same side as the xt90 anti-spark plug, there would be zero potential difference because the xt90 is essentially just a wire connection. As such, there would be no change of potential at that end. However, the LCD would have a potential difference on the side with a load (VESC). The Vesc will has a significant resistance and will draw current. Thus, on the positive lead of the VESC there is the full 10s voltage and on the negative lead there is zero (the actual point of zero voltage in a circuit is arbitrary, but i chose that in this example).

In short, on the xt90 end there is no voltage drop for the lcd to measure, whereas on the other side, the VESC causes a voltage drop that can be measured.

To further clarify things (hopefully), say for example you have just a battery with positive and negative leads. you could connect the lcd to both leads and it would work. 

Now connect the vesc in parallel with the lcd, like this:

Battery+ -------> vesc and lcd -----> Battery-

and it will still work. But, connect the vesc and then the lcd/xt90 in parallel:

Battery+  -------> vesc -----> lcd/xt90 -------> Battery-

and the lcd wont work

TL:DR The problem comes from connecting the lcd in parallel with something that effectively is just a wire so the lcd does not have a difference in electrical potential. I hope this helps. :smiley:
```

---
## \#21 Posted by: michaelcpg Posted at: 2017-07-23T21:13:59.691Z Reads: 114

```
Ah I see, thanks for the detailed explanation :)
```

---
## \#22 Posted by: gpauwels0820 Posted at: 2018-04-02T04:09:07.676Z Reads: 76

```
Great layout, i wonder though how the current will affect the longer wires vs. the shorter wires on the battery packs?

I too have a battery pack for a 12S8P configuration however double stacked the batteries. I am wondering if my BMS connections are correct... Each connection is numbered 1 - 12. 

![2018-04-01_20-22-18 - battery BMS example|690x331](upload://kOn3wsYkVdVyViS6q1otQYZT6Su.jpg)
```

---
