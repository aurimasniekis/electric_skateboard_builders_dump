# That Escalated Quickly &#124; Ehler DH &#124; dual SK3 6864 190kv &#124; 12s4p &#124; Ollin VESC &#124; Torqueboards mount/gears (18/36)&#124; GT2B MadMonkey &#124; 97mm clones

### Replies: 9 Views: 1722

## \#1 Posted by: ROFEN13 Posted at: 2017-10-26T21:47:42.201Z Reads: 313

```
Soooooo my wife got me a Lectric board for fathers day. It was $300, and perfect for an entry board. The issue is that it left me wanting more. So i decided to buy a VESC to modify the Lectric board. The issue was that as I started researching, I realized that the 6s battery and (MAYBE) a 260kv motor was not the best option for the VESC. The parts started to be ordered like dominos. I realized that a lower KV motor would be better and a larger battery would then be needed. And I may as well buy new trucks since the Lectirc trucks sucked.... and so on. 

**Deck:** Ehler Switch Ninja
**Trucks:** Caliber II 44
**Wheels:** ABEC Flywheel 90mm (I had these on a long distance push board I had)
**Motor mount/Gears**: Touqueboards 16/32t
**Motor:** SK3 6364 190KV
**VESC**: Ollin
**Battery:** Samsung 25R 12S4P (I built this as 2 6S4P. They are charged using a hobby charger in parallel  but the Loop key connects the batteries in series)
**Enclosure:** KYDEX enclosure (I know my molding skills suck)
**Remote:** Hobby King GT2B modded using Mad Monkey Controller

I got my inspiration for this build from [Dunkirk](http://www.electric-skateboard.builders/u/Dunkirk)'s [Vanguard Orange](http://www.electric-skateboard.builders/t/vanguard-orange-10s-sk3-i-vesc/1337). I wanted to build the best board I could afford but try to limit cost by not using a BMS since I already had a hobby charger.

I haven't fully tested the board with range and speed but just a short test at a half depleted battery reached top speed of 27. 

I also heated the PID on the remote too much while soldering and am using the steering one so my break is weak. I still need to add a battery monitor, I shorted the 2 I bought already (stupid mistake) and plan on hooking them up to each battery. Here are some pictures!
<img src="/uploads/db1493/original/3X/2/b/2bc1e645224330ed3e232befc68302d459b30072.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/1/c/1c79935f00b45623141aa5b65c8a322f1b1cbb66.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/1/0/10e53545a994f2f6986485cbf8ff98f513e81665.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/6/168400761a45bfa65b99c8fec692e9b56c9e4237.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/0/0014df8a0d5e54302d78fe0c63b3940ed570d3f6.jpg" width="374" height="500">
```

---
## \#2 Posted by: ROFEN13 Posted at: 2018-01-15T18:24:37.916Z Reads: 218

```
So after completing the build, I kept wanting more. More speed, faster acceleration...
After changing the settings on my VESC and upgrading to 97mm wheels, I was able to get a top speed of 29. BUT, I still wanted more. That's where the dual started. 
![20180115_125537|281x500](upload://dGQmRUiVohHc0EnE3f6H8PKQ6Fr.jpg)
I also have 18t motor pulleys on the way.
I will be running split ppm on the VESCs.
I also have some small bike lights on the trucks just for visibility. ![IMG_20180115_132017|500x500](upload://kjK7sLr6cDpNxNMD3gLit6GnMXz.jpg)
With my enclosure, I decided to print the xt90 housings to run my motor wires through. 
![20180115_125552|690x388](upload://ujrJrc9ampZVNcuyAdmJH1ziglq.jpg)
I am hoping to get close to 35 out of this (I'm a little over 200lbs So that really effects my efficiency).

I do have one question for anyone out there, can I run a battery monitor led from the extra 5v on the second vesc?
```

---
## \#3 Posted by: E1Allen Posted at: 2018-01-15T19:38:53.650Z Reads: 192

