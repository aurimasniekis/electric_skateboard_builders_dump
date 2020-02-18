# FOCBOX Unity UI for Mac OS

### Replies: 11 Views: 783

## \#1 Posted by: janpom Posted at: 2019-03-26T22:36:54.327Z Reads: 174

```
I tried compiling the [FOCBOX UI sources](https://github.com/EnertionBoards/FOCBOX_UI) on my Mac and it seems to have worked just fine. The compiled app is here: [FOCBOX_UI_1.1.app](https://drive.google.com/open?id=18KFVVznlPuF1Y8EFxoxjTRtuXRDJK_nO). I tested it only very briefly. I can connect to my Unity and changing basic settings worked (tried changing the controls from Forward/Brake to Forward/Reverse and back). Use at your own risk.

![53|287x500](upload://kJrNW0VfOIz0w3EVYQMFgJq4lWF.jpeg) 

@EnertionSupport @Deodand Is there a reason the Mac OS version is not officially available given it's straightforward to compile the sources for a Mac?

Are there plans to releasing the FOCBOX Tool sources? That one is clearly based on the [vesc_tool](https://github.com/vedderb/vesc_tool), which is GPL, so you are legally obliged to release the sources.

Nice work on the Unity, BTW. So far I like everything about it a lot... except the missing Mac software. ;)

Edit: The FOCBOX Tool sources are available (same repository as the FOCBOX UI, only different compile options). The compiled Mac OS app is here: [FOCBOX_Tool_1.1.app](https://drive.google.com/open?id=1tpgb5NapwmkNNClr87ntzkL_TsGKCf5Y).
```

---
## \#2 Posted by: Deodand Posted at: 2019-03-27T14:32:43.201Z Reads: 139

```
The FOCBOX Tool is just a #define in the .pro file of the FOCBOX UI project. "BUILD_MOBILE "  or some such. 

Mainly it has to do with my lack of familiarity with Mac and juggling a lot of different projects we want to see successful. I didn't have an apple computer to test these releases so didn't feel comfortable having them as an official release. That is changing soon :smile:
```

---
## \#3 Posted by: janpom Posted at: 2019-03-27T16:51:23.512Z Reads: 124

```
I see. Cool. I compiled it successfully as well. Here's the app:
[FOCBOX_Tool_1.1.app](https://drive.google.com/open?id=1tpgb5NapwmkNNClr87ntzkL_TsGKCf5Y)

I briefly tested it and it seems to work OK. Thanks!

![02|690x354](upload://zdogIuxrzgg0VeqnOqcXQSOsBQk.png) 

![21|690x355](upload://kV0aNVYYr2oKnURD0mwLx1Y6c1J.png)
```

---
## \#4 Posted by: janpom Posted at: 2019-03-27T22:09:34.812Z Reads: 109

```
@Deodand A few more questions: You advertise iOS support [here](https://www.enertionboards.com/focbox-speed-controller/focbox-unity-dual-motor-foc-controller-esc/). Where's the iOS app? Also, I have two Android devices and I wasn't able to install the Android app on any of them. Are there specific requirements?
```

---
## \#5 Posted by: Deodand Posted at: 2019-03-27T22:47:36.593Z Reads: 103

```
IOS app is currently under development. Can you be more specific on why you were unable to install?
```

---
## \#6 Posted by: janpom Posted at: 2019-03-28T08:04:32.552Z Reads: 92

```
It just said "unable to install app". I didn't dig into details, sorry. The devices used were Google Nexus 5 and Nvidia Shield tablet.
```

---
## \#7 Posted by: ankjaers Posted at: 2019-04-04T12:30:22.363Z Reads: 75

```
App crashes on launch. Can you try put it into a zip archive before uploading?
```

---
## \#8 Posted by: janpom Posted at: 2019-04-04T12:39:30.417Z Reads: 75

```
I can if you ask me nicely :slight_smile: but that won't make any difference. I just tried downloading from the link and running. It worked just fine.

What system do you have? Does it give you any errors?
```

---
## \#9 Posted by: ankjaers Posted at: 2019-04-04T13:46:42.413Z Reads: 66

```
I have a 2019 macbook pro. 

In the os x "Error Report":

Dyld Error Message:
  Library not loaded: /usr/local/opt/qt/lib/QtPrintSupport.framework/Versions/5/QtPrintSupport
  Referenced from: /Users/USER/Desktop/FOCBOX_Tool_1.1.app/Contents/MacOS/FOCBOX_UI_1.1
  Reason: image not found
```

---
## \#10 Posted by: janpom Posted at: 2019-04-04T13:50:10.340Z Reads: 64

```
OK, it's not statically linked.

`brew install qt`

should fix the problem.
```

---
## \#11 Posted by: andrew_b Posted at: 2019-06-27T23:03:56.657Z Reads: 40

```
I have the same problem how do I fix that?
```

---
