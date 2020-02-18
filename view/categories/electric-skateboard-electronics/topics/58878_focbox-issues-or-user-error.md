# Focbox issues or user error?

### Replies: 26 Views: 607

## \#1 Posted by: trancejunkiexxl Posted at: 2018-06-14T17:17:32.587Z Reads: 130

```
I purchased a bunch of Focboxes last year in case of an emergency, and well I couldnt get them to work a year later.. I started using the new vesc tool and well they all failed motor detection. Im coming from a Mac and it was really annoying so i switched.. all units stored in esd plastics and kept with my other gear. I have 2 working Focbox left, so I am really lost here...

video clips here
https://www.youtube.com/channel/UCylOj4GQJylVcgIffxXt5ZQ?view_as=subscriber

steps i followed were

1.) find working power,sensor,phase cables use them for every test.

2.)verify correct hw version and install corresponding f/w version from

https://github.com/vedderb/vesc_tool/tree/master/res/firmwares

3.) utilize wizard and setup correct battery max and motor values for 12s setup

4.) test sensorless first then proceed to test sensors.

![focbox|690x352](upload://jPX3FdSshOu2a1UTHM72Yp5RrM1.png)
i know these settings are not optimal I should still be able to motor dectect however

![20180614_095546|281x500](upload://crTaLOlA2kCrYyJVB5YlZvaVHWj.jpg)

I was able to verify all my other gear was OK using different motors and cables so, I know my new battery build is not the issue nor is the cables.. I have been working with Johnny on this issue, and have exhausted all my resources.  Thanks for your time,
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2018-06-14T17:44:48.709Z Reads: 119

```
attempts to utilize enertion software result w/

