# Windows BLDC 2.17?

### Replies: 40 Views: 3626

## \#1 Posted by: cmatson Posted at: 2016-05-13T23:31:40.755Z Reads: 145

```
Does 2.17 exist yet, or do I need to downgrade my firmware and use an older BLDC tool.. I can only seem to find 2.16 on windows.

Maybe @chaka  or @jacobbloy knows
```

---
## \#2 Posted by: jacobbloy Posted at: 2016-05-13T23:44:25.911Z Reads: 145

```
yes it does but I'm hoping that in the next 3 days i will be merging my work into bldc tool, this will add some cool features, if your in a rush let me know and i will send u a link
```

---
## \#3 Posted by: cmatson Posted at: 2016-05-14T01:11:52.198Z Reads: 140

```
yea man, we have a group ride planned for next week, so if you could shoot me that link it'd be great!!
```

---
## \#4 Posted by: chaka Posted at: 2016-05-14T01:23:29.308Z Reads: 138

```
You should get a ubuntu/linux machine going if you want to stay current.
```

---
## \#5 Posted by: squad Posted at: 2016-05-14T16:26:24.615Z Reads: 112

```
So that's why I can't connect my new VESC from chaka with my mac... :unamused: FW downgrade seems like the only option for now then.
```

---
## \#6 Posted by: Jeff Posted at: 2016-05-25T22:28:29.318Z Reads: 104

```
Hi @jacobbloy & @chaka 

Just wondering if there is any update on BLDC version 2.17 for Windows? I am trying to configure my latest VESCs from @chaka and only see version 2.16 available on the site: http://vesc.net.au/download-now/

Thanks!
```

---
## \#7 Posted by: jacobbloy Posted at: 2016-05-25T23:01:29.935Z Reads: 103

```
Hey mate last night I updated to version 2.18 for Windows but I don't have the firmware updates yet I'll try and do this today
```

---
## \#8 Posted by: cmatson Posted at: 2016-05-25T23:17:35.500Z Reads: 99

```
can you use the BLDC tool v2.18 with a VESC running 2.17?
```

---
## \#9 Posted by: Jeff Posted at: 2016-05-25T23:22:23.525Z Reads: 97

```
Hey thanks!

I still only see v2.16 uploaded. 

<img src="/uploads/db1493/original/2X/7/71c5efa8b8751bc66a7fa61ecd1bc8fd4ad56d62.png" width="690" height="345">

I apologize if I am missing something, thanks so much for all of you work on this.
```

---
## \#10 Posted by: jacobbloy Posted at: 2016-05-26T01:52:20.157Z Reads: 89

```
The text needs tone updated. I'm testing it know guys!
```

---
## \#11 Posted by: jacobbloy Posted at: 2016-05-26T03:21:51.071Z Reads: 85

```
Having some problems with Windows I will update tonight!
```

---
## \#12 Posted by: elkick Posted at: 2016-05-26T18:05:33.616Z Reads: 80

```
Yes you can. :slight_smile:
```

---
## \#13 Posted by: jacobbloy Posted at: 2016-05-27T08:22:48.882Z Reads: 77

```
Hi guys it's updated!

Improvements
•as5047 encoder support
•improved FOC start up
•easy online firmware updates
•BLE support needs more testing for Windows 

Check out the video
https://youtu.be/Ntt5vjpNwek
```

---
## \#14 Posted by: pcdiy001 Posted at: 2016-05-27T16:11:42.433Z Reads: 80

```
<img src="/uploads/db1493/original/2X/c/c0ea94389aeab1c809f60ed998cddca154682434.jpg" width="506" height="165">
```

---
## \#15 Posted by: Jeff Posted at: 2016-05-27T16:21:46.951Z Reads: 79

```
Thanks @jacobbloy, it worked great for me! Love the new firmware update feature.
```

---
## \#16 Posted by: longhairedboy Posted at: 2016-05-27T17:19:53.654Z Reads: 78

```
and don't use your wife's old shitty laptop to do it with bad USB ports. I was all ready for 2.17 goodness and had bldc tool compiled running and ready. then i had to downgrade to 2.16 using my mac because buggy windows but then used windows to do my settings because buggy mac. 

i need a decent linux laptop with good USB ports i can keep in the garage. It will save me money on playstation controllers. (because that's what i throw when i'm mad)
```

---
## \#17 Posted by: chaka Posted at: 2016-05-27T18:35:03.609Z Reads: 85

```
A crappy laptop will work too.....Linux doesn't care. Linux is the honey badger of the pc world.

https://www.youtube.com/watch?v=4r7wHMg5Yjg
```

---
## \#18 Posted by: longhairedboy Posted at: 2016-05-27T18:38:02.497Z Reads: 83

```
i think it was more about the bad USB ports or possibly drivers than the general crappiness of this antique Compaq. My experience with linux is that it almost always breaths new life into 10 year old hardware.
```

---
## \#19 Posted by: hexakopter Posted at: 2016-05-27T20:23:33.667Z Reads: 83

```
I think you should mark that this is a beta software and the people using it be aware that they maybe damage something. I think it would be better to upload benjamins version of bldc-tool and not your beta software without saying that it isn't the official.

Let me explain. I had a freak out with your version where the motor was spinning from one direction in the other without doing anything. I don't touched my keyboard or mouse and the motor was doing what it wants to do. Dangerous when you didn't expect that.

There are also other bugs I noticed just in a very short time of testing.
- The right and left arrow keys doing other things than in benjamins original firmware
- Tested BLE with my HM-10 module and it is useless, because writing is not possible
- After connecting over BLE once it isn't possible to disconnect and using USB when you have it available. You need to reopen bldc-tool and then connect to USB without BLE first

All tested under Mac OSX.

I also compiled your GUI by myself and putted it on an iPhone, because you didnt share it after PMing you. There it is also not possible to write settings and after seeing some strange minimum duty cycle readings etc. its maybe better that this isn't working and destroying some settings. :grin: (But there I know that I am a beta tester, because compiling it myself and that is ok for me) Not like the bldc-tool for Mac where no one knows that he maybe drive his board into the wall, because of a bug.
```

