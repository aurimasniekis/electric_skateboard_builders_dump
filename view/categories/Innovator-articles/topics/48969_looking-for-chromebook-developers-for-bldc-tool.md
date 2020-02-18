# Looking for chromebook developers for BLDC tool

### Replies: 37 Views: 1119

## \#1 Posted by: dg798 Posted at: 2018-03-13T12:57:26.806Z Reads: 134

```
I am a high school student and I have a chromebook as I don’t really need a windows or Mac. I was wondering if anyone knows or can make a bldc tool chromebook app or extension. I think it would also be very useful to students who have chrome books as well who want to be able use the bldc tool on also.
Chears
```

---
## \#2 Posted by: laurnts Posted at: 2018-03-13T13:44:00.111Z Reads: 133

```
It's cool to have this on browser (browser bldc tool), however I think doing this type of development is quite some work since there is less browser developer instead of standard unix / windows app developer. Nevertheless you don't have to use it every single day to switch it on (bldc tool), so you could always ask a friend to help you out by borrowing their windows PC for 10 min. I think it's also possible to change VESC configuration using @Ackmaniac firmware just by your phone.

Anyway might be good to move this post to a more appropriate categories :smiley:
```

---
## \#3 Posted by: b264 Posted at: 2018-03-13T14:28:02.879Z Reads: 116

```
There are Ubuntu builds which run on the same kernel, it may not actually be that hard to do.
```

---
## \#4 Posted by: trigger4point7 Posted at: 2018-03-13T15:34:20.288Z Reads: 101

```
There's many ways to get Ubuntu on a Chromebook apparently. https://www.google.com/search?q=run+ubuntu+software+on+chromebook&oq=run+Ubuntu+software+on+chrome&aqs=chrome.1.69i57j33l3.16374j0j9&client=ms-android-verizon&sourceid=chrome-mobile&ie=UTF-8
```

---
## \#5 Posted by: b264 Posted at: 2018-03-13T16:29:36.018Z Reads: 81

```
That too.  I was referring to getting the Ubuntu version to build for ChromeOS though.  They both have the same kernel if I recall correctly
```

---
## \#6 Posted by: dg798 Posted at: 2018-03-13T16:46:38.400Z Reads: 72

```
I know I could download it through Linux if I get into developer mode and download crouton but I would love to have an extension or app or browser of the bldc tool
```

---
## \#7 Posted by: dg798 Posted at: 2018-03-13T16:46:56.577Z Reads: 74

```
I would have to install crouton to get Ubuntu
```

---
## \#8 Posted by: b264 Posted at: 2018-03-13T16:48:10.062Z Reads: 72

```
...still not talking about "getting Ubuntu"...
```

---
## \#9 Posted by: dg798 Posted at: 2018-03-13T16:48:14.640Z Reads: 71

```
I know I don’t need the tool to turn on but it’s annoying to borrow someone else’s pc every time I need to adjust something
```

---
## \#10 Posted by: dg798 Posted at: 2018-03-13T16:49:00.969Z Reads: 70

```
Chrome OS is a highly modified version of Ubuntu/Linux  and it’s inky terminal is called crosh and you can’t even download stuff from it without going into developer mode
```

---
## \#11 Posted by: Apolo Posted at: 2018-03-13T16:52:22.062Z Reads: 66

```
My school uses chromebooks too lol. Hate them so much
```

---
## \#12 Posted by: dg798 Posted at: 2018-03-13T16:53:01.624Z Reads: 63

```
They are good for basic tasks but not good for coding and running programs as it only used the play store and chrome store
```

---
## \#13 Posted by: briman05 Posted at: 2018-03-13T17:41:57.246Z Reads: 57

```
Just get a basic laptop with windows 7.  Chromebook are basically made for one person and that is old people who still have an aol.com email account and everyone else in there family is trying to switch them over to gmail
```

---
## \#14 Posted by: dg798 Posted at: 2018-03-13T22:33:23.678Z Reads: 50

```
Nah I like my chromebook. Works fine except for certain programs.
```

---
## \#15 Posted by: dg798 Posted at: 2018-03-14T00:45:15.247Z Reads: 46

```
anyone have any ideas??
```

---
## \#16 Posted by: Kug3lis Posted at: 2018-03-14T00:49:51.158Z Reads: 46

```
Chrome OS uses web based extensioms (basically chrome apps) they do not have access to hardware layer so no apart some kind TCP bridge to serial or uart to bluetooth to phone app to tcp
```

---
## \#17 Posted by: dg798 Posted at: 2018-03-14T00:50:30.366Z Reads: 45

```
darn thats what i was afraid of
```

---
## \#18 Posted by: Kug3lis Posted at: 2018-03-14T00:50:53.087Z Reads: 46

```
Oh wait sorry I am wrong there is specific extension for hardware layer :smiley:

https://developer.chrome.com/apps/app_serial
```

