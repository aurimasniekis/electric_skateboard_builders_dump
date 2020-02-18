# Nano (winning) V2 Stopped working

### Replies: 13 Views: 718

## \#1 Posted by: MrHappy Posted at: 2017-09-22T05:14:40.610Z Reads: 86

```
My board was in the shop for a while i was getting a new battery. I finally got everything setup again, but the nano v2 isnt giving any ppm signal to the vesc. It is paring fine, and my old gt2b remote works fine. Any advice?
```

---
## \#2 Posted by: Jinra Posted at: 2017-09-22T05:16:22.293Z Reads: 86

```
open it up and check the potentiometer cables, maybe a broken solder joint
```

---
## \#3 Posted by: MrHappy Posted at: 2017-09-22T05:19:11.664Z Reads: 86

```
Nope, wasn't that. ill upload a pic of the pcb in a sec.
```

---
## \#4 Posted by: MrHappy Posted at: 2017-09-22T05:22:39.160Z Reads: 83

```
<img src="/uploads/db1493/original/3X/9/0/909afebfe43c0343d34bddc648681d097e574438.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/d/0d9e6f77fde6e05f1019d894cb74628387db202e.jpg" width="666" height="500">
```

---
## \#5 Posted by: Jinra Posted at: 2017-09-22T05:28:37.085Z Reads: 80

```
You're using the middle set of pins right?
```

---
## \#6 Posted by: MrHappy Posted at: 2017-09-22T05:30:18.796Z Reads: 79

```
Yup. (10chars)
```

---
## \#7 Posted by: MrHappy Posted at: 2017-09-22T05:32:26.490Z Reads: 79

```
I just found this: https://www.electric-skateboard.builders/t/what-could-be-the-problem-winning-remote-stopped-working/8122/3
I know its on the last gen of winning remote, but maybe its the same fix?
```

---
## \#8 Posted by: Blasto Posted at: 2017-09-22T05:35:22.746Z Reads: 79

```
Edit bad info

Good info

<img src="/uploads/db1493/original/3X/5/1/51a547e70d5887ddc690341cd8f60ccdb74a033f.PNG" width="374" height="500">
```

---
## \#9 Posted by: Jinra Posted at: 2017-09-22T05:37:11.038Z Reads: 76

```
First set of pins only provides power, middle set is CH1, bottom is CH2
```

---
## \#10 Posted by: MrHappy Posted at: 2017-09-22T05:41:37.200Z Reads: 75

```
I wish i had my ohmmeter on me to check the potentiometer output. Ill do that tomorrow hopefully.
```

---
## \#11 Posted by: MrHappy Posted at: 2017-10-03T01:22:01.526Z Reads: 53

```
So the remote worked fine with one of the enertion nano recievers, it paired in an instant. Does anyone know of a place i can buy one of the nano recievers? or any of you have a spare lying around?
```

---
## \#12 Posted by: Dizzee Posted at: 2017-10-31T10:34:58.720Z Reads: 44

```
I know this is an old thread but I thought it might be helpful to add that the HobbyKing GT-2 2.4Ghz Receiver 3Ch that was listed in [this](https://www.electric-skateboard.builders/t/what-could-be-the-problem-winning-remote-stopped-working/8122/3) thread as working with the Winning uses the old AFHDS FlySky protocol. Since the Winning receivers work with the Nano V2 remotes the GT-2 and all AFHDS receivers should work with the Winning, Nano V2 and Enertion remotes. This is not the same as the FlySky's newer  AFHDS 2A protocol so be sure to stay away from the GT-2E and others that use AFHDS 2A.
```

---
## \#13 Posted by: MrHappy Posted at: 2017-10-31T14:55:24.093Z Reads: 39

```
The receiver they are selling pairs with the new gt2b's. I bought one, and it did not pair with the nanos.
```

---