```
[quote="ROFEN13, post:2, topic:36603"]
I do have one question for anyone out there, can I run a battery monitor led from the extra 5v on the second vesc?
[/quote]

It's just 5v 1a output so whatever works at ~5v

Your max speed on 16/32 should already be over 35mph.  Something seems off.  

I think your PPM settings are off. Since you are using the wheel and your brakes suck.  It's like your not getting 100%.

![IMG_3947|374x500](upload://tV56aKG7rXNJ3mdZuEYWezH0jhR.JPG)![IMG_3948|374x500](upload://8K69myhpz90rzTFRVfdDRhFQOLz.JPG)![IMG_3949|374x500](upload://bICeFW7wUCPsbelg7kxehDvI9dD.JPG)

Disable your motor first. Then with the controller go full brake and read the number then full forward.  Read the numbers in the bottom right and those are your controller min and Max pulsewidth which can be different from one remote to another. Enter those numbers in their respective locations. Enable your motor then try again.  Do it for both motors separately.  Save settings👍👍
```

---
## \#4 Posted by: ROFEN13 Posted at: 2018-01-15T20:16:04.406Z Reads: 159

```
I used the ackmaniac bldg tool to do my ppm settings (it's automatic). So I know it is centered and works. I did get another controller so I am actually using the throttle PID now. My efficiency is about 70% in the speed calc to give me my current top speed (29mph). Based on my weight and only a single motor, 70% efficiency didn't seem unreasonable.

P.S. -When I last tested, it was only 30 F outside....
```

---
## \#5 Posted by: Youssless Posted at: 2018-01-15T20:41:53.096Z Reads: 157

```
Welcome to DIY! Where your board always needs that little bit more lol :smile:
```

---
## \#7 Posted by: ROFEN13 Posted at: 2018-02-04T21:26:23.346Z Reads: 140

```
UPDATE!
So with the second VESC,  i am now out of space. I decided to make a fiberglass enclosure to fit everything and make it prettier :slight_smile:
I had to seal up the holes from the t nuts I used. 
![20180204_161751|690x388](upload://cCtCWW2jObre1wT4OgkQtVPdemX.jpg)
I used titebond 3 and dowels to fix it. When I removed the grip I noticed some splitting by the bold holes for the trucks. Is this normal? Should I fiberglass over the deck for strength?
![20180204_161801|690x388](upload://pxXMqlyRaRuYBRp8sbVhmffTt2g.jpg)
Here is the design for my new enclosure. 
![20180121_104502|690x388](upload://fPvM8F2NhAVKUqzs0PDriJI39zR.jpg)
```

---
## \#8 Posted by: ROFEN13 Posted at: 2018-03-30T21:12:23.031Z Reads: 109

```
Finally done! Still no bms, but I used a VGA port to run the balance leads. Fiberglass was not the easiest to work with, and the rubberized car undercoating is not sticking for some reason. But I can finally ride it again!
![20180330_170218|374x500](upload://hUEJHwf7c92X9HcBIYb1PmyPCEW.jpg)![20180330_170153|666x500](upload://2JtNvXB8RPZblmsfOX2VAG0hdsT.jpg)![20180330_170125|666x500](upload://wQVkNCnWDAic2FyAmRPDnCaqmEm.jpg)
```

---
## \#9 Posted by: ROFEN13 Posted at: 2018-04-01T00:50:07.482Z Reads: 92

```
Here is a picture of charging. I have seen many posts of people not wanting to use a bms because they already had a hobby charger, and I was in the same boat. 
![20180331_204536|374x500](upload://4tB6x6iB2gfY1jyrnXTOAnqgKy8.jpg)
```

---
## \#10 Posted by: ROFEN13 Posted at: 2018-05-25T02:32:05.114Z Reads: 62

```
Wow, I have been riding this a bunch and it is a blast. The bummer is that I dont have a lot of open stretches in the city. BUT I was able to get one tonight when I hit all the lights right on new pavement!!!! :smiley: the best part is that I still had room left on the top end. 
![Screenshot_20180524-210506_Strava|243x500](upload://2RMMxL2bsOp3NGDwqHmF2eul14d.jpg)
```

---
