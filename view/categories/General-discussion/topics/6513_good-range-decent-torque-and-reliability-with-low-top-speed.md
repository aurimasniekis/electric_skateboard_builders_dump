# Good range, decent torque and reliability with low top speed?

### Replies: 10 Views: 1175

## \#1 Posted by: shveddy Posted at: 2016-07-23T09:01:30.859Z Reads: 118

```
Hi everyone!

I'm looking to make an E-board for commuting purposes, but I have some unique circumstances that I think might lead to unique priorities in the design and component choice. 

The main issue is that I have suffered a couple of relatively severe injuries in the past few years that have left me with certain physical disabilities. For the most part I can work around my limitations and you wouldn't be able to tell that anything happened if you saw me on the street, but I still have to think very carefully about the pros and cons of pretty much any physical activity I want to do, particularly if it is something as potentially dangerous as an electric skateboard. 

Injury wise, I have weak ankles because I broke my back and paralyzed myself for a while. Most of my muscles came back to 80-90% strength, but my left ankle is pretty much useless and I can't run all that fast. As far as skateboarding goes, this means that I can't really balance on one foot and propel myself forward with the other, and it means that I shouldn't go very fast because I can't jump off and run it out at higher speeds. That being said, I can ride just fine if the propulsion comes from elsewhere (e.g. I can still snowboard fairly well, and I can easily ride a longboard down a hill).

So  in light of all this, here are the pros and con.

Pros:

1. An electric skateboard would help me get around town. It isn't easy for me to walk long distances. I can do it, but it's a chore. Imagine having to run a mile or two every time you wanted to go someplace - it's doable, but you have to be pretty motivated and you end up at your destination seriously drenched in sweat. Because of this I rarely go anywhere without my bike, but that still leave me sweaty and more importantly it isn't nearly as portable. Which leads me to #2...

2. I can take an electric skateboard with me on airplanes and public transportation. I honestly don't mind the workout, and I would be perfectly happy with my bike if not for the fact that I can't easily travel with it. Whether I'm taking a bus to another city or flying to a different country, I have to leave my bike behind deal with the city as a pedestrian. I travel quite a bit for work and for fun, and again, while I manage just fine - it's just quite the chore and it would be awesome to grab my skateboard and have options.

Con:

1. Increased chance of injury. I'm terrified of this one. I've already hit the ground hard a couple of times because of oddball sports that involve a certain degree of speed (I broke my back and paralyzed myself for a while while skydiving and then I later shattered my wrist paragliding), and I'm very wary of doing things that increase my risk of something like that happening again. That being said, I still want to live life so I'm still willing to take on risks if the benefits are significant enough and if I feel like I can be reasonably careful and keep the odds reasonable. 

So finally and without further adieu, here are a few design priorities I have for my electric skateboard and why:

1. Good torque, good range and a boring top speed. I live in a city with a decent amount of hills so I need good torque to get up them, and obviously range is good just because I would like to get through a day without having to worry about finding time to recharge it. But the last thing I want is a high top speed. I'm basically looking for something that is about as boring as a Segway but isn't ridiculous looking or prohibitively expensive. I don't plan on going much faster than a comfortable pace on a bike. If there is no way to achieve decent range and decent torque while limiting top speed then I can just get something fairly powerful and use self control, but ideally I would like to end up with a motor system or a drive train that is somehow tuned for torque and efficiency at the expense of top speed. 

2. Reliable and powerful braking. If it comes down to it, I'm confident that I can jump off and run/roll it out and I might even have a chance at learning to slide stop a long board since I have a lot of snowboarding experience and the injuries don't seem to have affected that too much, but for the sake of comfort I will be using the motor/s to keep me from speeding down hills and generally relying on them to stop me. 

3. Light, portable and legal to take on airplanes. 

So I have a few questions about how to achieve this:

1. Is there a way to tune the motors and drive train for torque and distance at the expense of top speed? What combination of motor(s) and gearing is best for this? Obviously a low gearing will lower top speed and improve hill climbing, but how do these motors handle the increased RPM in terms of power draw?

2. How reliable is braking on DIY boards? Can you even get regenerative braking? I know that some retail models will actually turn off the braking function if the battery is too full to avoid overcharging it, and I imagine that engineering a solution to this might be beyond the scope of a DIY project. 

3. How reliable is the wireless connection on DIY boards? I would definitely want to minimize dropped connections, and I'm worried that cobbling together a bunch of third party parts would not be good for reliability. 

4. Can issues of reliability be mitigated somewhat by having dual motors for redundancy or by using quality components? Obviously I'd like to get a good price, but I'm also willing to spend the money if it has an effect on reliability and safety. 

Thanks!
```

