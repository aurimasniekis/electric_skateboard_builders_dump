# 6s lilo BMS problem(smoke lots of it)

### Replies: 32 Views: 2542

## \#1 Posted by: Daniel.henn Posted at: 2017-01-22T14:03:28.728Z Reads: 150

```
Hi i have recently posted about 6s lilo BMS and i got told to snip the positive and negative wires off the balance lead on the battery which i did and worked fine however when i connect the battery one of the chips smoke when i connect the balance lead why may this be <img src="/uploads/db1493/original/3X/f/1/f1d1d94b6da5231efbf8385586d07451914ad209.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/b/9/b966394b4618fac08f6b674a188d26ab08b58bed.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/4/7/472fa830513a8a9ac6dc86a932e4cd8b234f9384.jpg" width="374" height="500">
```

---
## \#2 Posted by: Okami Posted at: 2017-01-22T16:21:20.399Z Reads: 135

```
Did you connect it correctly/ I cannot get a thing out of your description and pics.. but I just burnt one bms too by accidentally contacting the wrong pins..
```

---
## \#3 Posted by: Daniel.henn Posted at: 2017-01-22T17:05:48.273Z Reads: 129

```
Yes i connected them correctly how they are supposed to be . if i push balance cable in from the lipo no smoke if i put the main red and black in no smoke however when i push all of the connectors in the one chip smokes i have tried this on both circuit boards i have
```

---
## \#4 Posted by: Okami Posted at: 2017-01-22T17:07:54.803Z Reads: 125

```
Do you still think they will work at all now?  Since they gave off the smoke..

 I believe there is a short circuit.. which is happening in the circuit.. just not sure why you have it.. do you have some of datasheet or wiring diagram for it'?

Im not sure but are you really supposed to connect both leads to the circuit? Im actually not that good with bms.. but I undestand there are balance wires you need to connect and then there are main leads you need to connect..

--

If it is a balance connector which is put inside when the smoke starts to come off.. I would guess the + wire and - wire have been switched sides.. This happened to me a few times when I made balance connectors.. but im not sure who would install the connector ''upside down'' for you to install in the wrong way..
```

---
## \#5 Posted by: Okami Posted at: 2017-01-22T17:14:41.037Z Reads: 106

```
From your description I assume you connected the wrong balance  lead to the circuit.. they are the most easiest to mess up.. since they are also colored..

So which color wire is the ''first'' one?

First one have different polarity from the rest of the balance wires..
```

---
## \#6 Posted by: Daniel.henn Posted at: 2017-01-22T21:00:10.279Z Reads: 86

```
No balance connector only goes in one way if you look at my other posts you will see that my balance plug on the battery had 7 wires and the BMS only had 5 two of the 7 wires were red and black i got told to snip them as they wont be needed due to using main leads to charge the battery however i am starting to think that is why ...... But then where would i put the red and black to as there are only 5 wires for the balance bit which would be the individual cells
```

---
## \#7 Posted by: Okami Posted at: 2017-01-22T21:02:15.573Z Reads: 87

```
uhh I really need to take a look at your bms board..

im not sure what B0 stands for in your bms.. but I think it should have been the - wire which needs to go first.. I will check this once again I get back to my board.. I dont remember in which way the polarity went..

There's a likely hood you cut the wrong wires without checking the polarity.. just messed it up when plugged into the bms as the incorrect wires were cut or they needed to be in ''different formation''
```

---
## \#8 Posted by: Daniel.henn Posted at: 2017-01-22T21:17:52.847Z Reads: 86

```
Ok here is the link to the BMS i have http://m.ebay.co.uk/itm/25V-Protection-Balance-Module-BMS-PCM-12A-For-6S-22-2V-Li-ion-Li-Po-Battery-/322317909787?nav=SEARCH
```

---
## \#9 Posted by: Okami Posted at: 2017-01-22T23:38:51.426Z Reads: 83

```
<img src="/uploads/db1493/original/3X/a/7/a71ef2bdb9f4e2079bf2caca7b57cd35847cee8b.png" width="281" height="500">

Did you wire it up this way?
```

---
## \#10 Posted by: Okami Posted at: 2017-01-22T23:40:25.761Z Reads: 75

```
I think you did not carefully check the connections. If u had multimeter u could check them.
```

---
## \#11 Posted by: Daniel.henn Posted at: 2017-01-22T23:52:51.061Z Reads: 72

```
How would i check it with my multimeter but i have wired it up the way other people have told me only other think is i need to check which way the balance plug is wired but i prosume its the same way
```

---
## \#12 Posted by: Okami Posted at: 2017-01-23T00:02:52.341Z Reads: 72

```
Once i get to see some lipo pack i can tell. Im running li ion now. So i have to look up how i wired it up.but thats for tomorrow
```

---
## \#13 Posted by: Daniel.henn Posted at: 2017-01-23T00:16:13.215Z Reads: 74

```
Ok my lipo is a 6s 5000mah zippy 20c or 25c <img src="/uploads/db1493/original/3X/f/1/f1d1d94b6da5231efbf8385586d07451914ad209.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/4/d/4dc05a17cf6d3a1114397188adaa9f63baa248cb.jpg" width="500" height="500">
```

---
## \#14 Posted by: Okami Posted at: 2017-01-23T00:22:01.543Z Reads: 64

```
Ok will report tomorrow (unless someone steps in and clears up this bms smoke thing)
```

---
## \#15 Posted by: Daniel.henn Posted at: 2017-01-23T00:24:47.493Z Reads: 65

```
No worries thank you so much for the help really appreciate it!!
```

---
## \#16 Posted by: Okami Posted at: 2017-01-23T00:33:50.918Z Reads: 66

```
Which chip smoked? If it is a resistor u can easly replace it.. otherwise not so cool if it is charge regulator with many pins..
```

