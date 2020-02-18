# The Green Missile &#124; First Build &#124; Planning Stage: Figuring out the electronics

### Replies: 24 Views: 1823

## \#1 Posted by: NerdNinja Posted at: 2017-05-18T18:02:15.226Z Reads: 174

```
Alright, Hi guys! I'm new here :stuck_out_tongue:

Been reading for a few days and now I think I'm ready to get everything planned out so I can buy parts and get building!
So far I've figured out the board part, But I'm more than willing to take advice!!

-Deck: The one part I'm set on! Gonna have my artsy GF design some awesome graphic!
https://goo.gl/55UzIM
-Wheels/Tires: I need some larger tires so I can handle the rough blacktop for long distances, Plus AT is sweet! Gonna try Maxid's 3d printed hubs.
https://goo.gl/EwG3oH 
-Trucks: Just some wider skate trucks.
https://www.amazon.com/Paris-195mm-Black-Skateboard-Trucks/dp/B00EKR48T8
-Motor Mount: Thinking DIY
-Battery: DIY 10S4P with Samsung INR18650-30Q 3000mAh - 15A
https://goo.gl/gYjr0w
-BMS: No idea, Need to look into this one
-VESC: This guy seems to be the forum go-to
https://goo.gl/5uiduT
-Motor: I had one recommendation to use this guy, so unless I get some other answers I guess that's what I got.
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html

Annndd that's all I got :confused: I know I still need some more parts. This stuff is hard for me to wrap my head around because it's just so much information all at once!!

All I know is I want to go between 20-30 MPH. I have some hills along the way but it's mostly flat worn blacktop. I weigh ~170Lbs. And price, I'm not made of cash, but I'm not super poor either. I think that's everything. Oh, and I wanna do this as the controller https://www.instructables.com/id/DIY-Nunchuck-Controller-for-Electric-Skateboards/ I don't know if that affects part deciding...

I really hope I'm not breaking any rules with this post :o I plan to update it as the building process goes along so as to only have one build thread. :grimacing:
```

---
## \#2 Posted by: IsTalo Posted at: 2017-05-18T20:40:42.442Z Reads: 138

```
Sorry, but where is your motor? And Esc? And Switch? 

Another thing, do you know the time of the shipping of the Custom Boards? I want a blank deck from them and I wanna know (Will be only 10 days in NYC)?
```

---
## \#3 Posted by: NerdNinja Posted at: 2017-05-18T20:54:39.154Z Reads: 129

```
Still working on those bits. I'm not sure what I'll need to get the proper speed and torke. As for shipping I don't know, first time ordering a deck from anywhere, and my GF still needs to design the graphic, but I'll let you know. It'll probably be the first thing I buy.
```

---
## \#4 Posted by: IsTalo Posted at: 2017-05-18T21:01:48.567Z Reads: 125

```
Nice! Maybe you don't want, but I will give my opinion, Buy a Vesc from Ollin Boards, the Motor you can use a Sk3 190kv or The Polars ones, it would work perfectly with the right pulleys, don't know which because I use normal wheels. 10s4p with a Bms, buy from @barajabali, it is not as cheap as HK, but it is High Quality and have a Bms and Switch. The enclosure you can buy from Enertion, they have a few for 30$. and good luck man, you will have a lot of headache with the esk8, but it is worth the pain.
```

---
## \#5 Posted by: Lukas Posted at: 2017-05-18T21:26:40.105Z Reads: 110

```
I don't think that the trampa wheels with the 12mm bearrings will fit the paris Trucks
```

---
## \#6 Posted by: NerdNinja Posted at: 2017-05-18T22:52:57.190Z Reads: 105

```
Ah thanks for the suggestions! I'm completely new so anything to help is appreciated!! I'll look into the motor! Seems to be the go to around here. Hmm batt will be tough, I know 10s means 10 cell but I don't remember the P... She's he use the 18650 cells? I guess that doesn't matter too much. I'm gonna try to make a split system. I don't want to cover up my graphic if my girl makes it. 

As for enclose I think I have 3d printer access so I'll probably go that route. I'm familiar with CAD so that'll be easy 😏.
Haha and headache is right! But it's thrilling! Brings me back to when I was researching how to build a PC!!

(I don't know how to quote) @Lukas huh. Guess it's a good thing I made the post! I'll have to look that up. Any recommendations if it doesn't fit?
```

---
## \#7 Posted by: IsTalo Posted at: 2017-05-18T22:56:54.044Z Reads: 100

```
Show us yours GF graphics! About the Battery, 10s4p is a good battery, but you can go with 10s3p too, less range, but lighter and less space used!
```

---
## \#8 Posted by: NerdNinja Posted at: 2017-05-18T23:02:41.584Z Reads: 96

```
She's gotta design it yet 😂 hmmm I'll have to see about the battery. I live about 6 miles from town so range is something I want a fair bit of
```

---
## \#9 Posted by: IsTalo Posted at: 2017-05-18T23:30:43.688Z Reads: 91

```
10s4p is 13 or 14 miles of range, but with a Bms you can charge it in 1 and a half hour
```

---
## \#10 Posted by: NerdNinja Posted at: 2017-05-19T03:26:38.951Z Reads: 78

