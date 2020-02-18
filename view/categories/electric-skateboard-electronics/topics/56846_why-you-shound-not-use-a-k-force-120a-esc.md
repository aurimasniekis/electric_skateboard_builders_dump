# Why you shound not use a K-Force 120a ESC

### Replies: 3 Views: 376

## \#1 Posted by: slick Posted at: 2018-05-26T16:47:44.520Z Reads: 126

```
Hey guys,

I´ve been lurking around here for about a year or so now and I recently decided to join :grinning:
I bought a Turnigy K-Force 120A out of ignorance and had it lying around for almost a year. I Finally reached
the point where my second build was "road ready" and all was fine and dandy for a week or two. Until my ESC (or so I think) died. I can´t confirm it yet but regardless - I´m here to share my thoughts on the ESC´s performance on the road.

The K-Force combined with an SK3 236KV 5065 was´nt too bad from a performance perspective. I never had cogging or unpleasant whining sounds from the motor. Accelerating from a stand still was possible with a 72kg rider, 6kg board, 3:1 gear ratio with 83mm Trampa Stickies and 8S Lipo. Bombing uphill was a blast. I´ve yet to find a hill that would stop me. Never got too hot either but then again - I never had the chance to push it to it´s max since something died on my setup and I´m not yet sure what.


Here´s the scary part.

**Brakes**
  You can choose between "soft" "hard" and "very hard" - soft was not enough for me so I had it on "hard" and it was scary! Coasting is not really possible with this ESC when drag brakes are on. So if you want to brake - you have to actively decrease you speed - meaning slowly let go of the throttle and wait for the drag brake to kick in and pray to god you don´t plant your face to the ground. This means that you as a rider need to be extra careful since just letting go of the throttle at higher speeds  definately mean trouble.

**Inconsistent throttle respond**  
How do I describe this best? I think "squishy" does it? I experienced some kind of lag sometimes when I was riding. I had to let go of the throttle a bit and squeeze again to get a respond. It´s annoying at least and dangerous at most - I almost fell off a few times when the torque kicked in and I was´nt ready for it.

**Runaway board**
This is one of my biggest fears - a runaway board. I simulated a signal loss to see how my setup would react.
I flipped my board around and turned it on and turned off my remote. What happened next scared me. **The ESC went full throttle!** Luckily I did´nt have to find this out the hard way. If you never experienced this before then flip your board and do a controlled test. This might keep you and others from finding out the hard way.

With all that said, I´d say **stay away from this ESC**. It´s not safe for you and everybody else around you. Even though I never had an accident with this setup and I was actually having fun with it,  I´m not sure yet if the ESC, Motor or SBEC etc. died I´m glad that something died before anything serious happened. This gave me some time to think about my health, my family and everybody else in my surrounding while I´m on my board. 

**Moving on**
So now, I´m waiting for my Turnigy SK8 (V)ESC HW 4.12 to arrive. Should be arriving any day now. I downloaded the VESC TOOL already and had a peak. Hmmmm...I´m sure I´ll be dropping by with a question or two about the VESC and VESC Tool. @squishy654 I read it´s reputation sounds worse than it actually is. So I decided to grab one and I hope that the damn thing lasts. It also sounds like it´s reliable so....

see you around!
thanks for sharing!


ps. I don´t want to post my second build yet but here´s my first build form 2016

blog
https://www.christianmendez.at/2016/08/11/life-on-a-longboard/

youtube
https://www.youtube.com/watch?v=TWTiX8tepN0
```

---
## \#2 Posted by: DavidC Posted at: 2018-05-27T09:28:17.470Z Reads: 60

```
[quote="slick, post:1, topic:56846, full:true"]
I simulated a signal loss to see how my setup would react.
I flipped my board around and turned it on and turned off my remote. What happened next scared me. The ESC went full throttle!
[/quote]

Maybe you didn't set the failsafe of your receiver?
```

---
## \#3 Posted by: slick Posted at: 2018-05-27T18:55:32.387Z Reads: 31

```
You could be right on that. I can't remember what I did when I bonded the mini remote with the receiver. I was surprised to find out that the K-force was actually not the component that failed. It was the SBEC that fried which also killed the mini remote receiver in the process. I'm kind of happy about the fact that I still have  a working ESC. Now I can compare it to the VESC and experience the difference. I'very already ordered a new receiver from Ali Express for the mini remote. I'll follow the binding steps as described by @Ackmaniac in this [Thread](http://www.electric-skateboard.builders/t/fail-safe-on-mini-remote-not-working/31104/10) and see what happens. Luckily I have a GT2E as a backup but since I've been using the mini remote, I feel awkward using that huge remote. Maybe I should try to see what happens with the GT2E when it loses signal...

Thanks for the Tip!
```

---
