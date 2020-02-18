# Problem with space cell..any solutions?

### Replies: 10 Views: 754

## \#1 Posted by: theviith Posted at: 2016-07-13T01:48:07.218Z Reads: 90

```
Hi guys,

So I've had my space cell for a good couple months now and just today, it decided to quit working. I ran over a small pothole and next thing I know, the battery was off and I couldn't get it turned on or charging. I have the later version of space cell so it is equipped with the new toggle switch. I've tried replacing the in-line fuse with replacements but that didn't work. So now, I can't power on the battery and when I try to charge the battery, the LCD display just shows 100% with the intelligent charger light is green. But I know for a fact that my battery was not fully charge when this happened. In fact, it was at about 32%.

It sounds to me like it could be the toggle switch, or the BMS. I could open up the space cell to test it but I want to see if anyone know or had similar problem with solutions before doing so.
```

---
## \#2 Posted by: theviith Posted at: 2016-07-13T03:47:53.128Z Reads: 86

```
Nevermind, I found the problem! It was a connectivity issue where two of the metal tabs connecting the batteries broke off..shown in the picture. Anyone have any idea how to make the connection solid again? I don't have spot wielder so can't redo the tabs and I don't want to solder bc it's such a small area to work with that I'm afraid I'll kill the cells due to heat. 

Thanks in advance
<img src="/uploads/db1493/original/2X/4/4e49ae6b63ebf0d816f0a32abadd7dd4645ba79a.jpg" width="690" height="388">
```

---
## \#3 Posted by: Namasaki Posted at: 2016-07-13T03:51:04.418Z Reads: 80

```
If you live in the US. there are a couple battery builders on the forum that could probably fix it
@barajabali
```

---
## \#4 Posted by: barajabali Posted at: 2016-07-13T03:55:25.778Z Reads: 78

```
Thanks @Namasaki

@theviith Ill take care of it for a minimal charge.  pm me if interested
```

---
## \#5 Posted by: Eboostin Posted at: 2016-07-13T04:15:14.813Z Reads: 77

```
Isn't there some type of warranty on the space cell?
```

---
## \#6 Posted by: c4Lvin Posted at: 2016-07-13T04:35:48.234Z Reads: 73

```
I'd like to know about that too. Kinda odd that those tabs broke off. Even when fixed others will break once again. How are you mounting the pack @theviith?
```

---
## \#7 Posted by: theviith Posted at: 2016-07-13T20:42:58.985Z Reads: 54

```
thanks guys @barajabali @Namasaki for the offer but I got it fixed!!! After fiddling around, I realized that I could just add another nickel plate in between the contacts and hot glue them down to secure the connection...and it worked! I've test ridden them earlier today with no problems!
<img src="/uploads/db1493/original/2X/9/936be0788be4e16b1715c2f7bed8ff93cc9674d3.jpg" width="690" height="388">
```

---
## \#8 Posted by: theviith Posted at: 2016-07-13T20:47:05.160Z Reads: 53

```
@Eboostin yea I thought so too, but apparently not lol. I don't think Enertion offers any warranty to its products other than the VESC..but even with that, you'd have to pay extra for the warranty lol

@c4Lvin I will post a pic of my build soon, it's a little beaten up right now so will needs some re-polishing before going public haha
```

---
## \#9 Posted by: Namasaki Posted at: 2016-07-13T21:04:16.065Z Reads: 51

```
Caution: if the tab patches are not soldered or welded to the original strips, you could have arcing between them because of vibration and it could be some heavy arcing with 10s.
```

---
## \#10 Posted by: onloop Posted at: 2016-07-14T01:08:22.047Z Reads: 46

```
[quote="theviith, post:8, topic:6010"]
I don't think Enertion offers any warranty to its products other than the VESC..but even with that, you'd have to pay extra for the warranty lol
[/quote]

if anyone is wondering about our warranty it is written here: http://www.enertionboards.com/pages/enertion-boards-terms-conditions.html

to summarise, most electronics have 60 days warranty covering manufacturing faults. (vesc platinum & raptors have longer warranty)

i would need to see a picture showing the enclosure you mounted the battery inside. was the battery protected from board flex & vibrations?

to fix this problem i suggest lifting up one side, like you a turning a page in a book, then you will be able to see inside, in the middle between the cells. you will then need to use your soldering iron to bridge the gaps.
```

---
