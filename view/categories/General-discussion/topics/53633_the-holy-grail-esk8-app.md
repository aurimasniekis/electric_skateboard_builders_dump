# The holy grail esk8 app

### Replies: 30 Views: 1941

## \#1 Posted by: Trdolan03 Posted at: 2018-04-27T06:30:27.182Z Reads: 380

```
Hello everybody,
I have seen so many people request this that i figured I may as well try to facilitate it. I am a freshman in high school and I have an end of year freedom project coming up. I have been into esk8 for about 3 years. I have seen many attempts but none complete. I want to create the holy grail or esk8 apps programmed by everyone here who wants to contribute. I totally understand if you aren’t interested in sharing your code or knowledge but I feel that it is a component which is currently lacking in the market. 
Here are the current requirements:
Cross platform (android and IOS)
Smart watch/Apple Watch functionality 
Setting and mode changes (on @Ackmaniac firmware)
Please tag anyone who might be interested in working on this project. Though I do need something by mid June, I plan to run with this for many years. I think the app should be free but I am open to opinions. 
Alright, who is interested?
```

---
## \#2 Posted by: b264 Posted at: 2018-04-27T07:04:03.328Z Reads: 367

```
You should work with @bradrisse, making more half-done things is the cause of all this.  At least start with what he has done.
```

---
## \#3 Posted by: Toleg Posted at: 2018-04-27T08:46:00.341Z Reads: 359

```
Definitly need an UX designer
```

---
## \#4 Posted by: banjaxxed Posted at: 2018-04-27T08:57:22.438Z Reads: 343

```
Did @bradrisse not decide to keep source proprietary, but offer to release the app for free? Not sure where this leaves it if the app remains unfinished,it did look really good.

My suggestion is to get together with @twan here -
http://www.electric-skateboard.builders/t/ios-app-almost-done/53479?u=banjaxxed

Currently for IOS there is the choice of buying a BTmodule from @rpasichnyk  whoose app checks the module's serial, or paying for the actual app from @emmaanuel
```

---
## \#5 Posted by: banjaxxed Posted at: 2018-04-27T09:03:06.741Z Reads: 308

```
Looks like I'm mistaken about Brad's work, from the screens it would be a really cool incorporation to use his work as a foundation assuming you can use React framework

http://www.electric-skateboard.builders/t/new-esk8-app-for-ios-and-android/

https://github.com/bradrisse/Esk8

https://projects.invisionapp.com/share/C4EWD1ZDP#/screens

It's easy to see Brad s a busy startup dev and is understandable in demand by paying companies, but what he did already for esk8 app looks like real commercial quality.

If you can use it licence-wise, then use it
```

---
## \#6 Posted by: Jc06505n Posted at: 2018-04-27T10:45:18.379Z Reads: 252

```
Ok with all these apps coming out I have 1 question: what are you doing that METR, PERIMETR, Ackmaniac, or eSkate VESC has not already accomplished? If it’s just a project to cultivate your skills then I fully understand but if it’s an attempt to make a free version of applications that are already far along and more advanced in what they do for cost that’s not even over $50...
```

---
## \#7 Posted by: Deckoz Posted at: 2018-04-27T12:19:36.884Z Reads: 233

```
I've built alot of boards.... Every single one of them has a MetR module in it... 

I get y'all want something free and open source... But unlike the VESC, Android and iOS have alot more platforms. Making apps that span generations of OS's and multiple platforms is alot different then changing the pin numbers in the header file before compiling vesc firmware for your hardware revision.

Sure I'll be glad to see another option. But $23 a module for a build, is cheap in comparison to your build. And that money supports Roman's time he's spent, building and improving the app, I've put in at least 10 bugfixes over the past year. Guess what? Roman has fixed them all promptly, because it is rewarding, he has incentive to do such. 

You've got alot to compete with, and keep up with, if you plan to change the hearts of people like me. Even more so if you offer an app without support. When you run into a bug, that's from a phone, you don't have, on an OS you don't have. Where is your incentive to fix it?

If you want to change the hearts of people that run MetR
- you need to be on top of your bugfixes, and know how to setup runtimes to debug in OS your using
- wear and iwatch integrated
- record logs and share them, or use them for viddo overlays
- have a TCP bridge
- have modes
- be able to do motor configs from the app
- be able to write/change any setting on the vesc from your phone
- customize your UI layouts for you, and color schemes
- have a built in terminal for listing faults during a ride(not near PC)

If you somehow manage to do all those, well it would just be a copy. But hey feel free to make something better and change my mind,
```

---
## \#8 Posted by: Scoo_B_SK8 Posted at: 2018-04-27T12:47:47.445Z Reads: 206

```
2 cents...

There will never be a “holy grail” of anything technology wise.  In fact Not sure if that’s the actual name of your app, but I would seriously reconsider renaming it, people’s expectations would be rediculously high.

As a freshman trying to tackle something like this is pretty impressive. Best of luck and look forward to seeing what you come up with.
```

---
## \#9 Posted by: b264 Posted at: 2018-04-27T15:20:36.590Z Reads: 176

```
[quote="banjaxxed, post:5, topic:53633"]
assuming you can use React framework
[/quote]

You can use the react framework if you have wifi at home.  If you don't, then you can't.  It appears to be a bug in the framework.

edit: To be clear, it works for the end-user no matter what.  It's just that you can't actually work on the application without home WiFi.
```

