# Help! VESC broken?

### Replies: 9 Views: 204

## \#1 Posted by: Liam Posted at: 2019-07-26T17:27:02.825Z Reads: 64

```
![image|375x500](upload://6NMnXOcUD9hDav8QbHAeSTCDOvt.jpeg) 

Hi, I think I may have broken my VESC or some part of my setup. I had been trying to build my esk8 and i had some problems while programming the VESC. Now when I plug my battery into the VESC the battery shuts off and it will only turn back on if I plug it into the charger. Does this sound like a problem with the VESC or something else? Thanks
```

---
## \#2 Posted by: gee Posted at: 2019-07-27T04:16:46.058Z Reads: 58

```
I don't really understand how a battery can shut of. Like it turns the VESC on then off? 

Need more info. Even better a video.
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-07-27T04:44:05.524Z Reads: 56

```
bms probably died.

@torqueboards
```

---
## \#4 Posted by: Liam Posted at: 2019-07-27T16:12:20.585Z Reads: 43

```
https://vimeo.com/350490070

Here you go, hopefully this helps.
```

---
## \#5 Posted by: gee Posted at: 2019-07-28T00:39:42.623Z Reads: 32

```
Did you turn on the remote and see if the motor runs? Maybe get a multi-meter and check the voltage and current? 
My best guess would be the bms also. I'm guessing you have to take the battery apart. If there's voltage and current it should power the vesc.
```

---
## \#6 Posted by: Darkie02 Posted at: 2019-07-28T03:12:45.781Z Reads: 29

```
I’d start with the battry that looks as tho the BMS is cutting the Battery voltage out put as if it’s too low and the meter is miss calibrated when charger is plugged in temporary increases voltage over threshold.

Solution
Manually check the output voltage with a multimeter. 

If that’s ok then check each p group voltage with a multimeter that it’s not over discharged a p group. If that’s the case it could be any thing from bad cell to bad charger.
```

---
## \#7 Posted by: GoofyRider89 Posted at: 2019-07-28T04:54:55.002Z Reads: 30

```
Can confirm, this happened to my last 10s3p 30q pack. Was using a laptop style charger. Would only turn on with the charger on, measured the voltage and got 25v or somewhere around there. Started testing the cells individually and found 3 cells were low.
```

---
## \#8 Posted by: torqueboards Posted at: 2019-07-29T01:13:56.463Z Reads: 18

```
@Liam Please email our support email that way we can take a look at this.
```

---
## \#9 Posted by: Liam Posted at: 2019-08-01T20:54:15.014Z Reads: 14

```
Update: checked battery with a multimeter and it seems fine, but once plugged back into the Vesc it won’t turn on by itself.  ![image|375x500](upload://vGQhhKqnJu92m12h2EuVXuTWSey.jpeg)
```

---