```
Awesome! Sounds perfect! Now I just need to figure out the damn pulleys! I'm good at math but man, that's a beast for my brain :frowning:
```

---
## \#11 Posted by: NerdNinja Posted at: 2017-05-19T19:00:28.570Z Reads: 67

```
I made some changes! Added a few of the electronics!
```

---
## \#12 Posted by: IsTalo Posted at: 2017-05-19T19:26:45.293Z Reads: 66

```
Nice, tell us what you did!
```

---
## \#14 Posted by: NerdNinja Posted at: 2017-05-19T19:38:49.246Z Reads: 71

```
Now I'm looking into pulley's / motor mounts Can't find much here, I do have access to a mill so I could craft my own, but I still need to figure out the gears!

@trampa I'm wondering if you could offer me some help. I was looking at your motor mount kits but I'm not totally sure if my config would even work with what is offered. I was thinking this one.

http://www.trampaboards.com/trampa-urban-carver-motormount-66-with-tooth-pulley-kits-p-13624.html

But I'm not sure if it would fit the Cal II trucks!! And I don't think this one would allow/ fit a larger gear for the Hypa hub! 
http://www.trampaboards.com/caliber-ii-carbon-fiber-motormount-with-axle-support--pulley-kit-p-13090.html
```

---
## \#15 Posted by: trampa Posted at: 2017-05-19T21:11:50.378Z Reads: 64

```
Hi NerdNinja, there is no kit fitting both, caliber II and Hypa hub setups. A caliber truck is designed to work with street wheels.
The only dual setup capable design is the carve board fleet. This can take 83,90,125mm and pneumatic wheels. It's an awesome board! I have a build thread going on. Official Trampa build thread...

Frank
```

---
## \#16 Posted by: NerdNinja Posted at: 2017-05-19T22:30:02.240Z Reads: 59

```
Ok, well I'm 100% set on the board. 
The next thought in my head is to get the urban Carver infinity trucks. But looking at then it seems they're designed for boards with angled mounting plates. Witch I could easily build on to my board. 

Would that then work with the urban Carver mount?
I don't see why not.
```

---
## \#17 Posted by: trampa Posted at: 2017-05-20T02:23:18.214Z Reads: 60

```
Yes, works. Do yourself a favor and go for the carve board deck. It's a fucking lush setup mate. Outperforms anything out there. The angled nose section lower your feet in reference to the trucks pivot point. Standing above the pivot point, using wedges, doesn't give the same feeling.

Frank
```

---
## \#18 Posted by: NerdNinja Posted at: 2017-05-20T04:02:21.646Z Reads: 53

```
Sounds awesome but I think it'll have to wait for a future build 🙂 the only reason I'm going with custom skateboards is because my girlfriend agreed to draw me a graphic. I don't think I could do that as easily with a carve board!
```

---
## \#19 Posted by: trampa Posted at: 2017-05-20T06:57:23.408Z Reads: 57

```
You can. Just print it on foil and stick it on. 
Some people have done lush stuff.

Frank
```

---
## \#20 Posted by: hornet90 Posted at: 2017-05-20T10:56:41.902Z Reads: 48

```
have a look at lipo 5 x 2s 5000mah 65c with a bestech bms theres more work wiring and reading heres the link
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014?u=hornet90
```

---
## \#21 Posted by: NerdNinja Posted at: 2017-05-20T15:31:11.180Z Reads: 45

```
That might actually be cheaper... I'll look into it!

@hornet90 Any reason to do this over a diy 10s4p with li-lion cells?
```

---
## \#22 Posted by: hornet90 Posted at: 2017-05-20T15:37:43.057Z Reads: 46

```
im finding constand power is a lot better less sag you should get 13 to 14 miles out of that set up im just waiting on my bms i should be testing within a week or so
```

---
## \#23 Posted by: NerdNinja Posted at: 2017-05-20T15:44:39.137Z Reads: 46

```
Huh, well I think I'm gonna stick to the 18650 cells. 

https://www.electric-skateboard.builders/t/18650-li-ion-vs-lipo-battery/5346

Check this out! It's short but... yeah. Oh and this!

https://youtu.be/LqgP16JQ24I
```

---
## \#24 Posted by: hornet90 Posted at: 2017-05-20T16:04:47.013Z Reads: 44

```
i have the  (36V 8AH)  and i had 2 x3s 5000mha 65c lipo im going back to lipo,

you know its up to u but do more reading on it there are people on esk8 that would agree and disagree but u cant beat the real feel ive lost a lot of money on batterys im lipo all the way now,

let me know how u get on,
good luck with the build
```

---
## \#25 Posted by: NerdNinja Posted at: 2017-05-23T18:39:22.324Z Reads: 39

```
Can someone tell me if these will work together? I'm only not sure about the belt length....

http://shop.sdp-si.com/catalog/product/?id=A_6A35M060NF1008
http://shop.sdp-si.com/catalog/product/?id=A_6A35M016DF1006
http://shop.sdp-si.com/catalog/product/?id=A_6T35MF126100

I guess I should also find out if the large pulley will work with @Maxid 's hub design...
```

---
