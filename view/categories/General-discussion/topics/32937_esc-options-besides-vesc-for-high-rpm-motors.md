# ESC Options besides vesc for high rpm motors

### Replies: 20 Views: 1007

## \#1 Posted by: Dariks Posted at: 2017-09-12T05:09:56.533Z Reads: 96

```
Hay guys I'm trying to find a solution for a super light weight setup that goes about 15mph. I heard the vesc has problems with higher rpm motors. So I'm looking for other options. Going for a 6s setup or less if possible. The motors I'm planing are using are 500-600kv.
```

---
## \#2 Posted by: JdogAwesome Posted at: 2017-09-12T05:37:50.135Z Reads: 93

```
I'd say just using a normal RC car ESC would work, I know they work with Kv motors in the thousands so it should work fine. Though why are you using such a high Kv motor in the first place? And does the VESC really not work well for higher Kvs I'd like to hear more from other people.
```

---
## \#3 Posted by: Dariks Posted at: 2017-09-12T05:40:24.959Z Reads: 91

```
Oh I'm using a high rpm because the motors are way lighter which translates into a lighter set up its for a 80lb/40kg person so torque is not really a issue.
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-09-12T05:45:03.155Z Reads: 83

```
260kv 1:3ratio 6s boom 25mph. u dont need to go that high kv
```

---
## \#5 Posted by: pat.speed Posted at: 2017-09-12T05:45:43.412Z Reads: 82

```
Even for someone that light those motors might not produce enough torque although it will depend on your gearing and wheel size. I would not go over about 350kv
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-09-12T05:47:08.996Z Reads: 82

```
if u go high rpm u loose more energy to heat and friction. it will loose much range
```

---
## \#7 Posted by: Cobber Posted at: 2017-09-12T05:51:59.947Z Reads: 80

```
these have been thrashed and abused by the best. I've never read of one being roached?
https://www.hobbywingdirect.com/products/ezrun-max6-esc?variant=4075925316
not the cheapest option but it is also water proof...
```

---
## \#9 Posted by: trampa Posted at: 2017-09-12T06:11:11.523Z Reads: 69

```
Power has nothing to with KV. The motors are all identical as long as the copper fill is identical. Weather you use a longer and and thinner wire or a shorter and thicker wire doesn't matter for the motor. High KV just puts more strain on the ESC and Battery. In consequence a high KV setup needs a stronger battery, which is heavier (more cells in parallel).

If you want it light and slow you need to limit amp flow and choose a low KV motor, not a high KV motor. In that case you can use VESC-based HW, offering all the benefits it brings on the table.

Frank
```

---
## \#10 Posted by: Dariks Posted at: 2017-09-12T06:14:26.194Z Reads: 67

```
Oh umm I want to use 6s max though so I can use rc charger balancing. And whats this VESC-Based HW?
```

---
## \#11 Posted by: pat.speed Posted at: 2017-09-12T06:19:05.928Z Reads: 64

```
He just means a type of Vesc
```

---
## \#12 Posted by: Dariks Posted at: 2017-09-12T06:20:39.821Z Reads: 62

```
Oh ok lol I didn't even know there are different vesc's aren't they all the same?
```

---
## \#13 Posted by: trampa Posted at: 2017-09-12T06:34:06.895Z Reads: 64

```
You can use any quality HW offering vendor offering VESC-Project based ESCs. I would invest in a quality product - there are some options on the table. Search the Forum....
The 4.12HW probably does the Job to get started.
Our VESC SIX might be overkill, but if you have the cash, it's also an option. Would be very smooth and bullet proof. The hobby ESCs are very aggressive on the throttle and brake, you can't adjust them properly, since they are voltage controlled and not current controlled.
Such an ESC is a simple rpm adjuster only.
There is no smart software behind these products allowing a reasonable adjustment of relevant parameters. You can adjust any VESC-based ESCs in a wide range, allowing settings in a range from from child friendly to rocket boost. 

Frank
```

---
## \#14 Posted by: rojitor Posted at: 2017-09-12T11:00:36.097Z Reads: 55

```
For 6s this is good:

[https://www.banggood.com/FVT-CBWI120A-ESC-Brushless-Speed-Controller-For-110-and-18Series-RC-Cars-Skateboard-ESC-p-985970.html?rmmds=search](https://www.banggood.com/FVT-CBWI120A-ESC-Brushless-Speed-Controller-For-110-and-18Series-RC-Cars-Skateboard-ESC-p-985970.html?rmmds=search)
```

---
## \#15 Posted by: gogomrrobot Posted at: 2017-09-26T01:48:53.435Z Reads: 41

```
Just got back from a ride with a dual Max6 --- tearing up a golf course :slight_smile:

Do I just have the wrong controller or something? Is my board too heavy? I get almost knocked on my arse every time I touch the throttle. I am trying to like ease into the throttle and sometimes I can get that to work.  I feel like maybe my mistake with this build was that I got a Trampa Long deck + TB motor mount... it was my first noob build so I had no clue. I got a deck that is heavy and TB motor mount is heavy... so I feel with my weight on it (80-82 kgs with gear on)... the board doesn't move and then BAM each time. I had my buddy try it out.  We figured out a trick where you can roll your thumb so slowly on the accelerator that the jerkiness doesn't happen. It's easier on the grass, on the pavement its a hit or miss if the jerky takeoff can be avoided :frowning:  FYI I did set the punch on the Max6 to level 1 (the lowest).

This is my controller:

https://www.amazon.com/gp/product/B073XSL89B/ref=oh_aui_detailpage_o07_s00?ie=UTF8&psc=1

Maybe I should switch remotes?
```

---
## \#16 Posted by: GrecoMan Posted at: 2017-09-26T01:52:37.828Z Reads: 40

```
did you calibrate ppm?
```

---
## \#17 Posted by: gogomrrobot Posted at: 2017-09-26T01:55:04.660Z Reads: 40

```
what is that? I am looking at the HobbyWing program card... options #1 to 11.  That's not on there
```

---
## \#18 Posted by: GrecoMan Posted at: 2017-09-26T01:57:41.549Z Reads: 39

```
oooohhhh thought you were using vesc.  Is there a throttle trim on the remote? any sort of dials?
```

---
## \#19 Posted by: gogomrrobot Posted at: 2017-09-26T02:01:20.520Z Reads: 38

```
Nope just forward and back.  I tried Up, Up, Down, Down, Left, Right, Left, Right, B+A + start... no use.
```

---
## \#20 Posted by: gogomrrobot Posted at: 2017-09-26T02:04:05.294Z Reads: 39

```
Ok that was a reference to a video game before your time... likely ;)

But seriously... you think it's the remote?
```

---
## \#21 Posted by: JdogAwesome Posted at: 2017-09-27T16:22:12.002Z Reads: 26

```
No I think it's because that ESC simply isn't made for EBoards so it has a lot of kick and very fast ramping. Though did you calibrate your throttle end points? If not I'd recommend doing that and see if it helps.
```

---
