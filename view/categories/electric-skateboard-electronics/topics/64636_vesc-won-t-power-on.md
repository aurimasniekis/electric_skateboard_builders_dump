# VESC won`t power on

### Replies: 15 Views: 493

## \#1 Posted by: epster Posted at: 2018-08-12T11:52:04.980Z Reads: 91

```
Hey guys,

So i was trying to configure my vesc today but it won`t power on. I checked the battery and it is at full charge so that shouldn`t be the problem. I never had any sparks or shortage while connecting wires or batteries to the vesc. It just got out of the box and on the diyelectricsite they say they check it before shipping so it should work right?!

[20180812_134332|374x500](upload://jt4df7OgH0o1csCZhzrRDVd5mpb.jpg)
![20180812_134529|666x500](upload://8IbpeD6DRUUuG8saUXsiNTBDa4H.jpg)
![20180812_134634|374x500](upload://9a9IFlfLqMN8V7LoIjyOjYauYiN.jpg)

I don`t have that much experience with electronics so help would be appreciated. I tried to look this problem up on the forum but no-one had the same problem as i do for as far as i could see.
```

---
## \#2 Posted by: epster Posted at: 2018-08-12T11:53:21.433Z Reads: 85

```
![20180812_134332|374x500](upload://jt4df7OgH0o1csCZhzrRDVd5mpb.jpg)
```

---
## \#3 Posted by: Andy87 Posted at: 2018-08-12T12:18:40.078Z Reads: 78

```
You plugged your plus into minus and minus into plus...check the colors of your wires
```

---
## \#4 Posted by: epster Posted at: 2018-08-12T12:21:28.744Z Reads: 79

```
I am sorry I don`t think i understand you you mean the plus and minus of the motor wires? or are you talking about th xt90 connectors
```

---
## \#5 Posted by: Andy87 Posted at: 2018-08-12T12:23:34.587Z Reads: 76

```
The red wire coming out of your battery goes through your loopkey and than in the black wire of your vesc. The black wire out of the battery goes into the red wire of the vesc. You mixed the polarity
```

---
## \#6 Posted by: epster Posted at: 2018-08-12T12:26:14.082Z Reads: 75

```
Oh shit thanks mate, I will resolder it.:smile:
```

---
## \#7 Posted by: epster Posted at: 2018-08-12T20:39:57.476Z Reads: 66

```
Think i did it wrong again........ I swear i did it right i followed the lines like you said.![20180812_223607|374x500](upload://qme2x7y9u0BKgYGDVTrbBEugY1F.jpg)![20180812_223546|666x500](upload://9LnE9uj2k5QBehGoZ9VK3deoNvo.jpg)
```

---
## \#8 Posted by: Ubbiedude Posted at: 2018-08-12T20:53:52.610Z Reads: 61

```
Could be that you fried your vesc because you reversed polarity
```

---
## \#9 Posted by: epster Posted at: 2018-08-12T20:55:52.646Z Reads: 61

```
Now i feel even more stupid. Is that possible if you input a 4s battery? Didnt hear any bangs or sparks.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-08-12T21:27:21.545Z Reads: 58

```
It’s lined up right now. If your vesc like this not powering on now you probably fried your vesc with the last mistake.
Not sure if this vesc has a protection circuit against wrong polarity.
One thing you can try.
Disconnect your loop key circuit from both sides (battery and vesc). Then take a Multimeter if you have one and check the resistance from the xt 90 plugs. Black wire from right to left than red from right to left(with plugged in key) if the resistance shows open end than it means the wires or the plug somewhere faulty. In this case you need to check your solder joints or replace the plugs.
```

---
## \#11 Posted by: dareno Posted at: 2018-08-13T05:24:49.536Z Reads: 48

```
Mate that is so easily done if you don't follow the rules.  The positive wire (red) is always on the square side and the negative (black) is on the rounded side of an XT connector and if you always use the same colour wire throughout your build, red for positive and black for negative you can not go wrong. 
![wiring_LI|666x500](upload://9zuucOIl48dEEx5hhUlez7jKrcy.jpg)

On a genuine xt connector + and - is actually embossed on the casing too
Sorry to say it but if there are no lights on your vesc then it is very probably toast and the only consolation is I bet you never do it again.
```

---
## \#12 Posted by: nuttyjeff Posted at: 2018-08-13T05:35:33.701Z Reads: 46

```
sorry to say, but you probably fried your VESC.

Things to look out for next time:
1. Check polarity before connecting.
2. Check polarity again, (use a voltmeter if you want to be really sure.)
3. Install a temporary fuse between your VESC and your power source for your first connection.
```

---
## \#13 Posted by: epster Posted at: 2018-08-13T09:10:21.094Z Reads: 44

```
Thanks for the replies guys. I will pay more attention next time and redo the colour of the lines. I was looking up which multimeter i should buy but the problem is that my battery is 4S 14.8v 10.000mah 10C continuous and 24C peak. Does that mean I need to get a 10x10=100A multimeter or even a 10x24= 240A multimeter!? Or are there other devices that you guys recommend with my setup. Doing 12S made out of the 4S so 44.4V and 45A so i dont overload the vesc.
```

---
## \#14 Posted by: Andy87 Posted at: 2018-08-13T10:50:29.445Z Reads: 41

```
Just get a hobby multimeter. If you want something good get a Fluke.
You don’t measure under load, so no need that it needs to handle that current. It’s just to check the voltage, polarity or resistance.

PS: here some guys like @Martinsp who repair vescs. Maybe they can help you and will be more cheap than to buy a new one
```

---
## \#15 Posted by: epster Posted at: 2018-08-13T13:13:34.662Z Reads: 30

```
Hey guys quick update, just bought a multi-meter the one andy recommended. Looked through some forums and managed to repair my vesc :grinning: .  There was some built in reverse polarity protection for the noobs like me hahah. Just tested everything and everything works great. Now planning on making an enclosure and connecting my bluetooth module. 

Have a nice day guys and thanks for the tips
```

---
