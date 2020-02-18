# VESC 4.12 DRV error but still works

### Replies: 9 Views: 392

## \#1 Posted by: Kevins Posted at: 2018-09-28T07:49:13.419Z Reads: 113

```
Yesterday, I started getting DRV8302 errors on my TB VESC 4.12 after riding the board without issues for more than 600km. This would happen most of the time as soon as I pulled the throttle on startup, but sometimes it worked fine without giving any errors. As soon as the board started rolling, I could pull the throttle without any errors at all and it would work perfectly.

When I got home, I connected the VESC to the VESC tool to see if anything was wrong with the settings. After that, it stopped working completely and the VESC would only make a high pitched noise whenever I pulled the throttle (https://www.youtube.com/watch?v=kya4sDUbt1U).

I then decided to swap around the master and slave VESC (dual setup), and it seems that the VESC causing the issues was the master VESC (now the slave VESC). The other VESC works fine. After swapping them around, both of the motors are spinning again. However, upon startup the bad VESC seems to lag behind a little bit (good VESC starts spinning immediately upon pulling the throttle, other one takes a second or two and then immediately spins at full power). There have been no more DRV errors after swapping around the VESCs.

There are no visible signs of damage on the DRV chip or anywhere else on the bad VESC. When the board is moving, both VESCs work perfectly. The only time issues arrive is during startup. Sometimes it feels like the bad VESC completely cuts out during startup, and then starts working again once the other VESC has the board moving. 

My board has the following specs:
Trampa 35º holypro deck 15ply, ratchet bindings, vertigo trucks, superstar wheels
8S 25Ah 20C lipo, 740Wh (10x 4S 5000mAh zippy flightmax)
dual TB VESC 4.12 (running in FOC mode)
dual turnigy aerodrive SK3 6364 245Kv motors
metr pro bluetooth module

Gearing ratio 13:72. The top speed of the board is around 45km/h. I usually ride close to the top speed, and this gives me a range of around 35km (I charge the lipos to 4.15V and stop discharging at around 10% to increase their cycle life).

Is there anything else that could be wrong with the VESC besides the DRV chip? I know running in FOC mode increases the risk of the DRV chip frying, but it seems weird that the VESC still works normally when the board is ![image|443x500](upload://uLTvOPHiqfufrGjlLyj5okbbxMe.jpeg)
```

---
## \#2 Posted by: dareno Posted at: 2018-09-28T12:58:58.508Z Reads: 92

```
[quote="Kevins, post:1, topic:69443"]
However, upon startup the bad VESC seems to lag behind a little bit (good VESC starts spinning immediately upon pulling the throttle, other one takes a second or two and
[/quote]

this is normal.  they can have a delay between starts.  Have you re done the motor detection for both vesc since the swap?

[quote="Kevins, post:1, topic:69443"]
The only time issues arrive is during startup. Sometimes it feels like the bad VESC completely cuts out during startup, and then starts working again once the other VESC has the board moving.
[/quote]
How do you know that?  does it stutter on start up?  Very difficult nay impossible to tell which vesc is playing up.
```

---
## \#3 Posted by: Kevins Posted at: 2018-09-28T17:46:24.059Z Reads: 80

```
I attempted to redo the motor detection, but on the bad VESC the VESC tool gave some sort of error and it wouldn't do the detection. On the other VESC the detection worked fine. 

Sometimes when I accelerate on startup, the torque is very low in the beginning as if only one of the motors is working and  then after the board starts moving the torque suddenly increases a lot. I think this is because one of the VESCs shuts down due to an error and then reboots itself, which takes a few seconds.

When spinning the wheels freely, the motor that's driven by the bad VESC sometimes refuses to spin or even slowly spins in the opposite direction. I also get the red blinking light on the VESC indicating that there is an erorr and it reboots the VESC. Other times it seems to spin perfectly just like the good VESC. I made a short video to clear things up a bit: https://www.youtube.com/watch?v=300gQaQ_f1c
```

---
## \#4 Posted by: Florida Posted at: 2019-05-12T21:28:36.026Z Reads: 51

```
I have the same error with my vesc, but with 12s it works even worse than with 8s. Gonna buy a new one, but still curious why it didnt work. I have tried motor currents from 30 to 90 amp and even swapped the caps for some high quality Panasonic ones.
```

---
## \#5 Posted by: Kevins Posted at: 2019-05-14T17:38:37.640Z Reads: 49

```
It turned out to be a bad DRV chip. Running FOC at 8S (any voltage really) on the VESC 4.12's is a bad idea. I ended up frying both of my VESCs DRV chips and then replaced them with a dual FSESC 6.6 from Flipsky which is based on the VESC6 so it handles FOC very well. I haven't had any problems since.
```

---
## \#6 Posted by: Florida Posted at: 2019-05-19T13:29:07.595Z Reads: 39

```
I honsetly dont know what really caused my problem because I really abused the VESC, but i opted for a Kelly controller which runs FOC and has a claimed efficiency of 99% and can reach Phase amps of 200 Amp
```

---
## \#7 Posted by: seaborder Posted at: 2019-05-19T13:56:03.685Z Reads: 33

```
You can send the focbox to many people here in the forum they can repair it for you, I can do too.

Greets! :)
```

---
## \#8 Posted by: Kevins Posted at: 2019-05-20T20:41:01.734Z Reads: 24

```
How much would it cost to repair two vescs? 

I tried to repair them myself first by replacing the DRV chip, but I think I may have caused a short somewhere because on one vesc the copper trace leading up to the mosfet evaporated when I connected it, and the other vesc only works at low power and then gives overcurrent errors when I push it harder.. I repaired the copper trace with some solder, but still no luck. So I'm not sure what the exact issue with the vescs is at this point. 

They have been laying around for about half a year now, since I got my new flipsky vesc. I wouldn't mind sending them to you or someone else on the forum (preferably in or close to the Netherlands), just to see if they're still fixable and shipping + repair costs aren't too expensive. Let me know what you think :wink:
```

---
## \#9 Posted by: seaborder Posted at: 2019-05-20T20:52:40.918Z Reads: 22

```
@Martinsp ✌️✌️
```

---
