# VESC Tool &amp; Ackmaniac Vesc Tool Mac Builds

### Replies: 34 Views: 1921

## \#1 Posted by: Kug3lis Posted at: 2018-07-25T13:58:53.280Z Reads: 338

```
Hi guys, several people asked how to run VESC Tool or Ackamaniac VESC Tool under mac, many suggested to install Windows through Bootcamp, but I thought it's a bit overkill so I went and built both tools for Mac.

https://github.com/aurimasniekis/vesc_tool_official/releases

https://github.com/aurimasniekis/vesc_tool_ackmaniac/releases

The only problem is that if you running latest version Gatekeeper will not allow running unidentified applications. At the moment I don't have Apple Developer license membership so I can't sign these applications to run without problem. But there is a fix:

You will need to open the application called Terminal which is located in:

`/Applications/Utilities/Terminal.app/`

and paste this line of code to disable Gatekeeper (allows to run apps not verified by apple)

```
sudo spctl --master-disable
```
and enter your password and press enter now it should work.

If I am missing latest version just mention me in this topic I will build and release it right away ;)
```

---
## \#2 Posted by: DavidC Posted at: 2018-07-25T20:59:45.750Z Reads: 260

```
Thank you! :stuck_out_tongue:
```

---
## \#3 Posted by: Slak Posted at: 2018-07-26T10:27:09.300Z Reads: 236

```
Nice job !

But I think there is an error in your first phrase (windows instead of mac)...
```

---
## \#4 Posted by: Kug3lis Posted at: 2018-07-26T10:28:53.375Z Reads: 219

```
Oh thanks for notice :P
```

---
## \#5 Posted by: Pimousse Posted at: 2018-07-26T13:29:17.620Z Reads: 207

```
What's the difference with the official VT already available from @rpasichnyk repo ?
https://github.com/rpasichnyk/vesc_tool/releases
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-07-26T13:32:29.719Z Reads: 192

```
No difference I guess ;) I just saw people asking, so I went and made it, as I am compiling it for myself already :) I guess there are probable every tool compiled to mac, but just lost in the posts :)
```

---
## \#7 Posted by: briman05 Posted at: 2018-07-26T15:46:52.619Z Reads: 180

```
I was able to run acks esc tool no problem only problem I encountered was the freezing after firmware update.  but after that it ran with no issues
```

---
## \#8 Posted by: Kug3lis Posted at: 2018-07-26T16:05:42.307Z Reads: 171

```
It's mac issue with  serialport sometimes it freezes then can't find serialport...
```

---
## \#9 Posted by: karma Posted at: 2018-07-27T08:24:11.171Z Reads: 157

```
I can't run it because it says macOS version might be different. What version is this for?
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-07-27T09:09:51.604Z Reads: 152

```
Ahm, minimum version is 10.11
```

---
## \#11 Posted by: Battosaii Posted at: 2018-08-14T01:04:36.876Z Reads: 144

```
WOW thank you so much i hate having to run bootcamp, if it wasnt for my AEM computer for my car i use for tuning id get ride of bootcamp all together but that damn thing only works on windows
```

---
## \#12 Posted by: ArnhemAnt Posted at: 2018-08-27T04:10:36.125Z Reads: 135

```
Not sure what I'm doing wrong, but I have followed the link for the ackmaniac download and when I try open it I get this message.

![32%20pm|423x156](upload://tfBClYlQLejl2EWZvYWKr6YYDnf.jpg)
```

---
## \#13 Posted by: Kug3lis Posted at: 2018-08-27T12:03:49.939Z Reads: 129

```
It's a zip file dont know what are you doing wrong mac should support zip files ;)
```

---
## \#14 Posted by: Andy87 Posted at: 2018-08-27T13:51:53.427Z Reads: 127

```
I had problems to extract the zip file. Tried it on a windows pc and made it with ignoring all error messages but didn‘t tried on Mac yet if really all files extracted
```

---
## \#15 Posted by: Kug3lis Posted at: 2018-08-27T14:00:30.841Z Reads: 124

```
Ahm what kind of error messages? I have tried on multiple macs without a single error on extracting zip file. There was issues with ack build as I haven't included linked QT libs inside application but I fixed it.

Vesc tool is better use the one @Pimousse linked I am bit lazy to go god lengths to relink global libs to internal ones...
```

---
## \#16 Posted by: briman05 Posted at: 2018-08-27T14:01:27.388Z Reads: 123

```
You have to enable the ability to download from an unsecured site basically Max’s really only want to download from the App Store
```

---
## \#17 Posted by: Kug3lis Posted at: 2018-08-27T14:02:48.864Z Reads: 126

```
I think his issue is either zip file is not recognised or he tries to open something wrong. @ArnhemAnt can you make a screenshot what you trying to open?
```

---
## \#18 Posted by: Andy87 Posted at: 2018-08-27T14:05:03.980Z Reads: 125

```
Something like ...not possible to encrypt file...
Unfortunately i‘m out of the office and didn’t made a screenshot.
But in the end it unzipped. Don’t know if everything but will check it in the evening
```

---
## \#19 Posted by: ArnhemAnt Posted at: 2018-08-27T21:35:34.981Z Reads: 118

