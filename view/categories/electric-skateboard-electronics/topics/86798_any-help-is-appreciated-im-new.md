# Any help is appreciated - I&rsquo;m new

### Replies: 17 Views: 390

## \#1 Posted by: Resonant Posted at: 2019-03-10T23:25:47.192Z Reads: 146

```
I am planning on building my own board but I have just been trying to figure out all the parts I will need, also to not go overkill and have wasted/unused power + money. Also I am completely new to this. I am trying to make the board have good amounts of torque to climb any hill, good range 20+ miles, and high top speed around 34 mph (if chosen to go full throttle)

Dual Eskating PRO motors 6374 190Kv (I need that water resistance) 
Specter Bintang Deck
218mm TB Trucks
12s4p battery pack + enclosure from @eboosted 
16T Motor pulley
97mm TB Flywheels
40T wheel pulley for ^ wheels

I need help determining the belts I would need for this setup. 

All the TB stuff for mounting motors > what I have decided on for now

FocBox Unity ESC


Remotes: 

This remote from slick revolution: https://slickrevolution.co.uk/product/advanced-wireless-controller/

^ I am trying to figure out if that would work with the ESC, or possibly use this flipsky remote: https://flipsky.net/collections/new-accessories/products/flipsky-remote-vx1?gclid=CjwKCAiAiJPkBRAuEiwAEDXZZZHrd8oLN4aA7igJEz2kJp5sDQ3vHLQ-yV9uaPoT4I677KdxlKoZoxoCfm0QAvD_BwE

I have heard bad things about flipsky's products but I am unsure of any remote that is boosted board style that will work with any ESC besides their own + exway etc. I really wish I had the choice of Exway's remote, I love the look of that remote but I read on a thread that the suppliers don't sell individual remotes. I am curious if anyone knows of any other remote that has a similar style that I can use to DIY. 


I don't think I am missing any of the other core components.
I haven't heard much of Eskating's motor quality but I assume it may be similar to TB I do not know the differences besides one being sealed. 

I used an online calculator and the numbers specify 39 mph max. It also said 53 miles on range but I know that number is entirely unrealistic, and maybe more 25-30 miles max as TB website says thats the range they get on their 12s4p battery. Are these numbers reliable for the setup I would be using?

And does anyone know if it is possible to add a gps chip and maybe link it to an app in case it gets stolen. 

I also want to add LEDs to the bottom of it but I will have to do more research into that.

Any ideas or improvements I could make? or any knowledge on any of the particular subjects mentioned?
```

---
## \#2 Posted by: Jacobee Posted at: 2019-03-10T23:33:59.596Z Reads: 127

```
With that gear ratio you'll get around 32 mph. you'll get about the 20-25 miles out of a 12s4p that torqueboards advertises but remember if you stay above 30 mph for extended periods of time you will drain your battery quickly because of the air drag. Also the tb battery is double stacked and I'm pretty sure the eboosted enclosure is built for a single stack battery.
```

---
## \#3 Posted by: Resonant Posted at: 2019-03-10T23:35:14.742Z Reads: 121

```
he said he would make me a 12s4p to fit his enclosure, I was referring to the TB battery as the range for a 12s4p, and maybe what gearing what i need to keep a good amount of torque to climb steep hills but increase the top speed to 35-37 mph? I wouldn't ride for extended periods of time at this speed, of course.
```

---
## \#4 Posted by: Jacobee Posted at: 2019-03-10T23:41:02.911Z Reads: 113

```
Also any remote with a reciver will work with a vesc. I've heard that one ot the models of the flipsky dual esc was a little buggy but their remote should be fine. 
Also read this if you are trying to figure out what remote you want
http:///esk8-remotes-garbage-or-greatness/
```

---
## \#5 Posted by: J_Dizzle Posted at: 2019-03-10T23:42:30.342Z Reads: 101

```
If you are using Torqueboards motor mounts 265mm belts will work just fine
```

---
## \#6 Posted by: Resonant Posted at: 2019-03-10T23:59:50.582Z Reads: 99

```
Kinda going for enough torque board that will leave a boosted board stealth in its dust, I have a feeling with the current motors and maybe any ratio above 2:1, it will do just that torque wise. But how to get a 33-35 mph top speed to have the ability to destroy on flat surfaces.

What do you think I should change to accomplish that? Gearing ratio maybe 2, 2.25 or lower?

And to clarify you were saying the that a VESC will work with any remote with a reciever, but does that include the Focbox unity?
```

