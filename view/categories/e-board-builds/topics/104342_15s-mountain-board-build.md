# 15S Mountain board build

### Replies: 12 Views: 293

## \#1 Posted by: thatguy614 Posted at: 2019-11-28T15:33:26.055Z Reads: 104

```
Hey guys, 
I am in the middle of my first mountain board build. I have already built a board that runs on a vescx and a 13s3p pack. The mountain board is going to be a dual motor build running 6355s. I want to see if I can use dewalt 60v battery packs for this build but the issue that I am running into is all the vesc's I can find have a 60v limit and the dewalt packs are actually 15s meaning they push 63v when fully charged. Is there a way to limit the power some so I don't fry another makerX dual vesc? (I was doing initial setup with the vesctool wizard and the dang thing caught fire). I understand that I may have been a little careless which is why I am starting this thread. I want to see any and all recommendations yall might have to make this build work. ![IMG_1242|375x500](upload://2Z6yCHLmJCfBJITLuvn7eXwMcUH.jpeg) ![IMG_1241|375x500](upload://fe1wp9Kgf0XN6DgjfHY6ONOUikd.jpeg)
```

---
## \#2 Posted by: Benjo Posted at: 2019-11-28T16:24:01.040Z Reads: 99

```
I think 13s is already too high. There is a reason why the VESCs are rated for 12s. The DRV and other components are voltage sensitive and max out at 60v according to datasheet. If you use regenerative braking you will come very close to that already when running 12s. With 13s or more the esc will fail sooner or later. No way to limit the voltage other than removing series cells.
```

---
## \#3 Posted by: thatguy614 Posted at: 2019-11-28T17:29:37.442Z Reads: 94

```
So theres no BMS or anything that might be able to limit the battery output that reaches the vesc? I still use the dewalt packs for tools so im not about to open them up and running them on 20v is just too low for a mountain board set up
```

---
## \#4 Posted by: Benjo Posted at: 2019-11-28T17:43:16.414Z Reads: 90

```
That's not what a BMS does. I am not aware of any way to reduce voltage apart from a regulator. A regulator capable of 80A or more would be pretty beefy. Also most only output a fixed, commonly used voltage like 12 or 24v.
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-11-28T18:41:15.842Z Reads: 83

```
13s is fine for vesc's built with good components, ex, focbox, focbox unity, vesc 6, fsesc 6.6's
```

---
## \#6 Posted by: thatguy614 Posted at: 2019-11-28T22:12:41.225Z Reads: 75

```
I would like to note that my batteries were at about 2/3 charge so the actual voltage is at about 55v so the burn out of the vesc might have been for some other reason.
```

---
## \#7 Posted by: thatguy614 Posted at: 2019-11-28T22:14:46.625Z Reads: 73

```
I was reccomended a buck converter which can have a variable range for voltage reduction, however I haven't been able to find one that can do more than 12A. I know Vedder just came out with the 75/300vesc but im not trying to drop $550 for a replacement vesc right now
```

---
## \#8 Posted by: Chricious Posted at: 2019-11-28T22:38:32.748Z Reads: 68

```
Hey Aaron, nice project!

There are a couple ESCs besides Trampa and Maker X which are more affordable and capable of 15S+ like TTF http://teamtriforceuk.com/a200s-v2-2/ or if the upcoming Neo ESC ( up to20S).

But I would strongly recommande you to go 12S with 6384. You will be able to get more power out of your board.

Have fun and enjoy your build
```

---
## \#9 Posted by: thatguy614 Posted at: 2019-11-29T13:09:46.616Z Reads: 54

```
Thanks! With the Vesc you jsut posted do you have to run 3 motors or would it work with a 2 motor setup?
```

---
## \#10 Posted by: thatguy614 Posted at: 2019-11-29T13:17:49.621Z Reads: 55

```
A thought jsut occured, i could potentially connect the flexvolt batteries in series and run them at 20v so total it would be a 10s. You can see in the picture below how I could simply remove the center wire to run at 20v How do y’all think that’s would run? I love in the mountains so more than anything I want torque out of this board and maybe 20-25mph

![image|374x500](upload://nkbmqJk5mzjbEzCKxJ3PtYYJ0Sm.jpeg)
```

---
## \#11 Posted by: Chricious Posted at: 2019-11-29T13:24:15.296Z Reads: 49

```
It's 1 ESC per motor.
```

---
## \#12 Posted by: linsus Posted at: 2019-11-29T14:13:17.405Z Reads: 47

```
[quote="thatguy614, post:10, topic:104342"]
A thought jsut occured, i could potentially connect the flexvolt batteries in series and run them at 20v so total it would be a 10s. You can see in the picture below how I could simply remove the center wire to run at 20v How do y’all think that’s would run? I love in the mountains so more than anything I want torque out of this board and maybe 20-25mph
[/quote]

if that loop in the middle is the only series connector then I see no problem with it. Should work fine. Also. the 75/300 VESC will outlive you. Wouldn't call it a "replacement". Will be using it in one of my projects in spring :)
```

---
