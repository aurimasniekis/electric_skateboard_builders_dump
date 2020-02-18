# Upgrading VESC firmware, need same version BLDC-tool?

### Replies: 7 Views: 1817

## \#1 Posted by: 3sly Posted at: 2016-05-23T00:06:22.922Z Reads: 150

```
Hello everyone,

Since I'm soon diving into configuring the VESC, I've been reading up on it for the last few hours (2am right now yikes).
I've got mine from esk8.de and they have some straightforward tutorials: albeit in german.

At the bottom of the following link, those that can read german (or can find the google translate button), can see that they oblige you to use the BLDC-tool of the firmware currently installed to install a newer firmware: eg if I have currently 1.14 on the board and would like to go to 2.17, I'd have to use BLDC-tool version 1.14 to install firmware 2.17 after which you should switch the BLDC-tool to version 2.17 as well. 
[http://www.hellray.de/tutorials-d-e-f/](http://www.hellray.de/tutorials-d-e-f/)

How come? This is literally the only place I've read this, I can't find any info to back this up. Any suggestions or alternative sources? Finding this scattered info is quite discouraging, because I don't want to miss anything.

Kind regards,
Dries
```

---
## \#2 Posted by: DougM Posted at: 2016-05-23T02:08:05.568Z Reads: 140

```
Yes, the BLDC tool has to be matched to the firmware.  This is because the firmware adds new features that the old BLDC tool won't know about, and updating older versions is a lot harder than just releasing new versions.

If you are using the windows version of BLDC tool you might not be able to update the firmware from within the tool - I have never been able to get this to work.  So you have to be setup to flash outside BLDC tool.  Or use the Linux rev.

DougM
```

---
## \#3 Posted by: treenutter Posted at: 2016-05-23T02:39:59.311Z Reads: 124

```
@3sly what @DougM said is right. This is the way that BLDC tool currently functions for all VESCs. It's no problem though, you just start with a matching version of BLDC Tool and upgrade from there.
```

---
## \#4 Posted by: chaka Posted at: 2016-05-23T03:28:16.225Z Reads: 116

```
Well you guys are partly right. You need the matching bldc-tool to configure the VESC but you can update an older VESC/firmware with a newer bldc-tool. In fact I always flash my VESC's with an older version of the firmware and use the newest bldc-tool to update the firmware just to be sure the bootloader is working.
```

---
## \#5 Posted by: 3sly Posted at: 2016-05-23T14:16:13.159Z Reads: 104

```
Thanks @chaka, @DougM, @treenutter for the heads up. Do you guys happen to know a source where all these details are mentioned? As I said this was the only source I could find that said to do this. The info is truly scattered, and as updating wrong firmware is lethal for your VESC, I think this is pretty important information.

I'm probably planning on following vedders 1.3hrs tutorial video, although I have no idea yet if it will be mentioned.

Dries
```

---
## \#6 Posted by: Jinra Posted at: 2016-05-23T14:17:52.452Z Reads: 94

```
here's a great resource guide

http://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#7 Posted by: 3sly Posted at: 2016-05-23T14:20:01.154Z Reads: 89

```
That's a great link looking for that, can't believe I haven't come across it yet. Should seriously be stickied. Thanks!
```

---