---
## \#7 Posted by: M.Hboards Posted at: 2019-03-11T01:37:39.142Z Reads: 82

```
[quote="Resonant, post:6, topic:86798"]
And to clarify you were saying the that a VESC will work with any remote with a reciever, but does that include the Focbox unity
[/quote]
The focbox unity is a vesc!
```

---
## \#8 Posted by: Resonant Posted at: 2019-03-11T02:39:42.569Z Reads: 76

```
Aha I see thanks
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-03-11T02:47:08.653Z Reads: 70

```
[quote="Resonant, post:3, topic:86798"]
i need to keep a good amount of torque to climb steep hills but increase the top speed to 35-37 mph?
[/quote]

Pssst, once again if you use the search bar would find out that hitting that speed will be hard and uncomfortable, not only that but you need tons of skills (have you ridden a skateboard before)?

But mabye try 18/40, dual 6374 will have more than enough power and should rocket almost everyone up hills, traction will present as the greatest issue if you push the 6374 hard. (80a per motor) even though it only requires about 22a to get up to full top speed
```

---
## \#10 Posted by: Resonant Posted at: 2019-03-11T04:36:06.431Z Reads: 64

```
I have a meepo board v2p and gone full speed down hills at 25 mph, cruise at the full speed which when I first got it was 25 but now is around 22 probably due to the battery. I do know how to skateboard. If the speeds of 30+ are difficult to acheive Ill shift my worry about keeping 31-32 top and mainly traction since that means the torque will just be even more insane lmao. I would probably program the esc to make the speed curve smooth enough to keep traction and maximizing acceleration. The meepo is broken af rn and starting to get a little weak for me but thats probably because not as much power has really been getting to the wheels. If it only requires 22a does that mean I could have it set that low and get more range? Or what even is the point of running it at 80a if it can be done at 22a?
```

---
## \#11 Posted by: J_Dizzle Posted at: 2019-03-11T04:48:34.008Z Reads: 54

```
The higher the amps the faster you can go. You could not go 35 mph using 22a
```

---
## \#12 Posted by: rusins Posted at: 2019-03-11T04:55:07.659Z Reads: 52

```
Well, in a vacuum tunnel you could get to 35pmh with just 1A; point is that higher speeds have more air drag, which requires more power, thus more amps. Going that fast will decrease your range, but I don't think that's a problem, because you can just go slower when you know you'll need every bit of juice ;)

In Latvian we have a saying: "driving slower will get you further", and it never made sense to me until I got into eskating :slight_smile:
```

---
## \#13 Posted by: Resonant Posted at: 2019-03-11T05:12:15.567Z Reads: 53

```
No way I would go 30+ miles per hour for the full range, let just say its only for when I 'need it' ;) <-in combination with perserving as much range and a decent cruising speed. Since my meepo doesnt get good range right now, I have just full throttled it everywhere for the most part when I could since I wouldn't be able to use it for much else just commuting and uh being late to class so it was also necessary, have been unable to use it as a board to cruise for a good distance since I get back to my house to charge it and the board is nearly already dead after a few miles.
```

---
## \#14 Posted by: KaramQ Posted at: 2019-03-11T05:45:01.876Z Reads: 46

```
Your going to want to change the 97mm urethane wheels to pneumatic tires if your trying to go 30-40mph
```

---
## \#15 Posted by: Resonant Posted at: 2019-03-11T05:57:27.651Z Reads: 48

```
Would keeping the 97mm be fine for low 30-34 for short periods of time? im probably gonna change goal of the top speed to be 34 max cus I dont think Id feel safe going any faster if I werent on pneumatic tires like you said I should change to, I will probably do that for an offroad build. After I do this one as a starter. Offroading on an eboard looks fun.
```

---
## \#16 Posted by: KaramQ Posted at: 2019-03-11T06:02:12.624Z Reads: 44

```
It should be fine, but I would go with 107mm, the bigger the better, and the tb 97mm aren’t the greatest in my opinion, either get abec 11, or preorder the 110 mm kegel core tb wheels
```

---
## \#17 Posted by: Resonant Posted at: 2019-03-11T07:07:02.118Z Reads: 40

```
They only are in green thats why I was thinking to go with the tb 97 mm in the first place and a bit cheaper. Are there any decent clones with color choices and maybe decent quality better than tb?

110mm wheels seem too large / increased center of gravity but may be accounted for with the dropdown deck. Also they are tb u just said the 97mm ones arent great?
```

---