---
## \#2 Posted by: lox897 Posted at: 2016-07-23T09:38:13.518Z Reads: 104

```
[quote="shveddy, post:1, topic:6513"]
How reliable is braking on DIY boards? Can you even get regenerative braking? I know that some retail models will actually turn off the braking function if the battery is too full to avoid overcharging it, and I imagine that engineering a solution to this might be beyond the scope of a DIY project. 
How reliable is the wireless connection on DIY boards? I would definitely want to minimize dropped connections, and I'm worried that cobbling together a bunch of third party parts would not be good for reliability.
[/quote]

The VESC has regenerative braking. Braking is reliable, but you have to have the right VESC settings.

2.4ghz is super reliable. The most reliable remote is the GT2B but other 2.4ghz remotes are still good.

I have to say, you have some guts. Sounds like whenever you hurt yourself, you just got back up and kept taking risks. Good on you mate! Be careful though!
```

---
## \#3 Posted by: JLabs Posted at: 2016-07-23T12:56:24.014Z Reads: 86

```
If you do everything properly eboards are very very reliable. But you need to use quality components for it to last long. I would recommend buying all of your parts from  @torqueboards sells quality components and backs everything he sells, and if I'm not mistaken he has stock of most of his basic products. Just don't cut corners and don't mind spending money, when u don't do these things, things can go wrong. 

As for torque dual motors are the way to go, but make sure they have sensors, it makes the start up torque mug smoother and it didn't throw u off as much. Good luck! And hope everything gets better!
```

---
## \#4 Posted by: Pantologist Posted at: 2016-07-23T13:08:59.292Z Reads: 79

```
Correct me if I'm wrong, but I'm pretty sure you have to pass a  certification to bring your board on a plane. Boosted Boards are UN38.3 certified and even with that some Boosted boarders struggle to fly with em. Might want to consider a certified board unless you want to ship it when you fly.
```

---
## \#5 Posted by: mattdig Posted at: 2016-07-23T13:22:58.480Z Reads: 75

```
You definitely want a max of 190kv for the motor, maybe even as low as 145. 15:36 (the standard) should be a fine gear ratio. It also depends on how much you weigh but that configuration should power anyone up anything (slowly). For a battery you'll want about 300Wh total (Ah x V of the battery) for all day skating. After that you'll want a replaceable battery pack.

But you will never get that on an airplane, it's literally a home made bomb.
```

---
## \#6 Posted by: Pantologist Posted at: 2016-07-23T13:43:56.080Z Reads: 75

```
Is there anyway to get a personal device certified?

Make a Boosted Board clone? :smile:
```

---
## \#7 Posted by: mattdig Posted at: 2016-07-23T14:16:46.490Z Reads: 69

```
Maybe modify a Boosted so it still looks normal.
```

---
## \#8 Posted by: JLabs Posted at: 2016-07-23T15:10:34.044Z Reads: 68

```
I don't think u need to be certified, as long as it is 99Wh or below. @cmatson just flew with his to Australia, and I though I remembered reading that he didn't have any troubles.
```

---
## \#9 Posted by: Pantologist Posted at: 2016-07-23T16:22:06.058Z Reads: 57

```
Eh. I wouldn't trust myself bringing my own eBoard on a flight. Especially a Lipo build :stuck_out_tongue:

I would think for million dollar airplanes, they would require certain certifications. Boosted uses fire retardant coverings on their batteries. Seems like there is an industry standard to be followed.
```

---
## \#10 Posted by: Mrmoonlight Posted at: 2016-07-23T17:11:13.802Z Reads: 55

```
You can get everything you want with a DIY build, but you have to love the DIY aspect of it. Trying different parts, tinkering, building, research,... You have to keep in mind that DIY is not exactly cheap when you have very specific requirements and want a top quality build. If you go the DIY route, you've come to the right place. There's a lot of awesome people on this forum making it a fantastic resource for information.
```

---
