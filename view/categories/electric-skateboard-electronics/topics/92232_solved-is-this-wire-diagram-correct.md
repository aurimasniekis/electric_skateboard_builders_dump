# \[SOLVED\] Is this wire diagram correct?

### Replies: 9 Views: 342

## \#1 Posted by: Duy Posted at: 2019-04-29T19:06:38.272Z Reads: 84

```
Hi, this is my wire diagram for my build. I want to charge and discharge my battery with the BMS for saftey sake. Just wanted to make sure is this correct, can anyone verify? 

Assuming my wire diagram is OK, why is that I see others wire their +1 balance lead to the B- port together with the main battery negative (Thick black wire)?

![Wire%20diagram|420x500](upload://hQfCvzINAjMjnNP128wXWap61Dy.jpeg)
```

---
## \#2 Posted by: Duy Posted at: 2019-04-29T19:47:51.982Z Reads: 75

```
My bad, forgot to include what bms it is, Below is the wire diagram what the bms looks like.
![image%202|500x500](upload://ddR6jcbDDrGfT5CydXdwR5krgVR.jpeg) 
![image%201|682x500](upload://7kIBrNMioXn53hf12Nu1FXixwQk.jpeg) 

heres the link to the bms [https://www.ebay.co.uk/itm/10S-Li-ion-Lithium-Cell-36V-40A-18650-Battery-Protection-BMS-PCB-Board-Balance/232864260321?epid=23024661399&hash=item3637caa0e1:g:NBcAAOSwGZxbWie1&frcectupt=true](https://www.ebay.co.uk/itm/10S-Li-ion-Lithium-Cell-36V-40A-18650-Battery-Protection-BMS-PCB-Board-Balance/232864260321?epid=23024661399&hash=item3637caa0e1:g:NBcAAOSwGZxbWie1&frcectupt=true)
```

---
## \#3 Posted by: rich Posted at: 2019-04-29T21:22:14.458Z Reads: 61

```
Your diagram is correct, personally I prefer to connect B5+ of the BMS to B5+ of the battery but it's the same in the end.

[quote="Duy, post:1, topic:92232"]
OK, why is that I see others wire their +1 balance lead to the B- port
[/quote]

There are 10s BMS with 11 balance leads as well so B0- is the first cable of your balance connector of the first battery (standard on any battery). Your BMS has 10 balance leads and needs no connection of B0- so all good.

Now the bad news, your BMS is NOT for discharge, it would shut off at 40A so it's more a 20A BMS in reality. You could use it for charge only or you need to buy a bigger BMS like 60A (which normally cuts off at about 120A). It is shady to sell a 40A BMS with 40A over current and 40A short circuit protection.
```

---
## \#4 Posted by: Duy Posted at: 2019-04-29T23:51:29.992Z Reads: 48

```
[quote="rich, post:3, topic:92232"]
Your diagram is correct, personally I prefer to connect B5+ of the BMS to B5+ of the battery but it’s the same in the end.
[/quote]

![Wire%20diagram|394x500](upload://uy9gKtUCKAN4xFZnQIPnvjxbHCH.jpeg) 

Thanks alot mate, heres a gift.
Tada! i think...  :slight_smile:  


[quote="rich, post:3, topic:92232"]
Now the bad news, your BMS is NOT for discharge, it would shut off at 40A so it’s more a 20A BMS in reality. You could use it for charge only or you need to buy a bigger BMS like 60A (which normally cuts off at about 120A). It is shady to sell a 40A BMS with 40A over current and 40A short circuit protection.
[/quote]

I created a previous post a few weeks earlier asking if my setup was OK. They replied saying my dual hub motors pull 15a max, in addition esc draws 12a for each motor so probably wont even go over 30a. 
Here are the links to motor and esc which connects to esc incase you like to check:

https://www.banggood.com/Electric-Skateboard-Longboard-Controller-With-Remote-Dual-Motors-ESC-Substitute-p-1202299.html?rmmds=search&amp;cur_warehouse=CN

https://www.banggood.com/24V-42V-550W-70KV-Electric-Longboard-Skateboard-Brushless-90mm-Dual-6364-Hub-Motors-Drive-Kit-p-1186579.html?rmmds=search&cur_warehouse=USA
```

---
## \#5 Posted by: rich Posted at: 2019-04-30T00:49:10.409Z Reads: 37

```
Nice gift :grin:

[quote="Duy, post:4, topic:92232"]
esc draws 12a for each motor so probably wont even go over 30a
[/quote]

Ok that's a different story and you should be alright in this case. Just for safety I would check in the beginning if the BMS gets hot during/after riding but I don't think so.

Just for comparison, this is a "real" 50A BMS (Bestech) which is even bigger than the pic :laughing:

![214337h|666x500](upload://eR2o2gGecBoyhl2HuTC26feLXrf.jpeg) 

I use it on my MTB and draw up to 100A without any problems because the 50A is continious and peak 110-120A.
```

---
## \#6 Posted by: Duy Posted at: 2019-04-30T10:18:54.508Z Reads: 28

```
[quote="rich, post:5, topic:92232"]
Just for safety I would check in the beginning if the BMS gets hot during/after riding but I don’t think so.
[/quote]
 
Yup will definitely do, thanks for the tip man 👍.

And wow! Your BMS looks like a beast 😂. I too, will very likely go for a Bestech BMS whenever I plan to upgrade. They seem to be highly recommended by many people from this forum.
```

---
## \#7 Posted by: pat.speed Posted at: 2019-04-30T12:18:12.933Z Reads: 25

```
Yep bestech or suppower are good brands. 

[quote="rich, post:5, topic:92232"]
![214337h|300x225](https://www.electric-skateboard.builders/uploads/db1493/original/3X/6/8/681d4784c677d7e20104b9a3aad835210d193b8d.jpeg)
[/quote]

It’s so big 😱😉
```

---
## \#8 Posted by: rich Posted at: 2019-04-30T21:14:53.880Z Reads: 19

```
[quote="pat.speed, post:7, topic:92232"]
It’s so big :scream::wink:
[/quote]
:joy:

Not the size only, also had a big hole in my wallet, 2 pieces including shipping and tax was 160€ (180$) :face_with_raised_eyebrow:

It's set to 3V/cell over-discharge protection (highest possible value) for Lipo. I still have a new laying around.
```

---
## \#9 Posted by: pat.speed Posted at: 2019-04-30T21:29:53.524Z Reads: 17

```
That’s actually not too expensive, I’ve seen bestechs 80a going for around $70 each
```

---