![focbox1|499x122](upload://gI7JDg01INaLbaoY42aSlX0pktY.png)

i have an ST link, but its going to have to be rewired for focbox as i blv it was meant for TB speed controllers
![20180614_104329|690x388](upload://ejF56MNmILD9Vp2gqmtWeGm0xZ.jpg)
```

---
## \#3 Posted by: Blasto Posted at: 2018-06-14T18:08:41.345Z Reads: 106

```
I think you are confusing tools and versions.

If you are using the vesc_tool in your OP. you need to update the FW to 3.XX and make sure you select the fw for hardware 4.12
```

---
## \#4 Posted by: trancejunkiexxl Posted at: 2018-06-14T18:16:04.499Z Reads: 102

```
im on 3.101 hw:48

![version|364x85](upload://2otzVrN9aEbJM5imyPVrblzIVLy.png)

i have been trying to utilize ESC Tool, as enertion tool doesnt like any version
```

---
## \#5 Posted by: Blasto Posted at: 2018-06-14T18:37:46.115Z Reads: 93

```
You have the wrong HW type... thats why its not working. Focbox is 4.10_11_12
```

---
## \#6 Posted by: trancejunkiexxl Posted at: 2018-06-14T18:39:04.853Z Reads: 91

```
 I installed 

C:\Program Files (x86)\BLDC Tool\Drivers\firmwares\hw_410_411_412

Thanks for your patience, It didnt yield any changes unfortunately
```

---
## \#7 Posted by: Battosaii Posted at: 2018-06-14T18:42:14.399Z Reads: 86

```
I'm gona keep an eye on this since I have 4 newer focboxes I'm gona install soon
```

---
## \#8 Posted by: trancejunkiexxl Posted at: 2018-06-14T18:46:52.136Z Reads: 83

```
Ya man, it's always been easy for me.. now I have zero confidence in what I'm doing lol... building battery was easier than this haha
```

---
## \#9 Posted by: Battosaii Posted at: 2018-06-14T18:52:38.923Z Reads: 80

```
Lol well software is a whole other ball game, I'm not familiar with programming but I'm okay at building things thanks to my Mechanic background.
```

---
## \#10 Posted by: trancejunkiexxl Posted at: 2018-06-14T18:54:27.222Z Reads: 81

```
 @EnertionSupport any chance i could get a little guidance. all units boot up blue, and there haven't been any faults..
```

---
## \#11 Posted by: Ebisane9 Posted at: 2018-06-14T19:50:22.084Z Reads: 70

```
seems you have the wrong hw. what you now need to do is get an st link and reflash it back to hw 412. Pain in the ass but a forum member might have a spare they can ship quickly
```

---
## \#12 Posted by: trancejunkiexxl Posted at: 2018-06-14T20:05:29.585Z Reads: 66

```
i got the st link... focboxes still connect, blv i still got flash capabilities.. ill try to get the pin configuration later tonight, looks like i need a female usb also... :thinking:
```

---
## \#13 Posted by: Blasto Posted at: 2018-06-14T20:09:06.026Z Reads: 65

```
Use the vesc_tool, goto custom firmware tab, choose the default in the 412 folder. All can be done via usb
```

---
## \#14 Posted by: trancejunkiexxl Posted at: 2018-06-14T20:12:57.405Z Reads: 67

```
![location|690x345](upload://3CWmL0ucsctcI9UGx2N7qONpaki.png)

seems like this is the only directory that matches that desription and grabbed 410&411&412

these came with the BLDC installer package.
```

---
## \#15 Posted by: Blasto Posted at: 2018-06-14T22:21:00.963Z Reads: 57

```
[quote="trancejunkiexxl, post:14, topic:58878"]
410&amp;411&amp;412
[/quote]

Yes that is the one
```

---
## \#16 Posted by: trancejunkiexxl Posted at: 2018-06-15T00:32:02.565Z Reads: 51

```
i was afraid you were going to say that, if thats the case then ive been using the correct f/w
```

---
## \#17 Posted by: Blasto Posted at: 2018-06-15T00:36:32.670Z Reads: 50

```
[quote="trancejunkiexxl, post:4, topic:58878"]
im on 3.101 hw:48
[/quote]

I thought you said you’re on hw 48.

In that case, the vesctool might have overwritten the factory bootloader.

So try this:
On vesc_tool
-go to bootloader tab, load it
-custom fw tab, load the 4_10-11-12 default fw manually (yes i know again)
```

---
## \#18 Posted by: trancejunkiexxl Posted at: 2018-06-15T00:37:33.653Z Reads: 50

```
ok givin it a go now
i got a couple of units here the one i have loaded atm is 3.101 hw:48 so the ESC tool says.. well shit now it wont connect anymore. windows still recognizes it tho
```

---
## \#19 Posted by: trancejunkiexxl Posted at: 2018-06-15T01:32:07.493Z Reads: 49

```
thanks for your help guys, I hit enertion up and they will inspect tomorrow.. im hoping that even though I got some of them through a group buy that won't disqualify me from any additional assistance. I should have bought the extended warranty. hopefully since they dont have any miles on them I might be able to get lucky.. thanks @JohnnyMeduse and @Blasto for being patient with my dumbass.
```

---
## \#20 Posted by: Battosaii Posted at: 2018-06-15T01:47:20.828Z Reads: 47

```
I hope they can fix that for you, Focboxes are not cheap 4 of them already cost way more than a complete budget board
```

---
## \#21 Posted by: trancejunkiexxl Posted at: 2018-06-15T02:02:20.531Z Reads: 40

```
Got one up and running now its just 3 broki 🤙😃
```

---
## \#22 Posted by: Battosaii Posted at: 2018-06-15T02:21:01.901Z Reads: 38

```
That's good news!
```

---
## \#23 Posted by: trancejunkiexxl Posted at: 2018-06-16T15:27:27.528Z Reads: 31

```
ok, so after spending time with @CarlCollins in the team viewer session. we made some discoveries...

![152909348718318314049|281x500](upload://fbg7WVBTqMVlUfBCYjaNmgHMUqr.jpg)


i should have opened up the covers and inspected them sooner, could have saved me a little sanity..
Good news is we were able to recover another focbox!! so now i only have to send 2 back. I would really like to say more about what happened with the f/w on the working box however I still am not exactly sure where i went wrong with the fw push.
```

---
## \#24 Posted by: Battosaii Posted at: 2018-06-16T15:28:59.056Z Reads: 31

```
Fuck the DRV blew up and you burned up some direct fets :( man I knew there was something wrong with them I'm sorry dude that blows.
```

---
## \#25 Posted by: Battosaii Posted at: 2018-06-16T15:30:08.033Z Reads: 30

```
Btw did you find a plastic film on the heat transfer pad? That was a manufacturing defect and could have caused this.
```

---
## \#26 Posted by: trancejunkiexxl Posted at: 2018-06-16T15:31:58.360Z Reads: 29

```
they are open on my workbench.. fighting a nasty hangover atm.. LOLZ gonna need a bit more coffee before i get up..

the cause was overheating.
```

---
