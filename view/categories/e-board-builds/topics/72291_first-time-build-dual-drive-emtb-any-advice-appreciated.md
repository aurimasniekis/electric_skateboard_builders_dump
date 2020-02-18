# First time build! Dual drive eMTB &#124;&#124; Any advice appreciated!

### Replies: 14 Views: 342

## \#1 Posted by: LachMcK Posted at: 2018-10-25T11:40:11.359Z Reads: 115

```
Hey guys,

Sorry for the long post, but thought I should get enough. First a little about me...My name is Lachlan, I'm 23, from New Zealand. I have a background in mechatronic engineering and thought it was about time I started a bit of a project...with a mountainboard lying around (absolutely no Idea what make/brand) , I thought I could have a little fun. Where I live, there really aren't many hills...mostly I'll be commuting 10km to uni each day, but would also like some room to play around a bit offroad and small inclines (I know, a lot to ask, but thought I should aim high :P). Ideally, I would like a board that could top-out at 45-50km speed...of course I wouldn't immediately jump to these speeds, but I think in time I would quite like the option (I've been long-boarding for years, some downhill, and I think I would be comfortable with these speeds)

I've been doing a bit of reading on the forum and also endless-sphere etc, so slowly starting to learn something. So far, this is the build/components that I have come up with:

**Parts Acquired**

_Pneumatic wheels_ - 9" (I know, inefficient, but they're what I've got at the moment)
_Large pulley_ - HTD timing belt 5mm pitch 16mm wide  -  76T aluminium
_HTD timing pulleys_ - 5mm pitch 10mm wide  (http://www.ebay.com.au/itm/292307247956) 
_Motor mounts_ - @dickyho long motor mounts for paris trucks. Still in process but I have read good things about these :) 

**Parts (potentially) To Get**

_6x LiPo batteries_  -  5000mAh 3S 20C, wired into two sets of 9S 5000mAH in parallel...so 9S 10AH battery
(https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack-xt-90.html)

_2x Turnigy Aerodrive sk3 6364 213kv_ -
(https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html)

_2x motor pulleys_ - figured I'd get a 5mm HTD pulley somewhere between 12T and 16T for ~5:1 to 6:1~ gearing ratio. I've yet to source these but dont think they should be hard to find. I plan on filing the sk3 motor shaft and using a grub screw to fix.

_ESC / VESC_ - I've been reading a wee bit about these, and think I've just confused myself entirely. I'll definately have to do some more reading 

**Queries**
Firstly I'm a bit unsure as to which esc / vesc I should be investigation. Seems like a go to would be the VESC (what would be a good vendor for NZ based purchase?)...however, I've also read that these ones here are also pretty good and also cheaper (https://www.ebay.com/itm/Dual-motors-longboard-skateboard-control-modula-ESC-Substitute-with-remote/323326552273?hash=item4b47c3a8d1:m:mxSlsLM_-dEIr0XuDFII9Lg:rk:3:pf:0). For a 9S-10S dual drive mtb build, what would you recommend? I'm not too worried paying a little more for the motor controllers as I know they are a veeery critical part, but also wouldn't mind paying less than top end $$.

Secondly, I've read that pneumatic wheels are less efficient than longboard. This makes sense to me as they are squishy etc, but I would still like to get as much range out of my board with 10AH as possible. Do you think the current setup I have is somewhat efficient i.e. dual drive 213kv with 9S and gearing of 1:5 to 1:6 on 9" wheels? I was thinking of using 245kv motors to push them into the 8000-9000rpm range as suggested by @onloop in (https://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53...very helpful by the way), but thought that I should leave some room incase I was to increase my battery voltage in the future (I would love to make my own li-ion pack at some point).

What do you think of my choices? What would you do differently?

Any help whatsoever would be greatly appreciated :)...also, if I've posted this somewhere funky, or any of my questions can be easily answered in a different thread, then please dont hesitate to let me know.

Cheers my dudes,

Lachlan
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-25T11:54:04.794Z Reads: 89

```
Welcome here!
You can calculate your range and speed on this site 
http://calc.esk8.today/
The average wh you will use will be between 20-30wh per km round about.
I can’t say anything to the esc you bought as I didn’t used that one but if I remember right you can run them only in 6 or 10s (please correct me if i‘m Wrong) 
So if you want to go 9s it’s not the right choice.
If you have some money left, focboxes always a good choice as esc.
I personally would choose lipos with a higher c-rating as this would help you later if you want to go for some off road session.
```

---
## \#3 Posted by: Grozniy Posted at: 2018-10-25T13:51:36.698Z Reads: 81

```
Please don't buy ESC substitute, it only delivers 18a per motor. It can be set for 6,7 or 10s.
ESC is something you should not cheap out. Get focbox or unity.
Get graphene batteries with more than 60c. C rating is always overrated
I also remember that Roxxy esc is very good
```

---
## \#5 Posted by: LachMcK Posted at: 2018-10-25T19:41:41.180Z Reads: 67

```
Hi guys, thanks for the fast replies, it really helps when there's a responsive community :).

