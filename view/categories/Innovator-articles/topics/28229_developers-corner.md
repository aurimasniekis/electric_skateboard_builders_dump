# Developers Corner

### Replies: 12 Views: 947

## \#1 Posted by: evoheyax Posted at: 2017-07-21T22:30:29.638Z Reads: 164

```
Hello community!

It dawned on me today the amount of time that I spend writing code that interacts with the vesc: in objective-c, in java, in python and in php so far. But what I also realized is that as it is right now, we are mostly keeping the classes we write to ourselves.

I wanted to create a thread where those who wish to contribute their code on any thing electric skateboard related. Maybe your code will help others solve a problem or understand a complicated concept.

I would encourage those who understand certain concepts to share their knowlegde, so we can all learn and grow together.

The way I see it, between remotes and esc's, and the tools and sites that go with them, we are talking about a lot of code that needs to be developed over the coming years. The more we help each other, the faster we can bring innovations to the community.

So share away...
```

---
## \#2 Posted by: wmj259 Posted at: 2017-07-21T22:54:46.170Z Reads: 154

```
print ('hi')
```

---
## \#3 Posted by: wafflejock Posted at: 2017-07-21T22:55:31.056Z Reads: 153

```
The main thing I've worked on with my skateboard is the controller.  At the time when I started working on it seemed like there weren't a lot of good stable small options around and the RC controller I was using was a monster and chewed through AAs all day.

https://github.com/shusain/eskatecontroller

Shared it a few other places but since we're trying to share code here seems like the right place.  The code has been working for me in a 3D printed shell for about a year (if we don't include the time it didn't work but bug "fixed" or at least worked around).  Definitely had a lot of issues with getting it working but included instructions on the hardware side of things too, just started sending out some of the PCBs to people on the forum here who were interested in being alpha testers and making their own remotes (so far just people getting them and doing basic assembly so not much feedback as of yet, few better diagrams calling out the key pins).

---

Also started working on a web interface to help noobies or veterans alike to find information on parts and piece together a full build to get an idea on price and any other specifications that can be readily computed based on chosen components.  As is it's just a couple hours of tinkering around and mulling things over but possibly will be developed into a thing if I can find a way to reasonably finish and then manage it, just has the basics of some navigation between different component types (categories, and sub-categories) and components.

http://plnkr.co/oh8VtizqeLvDVmHsQjvo

---

@wmj259 I'll be sure to put this in my snippet saver :slight_smile:
https://shusain.github.io/snippetSaver/

^^ works off of local storage so will be blank initially but can populate it with your favorite scripts and quick fixes and does syntax highlighting (ooooo ahhhhh)
```

---
## \#4 Posted by: thisguyhere Posted at: 2017-07-21T23:34:14.347Z Reads: 131

```
i'm on .net stack and kind of started on a group buy management page but haven't had the time to complete it.

may have some time coming up to complete but we'll see.
```

---
## \#5 Posted by: DeathCookies Posted at: 2017-07-24T08:57:56.477Z Reads: 107

```
[quote="evoheyax, post:1, topic:28229"]
I wanted to create a thread where those who wish to contribute their code on any thing electric skateboard related. Maybe your code will help others solve a problem or understand a complicated concept.
[/quote]

Maybe you provide yome Information too? You have not sent me a log file of your app yet that i could integrate it into VDLA....
```

---
## \#6 Posted by: evoheyax Posted at: 2017-07-24T16:17:23.925Z Reads: 98

```
Yes, I forgot about that (the time you first asked me for it was a crazy busy time for me). I'll send you a sample file.
```

---
## \#7 Posted by: darkkevind Posted at: 2017-07-24T16:21:22.637Z Reads: 97

```
I'm .NET stack developer too :smiley:
```

---
## \#8 Posted by: thisguyhere Posted at: 2017-07-24T18:32:40.898Z Reads: 87

```
🤜🤛

Ten chars
```

---
## \#9 Posted by: longhairedboy Posted at: 2017-07-24T18:45:35.720Z Reads: 86

```
I have contributed tears. Not like tears of joy from programming because i don't program these things at all, just play with settings because i don't have time these days to learn lower level languages, but i mean literal tears as i have cried on them when i can't get things to work right so i hope that helps somehow.
```

---
## \#10 Posted by: FredSaberhagen Posted at: 2017-10-14T14:38:13.351Z Reads: 64

```
Dude you put the antenna for your controller right in the middle of the handle - your hand is gonna attenuate the shit out of that signal when you hold the remote
```

---
## \#11 Posted by: wafflejock Posted at: 2017-10-14T16:31:31.978Z Reads: 54

```
You're not wrong but it doesn't really matter signal needs to go 3ft.   I used one for an RC car and used external antenna and power amplifier on that one and works as far as I can see the thing over a block away.

https://youtu.be/juJ8yOPrZew

I guess it makes it sort of a plus that my hand doesn't actually grip around the entire thing but yeah can see in the vid above it works fine, if you put your whole body in front of it you can block it even at a few feet away.
```

---
## \#12 Posted by: philvanzu Posted at: 2017-10-14T16:49:46.810Z Reads: 50

```
lang / env : Java / android
purpose : If you enable bluetooth logging in the developper options, this app can parse the log and extract telemetry data from communications between your vesc and vesc monitor app by ackmaniac, I use it to setup custom audio alarms for faults / temperature / low battery. Could be used for wathever you wanted, advantage is you don't need to build your own  app for vesc monitoring. disadvantage is you need to log all bt traffic in a file and erase that from time to time.

Theoretically you can adapt it to work with any firmware / vesc android app but only tested with ackmaniac fw / app.

That's pretty niche at best, but there may be a few classes of general interest in there.

[github.com/philvanzu/VescAlert](http://github.com/philvanzu/VescAlert)

[youtu.be/qWAfRXSiL5Y](http://youtu.be/qWAfRXSiL5Y)
```

---
