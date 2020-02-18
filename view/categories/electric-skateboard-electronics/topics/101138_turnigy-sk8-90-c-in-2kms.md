# Turnigy sk8 90°C in 2kms

### Replies: 16 Views: 188

## \#1 Posted by: Djawho Posted at: 2019-08-31T03:50:19.220Z Reads: 73

```
Hi , i coming to have the sk8 149kv . I use this with 10s batterry and focbox . Normally we can use this at 3500w . But mine , are hot after only 2km (90°c motor, outside 30°c,and flat road) :face_with_thermometer: . And that with only 60a motor for 1380w max (in ackmaniac app) 
My config app is normal , motor max/min 60/-60 , battery max 60 , min -14 .
 And the brake are very soft to hight speed :scream: . Do you understand what’s problems ??!! I have tested with 2 motors and it’s same for the two . I have motor mount carbon of trampa  ,and i can turn my belt at 80° easily . I don't understand why this temps are so hot . If you have any idea thx …
```

---
## \#2 Posted by: ZackoryCramer Posted at: 2019-08-31T04:32:24.496Z Reads: 68

```
A picture of your setup will be colossally helpful.
```

---
## \#3 Posted by: dareno Posted at: 2019-08-31T04:46:53.330Z Reads: 65

```
Is this a dual set up?  What cells and p count is the battery?  Questions Questions Questions
```

---
## \#4 Posted by: Djawho Posted at: 2019-08-31T10:05:31.719Z Reads: 56

```
Hi , for the moment it' only one motor (unity in september only) . My battery is an 10s4P of Samsung 25R autenthic (discharge max 80A , charge max 20A). With bms bestech 223v1 buy in aps webshop . Motor pulley 14T , wheel pulley 44T . Focbox on last ackmaniac , with box alloy 3D Servisas . And these connecting wires are to 29cm . :flushed:
![20190831_113645|281x500,50%](upload://mh2VptYrzD9KfcY3fbJgsP5IkWb.jpeg) 
![20190831_113709|281x500,50%](upload://liuf0lmjsIy0vvirdIcofbRNmKs.jpeg) 
![20190831_113724|281x500,50%](upload://goRK4WZkJZxrlLLzu03WUES6Sz0.jpeg) ![20190831_112931|690x388,50%](upload://mXWIi2soZoyIYbMR9sivXzm5qTG.jpeg) ![20190831_113103|690x388,50%](upload://G9gWIuxwnC3rD4QLaqH4JAP1Sn.jpeg) ![20190831_113830|690x388,50%](upload://xrxm0baawXQItnsyQs9t0tV3HIP.jpeg) ![20190831_113904|690x388,50%](upload://taQ0kyXsdqp4zegbWXtt7SiTW8W.jpeg)
```

---
## \#5 Posted by: Okami Posted at: 2019-08-31T11:49:26.211Z Reads: 49

```
As about.motor u should contact turnigy i think.

Increase regen current gor better brakes
```

---
## \#6 Posted by: Djawho Posted at: 2019-08-31T12:26:33.548Z Reads: 44

```
i have contacted the online service of hobbyking . And the guys speak to changed the parameter " Motor timing: 0°/6°/12°/18°/24°/30°" in esc ??!! That's existe ? What is that ???? Do you know , what's same in the app ? maybe this ? @Ackmaniac , Can you help ?
![sk8|690x391,50%](upload://lZry74HWD6rYi5ZdasRgrfL4pTi.png)
```

---
## \#7 Posted by: Ackmaniac Posted at: 2019-08-31T13:48:32.784Z Reads: 37

```
WHat do you want to achieve, doesn't the motor work after the motor detection?
```

---
## \#8 Posted by: Djawho Posted at: 2019-08-31T13:53:32.438Z Reads: 37

```
hi @Ackmaniac  , no it's a problems of temperature . I have 90°c after only 2 kms . When i have contact the online service Hobbiking they say to change this value for more cooling motor . with this link for exemple . [https://hobbyking.com/en_us/yep-esc-programming-card.html](https://hobbyking.com/en_us/yep-esc-programming-card.html)
```

---
## \#9 Posted by: taz Posted at: 2019-08-31T13:54:20.547Z Reads: 36

```
14/44 for a single motor with this big wheels is ridiculously tall gearing. No wonder it overheats.
```

---
## \#10 Posted by: Djawho Posted at: 2019-08-31T13:55:44.104Z Reads: 36

```
i have use an euskating 6374 170KV , since 2 years before , and trampa put 66T . And never problems with temps .
```

---
## \#11 Posted by: taz Posted at: 2019-08-31T13:58:27.137Z Reads: 36

```
Sk8 heat up faster than Maytech 6374.
That does not change the fact that your gearing is wrong.

I see you edited your post.
So you used 66T before and now you use 44T?
```

---
## \#12 Posted by: Djawho Posted at: 2019-08-31T14:01:23.764Z Reads: 36

```
no , trampa use the 2 models 66T and 44T . I use the 44t . It's an urban carver with motor pulley of trampa...
```

---
## \#13 Posted by: taz Posted at: 2019-08-31T14:05:09.610Z Reads: 36

```
Trampa also sells this board with 90mm, 125mm etc wheels.

14/T44T with 7" or 8" wheels and a single motor is too tall end of story.
```

---
## \#14 Posted by: Andy87 Posted at: 2019-08-31T14:20:38.986Z Reads: 33

```
I can just second what @taz said. The 44th are used for the trampa gummies. For the 6.5“ urban threads the gearing will not work good and could be the reason why your motor overheat. I was running the exact same setup as you, also single drive and my vesc heat up in like 5min up to 80 degree and the motor has been hot to touch. My motor was a maytech, but if my vesc wouldn’t overheat so fast I would get the motor as well up to 90 degree within some more km.
```

---
## \#15 Posted by: Ackmaniac Posted at: 2019-08-31T14:25:16.821Z Reads: 34

```
Sadly Trampa sells the single setup with air Tyres which doesn't work. Go dual and you have fun. The Vesc itself works already at it's most efficient motor timing. So hobbyking only tells you some bullshit to be quiet. Sadly service these days only means that somebody with less knowledge then you answers until you loose interest.
```

---
## \#16 Posted by: Djawho Posted at: 2019-08-31T14:30:46.223Z Reads: 31

```
ok , i understand , thx for your explication and time. I will tested that with less amper , that can be help . I can't to put 2 motors before end september (unity)
```

---
