# TB Motor can loose from shaft

### Replies: 26 Views: 588

## \#1 Posted by: rusins Posted at: 2018-09-14T13:29:07.616Z Reads: 189

```
[https://www.youtube.com/watch?v=RU_QWrjOC7Y](https://www.youtube.com/watch?v=RU_QWrjOC7Y)
Video explains it best – the shaft has some wiggle room relative to the can of the motor. Didn't notice this when I first got them (been riding for just 2 days). The noise also troubles me a bit, as the 2nd motor I have doesn't do that. I'm guessing that the noise might be from a burnt component or something (They're sensored 6355 TB motors, and I accidentally burned the sensor on one because I connected the sensor wire to the wrong place on my vesc :man_facepalming:).

People on the forums with similar problems were told to tighten the grub screws of the motor, but I'm not sure if the grub screws are inside the can, or if they're supposed to be here: ![IMG_20180913_231819_2|666x500](upload://jcnynHvZlD9rQkM7doUSbSOvbSu.jpg) If so, then they're missing from both of my motors, but my 2nd motor is perfectly fine, so idk. :man_shrugging: 

If these so called grub screws are inside, then what's the best way to open up my motor? It took me half an hour just to get the pulleys on the shaft, because of how tight they sit, so I'm afraid taking the motor apart might be even harder :grimacing: What should I do? (I'd order a new motor if I were in the US, but shipping to europe + UK taxes ain't worth it)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-14T13:54:12.727Z Reads: 170

```
First...damn there should be screws fixing your shaft!!!
They usually inside, so take a second look.
Allen key should fit for it.

Secondly, it’s not hard to take away the motor can. Just open the snap ring on the side where the shaft is. After you can already pull away the can. Might be you need a bit strength as the magnets hold the can. But it shouldn’t be a big problem
```

---
## \#3 Posted by: rusins Posted at: 2018-09-14T13:59:22.218Z Reads: 165

```
Question is: would inserting these missing screws be enough, or do I also need to open the motor up? I'm not sure if the motors came with those screws missing, or if they fell out while I was riding...
```

---
## \#4 Posted by: Andy87 Posted at: 2018-09-14T14:05:20.926Z Reads: 160

```
I don’t know the English word for it 😅 but this screws should be fixing you shaft
![image|690x342](upload://vgKpHHi2RrKgTYIPCC3HFxTWXMw.jpeg)

Please double check it.
If they really missing than first step would be to replace them. Glue them inside with loctite too.

If you hear strange noises out of the motor better to open. It’s really not difficult. It always can be that magnets came lose or other shit is inside
```

---
## \#5 Posted by: rusins Posted at: 2018-09-14T14:07:57.379Z Reads: 152

```
Ok, thanks! Will open it up later and see what's inside! Also: are you sure the screw you sent in the picture should be there? It's a very small screw-hole, I doubt you can get a screw of this type so small :D I think a regular screw will do, as long as the head isn't too big.
```

---
## \#6 Posted by: Andy87 Posted at: 2018-09-14T14:09:41.300Z Reads: 150

```
No it’s just big picture 😅
It’s the same screw which often used to fix the motor pulley. If the crew on the pulley is inside of the teeth you need one there.

On the motor shouldn’t be a screw with head. Have never seen as min
```

---
## \#7 Posted by: Andy87 Posted at: 2018-09-14T14:12:32.391Z Reads: 145

```
![image|579x500](upload://vknA8lBbas7tFDQ0pCumyadswEI.jpeg)
Small picture but you should get the idea
```

---
## \#8 Posted by: Mikenopolis Posted at: 2018-09-14T14:24:21.449Z Reads: 139

```
I had this happen to the “Dark Matter” motors. Pretty sure Maytech makes the motors. Anyway the problem I saw when fixing it was that the shaft has a flat spot that the grub/set screw meets up with so the turning is locked in. Problem with that was the shaft was still able to move left and right becuase of the flat surface. When I opened up my motor, I saw lines of scratches from the set screw moving along the shaft,

My fix was dremeling a small dimple on the shaft where the set screw meets with it. Then I swapped in the POINTED screw pictured above instead of the flat one It came with.
```

---
## \#9 Posted by: amazingdave Posted at: 2018-09-14T14:56:52.829Z Reads: 124

```
My latest dark matter did the same.... the shaft had a dimple on one side and a flat on the other, but one of the grub screws was loose. I just loctited them back in. Done about 100k since then, all good.
```

---
## \#10 Posted by: monsterbuilder Posted at: 2018-09-14T15:34:04.110Z Reads: 122

```
Sadly, it seems like this is a common problem with TB motors.  I have had two of them now and both did the same thing as yours.  Here is the solution that is currently working for me:

1) Remove set screws completely.  Pour in a few drops of green Loctite 680 into the open holes.  Then spin the can around the shaft a few times and let it dry.  A few hours is probably enough time.  I'd like it dry overnight.  This will allow the can to be glued to the shaft.

2) Then put in new set screws with red Loctite.  I upgraded my M4 set screws to ones with a larger hex pattern, so that I could torque it down harder.  Let the red Loctite cure for another 24 hours.

