# Automated skateboard

### Replies: 8 Views: 400

## \#1 Posted by: LittleGiant Posted at: 2019-02-02T18:27:23.932Z Reads: 202

```
Hello, Im starting a project called Automated skateboard. There are not many simmilar projects, so I figured out it would be useful to create a new topic on this page. Also Im building everything from scratch so Im sure there will be many topics to talk about.
The idea is to connect Arduino to VESC via UART. Some functions are:
1) Drivers detection using flex sesnor. If driver is standing on the deck it bends a little, and flex sesnor changes it`s resistance.
2) Turn assistant. Using proximity sensor on the side of skateboard it will measure the distance between skateboards side and ground, that way Arduino will know which way skateboard is turning and adjust motor speed.
3) Signal lights. I will use RGB LED stripe on the back of the skateboard to signal turns and stop.
Will add more information soon :slight_smile:
```

---
## \#2 Posted by: CoolRextreme Posted at: 2019-02-02T19:24:09.501Z Reads: 174

```
They all sound like cool ideas! Can't wait to see them in action :slight_smile:
```

---
## \#3 Posted by: flozilla Posted at: 2019-02-02T19:29:57.703Z Reads: 165

```
Also had the idea for #1. 
Heard strong arguments against it.
Would love you to prove otherwise!

https://www.electric-skateboard.builders/t/inspiration-for-new-esk8-inventions/42894/68?u=flozilla
```

---
## \#4 Posted by: CoolRextreme Posted at: 2019-02-02T19:35:04.140Z Reads: 143

```
Yeah, maybe not do a **full break** when no one stands on the board.
I tend to tackle XL-sized potholes by jumping a bit off my board to lessen the weight and help it glide over a bit smoother (whilst saving my ankles)

I like to come back down knowing my board is still moving about the same speed as I am, and not just sitting on the other side of the pothole to afraid to cross :laughing:

I was thinking more of a weight sensor; Less weight = lower top speed overall, or something like that.
```

---
## \#5 Posted by: DerelictRobot Posted at: 2019-02-02T19:36:55.694Z Reads: 132

```
As a general rule of thumb, no critical control system should ever be tied to an uncertain or environmentally unstable input. 

Convenience should never impact reliability and consistent expected machine behavior.
```

---
## \#6 Posted by: DerelictRobot Posted at: 2019-02-02T20:15:05.799Z Reads: 110

```
Actually, I'll expand a little on this as I currently have an embedded quad core x86 Linux system inside my main board for tinkering with some advanced sensory running ROS.

[quote="LittleGiant, post:1, topic:82925"]
The idea is to connect Arduino to VESC via UART. Some functions are:

1. Drivers detection using flex sesnor. If driver is standing on the deck it bends a little, and flex sesnor changes it`s resistance.
[/quote]

Few things- a lot of skaters do not ride locked into a single stance. Depending on the terrain, weather, how fast I'm going, or how hard I'm carving, I'm all over my deck. I can't imagine riding a board knowing there was an ebrake attached to the deck's flex, I move around all the time and bounce up and down like a dickhead on my LaCroix flex deck. You're also going to find that most flex sensors suck- the ones you see online for $5-15? They suck. Bad. You'll end up paying a good amount for a decent FSR, and in the end you're still left with a dangerously unreliable input tied to a VERY critical control system (brake). This is a recipe for disaster. 

[quote="LittleGiant, post:1, topic:82925"]
Turn assistant. Using proximity sensor on the side of skateboard it will measure the distance between skateboards side and ground, that way Arduino will know which way skateboard is turning and adjust motor speed.
[/quote]

My points about critical control systems tied to unreliable inputs apply here. If you take the time to do sensory applications and log the output you'll see what I mean. It is never this simple. Look into 9-axis IMUs, there are some really low drift, affordable options these days that when combined with telemetry data from your encoders can be used to capture a useful motion profile. With that said, do no tie it to your throttle. 

[quote="LittleGiant, post:1, topic:82925"]
Signal lights. I will use RGB LED stripe on the back of the skateboard to signal turns and stop.
[/quote]

Go nuts. :slight_smile:
```

---
## \#7 Posted by: SeanHacker Posted at: 2019-02-02T23:22:14.375Z Reads: 81

```
[quote="DerelictRobot, post:6, topic:82925"]
I move around all the time and bounce up and down like a dickhead on my LaCroix flex deck.
[/quote]

I can vouch for this.
```

---
## \#8 Posted by: LittleGiant Posted at: 2019-02-16T16:33:08.422Z Reads: 48

```
Hello, guys, so the first thing I want to do is conect 2 3S batteries in series with 6S BMS. I want my BMS to onIy work on charging and bypass discharge. Did some research and drew a diagram, could any one experienced chek if it is correct? I would appreciate it.![image|491x500](upload://8la8RvofRwxgGsK5gBvWYYZPVHN.png)
```

---