I have a few follow up questions to ask if you don't mind?

1. Message received about the cheaper esc, will definitely look into better options such as the focbox, unity, or roxxy. Interesting that they only work on specific voltages rather than a voltage range (this is what I assumed). does anyone have experience in building open-source esc (like the vesc)? I have the resources to get pcb parts and assemble it....but in the end, does it end up much cheaper making them this way (although I'm sure theres much to gain learning-wise from the project)?

2. I note that both replies from @Andy87 and @Grozniy say to invest in lipos with larger C ratings. What sort of continuous discharge should I be aiming for (for offroad, I really just mean't going across a grass-maybe muddy field)? From what I calculate, with a C rating of 20C and a capacity of 10AH, I should get a continuous discharge limit of 200A, is this not enough? I know the lipos wont actually have the 20C and 10AH rating, but I'm expecting it should still do ~150A. Is voltage sag an issue at this range?

Thanks again,

Lachlan
```

---
## \#6 Posted by: b264 Posted at: 2018-10-25T20:03:13.505Z Reads: 65

```
Don't get motors with a kv over 190.

Even if you use them on 9S.  You can always add a bigger motor pulley to increase the ground speed.  But later if you decide to change something, you would have to buy new motors to change anything, instead of just getting a $15 pulley.

Plus motors with a kv over 190 have very little resale value.
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-25T20:09:08.436Z Reads: 65

```
I have the heavy duty lipos from hobbyking 5000mAh 60C and 6s is about 70€ for a pack.
I use them only 2 or 3month but till now they work great. Sag is minimal even with dual 6384 170kV motors. I think it’s a good deal for what you get. The still a bit warm when I run them till 3.5v so I don’t want to know how it would be with 20c rated packs.
C Rating is relativ... i heard that for example the multipower lipos from hobbyking have only 3-4c from there advertised 12c... the cheaper the cells the more sure you can be the c-rating is not related to there real constant current ability.

I don’t know how it is with hw 4.xx but for a hw 6.xx vesc the components should be around 80-90$. If you have skills and experience in soldering parts like the drv chip to a pcb than it’s maybe an option for you to totally diy your vesc.
If no, I think it’s not worth the time and money. Better go with one of the ones already out there.

If you go with 10-12s look maybe for motors with a bit lower kV. 150-190 on 10s or 150-170 on 12s is a good choice.

If you decide to use a vesc, take a look if you maybe want to upgrade your motors to sensored motors. They nicer in the start up (without chiggering) and even on small hills you can start from stand still. Buuut get sealed motors than or as min cover the sensors with some electronic lack (sorry don’t remember the English word for it) or epoxy/liquid tape or similar to prevent them from shorting when you go through wet areas
```

---
## \#8 Posted by: dareno Posted at: 2018-10-25T20:31:55.496Z Reads: 56

```
Welcome mate,  Just to add to the info received;  Always plan some expansion into the build so upgrades are easier and less expensive.
You will eventually want to 12s (trust me) so no motor over 190 and bigger can the better min 6374 for mtb
Don't cheap out on the batteries especially lipo's.  Esk8 puts them under a lot of stress so the higher the c rate the better and go for graphenes if you can afford them.  
Vesc all the way,  don't even think about an esc substitute or car version. Vesc is made for esk8.  
Get either the focbox at 4.12 or a 6 variant if you want to upgrade later.  
Happy building man and keep the thread updated with pics.
```

---
## \#9 Posted by: LachMcK Posted at: 2018-10-25T22:05:40.603Z Reads: 46

```
Good advice. I'll definitely be spending a bit more on batteries of proper quality...seems the more I look into this project, the more I want out of my board...therefore the stricter the specs for components haha.

I'm still at uni and have access to pcb pick n' place machine and oven..so maybe I'll look a wee bit more into open source stuff, but still undecided on that one.

As far as motors go, what do you think of the hobbyking sk8 6374 190kv?. I know some have had issues with can movement, but this seems to have been solved by using the copper shaft sleeve...these motors also appear to be sensored and sealed (correct me if I'm wrong on that). I'm also looking at maytech and alien power systems alternatives, but are they worth the higher price point?

Thanks
```

---
## \#10 Posted by: Grozniy Posted at: 2018-10-26T00:52:38.170Z Reads: 39

```
From other people experience, maytech are great. On Lacroix they work flawlessly
```

---
## \#11 Posted by: Andy87 Posted at: 2018-10-26T04:56:34.333Z Reads: 37

```
I don’t have sk8 and maytech motors but from what I read here they both a good deal.
The sk8s are kind a longer than usual but if you have wide trucks that shouldn’t be an issue.
I have 7aps motors. They usually not sealed and I still wait 2 of the 5 motors I ordered in middle of July...what kind a bit sucks... expected 6-8weeks, now it’s close to 4 month and winter in front of our door...
One of my 6384s magnets broke first time I made motor detection. They sent me replacement can without asking a lot of questions but I had to wait again for it and i don’t like waiting stuff 😅 

I have seen a time ago there was a group buy, sk3 sensored (yes sensored) as they ordered them custom made directly from the factory. Think that is the best you could get 😉

If you already up to want more and more... believe me it’s not getting better in future.
Best advice I can give you here, 
Better save some money get quality stuff, some vescs or focboxes and you ready to upgrade things easily in future. That will safe you money in the long therm as you will not need to swap all parts.
```

---
## \#12 Posted by: LachMcK Posted at: 2018-10-26T05:43:33.499Z Reads: 33

```
You make some good points @Andy87, thanks for the input. Think I'll go for some sk8 6374 190kv motors, they seem pretty good for the price point (if they go bung, its not much of a loss to get a different motor). Of course I'll have to properly measure up my trucks and hardware to see if they will fit. Could always do diagonal drive if I need to

Myself and a mate think that we'll look more into the vesc open source and see if we could make some ourselves. Even if they don't come out well, it'll be a good learning point for us :).

I'm a relatively slow worker so it'll probably be a while until I get everything together..still I can't wait haha.

Cheers, 

Lachlan
```

---
## \#13 Posted by: Andy87 Posted at: 2018-10-26T05:57:08.530Z Reads: 31

```
you know, if you get some experience to make your own vescs there is always a need here.
maybe one day it is an option for you to buy components in bigger amount and sell the assembled pcbs like @stewii made it with his escapes. Just take care you name it not VESC and don´t use the same designe like the VESC6 from trampa...
```

---
## \#14 Posted by: LachMcK Posted at: 2018-10-26T06:18:15.709Z Reads: 32

```
Would be pretty cool...maybe I'll call it the NotVESC  lol. Don't think that'll happen though ;p
```

---
## \#15 Posted by: Andy87 Posted at: 2018-10-26T06:26:43.177Z Reads: 32

```
as far as i know you can buy the pcb with layout form @stewii and just assemble the components by our own.
```

---