Then you should be good to go.  Here are some pictures:

![20180914_082726|374x500](upload://o3i4Ib29q8pl8iGlhrtib1EmtDs.jpg)![20180914_082759|374x500](upload://daPpMqbYC9qdRjdXE6XJnH5suBu.jpg)
```

---
## \#11 Posted by: rusins Posted at: 2018-09-14T22:18:17.393Z Reads: 100

```
Update: turns out there actually were grub/set screws still in place :smiley: I just had to use a flashlight to spot them. Tightening them did the trick; but will still be taking it apart to investigate the noise.
```

---
## \#12 Posted by: Mikenopolis Posted at: 2018-09-14T23:58:11.959Z Reads: 98

```
[quote="rusins, post:11, topic:68009"]
Tightening them did the trick
[/quote]

vibration is what loosens them over time, so the issue will return eventually. check them constantly
```

---
## \#13 Posted by: rusins Posted at: 2018-09-15T01:44:21.477Z Reads: 97

```
Of course! Bought myself 2 types of threadlocker: one that permits unscrewing the part later, and one that cannot be undone :smiley:  Bought the latter just in case, but am now testing the non-permanent one, and nothing has unscrewed yet. :)
```

---
## \#14 Posted by: rusins Posted at: 2018-09-16T22:23:51.793Z Reads: 92

```
Update:  took the motor can off (not sure why removing the circlip was necessary, as the shaft wen out one way, and the can the other way) and figured out what was making the slight scratching noise ( I think) – the sensor wires' protective tube/sleeve wasn't cut short enough, so its end must have been touching the can in some places, but not others (not sure why, as the can is symetric :man_shrugging: ).  After doing that, the sound is gone, and the motor is good as new! (Well, except for, you know, the dead hall sensor :laughing:)
```

---
## \#15 Posted by: rusins Posted at: 2019-02-16T22:05:24.874Z Reads: 79

```
Went out for a ride yesterday with my half-assembled board, and the motor can got loose from the shaft again. This time, however, it isn't the grub/set screws getting loose that's at fault – the can is swiveling perpendicularly to the screws! :open_mouth: I shot a video to explain the problem better:
https://youtu.be/UBYpz2FNmEw