---
## \#17 Posted by: Okami Posted at: 2017-01-23T00:35:32.852Z Reads: 68

```
From what i understand u should have connected only charge leads and battery (balance leads)  ..no main leads but will see tomorrow im stil not sure which 5wires you connected.. in theory there should be no short if these were the middle ones..
```

---
## \#18 Posted by: PXSS Posted at: 2017-01-23T06:09:03.407Z Reads: 63

```
You shorted your battery. The BMS burnt because that is the point with the most resistance.

You should NEVER EVER EVER have a male plug on a battery. I suggest you do tons of research before blowing the battery up...
```

---
## \#19 Posted by: Daniel.henn Posted at: 2017-01-23T08:01:22.098Z Reads: 64

```
<img src="/uploads/db1493/original/3X/4/7/472fa830513a8a9ac6dc86a932e4cd8b234f9384.jpg" width="374" height="500">on that photo it is the chip at the top right
```

---
## \#20 Posted by: Daniel.henn Posted at: 2017-01-23T08:41:21.927Z Reads: 60

```
What do you mean by i shouldn't have a male.plug on a battery
```

---
## \#21 Posted by: Okami Posted at: 2017-01-23T09:47:46.183Z Reads: 58

```
I think he meant the bullet connector u made.. they accidentally can touch something etc
```

---
## \#22 Posted by: Okami Posted at: 2017-01-23T09:49:29.980Z Reads: 59

```
Look up that 089 resistor if uu have free time perhaps u can try to resolder it. If nothing else burnt..

---

<img src="/uploads/db1493/original/3X/d/3/d3672e76b4955a607a2051c19ad9787c6e87ddfe.png" width="392" height="351">

From this picture, it looks like you should have connected the lowermost (red) wire to the B+ of your bms circuit.. The rest should have ''followed'' after that. 

The ''last wire'' the black one, should have went to B-. This is for ''low current application'', so possibly - charge only at up 2-3amps max I believe. (not sure about max rating for these wires, but still)

For higher currents (and ''discharge mode bms operation'') then it would need ''main plugs'' - , then you should have cut a wire from each side of the balance connector, and I assume just connect ''the middle 5' wires'' to the white plastic connector. Then for B+ would be the positve main plug and for B- would be the negative plug.

This seems to be the way others recommended do it.. but if you cut just two side by side wires (the negative side wires) and connected the plus wire to the the uppermost connector, this explains why exactly that resistor burnt up in in the smoke.. I believe, as you did not put everything in charge mode, perhaps the only current that went through was through this little resistor.. Check that Q2 chip too, if it is also black.. then no good.. and probably just buy new bms.. or try to look hard enough for a replacement chip like that.

----

Ok I think im somewhat finished with this.. did not intend to look up bms'es for now.. but okay will know a bit more about their wiring now..
```

---
## \#23 Posted by: Daniel.henn Posted at: 2017-01-23T11:08:38.368Z Reads: 54

```
This is the board i have can you try figure out which colour wire goes to which as i am very confused <img src="/uploads/db1493/original/3X/8/7/87e101f4abcd98a4959450f89c4bff07d8855371.png" width="281" height="500">
```

---
## \#24 Posted by: Maxid Posted at: 2017-01-23T11:20:32.460Z Reads: 53

```
That diagram indicates a 5S BMS not 6S

Edit: nevermind just saw that the image has one resistor missing - it is basically an image of the 5S version of your BMS.
```

---
## \#25 Posted by: Daniel.henn Posted at: 2017-01-25T22:17:06.966Z Reads: 46

```
Thanks for all the help i got the diagram of my battery from hobby king and it turns out i put it in the right way so now im completely confused on why this would blow the chip as everything was in the right way
```

---
## \#26 Posted by: Okami Posted at: 2017-01-25T22:30:50.510Z Reads: 46

```
Can u tell which wires from balance wires you cut?

Red one.. and which next?
```

---
## \#27 Posted by: Daniel.henn Posted at: 2017-01-25T22:46:04.990Z Reads: 47

```
I cut the red and the black the 1st and the last wire
```

---
## \#28 Posted by: Okami Posted at: 2017-01-26T06:43:43.075Z Reads: 41

```
mh then it theory it should have been all ok.. especially if you wired the next whire after the red one, to the b1.. or after the b+
```

---
## \#29 Posted by: Daniel.henn Posted at: 2017-01-26T18:47:34.991Z Reads: 39

```
Yeah i wired all of that the right way checked with board diagram and battery diagram
```

---
## \#30 Posted by: jmasta Posted at: 2017-01-26T21:52:36.216Z Reads: 39

```
For future reference, it would have been a lot better to get a female 6S JST connector (7 pin) and wire that directly to the BMS harness. In doing so, you wouldn't use all the output pins (i.e, 7 wires in / 5 wires out), and it would have prevented you from permanently modifying your battery

I'm not sure who told you to cut the balance leads, but I personally wouldn't have recommended that


Also, I noticed your BMS is only rated to 12A. Are you planning on only using it for charging?
```

---
## \#31 Posted by: Daniel.henn Posted at: 2017-01-27T07:48:05.778Z Reads: 35

```
Thank you for the reply i think.i am going to.order a male jst connector and put it back onto the battery as IG is useless at the momeny. I got told to cut it by a few people which is why i did but now regretting it, and yes i was going to use that board to charge it
```

---
## \#32 Posted by: SvantePanter Posted at: 2017-11-25T11:30:53.609Z Reads: 19

```
@Daniel.henn How did you solve this? Did you replace the burnt resistor or did you use a another, fresh BMS? Just burnt two resistors on my BMS, I have the exact one as you have although I have two 3s LiPO-s in series.
```

---
