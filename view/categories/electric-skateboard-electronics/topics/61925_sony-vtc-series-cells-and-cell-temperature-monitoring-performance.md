# Sony VTC series cells and cell temperature monitoring/performance

### Replies: 10 Views: 177

## \#1 Posted by: D_Sk8 Posted at: 2018-07-15T16:32:35.308Z Reads: 80

```
I noticed there are some cells that will provide 30a output at/under 80c and a safe output of 15a over that.

Couple questions that come to mind with this.

1. Taking Sony VTC6 for example. Do the cells auto-protect? They are unprotected cells, so I would guess no, which would suggest you would need to monitor the temperature and modify the amount power you pull from them at higher temps. 

2. VESC's mobile app seems to monitor VESC temp. Is anyone monitoring cell temps? (If so,  how?). I am basically trying to determine if it's realistic to pull 30a from the cells at any moment, even if it's just to get up to speed, or if standard operating temps of a cell would be close to 80c. (I wouldn't think so, that seems pretty damn hot).
```

---
## \#2 Posted by: visnu777 Posted at: 2018-07-15T16:41:56.414Z Reads: 76

```
Interesting question, I will try it out when I'm finished. I built a 10s3p battery made of VTC6 cells recently for my new build and I plan to integrate an ESP32 microcontroller in the deck which will do stuff like that and trigger an alarm etc.
```

---
## \#3 Posted by: Pedrodemio Posted at: 2018-07-15T16:42:11.341Z Reads: 71

```
1- no, you have to implement this limits

2- if you are not measuring motor temperature, you could use that with a thermistor on the cells 

But even if they allow you to get them up to 80C, they will have a pretty short life
```

---
## \#4 Posted by: D_Sk8 Posted at: 2018-07-15T16:43:31.752Z Reads: 65

```
Ohh, that sounds pretty cool. If you can remember, please keep us updated. That sounds like a great idea.
```

---
## \#5 Posted by: D_Sk8 Posted at: 2018-07-15T16:45:53.383Z Reads: 64

```
Interesting, so instead of monitoring the motor I can basically manipulate the controller to report cell temp. Great idea. I mean, even if it's temporary, I could fly up a couple hills and see how hot they get.

Thanks for the tip.
```

---
## \#6 Posted by: Pedrodemio Posted at: 2018-07-15T17:20:24.709Z Reads: 57

```
What's your setup? Unless you are running with only 1P, I doubt it will get this hot for the average riders, but do it to see what happens, you can use any data logging app to record cell temperature during the ride
```

---
## \#7 Posted by: Erniechan Posted at: 2018-07-15T19:04:43.869Z Reads: 50

```
Those cells only reach 80° for vapers. 
You can count on 30 amps.
```

---
## \#8 Posted by: D_Sk8 Posted at: 2018-07-15T21:21:40.353Z Reads: 42

```
Putting together some specs. Was thinking 10s2p dual 5045 motors on a smaller board. I have a ton of A123 26650 cells for longboards but trying to figure the best cells on a smaller build.
```

---
## \#9 Posted by: D_Sk8 Posted at: 2018-07-15T21:21:54.139Z Reads: 42

```
Gotcha, cool. Thank you.
```

---
## \#10 Posted by: Pedrodemio Posted at: 2018-07-16T04:13:43.512Z Reads: 30

```
Unless you are climbing a very steep hill for the full battery charge you won’t have to worry about battery overheating with this setup. We draw max power for a few seconds while accelerating and then settle at something between 300 and 600 W
```

---