```
[quote="Kug3lis, post:17, topic:62840, full:true"]
I think his issue is either zip file is not recognised or he tries to open something wrong. @ArnhemAnt can you make a screenshot what you trying to open?
[/quote]


Sorry for the delay. I've played around with this a little more and have discovered that my OS version is not supported - bugger....
![02%20am|424x182](upload://urnEm0SgoBuSSZibcCvP4G974oU.jpg)
```

---
## \#20 Posted by: briman05 Posted at: 2018-08-28T00:53:48.265Z Reads: 113

```
Just update your OS to El Capitan or High Sierra
```

---
## \#21 Posted by: ArnhemAnt Posted at: 2018-08-28T01:24:23.715Z Reads: 109

```
[quote="briman05, post:20, topic:62840, full:true"]
Just update your OS to El Capitan or High Sierra
[/quote]


Not that easy. I'm running the 'old' mac tower and I cannot install any of the latest OS versions on my current system and certainly can't afford to upgrade just yet.
I also tried to download the link above from @Pimousse, but it also won't open. Strangely, there are no error messages with that download, but when I go to open the app, nothing happens. I deleted the file and downloaded again and still the same - nothing. 
Frustrating.
Hopefully, the app that @twan is working on will have full functionality soon so that I can just configure the ESC's through his app. 
Until that time, I have no idea how to get around it.
```

---
## \#22 Posted by: Kug3lis Posted at: 2018-08-28T01:34:24.698Z Reads: 103

```
Get vmware fusion older version or parallels and run windows :)
```

---
## \#23 Posted by: briman05 Posted at: 2018-08-28T02:07:37.808Z Reads: 104

```
Virtual box is a free virtual system and you can load windows 3.1-win 10, Mac OS X also Linux.
```

---
## \#24 Posted by: Kug3lis Posted at: 2018-08-28T02:08:01.387Z Reads: 106

```
Oh right virtual box too... I am just used to vmware :D
```

---
## \#25 Posted by: ArnhemAnt Posted at: 2018-08-28T03:21:53.216Z Reads: 107

```
Thanks guys. I understand that there are ways around this, however, I'm pretty sure that I still have to buy Windows and I don't really want to be forking out additional cash, particularly when it is only to run one single application.
```

---
## \#26 Posted by: Andy87 Posted at: 2018-08-28T04:39:17.125Z Reads: 107

```
[quote="briman05, post:23, topic:62840"]
Virtual box is a free virtual system
[/quote]

...you don’t need to buy anything extra. It’s a free software. Install it on your Mac and it’s simulating the windows invironment. Means you can run windows software on your Mac. For free.

Here a link for download (hope you don’t mind that it’s in German 😉 )
https://www.chip.de/downloads/VirtualBox-fuer-macOS_36053602.html
```

---
## \#27 Posted by: Pimousse Posted at: 2018-08-29T11:00:19.790Z Reads: 107

```
You still need a Windows licence.
Install Ubuntu instead and download VESC Tool directly from vesc-project.com.
There is a linux version.
```

---
## \#28 Posted by: bsancken Posted at: 2018-08-30T19:24:59.861Z Reads: 109

```
[quote="Pimousse, post:27, topic:62840, full:true"]
You still need a Windows licence.
[/quote]

I beg to differ. You don't need a license to download or run windows. After the trial period, it just locks up certain customizations and a watermark which won't affect you.
```

---
## \#29 Posted by: mmaner Posted at: 2018-08-30T19:35:23.304Z Reads: 104

```
@Pimousse & @bsancken you are both correct.  You actually do 'legally' need a license after a 65 day trial period to 'legally' continue use, but ti will continue to run just in a limited sense.

Im an MCSE from way back, Microsoft licensing is shit BTW.  Better than Autodesk, but still terrible.
```

---
## \#30 Posted by: Pimousse Posted at: 2018-08-30T21:45:19.067Z Reads: 102

```
I mean, if it's just a virtualization for making run VESC Tool, the best choice is linux.
Sure you still can use Windows after the trial period.
But what for ?

I do have a virtual machine on Windows 7 with an expired licence. I don't really use it except for specific software only avalaible on this OS.

Open source with Open source.
VESC Tool with Linux.
:slight_smile:
```

---
## \#31 Posted by: evopanop Posted at: 2018-08-30T23:07:33.293Z Reads: 106

```
@ArnhemAnt Take a look here: http://dosdude1.com/software.html That'll let you patch the installer disc (USB) so that you can upgrade to Sierra, High Sierra, Mojave, etc. 👍
```

---
## \#32 Posted by: ArnhemAnt Posted at: 2018-08-30T23:37:44.773Z Reads: 105

```
Thanks for the link.

As for trying to run Windoze on mac, I give up. I borrowed a Windoze laptop from a buddy so that I can run the ESC program for the initial setup. Once I've done this, I'm just going to use the Android app that @Ackmaniac has developed so that I can change things via bluetooth.
```

---
## \#33 Posted by: taco Posted at: 2019-01-27T04:15:23.188Z Reads: 73

```
There's a really fast easy way to bypass the untrusted app blocking in OSX: instead of double clicking the app to open, right click the app and choose "open", then you'll be prompted only once (ever!) to accept the risk of running this software.
```

---
## \#34 Posted by: iespoba Posted at: 2019-08-27T00:40:14.270Z Reads: 23

```
Thank you!!
(you can also right click and choose open on the app rather than using the Terminal command)
```

---