---
## \#20 Posted by: elkick Posted at: 2016-05-27T21:03:46.193Z Reads: 79

```
Just FYI: Calc CC in FOC mode is wrong (BLDC Tool V2.17 and V2.18) in those Win and OSX versions.
```

---
## \#21 Posted by: hexakopter Posted at: 2016-05-27T21:23:20.203Z Reads: 77

```
Thats right. In the newest version by benjamin vedder available on github that problem isn't there.
I can only recommend compiling the official source by yourself. 
I am tensed when the first one fries his VESC when testing the online firmware update thing. Hopefully there is now bug in that firmware tab. That would be annoying.
```

---
## \#22 Posted by: Bender Posted at: 2016-05-28T02:37:40.197Z Reads: 72

```
Could you elaborate please
Are there settings that should be corrected?
```

---
## \#23 Posted by: elkick Posted at: 2016-05-28T07:11:36.890Z Reads: 69

```
The values which are calculated are wrong and then the wrong values are applied. Only work around is to either use Ubuntu 2.18 or to stay with 2.16 on those other OS.
```

---
## \#24 Posted by: Bender Posted at: 2016-05-28T12:12:28.373Z Reads: 68

```
Thank you!
That's pretty important stuff
```

---
## \#25 Posted by: elkick Posted at: 2016-05-30T09:03:34.541Z Reads: 65

```
Doesn't seem to be important for others. The faulty and modified versions of the BLDC Tool are still up and being downloaded. 

I only can urgently advice to use 2.16 Version of the BLDC Tool on OSX and Windows or go for the original one (currently V2.18) from Benjamin on Ubuntu! Using those faulty version of the BLDC Tool can cause fatal failures!
```

---
## \#26 Posted by: Jinra Posted at: 2016-05-30T09:09:48.451Z Reads: 64

```
Maybe you should message @jacobbloy directly?
```

---
## \#27 Posted by: elkick Posted at: 2016-05-30T09:18:53.595Z Reads: 63

```
Has been done already, also by others.
```

---
## \#28 Posted by: jacobbloy Posted at: 2016-05-30T09:44:06.391Z Reads: 62

```
hey guys yes this is correct but i am currently working on this as I'm typing, it is an error with FOC.
```

---
## \#29 Posted by: jacobbloy Posted at: 2016-05-30T10:30:19.501Z Reads: 60

```
ok guys atm the BLDC TOOL will just be benjamins version for windows and OS X.
i will fix the issue asap it will be done soon but i just ask if maybe 2 or 3 could jump on a pre release test group that i can send you the software before i release and you test as it is almost impossible for me to get all of these bugs out.
```

---
## \#30 Posted by: Randyc1 Posted at: 2016-05-30T16:20:50.017Z Reads: 60

```
Does this mean Jacobs 2.16 version I downloaded 3 weeks ago has bugs ?
```

---
## \#31 Posted by: jacobbloy Posted at: 2016-05-31T06:30:10.391Z Reads: 58

```
No! 2.16 was just behaving vedders code in 2.17 and 2.18 I interested some new features for those that wanted to use it but when doing so I have just over looked a few connections in the code!
```

---
## \#32 Posted by: longhairedboy Posted at: 2016-05-31T16:36:31.083Z Reads: 54

```
ugh i need a new laptop at home for this. i need to be running ubuntu, i'm tired of the osx/windows dance i have had to do the last couple of times.
```

---
## \#33 Posted by: jacobbloy Posted at: 2016-06-04T02:27:10.038Z Reads: 52

```
whats been up with it?

except for this one version that was only available for 1 day, it is always built direct from benjamin vedders git hub project, the one problem might be drivers on windows.
```

---
## \#34 Posted by: hexakopter Posted at: 2016-06-09T21:16:41.170Z Reads: 50

```
It was longer available then one day. Just saying. Don't lie to your customers.
```

---
## \#35 Posted by: flatsp0t Posted at: 2016-06-09T22:11:54.821Z Reads: 48

```
What are you paying for?
```

---
## \#36 Posted by: hexakopter Posted at: 2016-06-09T22:29:52.661Z Reads: 46

```
More bricked VESCs and electric skateboards?!?
```

---
## \#37 Posted by: flatsp0t Posted at: 2016-06-09T22:31:51.897Z Reads: 46

```
Well, i just asked because you spoke of customers, which implied you are actually paying for it?
```

---
## \#38 Posted by: hexakopter Posted at: 2016-06-09T22:39:06.211Z Reads: 44

```
No, that implied that customers are paying for it with destroyed VESCs and with the "random speed bug" (maybe you read my posts back) some electric skateboards.
What I destroy myself are my own problems when compiling my own code. But others are dependent from his builds and maybe trust that it is working.
```

---
## \#39 Posted by: flatsp0t Posted at: 2016-06-09T22:49:46.200Z Reads: 43

```
I agree fully with that, faulty code could cost money, i just wanted to say that nobody is his customer here(except for Hubs but this is a different story) as he does not actually sell VESCS or so.
```

---
## \#40 Posted by: hexakopter Posted at: 2016-06-09T22:56:05.057Z Reads: 44

```
Oh, interesting. When I am not fully wrong and remember correctly there was a ordering option a few weeks back on his website to order VESCs. So I was thinking he is still selling them and his customers download also his bldc tool versions. Sorry about that wrong outdated info I had.
```

---
