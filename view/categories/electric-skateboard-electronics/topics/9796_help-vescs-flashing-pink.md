# HELP VESCs Flashing pink

### Replies: 10 Views: 823

## \#1 Posted by: Spek Posted at: 2016-09-18T16:39:34.456Z Reads: 59

```
Please help. I turned on my board this morning and the remote wasn't responding. Opened it up and my vesc are flashing pink. I can't seem to find the button in BLDC to detect errors. It was working last night and all I did was open it up after a ride and repositioned the vescs a little bit. Nothing appears to be off. Its connecting to BLDC fine. AH!
```

---
## \#2 Posted by: ra.rend Posted at: 2016-09-18T16:40:41.280Z Reads: 59

```
Is it fully charged?
```

---
## \#3 Posted by: Spek Posted at: 2016-09-18T16:43:09.077Z Reads: 55

```
Yea charged over night
```

---
## \#4 Posted by: Spek Posted at: 2016-09-18T16:46:00.873Z Reads: 55

```
Oh I see a fault code in the real time data that says OVER_VOLTAGE. Is my fully charged battery exceeding my maximum voltage setting?
```

---
## \#5 Posted by: Spek Posted at: 2016-09-18T16:48:42.394Z Reads: 53

```
Okay, I set the battery max voltage from 42v to 43v (running 10s). That stopped blinking on one. Can I push the change to the second VESC via canbus or do i have to connect it individually and write settings?
```

---
## \#6 Posted by: Spek Posted at: 2016-09-18T16:54:07.935Z Reads: 50

```
Lol thanks @ra.rend you saved the day with your simple sentence. Im running!
```

---
## \#7 Posted by: flatsp0t Posted at: 2016-09-18T16:59:30.446Z Reads: 49

```
Leave the max input voltage at the default 57V, it is just to protect the components from more voltage as they can handle.
```

---
## \#8 Posted by: ra.rend Posted at: 2016-09-18T17:10:59.419Z Reads: 43

```
Your welcome :) I don't have dual vesc via canvas, but you should be able to.
```

---
## \#9 Posted by: Spek Posted at: 2016-09-18T17:55:31.785Z Reads: 39

```
I just did each one individually. If someone could comment on that it'd much appreciated. Stopped to give my feet a rest. I have to also remember poor Braking on a full charge :/ 

It's running great! Heat seems to be a non issue
```

---
## \#10 Posted by: flatsp0t Posted at: 2016-09-18T18:28:51.643Z Reads: 33

```
yes, you can. in the connection tab (left side of the window) select CAN FWD and fill in the id of your slave vesc(Propably 1).
<img src="/uploads/db1493/original/3X/e/5/e59ddfa4f8c73b55f3844df3b87bd0940b83736f.png" width="153" height="500">
```

---
