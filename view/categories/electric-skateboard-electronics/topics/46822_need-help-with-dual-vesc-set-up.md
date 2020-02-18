# Need help with dual vesc set up!

### Replies: 20 Views: 1322

## \#1 Posted by: lambievu0916 Posted at: 2018-02-19T06:24:06.475Z Reads: 154

```
I'm planning to build a dual set up and was wondering if anyone had suggestions or recommendations. 

Parts: 
-Motor 6374 190KV x 2
-2.4ghz Nano Remote Controller
-TORQUE ESC VESC (plan on running can bus) 
-12sp4 Samsung battery (Samsung 30q) (12,000 man, 532.80 watt hours)
(BMS is rated for 30A Continuous Amp Output and 80A Peak Amp Output)
-100mm abs all terrain 


Questions: 
-is can bus better? or run the vest individually?
-Is my battery compatible with my vesc set up?
```

---
## \#2 Posted by: Rayce Posted at: 2018-02-19T06:34:36.163Z Reads: 152

```
Waiting on the pros to chime in as I'm barely receiving all my parts for my first diy board. I went 10s5p dual 6374. 107 superfly wheels. So not sure about abs100mm. But I do know It was recommended I get 218mm trucks (tb) for my dual 6374 to fit rwd. Are you planning to do a diagonal set up?
```

---
## \#3 Posted by: High-roller Posted at: 2018-02-19T06:38:25.931Z Reads: 146

```
https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461
```

---
## \#4 Posted by: lambievu0916 Posted at: 2018-02-19T06:44:24.571Z Reads: 139

```
I'm going to be running the same set up as you! 218mm trucks rwd
```

---
## \#5 Posted by: lambievu0916 Posted at: 2018-02-19T06:45:53.755Z Reads: 137

```
I read this forum however I haven't really conclude which would be better so I'd thought if I gave my specs and see what people would know if they had problems with similar specs.
```

---
## \#6 Posted by: Rayce Posted at: 2018-02-19T07:15:46.198Z Reads: 129

```
Sweet I'll be following your tread since were going for the same thing..) curious have you made up your mind on a board, enclosure, mounts? I went with the v4s and under the board mount (regular) not the biggest fan. Of reverse mounts. Speaking from absolutely no experience haha. As my parts come in a fuel my itch with a lift board. GL can't wait to see pics
```

---
## \#7 Posted by: High-roller Posted at: 2018-02-19T07:21:25.107Z Reads: 122

```
I get it. That was simply the thread I found most helpful on the subject when I built mine. 
Personally I went with a split-y cable rather than canbus. I got the impression that it's more reliable, and I didn't feel that the advantages of canbus (traction control, etc) made it worthwhile, especially since I have 6374 motors.
```

---
## \#8 Posted by: E1Allen Posted at: 2018-02-19T07:26:20.638Z Reads: 111

```
Battery is fine.  You need to limit each vesc output to 40a at most for 80a total
```

---
## \#9 Posted by: lambievu0916 Posted at: 2018-02-19T08:34:34.579Z Reads: 103

```
ok! so when I do all the calculations I have to consider both so I can't do 50 amp output?
```

---
## \#10 Posted by: lambievu0916 Posted at: 2018-02-19T08:35:21.892Z Reads: 104

```
ok I see what you mean! but can you elaborate on how you did the split y cable? and how you controlled both motors with just one remote? I haven't got the clear message on how to do it from the forum.
```

---
## \#11 Posted by: lambievu0916 Posted at: 2018-02-19T08:36:15.825Z Reads: 101

```
I'll definitely keep you up dated with pics as well! and enclosure I'm not to sure yet waiting on parts to start brain storming!
```

---
## \#12 Posted by: High-roller Posted at: 2018-02-19T08:58:02.885Z Reads: 101

```
You can buy a Y-cable at any decent RC hobby store, and your vescs should have matching cables to each of the y-parts of the splitter. The other end goes in your reciever, usually channel 1 I think.
IMPORTANT- your reciever gets its power from the vesc (5v) and it only needs to draw that from one of them! On one of the ends that connects to a vesc you need to cut the red (power) wire so you don't fry your reciever.
![IMG_20171129_123817|666x500](upload://ylX3k1qPuuLAH0iOTYoM0oGyRbu.jpg)
Notice how the cable leading to the right hand vesc has had the red wire cut and heat-shrinked. That's how it should look.
```

---
## \#13 Posted by: TarzanHBK Posted at: 2018-02-19T10:33:11.597Z Reads: 92

```
(fixed the title for you)
```

---
## \#14 Posted by: lambievu0916 Posted at: 2018-02-20T23:21:52.303Z Reads: 84

```
thank you for the detail and the visual! this really helps! I'm leaning towards a master and slave rn. However I will try the y cable as well to see which I prefer!
```

---
## \#15 Posted by: lambievu0916 Posted at: 2018-03-06T09:15:30.021Z Reads: 78

```
So i got my parts and everything. Built it but there was a clearence problem when i had my mottors under the board. I decided to reverse it but it looks a bit too low. What do you guys think. ![image|666x500](upload://SKSszzey8OGnSrXPoW2JFZFCp8.jpg)
```

---
## \#16 Posted by: lambievu0916 Posted at: 2018-03-06T09:16:21.431Z Reads: 78

```
![image|666x500](upload://iu7L2PZSjuiurV81qTOD0Cpw3qh.jpg)
```

---
## \#17 Posted by: Bjork3n Posted at: 2018-03-08T17:05:56.702Z Reads: 75

```
What clearance issues?
The reverse mounting look super low, wouldnt do it myself.
```

---
## \#18 Posted by: lambievu0916 Posted at: 2018-03-11T17:44:57.520Z Reads: 66

```
Yeah i decided to get risers and made it higher to give me some clearance
```

---
## \#19 Posted by: Jake25 Posted at: 2019-05-03T13:18:10.728Z Reads: 22

```
Hey, 

You've done a great job but one question is it possible to add another vesc to this that can be controlled separately with different controller.

Thanks
```

---
## \#20 Posted by: High-roller Posted at: 2019-05-03T14:21:10.799Z Reads: 12

```
You mean a third one?

You can control each vesc with it's own controller simply by running a receiver to each one independently, instead of connecting them with a y-cable.
I'm not sure why you'd want to do this unless you want serious redundancy (backup controller).
Just make sure you pair the controllers and receivers correctly so you don't send signals to the wrong vesc.
```

---
