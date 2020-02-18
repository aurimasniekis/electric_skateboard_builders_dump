# mayoBoard &#124; Scrub mountainboard &#124; 190kV &#124; 6S &#124; FSESC Flipsky

### Replies: 11 Views: 440

## \#1 Posted by: Mayo Posted at: 2019-06-13T12:51:41.753Z Reads: 126

```
Hi Guys 😁

Student from Poland needs some help.Its my first project. One months ago I intersed build my own Electric mountainboard (one motor) . I was reading your forum and other sites. I knew something and probably need some sugestion

I bought used mountainboard 'scrub'

![IMG_20190613_142900|251x500](upload://81STqX98oy1kGNG9E8TavQQ4Y3w.jpeg) 

Motor- 190kV 

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html?___store=en_us

VESC 

https://flipsky.net/collections/electronic-products/products/torque-esc-vesc-%C2%AE-bldc-electronic-speed-controller

Battery (bought) 

3x ZIPPY 3000mah 6S 20C (9000mah 6S)

At the start should be good, in the future I would go 12S. 

Motor mount

I want project motor mount and print 3D

Pulleys 

Im thininkig about pulley, 15/60? 

Controler 

https://hobbyking.com/en_us/quanum-2-4ghz-3ch-pistol-grip-tx-rx-system.html

Deck changes

![received_258702284999464|250x500](upload://vK2FAwnuwdjov2BKv22cQloJJOm.jpeg) 
![IMG_20190612_170147|690x388](upload://yedTx9D5MbrEmXJ8adS7AnbTdsD.jpeg)
```

---
## \#2 Posted by: Riako Posted at: 2019-06-13T17:03:31.681Z Reads: 90

```
Nice one ;) I bought [the same used deck](https://monlongboardelectrique.wordpress.com/2016/01/28/i-plateau-de-mountainboard-custom/) in ... 2015 or before ...  
Love the shape (the stance is a bit too short for me for hard off-road or race mtb, but really cool for cruising and riding the trail on those 9" primo stricker :+1: 


For motor, if you can (like you will be riding strapped I guess), take the sk8, with low kv (130)
sk3 are better made, but I also use the sk8, and for a 1st build i think it should be ok.

VESC .... if can't get a good deal of 2 focbox or v6 like to ride in foc mode. It should work (it was my 1st emtb too, vesc 4.10, 12s5Ah, 6374 170kv ...etc) but prefer bldc. Try to get one more of your lipo maybe (12s6Ah looks good to start)

Try to buy Alloy mount as soon as you can ^^

Go with chain maybe ? (it could be cheaper if you drill it yourself)  
determine your ratio after choosing your battery setup, kv, and wheel size (but keep those 9" maybe just change rim in the future ;) )

Good continuation :v:

EDIT : :smile: mayoboard !.. awesome, definitly a right name !  

https://youtu.be/ph0P6J2xhVE
```

---
## \#3 Posted by: Mayo Posted at: 2019-06-13T22:50:01.336Z Reads: 78

```
Thanks for so long answer 😁 i have to think of about the motor and batteries.

Guys, what do you think about anit spark switch, and where I can buy it?

Meanwhile effect my free evening 

![IMG_20190613_214800|690x388](upload://dZEp5DRzuBKsmmnEUkWWJI1U04D.jpeg)
```

---
## \#4 Posted by: Riako Posted at: 2019-06-14T03:05:57.991Z Reads: 71

```
U're welcome ;)  
Choose a switch key, buy an xt90s (or I know overion.fr sell some with custom pcb support etc)
```

---
## \#5 Posted by: Mayo Posted at: 2019-09-19T19:57:07.719Z Reads: 50

```
Guys, I have problem...

Probably when I was updating firmware my vesc I bricked it. Any updates doesnt work. When I try to connect VESC tool 1.19, still this same 'too old firmware'

My Flipsky FSESC FW version 3.57

Could I trying looking for VESC tool v.1.15 which support fw 3.57? Or trying rescue bootloader by ST-link and programmator. Anyone can help?
```

---
## \#6 Posted by: Andy87 Posted at: 2019-09-20T05:47:57.368Z Reads: 39

```
if you can connect but not upload fw than the bootloader is missing.
load the bootloader first, than the fw and you should be good.
```

---
## \#7 Posted by: Andy87 Posted at: 2019-09-20T05:49:53.878Z Reads: 38

```
if you have a second vesc you always can uploade new FW via SWD port.
https://forum./t/problem-with-vesc6-forgetting-settings/3208/16?u=andy87

no need for st v2 link.
```

---
## \#8 Posted by: Mayo Posted at: 2019-09-20T09:50:36.946Z Reads: 36

```
Load bootlooader by st-link? 

Like on this video? [https://www.youtube.com/watch?v=LFgxvkzk9JU](https://www.youtube.com/watch?v=LFgxvkzk9JU)

I dont have second vesc, but maybe its a good plan. Somebody from my neighbourhood maybe help me.
```

---
## \#9 Posted by: Andy87 Posted at: 2019-09-20T09:57:30.283Z Reads: 35

```
no st link.
go to firmware in the vesc tool.
there is a tap for bootloader.
click on it and upload the bootloader file.
after that load the firmware like you did before.
```

---
## \#10 Posted by: Mayo Posted at: 2019-09-20T10:04:53.616Z Reads: 35

```
Andy, its a problem :frowning: I did it, doesnt working. I watched youtube, looking internet and nothing.
```

---
## \#11 Posted by: Mayo Posted at: 2019-09-28T07:12:04.578Z Reads: 24

```
Hello Guys. Two days ago I've finished!!! 😁 Im soo happy. Some corrections left but desk is riding

![IMG_20190927_142232|690x388](upload://wxtes0VOIOiTQzhLYIpFJDzNfi6.jpeg) ![IMG_20190927_141137|690x388](upload://dMhYGbMY3LiC9sc7RIxShR0FnuP.jpeg) 

About specification

➡️ Motor- Turnigy SK3 245kV
➡️ Battery- 3x ZIPPY Compact 6S 3000mah
➡️ Controller- FSESC Flipsky 4.12 50A
➡️ Mountainboard- Scrub furnace
➡️ Pulleys-12/60, belt HDT-5M
➡️ Motor mount- Turnigy motor mount
➡️ Switch- Flipsky antispark switch 

My problem is 'Tooth in mesh'. With this pulleys and short motor mount. My score is 4, correct is 6. Pulleys 16/72 and longer motor mount Will do the trick. 

Problem with Vesc firmware was solved by Flipsky support sent me VESC tool support my fw


Im suprised, because everybody said '6S is too weak for mountainboard'. On flat ground where is no asphalt desk have no problem. Riding on pavement, flat forrest Road or getle hills situation is the same. That was my priority 😁 

Its my first build. Little by little to check if it's for me. And I can say - ITS FOR ME 🤙😍 

Build cost - 500$
Max speed - 30km/h
Range - 12km

I already thinking about upgrades. Battery and more range is second thing after pulleys and motor mount. 

I will note about upgrades and change, greetings from Poland and thanks for help 😁
```

---
