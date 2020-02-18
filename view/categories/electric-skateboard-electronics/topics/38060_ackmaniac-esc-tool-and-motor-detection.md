# Ackmaniac ESC tool and motor detection

### Replies: 16 Views: 1103

## \#1 Posted by: longhairedboy Posted at: 2017-11-12T02:05:24.234Z Reads: 214

```
i know there have been a couple of threads about this already, but i can't find precisely what i'm looking for. I could be blind, or tired, i don't know. What's the fucking trick to easy motor detection in here?

I think i just destroyed a VESC-X doing motor detection. The first one i finally got to detect by bumping the ERPM up to 200 in the detection pane, but the detection process was disturbing and ind of startling. 

Then i did the second one and it stuttered really hard and now it won't detect at all, doesn't spin shit and just says bad detection. I hooked the motor up to another VESC-X and used a benchtop powersupply to run detection on it with 2.18 BLDC tool and its fine. 

spent the last year and a half getting BLDC Tool where i want it and i guess i'm sort of starting over with this. Shit's weird in here. 

Of course i go to load 2.18 back on it to see what's up and make sure i didn't cook something and it tells me i need a programmer for that. WTF, whatever.
```

---
## \#2 Posted by: Jinra Posted at: 2017-11-12T02:17:38.007Z Reads: 210

```
I can guide you if you wanna hop on Skype or something :joy:
```

---
## \#3 Posted by: longhairedboy Posted at: 2017-11-12T02:47:59.940Z Reads: 203

```
i may just do that. have you got an iphone? facetime is the shit.
```

---
## \#4 Posted by: Jinra Posted at: 2017-11-12T02:48:34.021Z Reads: 198

```
I'm on android :P also have Discord
```

---
## \#5 Posted by: longhairedboy Posted at: 2017-11-12T02:58:27.951Z Reads: 192

```
looks interesting, i'm downloading it now.
```

---
## \#6 Posted by: DanSkates Posted at: 2017-11-12T03:05:42.373Z Reads: 185

```
@longhairedboy it'd be great if you could share your results if you figure this out as I'm having exactly the same issues - motor detects fine on previous tool/firmware. Thanks dude! 😁🤘🏻
```

---
## \#7 Posted by: Jinra Posted at: 2017-11-12T03:39:24.091Z Reads: 186

```
Join our discord if you get it!

https://discord.gg/kjQ6VF
```

---
## \#8 Posted by: DanSkates Posted at: 2017-11-12T04:20:41.153Z Reads: 177

```
Thanks @Jinra - by the the pool with the kiddo at the mo - but keen jump on this with you guys another time. 😉 Just realised this app is made by the guys that made the Fates Forever moba - such a shame that game was culled - bloody awesome game!
```

---
## \#9 Posted by: longhairedboy Posted at: 2017-11-12T05:49:52.636Z Reads: 171

```
i literally blew a hole in one of my direct fets trying to run detection.
```

---
## \#10 Posted by: Jinra Posted at: 2017-11-12T05:52:52.790Z Reads: 166

```
Sounds like something was off on the VESC hardware or connection..
```

---
## \#11 Posted by: longhairedboy Posted at: 2017-11-12T06:00:05.403Z Reads: 166

```
i needed my board tomorrow so i dropped another couple of Xs in there and loaded 2.18 back up on there with my saved settings. Decided to try out the windows distro Enertion has posted from my laptop. Nice not having serial port connection issues constantly like i do using it from Mint. 

Anyway, is there secret sauce or do you really have to play with the ERPM every time to do detection? I think what happened to me is i was playing with the duty cycle and set it too low or something.
```

---
## \#12 Posted by: Jinra Posted at: 2017-11-12T06:02:32.295Z Reads: 167

```
not me, i've never had to touch eRPM. HOWEVER, ackmaniac has eRPM set to 60k by default which throttles starting at 80% (48,000 erpm) so I set that back up to 100,000 so it doesn't throttle on my setup.
```

---
## \#13 Posted by: yaca Posted at: 2017-11-12T19:21:30.091Z Reads: 140

```
I did motor detection on focbox with ackmaniacs fw 3.1 and I had to increase the BLDC Parameters to 500 ERPM. Below that value the detection failed with my hub motor. Ackmaniacs ESC Tool has originally w 150 ERPM. BLDC Tool from ackmaniac has 600 ERPM and in FOC even 700 ERPM.
```

---
## \#14 Posted by: longhairedboy Posted at: 2017-11-13T12:07:13.124Z Reads: 122

```
hmmmm. 

I'll try raising it more and see what happens. I ordered a couple of those uart/usb programmer things, not sure why i don't have one already, in case i need to go back on the one i didn't blow up. 

i totally smoked (read: blew the entire center chunk out of) a fet though along with about a dozen other tiny components. I've never seen anything like that. The miles long disclaimer about being able to destroy your hardware doesn't fully convey its ability to quite literally destroy your hardware. I'll post a pic in a minute.

I'm going back in though. I destroyed more 4.12s in BLDC Tool than this. This new challenge is kind of invigorating.
```

---
## \#15 Posted by: Zyb Posted at: 2018-03-16T16:51:00.753Z Reads: 83

```
thanks for this info. i was having bad motor detection and increased original 150 ERPM value to 500 and it came out fine.
```

---
## \#16 Posted by: DevinG Posted at: 2018-04-18T03:13:39.923Z Reads: 64

```
Damn I think I'll step back from this whole project for a few days before I fuck my foc...this bldc tool stuff is to heavy for me right now...:thinking:
```

---