The can ends up scratching against the non-spinning part of the motor, so creates a lot of resistance, and of course, noise when riding. Because I'm using standard caliber II trucks with 12mm belts, I'd need a motor of the same (or smaller) width, which I think leaves me with TB as my only option, but since this seems to be a common issue with their motors (and pebbles fly into them sometimes because they aren't sealed), I don't want to do that :grimacing:

(Edit: TB isn't my only option; Flipsky sell motors the exact same size. As of writing, they still have issues with loose magnets though, so no thanks :stuck_out_tongue: )

How hard would it be to drill through the motor can and the axle perpendicularly to the existing holes to just put a shaft through it? Any other ideas?
```

---
## \#16 Posted by: b264 Posted at: 2019-02-16T22:07:21.876Z Reads: 73

```
[quote="Andy87, post:2, topic:68009"]
it’s not hard to take away the motor can. Just open the snap ring
[/quote]

Opening snap rings is the definition of "hard" if you don't have a circlip tool.
```

---
## \#17 Posted by: chrischo1996 Posted at: 2019-02-16T22:42:11.492Z Reads: 69

```
Can confirm, took 30 minutes of trying different things to get mine off.
```

---
## \#18 Posted by: J0ker3366 Posted at: 2019-02-16T22:44:31.539Z Reads: 70

```
[quote="b264, post:16, topic:68009"]
definition of “hard”
[/quote]

Pick tools work the best lol
```

---
## \#19 Posted by: Skunk Posted at: 2019-02-16T23:00:36.002Z Reads: 71

```
And use ccorrectly so they don't brake :wink:
```

---
## \#20 Posted by: maxchilton Posted at: 2019-02-17T04:55:31.005Z Reads: 61

```
There are literally like 3 pieces to brushless motor.  Take motor off the mount and see what is missing/loose.  My bet is the circlip is gone.
```

---
## \#21 Posted by: rusins Posted at: 2019-02-17T14:51:44.421Z Reads: 49

```
Circlip isn't gone, and even if it were, that wouldn't impact the can moving relative to the shaft/axle anyway.
```

---
## \#22 Posted by: rusins Posted at: 2019-02-17T15:54:31.718Z Reads: 48

```
Taking the motor off the mount helped anyway – turns out the axle had rotated, so the swiveling was probably because of the axle not being round at that angle. I guess I must have tightened the grub screws with the axle in the wrong place somehow, or it moved when riding. Either way, I'll replace the grub screws again and hope that the issue is gone :crossed_fingers:

Edit: Nevermind, after taking the motor apart, I now see that the flat spots on the axle don't match up on one end and the other. Looks like I had secured the grub screws properly in place after all. :frowning:
```

---
## \#23 Posted by: Lunasi Posted at: 2019-02-17T17:25:50.762Z Reads: 43

```
Never had this issue myself with TB motors, but to your comment that buying a new motor would just be replacing the same thing, there has been some slight design changes in the TB motors, even in the last year. My older TB motors have had more issues than the current ones I've bought, I think he's cleaned them up a bit from older versions.
```

---
## \#24 Posted by: DerelictRobot Posted at: 2019-02-17T17:59:49.931Z Reads: 42

```
[quote="J0ker3366, post:18, topic:68009"]
Pick tools work the best lol
[/quote]

Naw. Wrong tool for the job.

[quote="b264, post:16, topic:68009"]
 a circlip tool.
[/quote]

Yes.
```

---
## \#25 Posted by: rusins Posted at: 2019-02-17T19:13:30.303Z Reads: 39

```
Have heard others say the same, thanks for your input. Destroyed the thread for one of the grub screws just now while drilling out a threaded screw, and have spent far too much time on this already for a motor that isn't THAT expensive to replace... Will order a new one, if anyone wants this one for parts / to fix on their own, then feel free to PM me.
```

---
## \#26 Posted by: rusins Posted at: 2019-03-16T14:36:50.504Z Reads: 23

```
Received the new motor. Tried to avoid the Parcelforce Clearance fee by doing what [this guy did](https://psych0naut.livejournal.com/36270.html), but the guy at the depot was having none of it. It's ridiculous that they can charge a hidden fee for no reason, and it still seems illegal to me. God I hate the UK.

Before purchasing I asked TB support if they had updated the 6355 motor's design (since I had seen a picture somewhere on theses forums), but they replied no. I bought it anyway, and to my surprise, it is the updated model!  On the left is the new version, on the right is the old.
![photo_2019-03-16_15-26-06|666x500](upload://uKDdvrM4iikecchYTs7Ff61NVgd.jpeg) 
![photo_2019-03-16_15-26-11|666x500](upload://a3C0PCUM1FBpxYLf4y4vgk30Mzv.jpeg) 

Less holes for pebbles to fly into, yes!

Still only has 2 grub screws unfortunately. My only question now is whether or not I should unscrew them and apply loctite, or if that's no longer needed with these motors. (IIRC they should have green loctite applied already. Don't see it spilling out anywhere though :smile: Can't unscrew them super easily, so :crossed_fingers: )
```

---
