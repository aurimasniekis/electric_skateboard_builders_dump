# (First Build) The Mighty Penny &#124; 22&rdquo; Penny &#124; Bennett Vector 4.3&rdquo; Trucks &#124; 6355 190 KV &#124; Turnigy Mount &#124; 2 5s 5000mah Lipos &#124; VESC

### Replies: 14 Views: 460

## \#1 Posted by: Zimm Posted at: 2019-06-21T06:32:54.204Z Reads: 149

```
Hi, first time builder/poster. I've lurked this site for months and I'm finally ready to begin my build. I will be heading to college soon and figured I should build a board to help get me around once I get there. While I'd love to build a large, dual motor board to get me around, its related size is not practical for me. I need something compact and easy to carry, and have batteries that are "plane-legal". So, I've decided to challenge myself to build around a 22" Pennyboard. 

My current (unpurchased) build plan goes as follows:

* Deck: 22" Penny (I actually own this bit of the build)
* Trucks: 4.3" Bennett Vector Trucks 
* Mount: Turnigy Mount
* Wheels: Abec 83mm's
* ESC: VESC
* Motor: 6355 260 KV from torqueboards
* Battery: Two 5s 5000mah Lipos wired in series
* Gear/Pulley: 36t and 18t | 12mm belt

I wanted to keep the overall aesthetic of the Penny unchanged, but by doing so I know the board will be slightly unstable given the truck's narrow size. I will be riding around a relatively flat college campus, so I don't need huge speed or power numbers (though a little power never hurt, right?) From my mock ups I'm fairly confident everything will fit, so long as I reverse mount the motor. 

My biggest concern is the electronic side of the build. I know my batteries should each hover at the TSA's limit of 100 watt hours (18.8v * 5000mah), but in series, the two 5s's should act like a 10s (I think). My main questions are: Is this a good battery/motor/ESC set up and what kinda of range should I expect from this thing. 

Any and all advice would be appreciated, like I said, I'm new to this, but plan to update y'all as I work on the build.
```

---
## \#2 Posted by: Grozniy Posted at: 2019-06-21T08:06:31.846Z Reads: 128

```
You can't use more than 200kv on 10s with a 4.12 ESC. Either lower S count or get <200kv motors.
```

---
## \#3 Posted by: Darkie02 Posted at: 2019-06-21T09:10:22.140Z Reads: 126

```
I’d recommend re looking at you gear ratio if you used a 190kv motor and the 18-36 ratio on 83mm wheels on a 10s your top speed would be 30 MPH 47kmh approx with you on it and you will pull of slowly. Personally I wouldn't want to be going much over 20 mph on a 22inch board (presuming this is board length not truck spacing as you said penny) it be so twitchy as well. I’d be wanting more tork for acceleration and way more brakes. As a heads up on real world experience a single drive 190kv 12-36 ratio 80mm wheels I’m using 50 motor -65a motor on a 6355 senesced motor doing 18 mph and I barly able to pull of up a slope and the motor heats up after a ride. Is your lipos able to discharge a good amount safely with out a huge voltage as I pull 35amp out my battery on a regularly. Hopefully the figures will give you a idea and push others to share there’s as well. so you can decide if you want more speed, acceleration or pushing components harder to get more every thing but sacrificing reliability. By the way I trash 9mm belts in a mile 1 mile. 12mm belts can handle the acceleration but not the brakes as it skips under hard braking. 15mm belts are still running grate. And I think I’m quite general and don’t tear around much.
```

---
## \#5 Posted by: Zimm Posted at: 2019-06-21T09:32:25.223Z Reads: 107

```
@Grozniy Is this because the higher KV at 10s voltages would overshoot the VESC’s 60,000 eRPM limit?
```

---
## \#6 Posted by: janpom Posted at: 2019-06-21T10:39:04.225Z Reads: 101

```
I don't think that's the main problem. You can always put a limit on eRPM in the VESC config. It's more about what @Darkie02 said. With 200kv you won't have a good trade-off between the speed and torque. You will want less kv for better torque at the expense of lower speed since 47 km/h on a penny-board is crazy. You don't need that much speed. I don't ride more than 40 km/h on my EVO, which is a downhill deck.
```

---
## \#7 Posted by: Zimm Posted at: 2019-06-21T14:39:18.558Z Reads: 93

```
@janpom So something like a 6355 with a 190 KV would be suited with more torque?
```

---
## \#8 Posted by: Darkie02 Posted at: 2019-06-21T15:12:55.877Z Reads: 95

```
The higher the motor KV the faster it spins at a set voltage 

The hire the voltage (eg 10s) the faster the motor will spin

The higher the number teeth on the motor pully the faster it will be

The lower the teeth count on the wheel pully the faster the board will go 

The larger the wheel diameter the faster the board will be

The faster your board will go the lower the tork at a set wattage.

Tork is needed for acceleration stoping and power to low and it just stall same as a car stalled motors pull huge amps and burn out motors coils. 

A VESC has a limit to the MAX RPM of the motor different VESC have different limits. Same as a car has a limit of its revs go to high and it can damage the electronics of the vesc. Think of it as snapping the needle of a Speedo in a car cos you went to fast.
```

---
## \#9 Posted by: Darkie02 Posted at: 2019-06-21T15:25:55.388Z Reads: 92

```
There’s more than one way to change gearing ratio see it as 

You could be filling a swimming pool with a bucket 

If 2 people fill the pool but had to walk 2 time feather it take the same amount of time 

If 10 people did it but had buckets 1/10 of the size it take the same amount of time

If 2 people want at 1/2 speed cos thay were cheating it take the same amount of time 

Etc etc 
Need to work out what you want and how to achieve it as there’s so many difrent ways of achieving the same gole

You need to reduce speed increases tork

You could

Smaller wheels

Larger wheel pully

Lower KV motor

Smaller motor pully 

Or any combination of the above but it’s down to how much speed your willing to trade for tork only you can decide what’s the right balance how to achieve it.
```

