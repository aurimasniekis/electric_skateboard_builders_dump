# Focbox confusion - Please help!

### Replies: 41 Views: 1791

## \#1 Posted by: Shaibazsayed66 Posted at: 2018-04-14T13:08:42.058Z Reads: 196

```
Hey Guys ,     

               I took a took a new focbox from enertionboards.com from the i got it im face problem, my motor is not moving at all i searched every were on YouTube and did  all  as per  video said to do yet facing problem,
after some days i brought a new ESC from amazon n wen i started the ESC  it worked flawless 
for battery im using benchtype power supply at 42v and it has a amp lemet of 10Ah
 plz help need to get my project done
```

---
## \#2 Posted by: anorak234 Posted at: 2018-04-14T13:47:08.210Z Reads: 192

```
Trust me, there are plenty of people that can and are willing to help you that are on this forum - however your formatting is a little hard to read, so I’m gonna clean up the thread a bit:

He can’t seem to figure out how to work a Focbox, so he bought a cheap ESC and that’s working but he’d like to get the focbox working. 

@EnertionSupport @scepterr @longhairedboy @JohnnyMeduse
```

---
## \#3 Posted by: Shaibazsayed66 Posted at: 2018-04-14T13:49:58.793Z Reads: 182

```
focbox # vesc-x isn't working my motor is not moving(spinning)  in terminal i'm not getting any faults
```

---
## \#4 Posted by: onepunchboard Posted at: 2018-04-14T13:51:44.246Z Reads: 173

```
screenshot every tab from vesc softwere and upload. thats the start.
```

---
## \#5 Posted by: Shaibazsayed66 Posted at: 2018-04-14T13:53:33.081Z Reads: 167

```
yup just a moment
```

---
## \#6 Posted by: FabianOdermatt Posted at: 2018-04-14T14:22:36.020Z Reads: 154

```
https://www.vesc-project.com/node/178

Go throught these, I think you can't do anything wrong then. :slight_smile:
```

---
## \#7 Posted by: Shaibazsayed66 Posted at: 2018-04-14T14:30:11.776Z Reads: 149

```
![Capture2|690x291](upload://t0bCLW4lAF8qsp4zuBnylezaIv6.jpg)![Capture|690x291](upload://vudd1ceXZp3ZjWGcByGUupdymfY.jpg)![Capture7|690x291](upload://3GafJAzjWQzeLZwJpbmsisaby7f.jpg)![Capture8|690x291](upload://jq0jv0HWq8Oh3prY7gk5aPZ4VK5.jpg)![Capture6|690x291](upload://lxojyan2mpoFpcBspTrnsKemy7V.jpg)![Capture4|690x291](upload://ixW7WbGBTU0sLhJRCz40gJHND7n.jpg)![Capture5|690x291](upload://xEyZqzJyLrECS4Kgx5DH5jYQgqu.jpg)![Capture9|690x291](upload://ks6MDTJKPQWXiZRljhjp4HeTARY.jpg)![Capture10|690x291](upload://yQaWoyzKDgZXBqBKm2gWzla9Iyr.PNG)![Capture3|690x291](upload://v1B7WxtoUnP7YtKF8cqMu6hHQWx.jpg)![Capture11|690x291](upload://obgvqkYMw1LmhjGpYM4WXlJY4GU.jpg)![Capture15|690x291](upload://cwbrflkv7jTjEsPNAceM4c4K43u.jpg)![Capture14|690x291](upload://gNj7mAYJOFxmx5pQOxxDqi88Xk2.jpg)![Capture12|690x291](upload://tUPRAO2SPUcyOdSeEEn7EaBKXE5.jpg)![Capture16|690x291](upload://sQ98iUQJrX6xVcgMtnrkEYNS32b.jpg)![Capture17|690x291](upload://vpQlUlr6l196ir7oovFVJduFvzC.jpg)![Capture13|690x291](upload://tIRnU4XTO82XpdquATatedGVObp.jpg)[Uploading...]() [Uploading...]() [Uploading...]()
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2018-04-14T14:42:45.808Z Reads: 127

```
Those are the Default parameter... DID you run a motor detection.. FOCBOX aren't plug and play device 

