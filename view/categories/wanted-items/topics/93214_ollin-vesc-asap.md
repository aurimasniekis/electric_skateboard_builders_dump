# Ollin VESC ASAP

### Replies: 22 Views: 335

## \#1 Posted by: xatonic Posted at: 2019-05-08T19:01:44.581Z Reads: 146

```
hello, I am attending Bay Area MakerFaire and doing a presentation on my board and In typical electronic fashion, one of my VESCs has failed. The fair is next week and my enclosure is designed to only fit the new Ollin VESCs is anyone interested in selling?
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-05-08T19:08:15.364Z Reads: 141

```
a normal 4.12 will fit.

although you should ask @chaka @OllinBoardCompany
```

---
## \#3 Posted by: Jinra Posted at: 2019-05-08T19:17:22.713Z Reads: 137

```
I'm in the bay area and might have an extra for you, I'll check when I get home.
```

---
## \#4 Posted by: xatonic Posted at: 2019-05-08T19:28:01.032Z Reads: 133

```
I have, he's out of stock and they're in production until next week
```

---
## \#5 Posted by: linsus Posted at: 2019-05-08T19:30:56.940Z Reads: 129

```
Must be more suppliers of the 4.12 hw then ollin..
```

---
## \#6 Posted by: xatonic Posted at: 2019-05-08T19:31:15.709Z Reads: 124

```
I wish that'd work but all my equipment to replace it is staying here in Vancouver when I go, you could ship it and I'll pay for 2 day? not sure if that'd work or not though
```

---
## \#7 Posted by: Jinra Posted at: 2019-05-08T19:32:04.804Z Reads: 120

```
Let me see if I have one first and i'll let you know later
```

---
## \#8 Posted by: xatonic Posted at: 2019-05-08T19:34:45.519Z Reads: 114

```
@linsus my design uses the heatsink on the ollin in it's design so they wouldn't fit
```

---
## \#9 Posted by: Jinra Posted at: 2019-05-08T19:35:21.877Z Reads: 111

```
You can transplant the heatsink to another 4.12 vesc
```

---
## \#10 Posted by: linsus Posted at: 2019-05-08T19:35:32.913Z Reads: 112

```
what he said.
```

---
## \#11 Posted by: xatonic Posted at: 2019-05-08T19:36:20.144Z Reads: 110

```
ok ill see if I can do that as a backup
```

---
## \#12 Posted by: linsus Posted at: 2019-05-08T19:36:43.493Z Reads: 108

```
wait, what fried? Mouser has like 2 days delivery time, just order a DRV and an MCU, reflash it. done
```

---
## \#13 Posted by: xatonic Posted at: 2019-05-08T19:38:43.379Z Reads: 108

```
I'm not sure I've never looked into the board and I've never smd soldered before
```

---
## \#14 Posted by: linsus Posted at: 2019-05-08T19:43:55.566Z Reads: 105

```
![tenor%5B1%5D|220x226](upload://zMS2uoWbjHhMvQGaDIihrCTOP82.gif) 

Go into vesctool and type faults in the terminal. It will tell you whats wrong. If you can start it i'd prob replace both just to be safe. Dont you know anyone that knows how to use a hotair station? Its literally 10 mins of work if your're used to it.

Guessing u might not be familiar with bootloader and how to flash? That could be abit of a learning curve as well.
```

---
## \#15 Posted by: xatonic Posted at: 2019-05-08T19:49:19.003Z Reads: 103

```
ok I'll See if that works when I get home and I know someone with a hotair station but last time i had them repair something they floated all the components and everything was out of place
```

---
## \#16 Posted by: chaka Posted at: 2019-05-08T20:13:51.830Z Reads: 97

```
You do not need to reflash a new drv chip. It is a mosfet driver not a processor.

@xatonic welcome to the forum! Wish we had some fresh units for you but we are all out till next week at the earliest.
```

---
## \#17 Posted by: linsus Posted at: 2019-05-08T20:14:34.088Z Reads: 97

```
Dude. I wrote MCU and DRV..
```

---
## \#18 Posted by: chaka Posted at: 2019-05-08T20:19:31.749Z Reads: 93

```
The proccessors rarely fail... I have only seen them fail due to shorts circuits from reverse polarization or leaving the canbus plugged and only powering one vesc. I hope I didnt hurt you too much with my words. Was just trying to eliminate unnecessary steps for @xatonic
```

---
## \#19 Posted by: linsus Posted at: 2019-05-08T20:57:22.144Z Reads: 78

```
Sorry, long ass day at work. Bit unhinged. Didnt mean to be rude.

Think Ive had MCU fails on 20-30% of all DRV failures. One of my older vescs had both swapped so many times it wont take another swap without pads getting ruined. 

Not knowing what problem he has I simply assumed it'd be safer to order both if hes up for the challange
```

---
## \#20 Posted by: xatonic Posted at: 2019-05-08T21:25:09.074Z Reads: 68

```
What's what? Sorry I'm a highschooler in the top of my engineering classes (they wanted me to show my custom flex deck battery and the hardware stuff) but I'm not the best with electrical engineering...
```

---
## \#21 Posted by: linsus Posted at: 2019-05-09T07:55:45.376Z Reads: 48

```
Given your short time span, best option is prob to find a piece of working hardware. You can repair the broken one after the fair and gain some knowledge :)
```

---
## \#22 Posted by: xatonic Posted at: 2019-05-09T07:58:38.633Z Reads: 47

```
Yeah that'd probably be best, I wonder if @Jinra ever found that spare vesc
```

---
