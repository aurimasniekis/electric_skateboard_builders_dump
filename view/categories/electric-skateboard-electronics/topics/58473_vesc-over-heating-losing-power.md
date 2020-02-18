# VESC over heating/losing power?

### Replies: 9 Views: 468

## \#1 Posted by: LAVAMAN Posted at: 2018-06-11T00:53:24.998Z Reads: 120

```
I got two 6S LIPO's last week. I was going to save them for my second build (in progress) but was having issues charging my 6S batteries (3x2S LIPO's) so decided to switch and use them on my current board (1st build). After charging them up and changing settings with VESC tool (6S to 12S) I went out for a test ride. They are excellent, super fast (faster than I really want to go) which is exactly what I was looking for but before I could finish my ride they slowed way down to a crawl, but got me home. I thought it might have been the capacity (old setup was 5600 mah, 50-100c discharge) and new batteries are 4500 mah, 40c discharge) but after balance charging them again (all cells at 4.20V) and going out for a second ride a few days later, I experienced the same thing. So I checked the voltage when I got home to discover all cells at 3.95 (70% of full charge) so I took off the VESC cover and found VESC to be a bit hotter than I think it should be. 

Here is my question. Is the VESC designed to reduce power automatically when it exceeds a certain temperature to prevent it from over heating? When I changed settings with VESC tool from 6S to 12S I also changed motor max setting to 85A and battery max setting to 50A which is higher setting than previous on 6S batteries. I have done a search for heat sinks for VESC and will probably remove the heavy rubber heat shrink that (Thermal M16) put on it after repairing it for me and also add a chunk of aluminum to draw heat away from VESC mother board. I can also drill ventilation holes in my VESC enclosure to increase airflow. I also must share that I live in Hawaii and am using my board on dry blacktop roads at low 80 degree days. Are there any settings I can change that will help the VESC run cooler without slowing me down too much? 
Thanks in advance for any advice you might be able to share.
```

---
## \#2 Posted by: CarlCollins Posted at: 2018-06-11T05:01:21.853Z Reads: 91

```
@LAVAMAN

Try reducing the Batt Max to 30A
also check if your motor is not faulty, Seems to be the issue with the motors
```

---
## \#3 Posted by: L3chef Posted at: 2018-06-11T06:55:26.856Z Reads: 73

```
Did you change the battery cut off voltage? Soft and hard?.
```

---
## \#4 Posted by: LAVAMAN Posted at: 2018-06-11T16:40:45.231Z Reads: 60

```
No, I did not. I thought with the new VESC tool that it made those adjustments for you when you select 12S in the battery App. I will look into that. Thx
```

---
## \#5 Posted by: LAVAMAN Posted at: 2018-06-11T16:42:58.990Z Reads: 58

```
Thanks, I will try that. Motor is Enertion "big boy" and has very little use so I don't think it is the motor. Never had any issues on 6S, just not fast enough.
```

---
## \#6 Posted by: wafflejock Posted at: 2018-06-11T20:41:40.899Z Reads: 54

```
If you are using lipo I believe you need to manually set the battery voltage limits I think the drop down selection thing just works for li-ion (could be wrong though haven't used it as much as bldc-tool yet).  With higher voltage you should need far less amps to deliver the same watts, 20V x 10A = 200W, 40V * 5A = 200W the higher amperage is what causes more loss as heat so I don't see how it would be getting hotter now than it was before really.  Would do some bench testing between the two batteries and see if there is anything obvious standing out in the realtime data section in the VESC tool with regard to amperage or temperature.
```

---
## \#7 Posted by: LAVAMAN Posted at: 2018-06-11T21:12:01.457Z Reads: 44

```
I went back into VESC tool and set my soft/hard LIPO cutoff to 36V and 33.6V. I also changed my motor max to 60A and Battery max to 40A. I then went out for a ride and experienced some slow down after it had a chance to heat up and some jerky throttle response. That bucking throttle response is a bit scary, can catch you off guard and could throw someone off (luckily not me today). I was very cautious after that. I have seen the internals of several store bought boards and never remember seeing VESC heat sinks or ventilation of VESC enclosures. I wonder how they are dealing with these issues? Most decent ready to ride boards have large batteries and above average power. I should be able to fix this with VESC settings alone. I have to keep experimenting.
```

---
## \#8 Posted by: L3chef Posted at: 2018-06-12T08:26:01.864Z Reads: 34

```
[quote="LAVAMAN, post:7, topic:58473"]
36V and 33.6V
[/quote]

Didn't you have a 12s battery?
```

---
## \#9 Posted by: LAVAMAN Posted at: 2018-06-12T16:54:55.475Z Reads: 25

```
Yes, just switched to 12S from 6S. I set soft cutoff at 3.0V (36V) and hard cutoff at 2.8V (33.6V)
```

---
