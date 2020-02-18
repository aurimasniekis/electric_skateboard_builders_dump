# Help strange noise, new motor and vesc 6

### Replies: 21 Views: 1007

## \#1 Posted by: Hardwiring Posted at: 2017-09-19T21:20:19.648Z Reads: 124

```
Twin vesc 6 118kv motors and 1 motor/vesc makes this noise like an aerosol spay as I start to apply throttle. Is it Ok? Thanks in advance my board is brand new and I don't want to hurt her 🙄 
https://drive.google.com/file/d/0B2sHUexB6I0eOFJOdG1Mdkk0ZVk/view?usp=drivesdk
```

---
## \#2 Posted by: Rinzler Posted at: 2017-09-19T22:05:48.032Z Reads: 115

```
Check if the motor circlip is rubbing on the motor mount.
```

---
## \#3 Posted by: Hardwiring Posted at: 2017-09-19T22:33:09.041Z Reads: 118

```
Thanks but nope, this is before motor starts to turn, I also checked running uncensored and results are still the same
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-19T22:35:09.417Z Reads: 107

```
Sounds like something rubbing inside
```

---
## \#5 Posted by: Rinzler Posted at: 2017-09-19T22:36:07.050Z Reads: 100

```
Do you run foc, sometimes the motor coils can "sing" when current is going through the motor, just a thought on what it might be.
```

---
## \#6 Posted by: Hardwiring Posted at: 2017-09-19T22:40:38.874Z Reads: 93

```
Thanks...I will unfoc the vesc tomorrow.... if I do another motor detection tonight she will cut me
```

---
## \#7 Posted by: Rinzler Posted at: 2017-09-19T22:46:33.638Z Reads: 90

```
You dont have to, that is likely not a culprit. I would open the motor because there is a rubbing noise, maybe you have a faulty bearing. If i were you if i didnt feel any resistance while turning it i would take it for a spin, buy you have a vesc 6 which is top dollar so i probably wouldnt :stuck_out_tongue:
```

---
## \#8 Posted by: Hardwiring Posted at: 2017-09-19T23:07:55.955Z Reads: 84

```
its not rubbing, the shaft isn't moving when it makes that noise... i'm probably worrying to much. I though it might be a hall sensor issue ........ **it's such an odd noise**, unless someone suggests otherwise I'll change it from foc tomorrow and see if that gets rid of the problem. Then see, my mate has the same set up and it's just silent????!!!!
```

---
## \#9 Posted by: Rinzler Posted at: 2017-09-19T23:12:34.417Z Reads: 81

```
Maybe there is a hall sensor that is sticking out and being hit by the stator magnets, which would cause sound intervals as the magnet hits it, try listening for that.
```

---
## \#10 Posted by: Clonkex Posted at: 2017-09-19T23:27:57.379Z Reads: 78

```
I think @Rinzler has got it firmly stuck in his mind that the shaft is actually rotating :P

Where does the noise come from? The motor or the VESC?
```

---
## \#11 Posted by: Rinzler Posted at: 2017-09-19T23:36:04.630Z Reads: 75

```
@Clonkex Hahhaahh,  didnt read the whole thing :grin:  The sound comes from the motor, maybe you have a special esc or didnt listen to the recording :stuck_out_tongue_winking_eye:
```

---
## \#12 Posted by: Clonkex Posted at: 2017-09-19T23:39:30.389Z Reads: 71

```
I didn't listen to the recording (at work currently) but I was wondering if it was a "coil whine" type noise like you get on high-powered GPUs sometimes.
```

---
## \#13 Posted by: Rinzler Posted at: 2017-09-19T23:42:24.124Z Reads: 68

```
The vesc 6 doesnt have such computing power, maybe the vesc 15 will :wink:. My guess- the coils sing, perfectly normal
```

---
## \#14 Posted by: Clonkex Posted at: 2017-09-20T05:34:38.143Z Reads: 56

```
@Rinzler Haha no, but coil whine can occur in a number of different components. Depending on the situation (usually involving to high power draw) inductors can whine, as can capacitors.

The only reason I'd be doubtful about it being the motor coils singing is that it's only happening on one motor (out of 3, if you count his friend's build).

(Incidentally Tron Legacy is one of my favourite films despite the slightly odd CG Jeff Bridges :grin:)
```

---
## \#15 Posted by: Rinzler Posted at: 2017-09-20T08:44:00.694Z Reads: 47

```
@Clonkex These are hand wound motors, so no motor is the same, windings are not sealed. (Well at least we agree on something) This is turning into a pointless discussion with no solution in sight.
@Hardwiring Change the title of the thread, put in vesc 6 in there. My guess more people are going to chime in.
```

---
## \#16 Posted by: Clonkex Posted at: 2017-09-20T09:12:47.471Z Reads: 47

```
@Rinzler Not pointless at all. I suggested coil whine, you said the VESC 6 doesn't have the computing power. I pointed out coil whine isn't (directly) related to computing power and suggested that because it's only on one motor, I was uncertain about motor coils singing. You pointed out the motors are hand wound (I didn't know that so I learned something :P ) and now I'm saying "Oh, ok, makes sense." Also having listened to the recording it does indeed simply sound like the motor. So yeah, it's just a discussion at this point, we're not really trying to solve anything, only having a friendly chat about what the possible causes of the noise might be :)
```

---
## \#17 Posted by: Hardwiring Posted at: 2017-09-20T19:34:04.238Z Reads: 45

```
thanks for taking the time to listen to sound of my motor, this isn't the first, second or even third board I've ever made, i have just never heard the likes from a motor, before I go riding and wreck a few hundred quids worth, I just wanna be sure. 
 So thanks for the input
```

---
## \#18 Posted by: Hardwiring Posted at: 2017-09-22T14:00:54.072Z Reads: 31

```
think i am going to risk it
```

---
## \#19 Posted by: Clonkex Posted at: 2017-09-23T00:47:05.908Z Reads: 27

```
Fingers crossed man!
```

---
## \#20 Posted by: scepterr Posted at: 2017-09-23T01:25:47.820Z Reads: 28

```
I had something making noise in a motor once, rode it and it went away....no idea what it was
```

---
## \#21 Posted by: pat.speed Posted at: 2017-09-23T06:34:56.953Z Reads: 28

```
Maybe just a bit of metal shaving or small object, try blowing into the motor first and try or maybe compressed air if you have some
```

---
