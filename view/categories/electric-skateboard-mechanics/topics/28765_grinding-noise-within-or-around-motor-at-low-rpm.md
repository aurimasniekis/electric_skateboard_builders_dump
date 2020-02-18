# Grinding noise within (or around?) motor at low RPM

### Replies: 16 Views: 2632

## \#1 Posted by: wald.adrien Posted at: 2017-07-27T14:55:52.875Z Reads: 135

```
Hello, this is my first post. I hope it's in the right place and in the correct format.

I'm currently in the process of building my first electric longboard, although most of the technicalities were taken care of by a friend of mine who built his own board over a year ago. I am mainly using parts from the EU GB run by @ajaynagra. The motor I have is from this GB and its origin is unknown(?). Specs are 190kv 6374 sensored. I've configured the VESC via the BLDC tool and all seems to be in order. The problem I have is not an issue of function, but rather the motor is making a weird metallic grinding noise, especially at low RPM. Once it spins sufficiently fast, the grinding stops and it sounds like any other BLDC outrunner motor I've heard.

I've attached some images of the motor as well as a video with audio.

<img src="/uploads/db1493/original/3X/8/2/829dbcf4f3f21a0d51fad7952b01ff94fff21e8e.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/4/7/47309848b6fa3ec29989e90c81f19f0491c529f9.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/7/a/7aaac96ed44ffa9e25adeb2a49bbad3bb0dcd72a.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/c/2/c2cd9991751a953330975f6e0511907c7741509c.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/f/6f955a1cd3a21414cf61e133328c9cb3100884ca.JPG" width="666" height="500">

https://www.youtube.com/watch?v=RKH0TY8kqkQ

Any help would be greatly appreciated!
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-27T15:07:51.697Z Reads: 126

```
Is the circlip on the motor shaft hitting the motor mount then grinding against the shaft?
```

---
## \#3 Posted by: Brycehoosiers Posted at: 2017-07-27T15:29:05.836Z Reads: 117

```
It seems to be the circlip on the motor shaft grinding against the motor mount when it spins. A way to fix this could be by adding some washers behind the motor mount to the the circlip enough room the spin
```

---
## \#4 Posted by: wald.adrien Posted at: 2017-07-27T16:38:42.884Z Reads: 110

```
By this you mean adding washers behind the mount under the three bolts?

<img src="/uploads/db1493/original/3X/3/0/302b526090a5b6615c5bd9e02375dd67c4fe40af.JPG" width="375" height="500">
```

---
## \#5 Posted by: Okami Posted at: 2017-07-27T16:53:46.406Z Reads: 103

```
yes that would be correct place.
```

---
## \#6 Posted by: wald.adrien Posted at: 2017-07-27T17:19:34.606Z Reads: 101

```
So I added washers to between the motor and motor mount and I think its less problematic now but during startup there is still some grinding. Any ideas?

https://youtu.be/nIZeb1iMcoM
```

---
## \#7 Posted by: Martinsp Posted at: 2017-07-27T17:30:04.960Z Reads: 97

```
I feel like it is just something vibrating or more like resonating at some RPM. check that everything is tight and you might find your problem. Try spinning the motor with hand, if you can feel some resistance you found your problem. Next step would be to remove the thing that is grinding out of the motor.
```

---
## \#8 Posted by: wald.adrien Posted at: 2017-07-27T18:14:30.853Z Reads: 95

```
So I've now added two washers and the problem is still persistent. Therefore, I'm inclined to say that it doesn't have anything to do with the circlip. Indeed when I first got the motor I noticed some friction-generated noise within the motor. However, I don't have the necessary knowledge to open up one of these motors. Could someone link a post that explains how to do this? I don't want to break my motor... :sweat_smile:
```

---
## \#9 Posted by: Martinsp Posted at: 2017-07-27T18:15:25.511Z Reads: 95

```
I dont know if there is a post about this but i know of some video I am going to try to find it. :)
```

---
## \#10 Posted by: Martinsp Posted at: 2017-07-27T18:28:07.901Z Reads: 95

```
I cant find the video but here is an article with pictures. https://www.flitetest.com/articles/brushless-motor-disassembly I know you dont have the same motor but it is pretty much the same. What you need to do is simply take that circlip out (ideally without bending loosing or destroying it.. but they are dirt cheap if you are not lucky) and grab the part that is spinning (rotor) and the other part that is not spinning (stator) and pull them apart. Because of the magnets it will not be very easy but easy enough. at that point you can just take a rag and clean everything so that there is no dirt and stuff in there. Dont scratch the windings! **Be careful when putting it back together because the magnets will pull themselves towards the stator and you dont want your fingers in there!!!** dont forget to put the clip back on. that is it :)
```

---
## \#11 Posted by: wald.adrien Posted at: 2017-07-29T00:22:13.442Z Reads: 89

```
So I opened up the motor... Was able to remove the circlip semi drunk, but not sober lol. Everything looks fine, except for one magnet which has a small chip in the middle (see attached picture). I rubbed my nail over it and its definitely chipped. Could this be the cause of the "grinding" noise? Might explain why it goes away at high speeds since the magnet spends less time in contact with each coil (??? pure speculation, I'm a complete beginner in electronics). If this is the source of the problem, is it actually going to pose any issues in the future, or is it worth fixing?

<img src="/uploads/db1493/original/3X/5/8/588367aefedaec6e5d7dda717f8b7bc57b18d680.JPG" width="375" height="500">
```

---
## \#12 Posted by: Martinsp Posted at: 2017-07-31T23:16:35.206Z Reads: 78

```
Hello, sorry for the slow reply, 

If you are talking about the small white dot in the center of the picture then it is really minimal, it wont affect the motor in any way as far as performance goes. It might vibrate a tiny bit more but it would be unnoticeable. just clean the motor and check the windings for something that seems out of order. scratched bent or something like that. Wipe everything to get rid of objects that are not supposed to be in there and you should have your motor fixed. If not post some more pictures and what it does now.
```

---
## \#13 Posted by: pat_arch Posted at: 2017-08-07T17:39:19.991Z Reads: 73

```
Were your able to fix this? I think I have a very similar issue. Thanks!
```

---
## \#14 Posted by: Jinra Posted at: 2017-08-07T17:43:06.752Z Reads: 73

```
Is your circlip on them motor shaft hitting your mount when the motor turns?
```

---
## \#15 Posted by: wald.adrien Posted at: 2017-08-08T16:58:56.785Z Reads: 68

```
So I'm currently on Holiday but I think I found the problem. Specifically, the inside of the shaft through which the rotating bit goes was not an even surface by any standard. I was able to remove some of the protruding parts for a more even surface which reduced the noise significantly, but not completely. I believe by completely smoothing it out I will be able to remove all unwanted noise.
```

---
## \#16 Posted by: ItsJinvy Posted at: 2018-09-10T22:39:11.145Z Reads: 29

```
How did you fix the noise? What was it?
```

---
