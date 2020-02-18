# FOCBOX programing help :&#124;

### Replies: 25 Views: 1421

## \#1 Posted by: Danny414 Posted at: 2018-04-17T00:11:07.687Z Reads: 241

```
Ok, so a tad bit confused..

I have dual focbox's.. and when programing the motors using the bldc tool.. do you have to program each motor separately and then CAN bus them together? or can do can bus them first and then do the programing? I'm trying to program them with the can bused together and when I click on measure R & L and measure A only the slave moves..

Thanks!
```

---
## \#2 Posted by: goldrabe Posted at: 2018-04-17T00:16:58.793Z Reads: 239

```
Yes, you have to setup both VESC's and motors first and then define master and slave for PPM.
Don't forget to set the fail save correctly on your reciever and remote!
Edit*
Don't forget to write config each time you do motor detection and setup.
```

---
## \#3 Posted by: skatardude10 Posted at: 2018-04-17T00:36:17.795Z Reads: 224

```
* Make sure to read motor and app settings each time you connect or you will overwrite the wrong settings. I like to read all settings every time I make a change to make sure it saved.

* I connected my canbus first, then got to updating firmware and programming.

* Set master to 0 and slave to 1. One of the can options is to send status to other ESCs. Set this on the slave. The other option to enable on the master is multiple escs over CAN, I think. Save, read, verify, disconnect

* I have ppm and uart set as my app mode for Bluetooth and controller on master. If you don't have a BT module, it's probably just ppm depending on your controller. On the slave I think I have none, because it takes what the master sends it... ppm in my case. Set up all your control config stuff and app settings on master only

* Motor detection has to happen separately for each vesc, and saved to each vesc in particular... Same with all your voltage limits etc under motor config.

Hope this helps. The tooltips are great, especially on ackmaniacs bldc tool. Download that tool if only to hover over settings for in depth tooltips.
```

---
## \#4 Posted by: Danny414 Posted at: 2018-04-17T02:49:23.687Z Reads: 182

```
Is multiple escs over can supposed to be ticked (app configuration/ ppm tab) ? If so on master or slave or both?

![image|666x500](upload://wDofuv8lz1r89YeV6pNfuP07ltC.jpeg)
```

---
## \#5 Posted by: CarlCollins Posted at: 2018-04-17T02:53:53.051Z Reads: 163

```
Multiple ESCs over CAN must be checked
```

---
## \#6 Posted by: Slak Posted at: 2018-04-17T08:50:56.655Z Reads: 147

```
@Danny414  What is the tutorial you're following to set your 2 Focbox up ? If those simple answers are not in your tutorial, it maybe is a bad one and you should contact the author so others people know what to do and how to dot it. Do you at least follow a tutorial ?
```

---
## \#7 Posted by: Bjork3n Posted at: 2018-04-17T09:31:35.619Z Reads: 137

```
Only on master vesc right?
```

---
## \#8 Posted by: Danny414 Posted at: 2018-04-17T15:32:47.941Z Reads: 124

```
I’ve just been searching on here and YouTube and it haven’t been really clear on what I’ve read. And most everything I find is only for one VESC not dual.. and not dual focboxs, it also isn’t clear if I should be setting the initial parameters like battery min max for just that motor or if I just take both into account.. would you be willing to voice chat or FaceTime? If so you can pm me your number and best time to call
```

---
## \#9 Posted by: Danny414 Posted at: 2018-04-17T15:33:52.023Z Reads: 121

```
I’m setting up 2 focboxs
```

---
## \#10 Posted by: Deckoz Posted at: 2018-04-17T15:34:40.779Z Reads: 120

```
Multiple ESC over can checked on master and all slaves


Send status over can only checked on slaves.
```

---
## \#11 Posted by: Danny414 Posted at: 2018-04-17T16:53:39.262Z Reads: 117

```
what is weird is I have it setup like that now but then after I connected the can bus cable and power on the focboxs.. the master automatically checks send status over.. it seems to be working how ever.. here are some pics

This is of the master before I plug in the canbus cable

![image|666x500](upload://9Tvufdy2K7HSfCqf0HimINRVEQB.jpeg)![image|666x500](upload://2rlw3oPz9CpYK0Ikt2NuRkhjzG1.jpeg)

Here is the slave before I plug in can bus cable

![image|666x500](upload://i4n4EtYfqTJI8rgaOg3Qu4RhLfY.jpeg)![image|666x500](upload://49CpBQkLr2dYSgZeoaGnEQtVSAJ.jpeg)![image|666x500](upload://rHPdIISTYKHSlvzaAwFzhBoTafz.jpeg)

Here is the master after I plug in the canbus cable.. it changed itself 

![image|666x500](upload://biuRRad491er31rKip1F7xrkap7.jpeg)
```

---
## \#12 Posted by: Deckoz Posted at: 2018-04-17T16:55:09.642Z Reads: 99

```
You have to READ configuration every time you switch can ID or plug in the USB.. otherwise it is just showing data from the last READ
```

