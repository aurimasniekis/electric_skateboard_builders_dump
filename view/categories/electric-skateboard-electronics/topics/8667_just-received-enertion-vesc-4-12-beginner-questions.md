# Just received Enertion VESC 4.12, beginner questions!

### Replies: 17 Views: 1928

## \#1 Posted by: jct1212 Posted at: 2016-08-31T01:19:57.120Z Reads: 171

```
Hi,

I just received my enertion VESC and I have some beginner questions that I couldn't fine the answers to.

1. Do I just plug my battery into the XT60 connector on my VESC? It seems that the red and black cables are connected to the opposite side rather than near the XT60, is this ok? Is the electricity transferred through the top small board where the XT60 is located? 

2. When connecting my GT2B receiver, do I need to disassemble the receiver plastic case and then solder the wires to the VESC?

Thanks in advance everyone, I really do not know much about the VESC.

Here are some pictures: <img src="/uploads/db1493/original/2X/1/143319b3d26001acfb9eacfe472eac8cd7ba0401.JPG" width="375" height="500">

<img src="/uploads/db1493/original/2X/4/4122d663175167d1d7a11605188d34fe3229bddb.JPG" width="375" height="500">

<img src="/uploads/db1493/original/2X/d/dcefa685f65a0983774fadf6ab0853fcbd8b5529.JPG" width="375" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-31T01:23:05.261Z Reads: 162

```
1. your assumption is correct. Current should pass through the board to the VESC.

2. normally you'd connect the receiver via a servo cable. However... it looks like the factory forgot to attach pins to the board.. You can certainly solder the wires direct to the board. It'd be more secure that way as well.
```

---
## \#3 Posted by: jct1212 Posted at: 2016-08-31T01:26:01.077Z Reads: 158

```
@Jinra Thank you so much! Could I install the pins and servo cable myself, or would soldering be easier and more reliable?
```

---
## \#4 Posted by: michaeld33 Posted at: 2016-08-31T01:28:49.866Z Reads: 157

```
 I personally would just solder pins to it, just because then I have the option of removing it later on
```

---
## \#5 Posted by: Jinra Posted at: 2016-08-31T01:29:52.073Z Reads: 157

```
If you want a detachable cable go ahead with the pins. Some people have said that the vibration sometimes knocks the servo cable loose but this has never happened to me. direct soldering would work fine as well. I'd probably wire direct if i were you.
```

---
## \#6 Posted by: jct1212 Posted at: 2016-08-31T01:38:38.654Z Reads: 149

```
<img src="/uploads/db1493/original/2X/6/60325f8cf942e24baf38fdca91b07444538d63f8.JPG" width="375" height="500"> 

That is my GT2B receiver. Where do I solder the 3 cables onto?
```

---
## \#7 Posted by: Jinra Posted at: 2016-08-31T01:42:03.497Z Reads: 143

```
I wouldn't solder onto the receiver (but you could). You'll want to use one of the channel rows (3 pins). You might want to reference Google to see which one are which.
```

---
## \#8 Posted by: jct1212 Posted at: 2016-08-31T02:00:07.666Z Reads: 141

```
Do you guys think I could buy something like this, connect the female side to the receiver and cut the other end off before the connector and solder the 3 loose wires to the VESC? 
http://www.ebay.com/itm/10PCS-150mm-Servo-Extension-Lead-Wire-Cable-Cord-For-Futaba-JR-Male-To-Female-/252324849763?hash=item3abfbba863:g:KusAAOSwxp9W67bG
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-31T02:01:28.163Z Reads: 132

```
yep, that's what I'd recommend! However you want a male to male servo cable (in case you decide on pins later) or male to bare wire like this

http://www.getfpv.com/5cm-male-servo-wire-to-bare-wire-26awg-jr-style.html?utm_source=google_shopping&m=simple&gdffi=747627bc7e464db68e5f529d971aacf3&gdfms=FC7E4D50C7094C52A1E32ED6ADEFE68A&gclid=Cj0KEQjw3ZS-BRD1xu3qw8uS2s4BEiQA2bcfM7r3t_RGjMTtfG_UTaR17pXlPo1oh3V1k8EtkkqW600aAqMf8P8HAQ
```

---
## \#10 Posted by: jct1212 Posted at: 2016-09-04T00:12:48.330Z Reads: 113

```
I took the whole clear plastic shrink wrap off to solder the wires (I should've just cut a hole :( ), but now I am left with an exposed VESC. Does anyone know how I should repackage it to make sure it doesn't short?
```

---
## \#11 Posted by: Jinra Posted at: 2016-09-04T03:39:18.441Z Reads: 106

```
Get some clear heatshrink or plastic case for it. If you want to be ghetto you could tape it up with electrical tape
```

---
## \#12 Posted by: lospollos Posted at: 2016-09-04T21:22:35.977Z Reads: 87

```
What?? Am I really going to have to solder my receiver to my enertion vesc? @enertionsupport
```

---
## \#13 Posted by: makevoid Posted at: 2016-09-04T21:35:50.407Z Reads: 87

```
You can just plug it in to try it out and for your first test ride, but it's suggested that when you're sure everything is working, before doing crazy speeds or crazy distances, to make sure all the connections are fixed. You can choose between methods like: soldering the wires, hot gluing the connectors, applying electrical tape... (from best to worse), or any other method that makes sure that the all the cables don't disconnect when you're riding at high speed due to vibrations.
```

---
## \#14 Posted by: FlashNova Posted at: 2016-09-04T21:37:49.083Z Reads: 92

```
Wth? There's no pins on the enertion VESCs? Wow. That's all I have to say.
```

---
## \#15 Posted by: jct1212 Posted at: 2016-09-04T21:46:07.981Z Reads: 92

```
This is the response enertion gave me:

"Hello Jacob, 

Thank you for contacting Enertion Support. Kindly please attach the images of the VESC you received and we will investigate this issue. We are really sorry for the inconvenience. However, This issue can be resolved at your end. If you follow this link. It should help you in connecting the receiver wires easy. 

http://www.electric-skateboard.builders/t/connection-from-receiver-to-vesc/1409/2"

I proceeded to send them pictures of my VESC 3 days ago and so far no response. I guess it's just my responsibility to solder which is fine, but the picture on their website showed the pins and I was expecting them.

This on top of them also sending me 2 sets of front trucks and so far ignoring my email about resolving that issue are annoying as I bought from enertion to streamline the building process.
```

---
## \#16 Posted by: FlashNova Posted at: 2016-09-05T08:19:57.760Z Reads: 77

```
Damn man. That really sucks. I haven't read anything good about enertion's vescs. My vesc from TB came with pins. I don't know why the enertion one wouldn't. It seems like a lot of people are getting burned by enertion. I just bought some motor mounts from them and one of the nuts for the bolts snapped after 2 rides. Not even gonna bother with their customer support.
```

---
## \#17 Posted by: Titoxd10001 Posted at: 2016-09-05T08:45:57.269Z Reads: 72

```
False economy
```

---
