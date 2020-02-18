# Battery changes Volts dramatically while not charging

### Replies: 7 Views: 199

## \#1 Posted by: Tomer Posted at: 2018-10-09T20:25:34.897Z Reads: 61

```
I built to a friend of mine an electric skateboard with 10S3P battery pack using genuine Samsung 25R cells. 
The BMS is a Bestech HCX-D131 model. My friend told me he noticed a really odd behavior recently.

He uses the eSkate VESC iOS app to see what is the voltage of the battery. 
Usually, the app shows about 42V when battery is fully charged. However, in the last couple of days, 
it shows around 37V. When the battery is being charged, it reachs back to 42V, but when you disconnect the charger, guess what? **It goes back to 37V**! 

Here is a video to see this "phenomena" -
https://www.youtube.com/watch?v=oE28ZIECETA
(You can hear the battery is being charged from the fan inside the charger).

I measured the voltage of the battery directly, without the BMS, and it shows 40V. It's still not 42V, but I
can live with that. I'm assuming the BMS is not letting it reach its max capacity. Something is wrong here. 

This board is up and running for the last 5 months with no any battery issues.
Does anyone have any idea what the hell is going on?
```

---
## \#2 Posted by: Fiori Posted at: 2018-10-09T20:33:46.193Z Reads: 53

```
Seems like one of your P groups is going bad. Check voltage of each group when it is fully charged
```

---
## \#3 Posted by: Tomer Posted at: 2018-10-09T21:08:47.600Z Reads: 50

```
I've checked the voltage of each P group (on the BMS connectors) all are 4 volts, so, to my opinion, no group is bad. The battery pack shows 40v after green LED lighted on the charger, via a multi meter. Can't get it to 42 volts.
```

---
## \#4 Posted by: Tomer Posted at: 2018-10-10T11:33:25.919Z Reads: 33

```
Any more suggestions?
```

---
## \#5 Posted by: Trdolan03 Posted at: 2018-10-10T14:37:58.282Z Reads: 25

```
Inverse of voltage sag. How many amp charger is it?
```

---
## \#6 Posted by: Jumpman Posted at: 2018-10-10T15:33:01.361Z Reads: 23

```
It’s normal for batteries not to keep maximum voltage once off the charger, especially if they are old or damaged, but it does seem a bit extreme in this case.  

You’ve also got to consider voltage drop, so maybe worth checking all connections.
```

---
## \#7 Posted by: Fiori Posted at: 2018-10-10T15:44:35.644Z Reads: 21

```
One of them has to be the issue. Charge to full, ride it a few miles and then re-check. See if any of the groups drop voltage faster than the others. Otherwise you will have to cut the heat shrink and look, you may have a bad weld or something too.
```

---
