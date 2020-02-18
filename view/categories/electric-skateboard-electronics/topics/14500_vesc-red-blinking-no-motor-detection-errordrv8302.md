# VESC red blinking no motor detection errorDRV8302

### Replies: 13 Views: 1177

## \#1 Posted by: William Posted at: 2016-12-11T10:27:50.244Z Reads: 108

```
I just received my vesc from Enertion a few days ago, and willing to use it i wired everything up but when i connected it to bldc tool, it would recognize my vesc, but it did not detect my motor at all. I am just not able to make it spin, and when i looked into the sampling area it tells me i have a fault code DRV8302 what i don't understand since i did nothing on the vesc to get that error.
Is there any possible way to fix it , i have seen some thread saying that this error means my vesc is dead.
Thank you for your help !
i am using 8s battery and an enertion motor, firmware version of my vesc 2.18
```

---
## \#2 Posted by: Blasto Posted at: 2016-12-11T16:23:54.093Z Reads: 92

```
Post pictures of your setup and settings of the bldc tool
```

---
## \#3 Posted by: William Posted at: 2016-12-11T19:42:23.286Z Reads: 86

```
of course sorry not to have done it before, here it is, i'm using a 4s battery
Thank <img src="/uploads/db1493/original/3X/a/5/a538135b219aace4d1ab9d23265568eb00b522f4.jpg" width="674" height="500">you for <img src="/uploads/db1493/original/3X/5/e/5eb91d5106bb88d3fd2d3b81e17f28488a61525a.jpg" width="674" height="500">your answer <img src="/uploads/db1493/original/3X/7/e/7edc5644cd75ce4f3b031c20860cee07c2af9863.jpg" width="674" height="500"><img src="/uploads/db1493/original/3X/1/8/181e367845a0e187fc4da54a81a93dd723ce4fd2.jpg" width="370" height="500"><img src="/uploads/db1493/original/3X/c/a/ca3546aedb7d0548d9e8b1fa1ed0f38d2174403a.jpg" width="370" height="500"><img src="/uploads/db1493/original/3X/5/4/54504c6cc412673891ac939afd6804b9a7573ca5.jpg" width="674" height="500">
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-12-11T19:59:15.726Z Reads: 75

```
Cover those motor lead.... , if they touch each other you will burn the drv....

Also, cutoff start should be higher (13) than cutoff end (12)
```

---
## \#5 Posted by: William Posted at: 2016-12-11T20:18:00.600Z Reads: 74

```
I covered the motor connectors and i also changed the values of the the cutoff as you said, i'm sorry but i really am new to the vesc and i should have taken more attention to what i did. <img src="/uploads/db1493/original/3X/d/5/d5cec50df48cca8151cf3087fc7f8b862984c87a.jpg" width="674" height="500">
```

---
## \#6 Posted by: William Posted at: 2016-12-11T20:25:08.655Z Reads: 72

```
i think the connectors of the motor touched and i fried the chip is their any way to repair it ?
```

---
## \#7 Posted by: Blasto Posted at: 2016-12-11T20:26:40.091Z Reads: 72

```
[quote="William, post:6, topic:14500, full:true"]
i think the connectors of the motor touched and i fried the chip is their any way to repair it ?
[/quote]

Need to replace the drv chip
```

---
## \#8 Posted by: William Posted at: 2016-12-11T20:44:55.347Z Reads: 70

```
Thank you for answering that quick but giving the size of the chip i think i will not be able to replace it.
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2016-12-12T01:25:21.458Z Reads: 64

```
Sorry for the late respond, but if you live In north America, I have a small VESC repair program. 

http://www.electric-skateboard.builders/t/johnny-vesc-repair-services/11267?u=johnnymeduse
```

---
## \#10 Posted by: William Posted at: 2016-12-12T06:47:35.355Z Reads: 56

```
thank you for your help but unfortunately I live in France. However, do you think that if I found the right chip it would be possible to change it using soldering iron ?
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2016-12-12T13:43:56.373Z Reads: 49

```
No you need a hot air station... Have you try to contact Enertion Support, also I think there someone in europe who does repair, just don't remember who :sweat_smile:.
```

---
## \#12 Posted by: flatsp0t Posted at: 2016-12-12T19:27:34.311Z Reads: 38

```
You can ask xlv on Vedders Forum, he is from Germany, and his service is good and fast:
http://vedder.se/forums/viewtopic.php?t=186

His Website:
http://www.lp-electronic.com/vesc-repair-service/
```

---
## \#13 Posted by: William Posted at: 2016-12-15T17:20:06.787Z Reads: 25

```
Sorry for answering that late and thank you very much for your answers, i think i'll have it repair !
```

---
