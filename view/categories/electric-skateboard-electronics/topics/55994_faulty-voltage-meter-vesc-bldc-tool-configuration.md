# Faulty voltage meter VESC BLDC Tool Configuration

### Replies: 8 Views: 429

## \#1 Posted by: sjors98 Posted at: 2018-05-19T12:05:33.590Z Reads: 43

```
Hi!

I have a problem with the configuration of my vesc. 
I just finished making my setup with:
**8s 6400mah battery **
**A vesc-x from enertion **
**A Nano-X hand remote controller from enertion**

I've build the battery myself and it outputs around **26 volt** right now (already used it a bit)
However the vesc says that the battery outputs **19.6** volts which I think is very weird.
When I plug the power cable in it says it has **29volts** in the BLDC tool.
Here are my BLDC tool Motor settings:
![35|690x431](upload://bCob9b84yyjdygolEsXqYceT631.png)


When I run the motor with the power in it works perfectly, but when I run it on the battery it stutters ofcourse because of the settings.
When I change the settings it works fine, but I don't want to do that ofcourse because I just want my 8S output!

Hope you guys can help me!

**Edit:**

After uploading this thread I realised something.
I use this splitter to split the power to two vescs, however I burnt my second vesc...
![Connector|640x427](upload://aBy3KXuEigtWMHJLXTMVE83y4r4.jpg)
The replacement is on it's way, but I wanted to test my board already
One of the ends is empty and when I measure the voltage here it says 19.7 volt. So the problem is in the splitter.
Can you guys maybe confirm for me that the voltage is dropping because one of the ends of the splitter is empty? Or is the splitter faulty and do I have to get a replacement?
```

---
## \#2 Posted by: Skitzor Posted at: 2018-05-19T12:21:02.097Z Reads: 39

```
Maybe post a picture of your battery. If it's a single 8s, this sounds like voltage sag.
Measure the battery directly. What voltage ? Why plug in the splitter when ur on a single FB.
```

---
## \#3 Posted by: sjors98 Posted at: 2018-05-19T12:25:24.737Z Reads: 39

```
Actually only using the splitter right now for extention of my cable.

However I just discovered that the voltage drops when the vesc is connected so the splitter is fine.

Is there a setting in BLDC that cuts of some of the voltage of the battery?

I've found this thread that has a similar problem:
http://www.electric-skateboard.builders/t/bms-lowers-voltage-once-plugged-into-vesc/53401/25

I will be home tonight so then I'll try to add the wire from the B- directly to the vesc as said in this thread^
```

---
## \#4 Posted by: Skitzor Posted at: 2018-05-19T12:30:02.767Z Reads: 37

```
You cannot compare a 8s to a 10s3p. the 3 parallel groups compensate the voltage sag.
Bypassing the BMS may help a bit, but I'm afraid not the solution to your problem.
Edit: What cell types are you using by the way, cause your settings look very optimistic
```

---
## \#5 Posted by: professor_shartsis Posted at: 2018-05-19T12:46:46.853Z Reads: 34

```
@sjors98 you’ve stated your battery is 26v... perhaps part of the problem is your battery cut-off setting is at 27.2v...

but on second thought, shouldn’t a fully charged 8s battery be closer to 30v+? if you’re at 8S and 26v maybe you need to recharge the battery? you’re already down to 3.25v per cell which is quite low...
```

---
## \#6 Posted by: sjors98 Posted at: 2018-05-19T13:08:02.040Z Reads: 29

```
But the motor still works but stutters, I have the battery on charge now so when I get home I will try again.
Still the voltage is dropping around 8 volts which doesn't seem right.

I drew a battery scheme very quickly (I apologize for the bad structure)
The battery's are 3400mah NCR18650B cells.
![BatteryLayout|562x500](upload://kiQ77zl2mCWCpefZa8FFo4V4dJW.jpg)

This is my first try for a electric longboard and I really want it to work haha
```

---
## \#7 Posted by: professor_shartsis Posted at: 2018-05-19T13:09:42.202Z Reads: 27

```
[quote="sjors98, post:6, topic:55994"]
the voltage is dropping around 8 volts which doesn’t seem right.
[/quote]

if the battery was already low (3.25v/cell) to begin with, the voltage sag could be much larger than usual, & it’s possible the low volt cutoff setting was the only thing protecting your battery from overdischarge and possible damage.
```

---
## \#8 Posted by: sjors98 Posted at: 2018-05-19T13:17:10.295Z Reads: 26

```
Okay so I asked my roommate who has little experience with wiring to check if he can see something and he just called me to tell there was jus a bad connection at the XT60 connector to the vesc. He fixed it and now it works as it should work.
Sorry I've wasted your time!
```

---
