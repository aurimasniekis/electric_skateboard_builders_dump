# Battery indicator (Baiway LY5) settings

### Replies: 24 Views: 4566

## \#1 Posted by: rwxr Posted at: 2017-01-12T12:33:53.954Z Reads: 236

```
I have one of these:
http://www.ebay.com/itm/Battery-Capacity-12V-24V-36V-48V-Tester-Indicator-For-Lead-acid-Lithium-LiPo-LCD-/221797490150?hash=item33a4291de6:g:9AwAAOSw3xJVd6jZ

**EDIT**
Here's the full datasheet: http://akkuplus.de/mediafiles/Datenblatt/BW-LY5.pdf (Thanks @Maxid) 

**EDIT 2**
Here's the post that explains how to use the F1-F6 for the newer versions of the display: http://www.electric-skateboard.builders/t/battery-indicator-baiway-ly5-settings/15942/8?u=rwxr
----
On the indicator there is a button on the front which lights up the display for about 10 seconds.
I would however like if the display was lit all the time when the board is on. Can I bypass the triggerbutton somehow?
Like desolder the trigger and connect the bridges permanetely?

<img src="/uploads/db1493/original/3X/c/a/cafd1117f1c83dbbd0b5e29992b2210a86e9648c.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/c/8/c86ef5fc7166f56cad50bae7852d8d11c38f8995.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/0/e0fad5e818b78195b4de7f78404553372b648072.JPG" width="375" height="500">
```

---
## \#2 Posted by: Maxid Posted at: 2017-01-12T13:12:45.713Z Reads: 206

```
I can't really tell you what to do, but I got a very similar looking battery indicator also from Baiway.
Mine does not have anything soldered on where your switch is:
https://www.dropbox.com/s/gopbdnxh47zyq3h/2017-01-12%2013.46.34.jpg?dl=0
https://www.dropbox.com/s/zuvdd5yqhk1n860/2017-01-12%2013.46.23.jpg?dl=0
```

---
## \#3 Posted by: rwxr Posted at: 2017-01-12T13:19:19.537Z Reads: 192

```
Seems to have been added in V7 then. But you have a hole in the front of the display?
Wonder if I can desolder it completely then..
```

---
## \#4 Posted by: Maxid Posted at: 2017-01-12T13:20:30.122Z Reads: 193

```
[quote="rwxr, post:3, topic:15942, full:true"]
But you have a hole in the front of the display?
[/quote]

Yeah seems odd - but I never bothered as long as it works and it was cheap.
```

---
## \#5 Posted by: Okami Posted at: 2017-01-12T13:32:44.842Z Reads: 186

```
@rwxr woah did not know they have so many versions :D

Btw - do you know the link for the topic in esk8 builders forum, where there were programming options mentioned for these displays ?

I think it was even possible to switch between voltage and percentage, it is just that not a lot of ppl know about this feature..
```

---
## \#6 Posted by: Notso Posted at: 2017-01-12T13:33:15.286Z Reads: 192

```
I have the same one, was also looking for an answer to this. There doesnt seem to be much info about them. But i found this on an amazon listing for a simular model without the button.
<img src="/uploads/db1493/original/3X/f/3/f3734a4d13e0844639e3ed27ba6869ad41399dff.jpg" width="500" height="500">

Maybe it can be changed by bridging a contact on the back?
```

---
## \#7 Posted by: rwxr Posted at: 2017-01-12T14:03:41.623Z Reads: 185

```
Yeah, I've seen that pic as well, but I don't have the F1-F6 bridges on mine.
```

---
## \#8 Posted by: rwxr Posted at: 2017-01-12T14:26:57.251Z Reads: 182

```
Okay, so I figured it out. In V7 of this the F1-F6 functions are integrated.

You'll find them by holding kDN while powering on and then pressing the button on the front. That'll bring up a menu for the F1-F6 functions which then can be switched on/off.

I'll put the brand in the topic and hope this helps other people as well.
```

---
## \#9 Posted by: mmaner Posted at: 2017-01-12T14:55:30.244Z Reads: 172

```
http://www.electric-skateboard.builders/t/battery-monitors-how-low-to-go/11895/3?u=mmaner
```

---
## \#10 Posted by: Maxid Posted at: 2017-01-12T15:44:56.890Z Reads: 164

```
I also found the data sheet. It explains the bridgeable connections plus the volt to percentage values quite nicely:
http://akkuplus.de/mediafiles/Datenblatt/BW-LY5.pdf
```

---
## \#11 Posted by: rwxr Posted at: 2017-01-12T15:58:32.354Z Reads: 149

```
Thanks, I'll add it in the first post.
```

---
## \#12 Posted by: Okami Posted at: 2017-01-13T21:53:37.553Z Reads: 137

```
@rwxr @Maxid  did you find is it possible to make the light stay on the whole time?

The manual is quite lenghty.. I will check it once again later.. I do hope they have the option to switch to the voltage mode in last versions, too..

Too bad the indicator is not weather protected.. I dont see how to to protect it from the rain unless it is encases in a box or the voids/empty spaces at the sides filled with a glue or some other material :confused:
```

---
## \#13 Posted by: mmaner Posted at: 2017-01-13T22:32:33.400Z Reads: 132