![cb4478a0a8c34cdc269bdea731313026dee6eb98|690x291](upload://FBFccMpqOXW3lqXLPqEAHdJCVn.jpg)
```

---
## \#9 Posted by: Shaibazsayed66 Posted at: 2018-04-14T14:44:35.335Z Reads: 125

```
ya i just ran it on default is it a problem
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2018-04-14T14:45:33.326Z Reads: 125

```
Yeah it could burn the DRV of the FOCBOX or blow some mosfet
```

---
## \#11 Posted by: Shaibazsayed66 Posted at: 2018-04-14T14:46:09.762Z Reads: 125

```
OMG thank u for trrelling
```

---
## \#12 Posted by: Shaibazsayed66 Posted at: 2018-04-14T14:46:31.449Z Reads: 129

```
can u plz help how  to make it work
```

---
## \#13 Posted by: RedEagle Posted at: 2018-04-14T14:47:02.952Z Reads: 128

```
Lots of things wrong here.
Motor detection failed. You didn't do a motor detection.
No app setup. You didn't setup the receiver
Max current ramp step doesn't show. CLICK READ SETTINGS FIRST, then screenshot it.
You've got a overcurrent error. Are you using battery or a power supply?

You didn't even setup the focbox. Follow the guide and report back if you have a problem.
Watch the video.

https://www.electric-skateboard.builders/t/vesc-faq-my-vesc-doesnt-work-help-qiqo/672
```

---
## \#14 Posted by: Shaibazsayed66 Posted at: 2018-04-14T14:48:52.101Z Reads: 119

```
yes Mr. RedEagle ill do as u  say
```

---
## \#15 Posted by: Shaibazsayed66 Posted at: 2018-04-14T14:49:14.934Z Reads: 116

```
its a bench type power supply
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2018-04-14T14:50:23.200Z Reads: 117

```
It look like you have a lot of catching up to do, please read this thread first:

https://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980

EDIT: Keep in mind that if it doesn't work, it could be because you've already damage it.
```

---
## \#17 Posted by: RedEagle Posted at: 2018-04-14T14:52:40.564Z Reads: 111

```
[quote="RedEagle, post:13, topic:52239"]
CLICK READ SETTINGS FIRST
[/quote]

You've got to do this everytime in every tab otherwise it just shows inaccurate settings.
```

---
## \#18 Posted by: Shaibazsayed66 Posted at: 2018-04-14T14:54:07.909Z Reads: 108

```
yes Mr. Johnny illread its :blush
```

---
## \#19 Posted by: Shaibazsayed66 Posted at: 2018-04-14T14:55:22.968Z Reads: 109

```
o i get it :blush:
```

---
## \#20 Posted by: Scoo_B_SK8 Posted at: 2018-04-14T14:55:42.337Z Reads: 110

```
did you smell anything funny when powered it up? could open box and send some quality pic of PCB to see if any obvious signs of damage.

otherwise yes, do as instructed by @JohnnyMeduse & @RedEagle  read, read, read.
```

---
## \#21 Posted by: Shaibazsayed66 Posted at: 2018-04-16T07:48:45.067Z Reads: 85

```
@Scoo_B_SK8 no i didnt smell any thing every thing is  perfect vesc is working and i read every thing from the form and  did all the calculation n now its not showing any fault and still motor isn't spinning pleace help
```

---
## \#22 Posted by: CarlCollins Posted at: 2018-04-16T08:09:47.176Z Reads: 79

```
@JohnnyMeduse and @RedEagle indicated.

You have to set it up according to your setup. Otherwise it will not work.
Also, any wrong input might fry your item, So carefully follow each guide.
```

---
## \#23 Posted by: Shaibazsayed66 Posted at: 2018-04-16T08:50:54.220Z Reads: 73

```
can u plz help me in doing it i did it asper it said but even do im facing the same problem can u help me in setting up like how u dow fro other peoples
```

---
## \#24 Posted by: RedEagle Posted at: 2018-04-16T08:54:29.982Z Reads: 75

```
At what point are you having trouble?
```

---
## \#25 Posted by: Shaibazsayed66 Posted at: 2018-04-16T14:16:40.746Z Reads: 66

```
from 1st u tell me how to  do and all.  cause i did it from all sides YouTube, forms ,and etc....
Mr. RedEagle think it your focbox and guid me from smallest to smallest thing like even connecting of that focbox wire cause im  trying it from 3 months invest a lot of money for bring it  from enertion bord even after so much of effort its link  nothing happening please helpme....
```

---
## \#26 Posted by: Shaibazsayed66 Posted at: 2018-04-16T15:29:39.715Z Reads: 62

```
now im not able to get Resistance (R) im getting l but not that  


![40|690x291](upload://b0oNQmqCbUufALp6UlKIuGActn1.png)![29|690x291](upload://5kPeMdh6So9zkh57NgwAQWeOzcR.png)![63|690x291](upload://fMAqnLanJYQ98wpYZXMYd4wRn83.png)
```

---
## \#27 Posted by: JohnnyMeduse Posted at: 2018-04-16T15:42:21.217Z Reads: 56

```
What firmware did you put inside... Because by default that tool will probably suggest you to put the firmware for the hardware 6.0.
```

---
## \#28 Posted by: RedEagle Posted at: 2018-04-16T17:23:23.485Z Reads: 54

```
Wait.. first you were using BLDC Tool and now VESC Tool?
You need to post your settings again. Remember: READ CONFIGURATION FIRST, then screenshot.
It would also help if you could post your battery and motor specs.
```

---
## \#29 Posted by: Shaibazsayed66 Posted at: 2018-04-16T20:13:59.524Z Reads: 51

```
ya i did for 4.12 
ok no problem ill use that bldc tool only the screenshot of setting are the same 

my specification are :- 

battery ,    bench type power supply # 42v    
motor  ,     ebike motor bldc outrunner 45kv sensorsed
ESC ,   focbox 1.3v # vesc-x


This is all what i have 


i read all what u sent to me even after knowing i read everything n did as been said  checked my wire for several times result motor not  moving i even checked with termenal no faults  :disappointed: 


then agen started searching on net n found it better to go with foc he told in video

so took vese  tool as he did in video did all correctly n will the time of measuring (R and L) vesc tool measured L as 0.88 and R = 0 :disappointed:  can u plz help me with this  setting up plz cause i have invest lot of time and  money for this one project :disappointed: 

thank you so much for giving ue precious time for readying request
```

---
## \#30 Posted by: JohnnyMeduse Posted at: 2018-04-16T20:40:15.217Z Reads: 48

```
[quote="Shaibazsayed66, post:29, topic:52239"]
so took vese  tool as he did in video did all correctly n will the time of measuring (R and L) vesc tool measured L as 0.88 and R = 0 :disappointed:  can u plz help me with this  setting up plz cause i have invest lot of time and  money for this one project :disappointed:
[/quote]

That is a known issus with the Vesc Tool and the focbox... you need to use the BLDC TOOL.
```

---
## \#31 Posted by: Shaibazsayed66 Posted at: 2018-04-16T21:09:39.016Z Reads: 45

```
ok can u plz help me in making it work plz
```

---
## \#32 Posted by: RedEagle Posted at: 2018-04-16T21:28:09.850Z Reads: 41

```
Are you using it on a ebike? 45kv is way too low for a esk8.
```

---
## \#33 Posted by: JohnnyMeduse Posted at: 2018-04-16T21:36:19.920Z Reads: 38

```
Have you done a motor detection in FOC or BLDC in the old BLDC TOOLs
```

---
## \#34 Posted by: Shaibazsayed66 Posted at: 2018-04-16T21:48:35.428Z Reads: 40

```
i tryed both foc n bldc but its not working :disappointed: 

sorry sorry  not kv
 kw its 35kw :sweat_smile::sweat_smile:
```

---
## \#35 Posted by: JohnnyMeduse Posted at: 2018-04-16T21:55:43.606Z Reads: 41

```
what the max power of you supply ????
```

---
## \#36 Posted by: Shaibazsayed66 Posted at: 2018-04-16T22:05:40.411Z Reads: 42

```
distributor told me it is better to be at 42v to 50v 
on box they have writen as 48v to 60v 

but this motor work even with 11.1v #3s
```

---
## \#37 Posted by: JohnnyMeduse Posted at: 2018-04-16T22:17:10.372Z Reads: 42

```
Yeah, but does your supply produce enough current to run your motor. Since it is a big motor, you might need around 5-6A Min at 42V.
```

---
## \#38 Posted by: Shaibazsayed66 Posted at: 2018-04-16T22:27:46.495Z Reads: 39

```
yes i do have a bench type power supply it has  a capacity of 10A  and i have run it on a cheap ESC from amazon just to check if im doing anything wrong but ya  it run'es on a cheape 11.1v ESC bet not on focbox which costs at lot and has good brain, a power to do any thing to make a motor work how we want plz can help some how or wait do u have team viewer that is the  best thing u can knw it closly and u can solve it in secounds cause your a professional :grin:
```

---
## \#39 Posted by: JohnnyMeduse Posted at: 2018-04-16T22:46:35.488Z Reads: 42

```
Are you trying to perform a motor detection a 11.1V or at 42V ? 

Yeah, the cheap esc could work with your supply at 3S, but it doesn't mean that a focbox would at 3S.... Especially if you haven't run a proper motor detection, I'm still afraid that you might have kill it at your first attempt at running it. 

here are the step to perform a motor detection in FOC for sensor motor, if your isn't sensor NUMBER 1 SHOULD BE AT SENSORLESS and you can skip step 7-8

![image|690x365](upload://c6bjdD3Agb3ZaNNCXOxqhtd5uFk.png)
```

---
## \#40 Posted by: Shaibazsayed66 Posted at: 2018-04-16T22:57:27.639Z Reads: 39

```
:joy::joy: y will i use it at 3s wen my foc has a 48v limit  i told u the 1st as well im using it at 42v #10s settup n dont worry foc is perfect ill show u pic i had take it last day only due to i was new her so ue site blocked me n told no more comments for new user n told to wait for 22hr so was wating n chill n chill im good in electronics i knw very well so i allways be on a safe side thank you for telling :relaxed:   just have a look it foc is perfect n fine 
![20180416_144554|243x500](upload://wZyRSUZILA6Gc5DRFWvPllYi6pq.jpg)![20180416_144603|243x500](upload://bK1Hz05Omu1jXmwaea4gEqA4DTU.jpg)
```

---
## \#41 Posted by: CarlCollins Posted at: 2018-04-23T17:44:01.721Z Reads: 32

```
@Shaibazsayed66

**Update from Tech Team**
10 amp psu is not enough for proper testing. We don’t think a Focbox would be ideal for a bike hub motor. Those are a whole lot larger than a skateboard motor thus need a lot more current. If he has a drv error, the focbox is toast and needs to be replaced.
So it also looks like he tried to run detections at 11.1 volts which some its so slow, pulled more current than his supply can handle. Which lead to an improper detection and after he test spun it, he likely ruined the drv chip.

**Sending a replacement to you and our tech team will guide you with the setup**
```

---