---
## \#10 Posted by: Zimm Posted at: 2019-06-22T01:46:48.000Z Reads: 71

```
Okay folks, ordered the parts this afternoon and I will edit the thread title to match:   

* Trucks: 4.3" Bennett Vector Trucks (US$ 27 a piece)
* Mount: Turnigy Mount (US$ 10)
* Wheels: Abec 83mm’s (USS 30)
* ESC: TorqueBoards VESC (US$ 80)
* Motor: 6355 190KV from torqueboards (As per @Darkie02 and @janpom suggestion of a lower KV) (US$ 90) 
* Battery: Two 5s 5000mah Lipos wired in series (US$ 48 a piece, 5 for a Y connector)
* Gear/Pulley: 36t and 18t | 12mm belt (US$ 30)

Along with a charger and a remote, this came out to about 500 dollars, I hope I can make it all work. 
Thank you to all who helped me so far, I will update when I begin piecing it together.
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-06-22T02:36:30.420Z Reads: 70

```
anything below 220kv is fine for 10s.

220kv on 10s is 55440 ERPM (a safe amount under the 60K ERPM max of vesc.)
```

---
## \#12 Posted by: Darkie02 Posted at: 2019-06-22T08:49:53.554Z Reads: 73

```
Wouldn't trust Turnigy motor mount you will end up replacing them quickly. it’s known for bending and braking on this forum plenty of posts about it.

If you want cheep mounts rated by the forum a quick seething brings up

@Boardnamics 
https://www.electric-skateboard.builders/t/15-20-boardnamics-caliber-motor-mounts/73643/830

@dickyho
 https://www.electric-skateboard.builders/t/new-designed-a-motor-mount-for-sale-looking-for-review/59212/1086

190kv a good middle ground KV. But I can see the top speed be around 45-50 kmh. If you increase the wheel pully mutch more you may get it grounding out. I can see you upgrading to a 14 or 12 teeth motor pully ones you have riden it for a bit. Giving you a top speed 36 kmh or 32kmh approx but that all important tork.

 190kv 18 36 is normally used on dule motor set up on longboards, bigger battery’s more amps delivey a average set up 10s 4p q30 deliver 80amps capability’s double the motor were you have loads of tork and trade it for speed. I don’t know what Lipo your intend using of but Lipo specks are wildly Ambitious and voltage will be a huge factor in a small build.![image|375x500](upload://t00neMUp6KaPCqa7xwYpLmCfzk7.jpeg) ![image|375x500](upload://lGvuCfBUWpHngnBcTYIYxar9rWC.jpeg) to put fact to what I’m saying I’m building a 10s 3p 18650 VTC5A battry thay max spec to deliver 105amp to dule 6355 170KV motors 14-36 gear ratio on 107mm wheels aprox 47kmh so with double the power I’m aiming for the same speed and I think I need more tork less speed but I’m restricted to the gear drive set ratio and I want a smother ride over bumps hence the massive wheels over my cure t 80mm ones.
```

---
## \#13 Posted by: Darkie02 Posted at: 2019-06-22T09:59:31.297Z Reads: 60

```
To put the speed in to prospective when passing people walking I ride 8-12 mph. cruse around corners and over bumpy things at about 15mph blasting down a smooth road or cycle lane 20mph. over than and the boards get twitch and you can’t stop quickly and can’t do much to avoid a crash you dident see coming till last second imo. but then I use my board mainly around city’s and short trips to the shops and work say up to 3 miles. That’s why I’m building a new shorter 32inch deck so it’s easer to carry. Most people ride in the 15-20 mph range it’s why most production boards don’t go much over 20 mph. People like to post there fastest trips and bost who has the biggest balls but there are always a few exceptions to the norm some speed lunatics that are doing 50mph most of them like to post how fast thay go. Top speed of 25 mph is more than enough for most people.
```

---
## \#14 Posted by: accrobrandon Posted at: 2019-06-22T14:41:10.281Z Reads: 52

```
my 2 cents on your penny..some already covered..lower kv motor... slightly larger wheels maybe 90mm and the gearing is going to be way to fast for a short board.. a longer board will have more stability at speed.. on a 22" board id probably only want to hit 20mph...i prefer to ride high 20s most of the time when/where possible... and thats on a 40" board....
15/36 is probably good for a short board and good torque especially it its a single
```

---
## \#15 Posted by: Zimm Posted at: 2019-10-18T05:42:13.396Z Reads: 33

```
I don't know who really cares at this point, but the build is mostly finished. I ended up using a cheaper eBay ESC and wider trucks (5.3 inch Bennet Vectors) but she rides amazingly and I can top out at 20 mph on campus. Range has yet to be truly tested, but with a 10s 5000mah I should be set. ![IMG_3871|666x500](upload://fwUnoJfbOOQThudWB809BFFRzjx.jpeg)
Clearance hasn't been an issue (yet!)

![IMG_3868|374x500](upload://xkBfT1TDZmvnFBj5mknk6QZBUd9.jpeg)  
Everything fits nicely into the plastic container, and it will be getting a coat of paint in the short term. 
 
![IMG_3870|666x500](upload://jzkbWy5qzk2FzxDZh1WVMUc17wP.jpeg) 

![IMG_3872|374x500](upload://tZaoMETO5Qebp55IKiQ6EYhe6WI.jpeg) 

For the mount, I ended up using a 3D printed square that friction fits around the trucks, and then screwing a mounting plate into it.
```

---