```
[quote="Okami, post:12, topic:15942"]
did you find is it possible to make the light stay on the whole time?
[/quote]

You can make the light stay on, go off after 10 seconds or only come on with voltage change.

    F1: the backlight delay turn-off function; enter the low-power state (100uA) after displaying 10 seconds, the LCD displays but the backlight turns off. Press the OK key and the backlight turns off again after 10 seconds’ lighting. This mode needs the OK key.

    F2: the backlight voltage trigger function; enter the low-power state (100uA) after displaying 10 seconds, the LCD displays but the backlight turns off. When the voltage changes, the backlight automatically lights on for 10 seconds, or press the OK key and the backlight turns off again after 10 seconds’ lighting.  This mode needs the OK key.

    F3: sleep function; enter the ultra low-power state (<20uA) after displaying 10 seconds , the LCD and the backlight turns off. Press the OK key and the backlight turns off again after 10 seconds’ lighting. This mode needs the OK key.

    F4: power-on self-inspection; every time the electricity module is powered on, the LCD displays strokes for 2 seconds, and then displays the selected battery type for 1 second, finally displays the electricity capacity.

    F5: voltage display; the current battery voltage is displayed only on the right, the battery symbol on the left is still in accordance with the selected type.

    F6: the LCD shows the Logo on the lower left.

    * The F1-F3 functions need the front key, the default is without this key.

Here's a link to the DROK DC8 Capacity Meter Spec Sheet, its essentially same (I think)

https://www.dropbox.com/s/sij6zuoawkxhqvk/drok%20battery%20meter%20-%20Capacity%20Meter%20Spec%20Sheet.pdf?dl=0
```

---
## \#14 Posted by: Okami Posted at: 2017-01-13T22:35:36.297Z Reads: 116

```
Yeah, I read through it.. seems like not possible, but a good thing, it does light up when the voltage changes..

I will probably look into making an arduino based percentage display at first.. after that a coulometer / wattmeter based arduino module might also be cool, let's see how it goes..
```

---
## \#15 Posted by: mmaner Posted at: 2017-01-13T22:37:13.894Z Reads: 108

```
What was not possible?  Making the light stay on the whole time?  Using function F1, if you leave/turn it off the backlight stays on as long as it receives voltage.  Maybe Im confused, it wouldn't be the first time.
```

---
## \#16 Posted by: Okami Posted at: 2017-01-13T22:48:27.136Z Reads: 103

```
ah, no, it seems it was my mistake! I somehow thought that it means that backlight stays lit for only 10seconds.. not that it is a seperate function for it to stay lit all the time.. 

Anyways, I hope that @rwxr by now has solved his issue, not sure which model he had but still :)
```

---
## \#17 Posted by: rwxr Posted at: 2017-01-13T23:01:22.077Z Reads: 95

```
@Okami: Yes, I solved it.
Hold Kdn and the power it on. Release Kdn and press the front button once. This will let you pick F1 to F6 by pressing Kdn or Kup.
To make the light stay lit all the time, select F1 and press the front button. When there is no bar in the battery symbol the light will stay lit.

Cheers
```

---
## \#18 Posted by: mmaner Posted at: 2017-01-13T23:03:53.598Z Reads: 86

```
Yeah, its a bit confusing when you don't have one to reference.  My favorite function is the Voltage display (F%).  That shows Volts instead of percentage.  Also, the DROK DC8 & Belway are the same meter.
```

---
## \#19 Posted by: rwxr Posted at: 2017-01-13T23:05:08.698Z Reads: 84

```
Yes, and you still have the battery symbol with the bars in it. I'm gonna use mine this way.
```

---
## \#20 Posted by: Okami Posted at: 2017-01-13T23:10:23.334Z Reads: 89

```
@mmaner  Would be cool, if you could take a picture of how the voltage / bar mode looks! This way it would be almost an ideal display for determining the left voltage (at least the mid range, as I know quite ok the high and low points of my boards voltage limits, personally.

Im not sure whenever someone had already a picture of it, but would be nice, perhaps, if it was inserted here, so that it can be clearly seen it is possible and how it looks! 

---
Sorry for not tagging you mmaner, Im not sure why but when I press reply button it does show im replying to you when im writing the text! But once I hit ''publish'' - the reply button, it does not show in the forum, that I was referencing to your post :/ not the first time it happens..
```

---
## \#21 Posted by: rwxr Posted at: 2017-01-13T23:17:22.750Z Reads: 85

```
Like this:
http://g02.s.alicdn.com/kf/HTB1ys.MOFXXXXbnXVXXq6xXFXXXm/229492169/HTB1ys.MOFXXXXbnXVXXq6xXFXXXm.jpg
```

---
## \#22 Posted by: mmaner Posted at: 2017-01-13T23:21:05.022Z Reads: 88

```
[quote="Okami, post:20, topic:15942"]
Would be cool, if you could take a picture of how the voltage / bar mode looks!
[/quote]

<img src="/uploads/db1493/original/3X/5/c/5cd2e1364496699c370b72142341a17bf419b5c7.jpg" width="650" height="500">
```

---
## \#23 Posted by: Okami Posted at: 2017-02-18T14:49:51.256Z Reads: 82

```
<img src="/uploads/db1493/original/3X/2/8/284ad670c4c205fdfcc4e38f723b89e6ec4f841c.jpg" width="690" height="402">

They come now in also nice black enclosure.. + blue color

https://www.aliexpress.com/item/8-70V-Blue-LCD-Acid-Lead-Lithium-Battery-Capacity-Indicator-Digital-Voltmeter-Voltage-Tester-Free-Shipping/32759918771.html?spm=2114.12010108.1000023.16.D6RkrF
```

---
## \#24 Posted by: Okami Posted at: 2017-03-10T20:33:14.148Z Reads: 73

```
Does anyone know at what voltage per cell the meter shows 0% percent? I would like to find this out before running down the battery fully :D i do have voltmeter but would be nice if I found out earlier than when riding tomorrow :)

For now I know that 56% is at ~3.7v per cell

So I assume it could be 3.2-3.0v ?
```

---
