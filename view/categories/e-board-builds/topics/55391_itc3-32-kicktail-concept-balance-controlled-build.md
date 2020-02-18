# ITC3 - 32&rdquo; Kicktail concept balance controlled build

### Replies: 6 Views: 422

## \#1 Posted by: oliverhopcroft Posted at: 2018-05-14T07:16:01.353Z Reads: 123

```
I posted this on my blog but nobody reads that so I'm copying it here. Feel free to skip the first few paragraphs if they're too narrative but I'm leaving them in.

Two weeks ago at a journalism convention in San Francisco, a friend and I rented and nearly crashed some exhilarating electric scooters. These have since been banned. About a week ago I stumbled upon a build log for a skateboard powered by an electric motor. After binging DIY electric vehicle videos on youtube for a few hours, I was hooked. Over the last few days, I've began a project to engineer and build my own.

My idea is to build upon already existing design by changing the control system from the current standard of handheld RC controllers to a balance-driven system in which the user leans forward or backwards to set the throttle. This has several advantages-- it's simpler, more intuitive, and eliminates the need for a separate battery-powered device. In addition to this, I have laid out some other design goals. The board should be small and light enough to carry, blend in with regular longboards from a distance, and travel fast and far enough to be a useful means of transportation.

To accomplish this I will use a combination of commercially available RC-car parts and modified or custom designed ones. Power will be supplied by some high energy density rechargeable batteries (Li-ion, LiPo, or LiPoFe4) to a control system made of an RC speed controller and an additional microcontroller. This system will get input from sensors to detect the rider's balance and possibly a gyroscope or accelerometer. Turning will be accomplished through the trucks by leaning, as is standard on a skateboard.

I have never ridden a skateboard or longboard before, so riding this will certainly be a learning experience. I also have no idea if the balance control will mess with the rider's ability to balance on the skateboard, but I hope that with the right settings I can get this to work out. 
       
For this project, I chose a 32" kicktail cruiser deck, 180mm trucks, and 90mm wheels. This deck is the smallest I could go while still fitting all the electronics and I opted for fairly large wheels to improve the ride. To sense the rider's balance, I'm using load cells. These are metal devices with strain gauges attached. When load is applied, a piece of metal flexes, and the gauge mounted on it changes resistance. 

The change is too small to detect directly, so I've added two HXT711 analog to digital converter boards to amplify the signal. These send a signal to an ATMEGA328p microcontroller (knockoff arduino UNO). There are several existing libraries for the HXT711, one of which I'm using to dump output on the serial port.

To mount the sensors on the board, I briefly considered having two pads on the top to step on. This, however, violates the design plan-- the skateboard needs to be balance controlled, and that would be no different than stepping on switches.

The current plan is to mount the strain guages inside risers. These are small, 1/8" to 1" pieces of plastic that go between the board and the trucks to add some height. My trucks came with 1/4" risers and hardware for them, so I want to see if I can fit the load cell within a riser of this size.

[img]https://i.imgur.com/7W8CEXh.jpg?1[/img]
[img]https://i.imgur.com/IlAzNfK.jpg[/img]

My first iteration, pictured above, was made of stacked laser-cut birch wood sheets, and amusingly, a piece of nail file. There was pocket for the load cell, space for the load-bearing part to deflect down, a hole for the wires, and a lid on top. This test was a great success-- all assembled, the board was able to detect the two load values and output a graph.

[img]https://i.imgur.com/uZMsYHq.jpg[/img]

Iteration two includes six stacked rubber sheets in the same design with some minor refinement. Instead of a lid, the top can now flex, and I hope the rubber will absorb some shock from the ride. 

I took a video of a test of this system. It's a bit hard to see but the two lines on the screen are values from the two load cells. The system is pretty responsive and it's clear that the concept works. There is some latency but I think I can sort it out.

https://www.youtube.com/watch?v=qLQW3EJW9R0

I've also started work, as well, on turning the raw data into usable control for the throttle. Right now, I'm using the formula
  
(F-front - F-back) / (F-front + F-back)

In addition, if F-front + F-back is below a certain value, the balance score is set to zero. This provides a score between -1 and 1 of the rider's balance on the board (1 is all weight on the front, -1 all weight on the back). I have no idea if an approach this simplistic will be enough to actually control the board. Since acceleration affects the rider's balance, I have a feeling the solution might end up being a model with differential equations.

For now, though, I'm satisfied with the performance of the sensors and I'm moving on to the drive system. I'll post here with updates as I make more progress.
```

---
## \#2 Posted by: linsus Posted at: 2018-05-14T07:26:07.976Z Reads: 104

```
Clever use of the straingauges, had similiar thoughts but been way too lazy to make it reality.
Also been pondering a flexresistor in a glove to make a fist for throttle. Skipping any handheld controller would be ace tho!

Gl!
```

---
## \#3 Posted by: philvanzu Posted at: 2018-05-14T07:44:01.618Z Reads: 98

```
You wont be using your kicktail much if your board goes full brake everytime you hit it no?
also when carving I think my weight is slightly oscillating from front to back. Not sure if it is normal but you will want your software to take that into account
```

---
## \#4 Posted by: lock Posted at: 2018-05-14T09:51:06.868Z Reads: 89

```
The signal you’re getting seems quite noise free. Maybe it’s the sensors, or you’ve already got a filter implemented. If not, I’d expect you may need one once you hit the road and all it’s imperfections.

Looking forward to see how this goes. Can’t imagine I’d ever go for this control method, but it’s certainly got applications for feeding these inputs into some sort of stability control system.
```

---
## \#5 Posted by: faithfulpuppy Posted at: 2018-05-14T11:22:34.196Z Reads: 66

```
I'm working on a glove controller right now. I'm either doing that or linear slide potentiometers on the back of my hand connected to wires that run to my fingertips
```

---
## \#6 Posted by: linsus Posted at: 2018-05-14T11:37:15.830Z Reads: 63

```
Cool!

Not sure if you can reach good enough accuracy with flexresistors.
Think jaykay e trucks had a throttle that was based on sensing the movement of tendons on your wrist. So kind of a wristband.
It was only a concept that i Think didint work out in the end tho
```

---