---
## \#19 Posted by: dg798 Posted at: 2018-03-14T00:51:45.990Z Reads: 43

```
oh wow i gotta look through that, thanks
```

---
## \#20 Posted by: dg798 Posted at: 2018-03-14T00:55:08.195Z Reads: 43

```
is there a way to impirt the bldc tool into https format?
```

---
## \#21 Posted by: dg798 Posted at: 2018-03-14T00:58:07.869Z Reads: 42

```
i can code using the dev app to get access to the vesc but i still need the bldc tool
```

---
## \#22 Posted by: b264 Posted at: 2018-03-14T14:33:28.283Z Reads: 35

```
[quote="briman05, post:13, topic:48969"]
Just get a basic laptop with windows 7.
[/quote]

It's rude to tell folks to change their computer.  It's usually a hallmark of apple people - but either way, if he likes chromebooks, that's fine.  I think they should be more popular, honestly.  If I didn't use my computer for work and need a faster one, I'd probably use a chromebook or multiple chromebooks.
```

---
## \#23 Posted by: briman05 Posted at: 2018-03-14T17:06:43.708Z Reads: 34

```
I am an apple user however I use and maintain Windows OS at work to run analytical instruments.  Chromebooks are a simple alternative to a PC where you don't need all the crazy specs and just want it to surf the web then yes chromebooks are fine but if you need to run any sort of program or want to load a program it is far easier and more cost effective to get a refurbed win7 system for a few hundred bucks.  I would have suggested to virtualbox the bldc tool as it is compatible several different OS's you could try virtualbox as chromebooks are a linux based OS  then you can load a windows VM and run the normal bldc.

https://www.chromium.org/chromium-os/developer-information-for-chrome-os-devices/running-virtual-machines-on-your-chromebook

https://techblog.jeppson.org/2015/11/install-virtualbox-on-a-chromebook/
```

---
## \#24 Posted by: dg798 Posted at: 2018-03-14T17:07:37.880Z Reads: 29

```
Wow ok I will definitely read up on this
```

---
## \#25 Posted by: dg798 Posted at: 2018-03-14T17:10:45.038Z Reads: 29

```
Although it appears the chromebook has to be in developer mode to get the virtual box.
```

---
## \#26 Posted by: thisguyhere Posted at: 2018-03-14T17:11:08.286Z Reads: 29

```
could you run the linux version of bldc tool on raspbian?  i bet you could with a bit of cajoling if it doesn't work out of the box.

if so, get raspberri pi for like $30.
```

---
## \#27 Posted by: b264 Posted at: 2018-03-14T17:11:46.597Z Reads: 31

```
That's not really a solution unless he wants to buy a Windows license.
```

---
## \#28 Posted by: thisguyhere Posted at: 2018-03-14T17:12:29.921Z Reads: 32

```
hell i might try this just for shits and giggles.

@dg798 how much u gonna pay me if i figure it out?
```

---
## \#29 Posted by: dg798 Posted at: 2018-03-14T17:12:51.877Z Reads: 33

```
What an app or web based bldc tool for chromebook?
```

---
## \#30 Posted by: briman05 Posted at: 2018-03-14T17:13:01.362Z Reads: 34

```
I will say getting virtualbox  to work can be a pain. I have had to set up a VM machine running w2k for older software and it works but its because I have a copy of my exact load that worked and was tested extensively.  You might spend alot of time researching the forums to get a answer to why it isnt working
```

---
## \#31 Posted by: thisguyhere Posted at: 2018-03-14T17:13:28.699Z Reads: 33

```
no, getting bldc tool to work on raspberri pi.
```

---
## \#32 Posted by: dg798 Posted at: 2018-03-14T17:14:16.167Z Reads: 30

```
@thisguyhere I cannot spend anymore money right now. I already have a chromebook
```

---
## \#33 Posted by: thisguyhere Posted at: 2018-03-14T17:16:22.393Z Reads: 32

```
i mean, you options are extremely limited and you're asking for a lot, porting source from one platform to another is not a trivial task.

i've got a rasp-pi kickin around somewhere, i might try it this week.  if it works maybe i lend it to you, no promises tho.
```

---
## \#34 Posted by: dg798 Posted at: 2018-03-14T17:16:52.341Z Reads: 32

```
@thisguyhere very curious to see what u can come up with.
```

---
## \#35 Posted by: dg798 Posted at: 2018-03-14T17:17:13.699Z Reads: 30

```
And I know my options are very limited however I was just curious if there is anything out there
```

---
## \#36 Posted by: b264 Posted at: 2018-03-14T17:18:22.007Z Reads: 30

```
[quote="thisguyhere, post:31, topic:48969, full:true"]
no, getting bldc tool to work on raspberri pi.
[/quote]

What a coincidence, just built this http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116/200?u=b264 for Linux
```

---
## \#37 Posted by: thisguyhere Posted at: 2018-03-14T17:22:12.537Z Reads: 29

```
dafuq, you got 92 repos...
```

---
