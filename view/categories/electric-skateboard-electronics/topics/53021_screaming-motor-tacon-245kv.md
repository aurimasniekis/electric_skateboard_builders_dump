# Screaming motor tacon 245KV

### Replies: 19 Views: 582

## \#1 Posted by: drassak Posted at: 2018-04-21T10:42:23.130Z Reads: 113

```
Hello all, 

I've been using this motor for a while and it makes this weird noise at 70% rpm. It does it regardless it is used in bldc or FOC. It can be heard at the end of the video: 
https://youtu.be/Vkd9B_jgkRg

Is there a way to remove this noise ?

Thanks
```

---
## \#2 Posted by: RedEagle Posted at: 2018-04-21T11:23:02.838Z Reads: 102

```
I don't think so. That noise happens when the motor hits its "sweet spot". Yours is quite loud. You might wanna check alignment of belt & mount.
```

---
## \#3 Posted by: drassak Posted at: 2018-04-21T11:35:20.961Z Reads: 96

```
Alright must be per design. The sound is purely magnetic, the best and drivers are aligned
```

---
## \#4 Posted by: GrecoMan Posted at: 2018-04-21T11:45:17.584Z Reads: 93

```
my Tacon did the exact same thing. couldn’t remove it so swapped to dual 6384s 🤷‍♀️
```

---
## \#5 Posted by: Eboosted Posted at: 2018-04-22T03:18:28.473Z Reads: 75

```
That means the windings do not have enough glue on them, and one of the wires acts as a guitar wire and sounds louder at certain frecuency.
```

---
## \#6 Posted by: pat.speed Posted at: 2018-04-22T03:23:45.892Z Reads: 71

```
Epoxy bath?
```

---
## \#7 Posted by: Eboosted Posted at: 2018-04-22T03:27:50.459Z Reads: 70

```
You could disassemble the motor and use epoxy on the windings
```

---
## \#8 Posted by: PatRocks Posted at: 2018-04-22T04:45:08.183Z Reads: 61

```
Sweet!!! I have the same problem,  but have been too lazy to search/post about it, lol.
Thanks @Eboosted , I was about to just replace it. Where'd you get that solution?
```

---
## \#9 Posted by: Eboosted Posted at: 2018-04-22T04:51:10.368Z Reads: 59

```
I had some motors with low epoxy quantity that started to unwind and the sound was louder everytime
```

---
## \#10 Posted by: Cobber Posted at: 2018-04-22T04:58:25.750Z Reads: 60

```
@Deckoz couldn't you also try changing the operating frequency of the motor in bldc tool?

trial and error, change, test... maybe up from 20khz to 30khz?
```

---
## \#11 Posted by: drassak Posted at: 2018-04-22T12:00:47.537Z Reads: 46

```
I have not seen that option in the motor tab nor in the bldc tab
```

---
## \#12 Posted by: Cobber Posted at: 2018-04-22T13:02:23.468Z Reads: 43

```
http://www.electric-skateboard.builders/t/changing-foc-switching-frequency/30928

point being not what you change it to, but that you change it to not get the harmonic resonance from the motor.

it is possible you will change the sound to a different pitch at a different throttle input, but also that it would no longer happen.

Where is @Deckoz?
DeckyBro you're better with this stuff than me, I have a grasp :sunglasses: where as I think you have a understanding :nerd_face:

Plus stuff is different on my RC controllers.
```

---
## \#13 Posted by: Deckoz Posted at: 2018-04-22T13:08:20.397Z Reads: 41

```
So... The only time I experience this was on @pshaws trampa with one of bkb original motors.

What I found after swapping bells and stators around. The noise followed the bell. The magnets looked to be glued, but one of the magnets had an air gap behind the magnet in the glue, that had not properly been seated. Basically the vibration was the magnet corner flexing, and resonating in the air gap behind the magnet against the bell housing

Otherwise sorry I have never heard this sound on any other motor. It was a rare "unicorn" @Cobber sorry I didn't see this before... So many notifications
```

---
## \#14 Posted by: Cobber Posted at: 2018-04-22T13:10:45.783Z Reads: 37

```
do you think changing the switching frequency of the motor would cause the harmonic resonance to happen at a different throttle input?
```

---
## \#15 Posted by: Deckoz Posted at: 2018-04-22T13:12:25.244Z Reads: 36

```
It could but only slightly, as the resonance is in the mass of the magnet. It may be a different rpm. But the mass and characteristics of the magnet will cause it to vibrate at what it wants to vibrate at... Like any material.
```

---
## \#16 Posted by: Cobber Posted at: 2018-04-22T13:15:40.629Z Reads: 37

```
what if the noise is coming from the copper (stator)?
```

---
## \#17 Posted by: Deckoz Posted at: 2018-04-22T13:21:13.985Z Reads: 37

```
How would you know it's coming from the copper, as the sound will resonating through the motor. Normally if one object of mass connected to another object of mass enters a resonance, it will translate all through any non isolated/dampened mass. 

The only way to tell if it's the copper is to swap bells and see if it follows the copper or the bell.

If it follows the copper then it's likely the stator,  not properly glued or welded, and the laminates are vibrating from eddy currents. The noise shouldn't be coming from the copper.
```

---
## \#18 Posted by: Cobber Posted at: 2018-04-22T13:26:52.518Z Reads: 37

```
ok so why does a BLDC motor hum or whine?
& why does that whine change with switching frequency?
```

---
## \#19 Posted by: Deckoz Posted at: 2018-04-22T14:11:53.201Z Reads: 35

```
Are you talking about a whine like the one in the video in the OP? Or are you talking about the normal vreee vreee vreee hum of a motor spooling? If your talking about the normal humming vree vree vree, yea you can hear a tonal change from the switching frequency. But the sound in the video of the OP. The only time I've ever heard anything like that was the bell magnet not glued.

From alot of what I see, most humming is from belt resistance, slack off belt, pulley type(steel vs alu). And the normal vreee vreee vree sound of the motor and the drivetrain together can make an interesting vibration. Changing switching frequency of course changes the mesh of the harmonics. Ie if the drivetrain oscillating at x frequency, and motor powered at 16khz, the two frequency collide and make a different harmonic tone then drivetrain and motor at 30khz. So for example my evo has a belt resonance at 12mph, that used to be at 18mph with a different switching frequency.

Starting at 14s
https://youtu.be/eSGENI_unS4

You can also hear it here at 9-10seconds, sounds kind of like an "errrklunk"
https://youtu.be/lLq1TqGgnI0

But that sound in the OP specifically I haven't heard any other time except with a magnet.
```

---