---
## \#13 Posted by: Danny414 Posted at: 2018-04-17T16:57:02.175Z Reads: 103

```
I do.. notice the controller ID in the last pic is still 0 I actually close the program right after a write.. so when I re-open it all the values are all 000000000's so I know to read
```

---
## \#14 Posted by: Deckoz Posted at: 2018-04-17T17:02:34.185Z Reads: 104

```
Without canbus plugged in.

Plug the USB and power  into the master. Program it with
iD 0
Multiple esc over can checked

Unplug it.

Plug in the USb to the slave and program it with
Id1 
Multiple esc over can checked
Send status over can checked.

Unplug

Plug the can cable into both. Power them both. Plug the USB into the master. go to the connection tab and click connect. It should be the master, and read. Still on the connection tab, type 1 into the can fwd box and enable can fwd on the connection tab. Click connect it should be the slave then read. 

You cannot plug in the usb to the slave and connect to master over can, because the master isn't sending it's status to the bus. 

Hope this helps...
```

---
## \#15 Posted by: Danny414 Posted at: 2018-04-17T17:25:23.941Z Reads: 102

```
Ok so here is what I did

![image|666x500](upload://cdFjwyNWOldgfKj3VECDdB4mH8s.jpeg)

After I do a write with this above pic and then close the program and reopen the program with usb plugged into the master and do a read it showed this

![image|666x500](upload://biuRRad491er31rKip1F7xrkap7.jpeg)

THEN I wait a couple minutes. Close the program, reopen, with usb connected to master I do a read and it shows this

![image|666x500](upload://n39nr155Jpchg47omSywAjsxOBj.jpg)

So it changed itself twice it looks like but the weird things is both motors are spinning as they should and seems to be working.. weird
```

---
## \#16 Posted by: briman05 Posted at: 2018-04-17T17:44:31.931Z Reads: 85

```
You shouldnt have to close out the program just press the disconnect button.  And you are making sure you do the changes then do a write config
```

---
## \#17 Posted by: Toughook Posted at: 2018-04-17T19:59:33.106Z Reads: 91

```
Sorry to jump on here, but this task is something looming for me in next few days. I also have dual focbox setup with can, and am looking for the #1 recommended YT tutorial you guys would point me too. Searching on there brings up a plethora of vids, but as a focbox noob I would take the advice gladly of which tutorial is the best / most thorough out there.

Thanks for any help
```

---
## \#18 Posted by: Slak Posted at: 2018-04-17T22:02:41.862Z Reads: 95

```
[quote="Deckoz, post:14, topic:52495, full:true"]
Without canbus plugged in.

Plug the USB and power  into the master. Program it with
iD 0
Multiple esc over can checked

Unplug it.

Plug in the USb to the slave and program it with
Id1 
Multiple esc over can checked
Send status over can checked.

Unplug

Plug the can cable into both. Power them both. Plug the USB into the master. go to the connection tab and click connect. It should be the master, and read. Still on the connection tab, type 1 into the can fwd box and enable can fwd on the connection tab. Click connect it should be the slave then read. 

You cannot plug in the usb to the slave and connect to master over can, because the master isn't sending it's status to the bus. 

Hope this helps...
[/quote]
It's all here, at least for the dual config in BLDC Tool (sorry, i don't know about VESC Tool usage) and plugging timing and setup. The rest is to define the values for your setup (motor max, min, batt max, min, watts if "watt control" is used, etc.) But you should already have those values as we're suppose to build around them.

Sorry, I can't point you toward a YT tutorial or something like that as I don't use them andr the infos I use are in this very forum or in French language. :frowning:
```

---
## \#19 Posted by: Deckoz Posted at: 2018-04-17T22:22:52.044Z Reads: 86

```
[quote="Slak, post:18, topic:52495"]
VESC Tool usage
[/quote]

Pretty much all the same tabs in a different layout that's pretty.;)
```

---
## \#20 Posted by: Deckoz Posted at: 2018-04-17T22:26:45.835Z Reads: 81

```
Do y'all need a YT video? Lol..

Ok..
```

---
## \#21 Posted by: Toughook Posted at: 2018-04-17T22:41:01.194Z Reads: 78

```
Not need, just politely asked.
```

---
## \#22 Posted by: Deckoz Posted at: 2018-04-17T23:24:39.585Z Reads: 79

```
Exporting from premiere now... ;)
```

---
## \#24 Posted by: briman05 Posted at: 2018-04-18T03:12:58.852Z Reads: 75

```
Look up esk8 support he does an hour long in-depth video on the vesc.
```

---
## \#25 Posted by: Danny414 Posted at: 2018-04-18T16:26:31.323Z Reads: 73

```
Just wanted to thank you for your response. It's working now :)
```

---
## \#26 Posted by: Danny414 Posted at: 2018-04-18T16:26:50.310Z Reads: 73

```
Just wanted to thank you for your help. It is working :)
```

---