---
## \#10 Posted by: b264 Posted at: 2018-04-27T15:21:54.671Z Reads: 173

```
[quote="banjaxxed, post:4, topic:53633"]
My suggestion is to get together with @twan here -
[/quote]

Nothing that only works on one kind of phone can even be considered for the title "holy grail esk8 app".  I think we can all agree on that.  So @bradrisse is a better choice
```

---
## \#11 Posted by: banjaxxed Posted at: 2018-04-27T15:23:02.287Z Reads: 161

```
Cross-platform makes sense, I meant for them to jump on Brad's repo
```

---
## \#12 Posted by: Trdolan03 Posted at: 2018-04-27T16:17:14.434Z Reads: 148

```
My biggest complaint about all the apps already available is that none of them have smart/ Apple Watch functionality
```

---
## \#13 Posted by: louwii Posted at: 2018-04-27T16:48:05.816Z Reads: 138

```
@Trdolan03
I'm a dev but I don't have time to work on yet another project right now.
Good luck with your app though :)
```

---
## \#14 Posted by: b264 Posted at: 2018-04-27T16:49:02.407Z Reads: 135

```
[quote="Trdolan03, post:12, topic:53633, full:true"]
My biggest complaint about all the apps already available is that none of them have smart/ Apple Watch functionality
[/quote]

Do you have wifi at home?  If so, jump in and help @bradrisse
```

---
## \#15 Posted by: Trdolan03 Posted at: 2018-05-15T04:03:45.455Z Reads: 115

```
So I was looking at his thread and it appears his framework is broken for react.
```

---
## \#16 Posted by: b264 Posted at: 2018-05-15T04:15:27.797Z Reads: 114

```
It's not his framework, it's facebook's framework.  They assume you have wifi at home and if you don't, they make it impossible to use.  I have wired gigabit Ethernet and cellular service.  If you have wifi it will work.  I'm not going to buy a wireless router that I don't want just for this.
```

---
## \#17 Posted by: Trdolan03 Posted at: 2018-05-15T04:36:25.366Z Reads: 119

```
[quote="b264, post:16, topic:53633"]
it’s facebook’s framework.
[/quote]
What does Facebook interact with in regards to his project? Also, I could use some help cloning his github project into react native if anyone is familiar with the process.
```

---
## \#18 Posted by: b264 Posted at: 2018-05-15T04:48:51.252Z Reads: 115

```
facebook created React Native.  Brad used it for this app.
```

---
## \#19 Posted by: Trdolan03 Posted at: 2018-05-15T04:53:32.070Z Reads: 111

```
Oh. Makes more sense. Didn’t know that Facebook is the parent company of react native.
```

---
## \#20 Posted by: b264 Posted at: 2018-05-15T04:55:17.557Z Reads: 110

```
React Native is not a company and thus doesn't have a parent company.
```

---
## \#21 Posted by: Trdolan03 Posted at: 2018-05-15T04:56:19.698Z Reads: 102

```
Yes. My mistake. Is there a simple process for cloning the project from github to a react native project?
```

---
## \#22 Posted by: b264 Posted at: 2018-05-15T04:57:30.700Z Reads: 98

```
What is your github userid?
```

---
## \#23 Posted by: Trdolan03 Posted at: 2018-05-15T04:59:21.186Z Reads: 102

```
[quote="b264, post:22, topic:53633, full:true"]
What is your github userid?
[/quote]

Trdolan03 10 characters
```

---
## \#24 Posted by: b264 Posted at: 2018-05-15T05:01:47.223Z Reads: 101

```
While signed-in to github, go to https://github.com/bradrisse/Esk8

Click Fork

go to your computer and start a bash shell

enter these commands

`cd`
`mkdir code`
`cd code`
`git clone git@github.com:Trdolan03/Esk8.git`
`cd Esk8`

all done
```

---
## \#25 Posted by: Trdolan03 Posted at: 2018-05-15T05:02:16.317Z Reads: 99

```
Thanks a lot. Very helpful.
```

---
## \#26 Posted by: Trdolan03 Posted at: 2018-05-15T05:24:53.723Z Reads: 96

```
[quote="b264, post:24, topic:53633"]
go to your computer and start a bash shell

enter these commands
[/quote]

I am getting an error after entering the command git clone git@github.com:trdolan03/Esk8
"git@github.com.com: Permission denied (Piblickey)
Could not read from remote repository."
Did I do something wrong?
```

---
## \#27 Posted by: Trdolan03 Posted at: 2018-05-15T05:34:29.692Z Reads: 100

```
[quote="b264, post:24, topic:53633"]
bash shell
[/quote]

Just to clear something up quickly. Is it a git bash window I need or is it some other program?
```

---
## \#28 Posted by: b264 Posted at: 2018-05-15T05:38:55.654Z Reads: 103

```
If you are in Windows, run the Linux subsystem for Windows first, then just open a terminal window with `Ctrl+Alt+t`.  On any other operating system, just open a terminal window..

https://en.wikipedia.org/wiki/Bash_(Unix_shell)
```

---
## \#29 Posted by: Colydog Posted at: 2018-07-27T01:57:19.279Z Reads: 64

```
@Trdolan03 Any update? (Asking as an annoying end user who cant help with development because I can't code)
```

---
## \#30 Posted by: Trdolan03 Posted at: 2018-07-27T02:12:08.076Z Reads: 62

```
I ended up changing my school project and dropping this. I no longer have a Mac
```

---
