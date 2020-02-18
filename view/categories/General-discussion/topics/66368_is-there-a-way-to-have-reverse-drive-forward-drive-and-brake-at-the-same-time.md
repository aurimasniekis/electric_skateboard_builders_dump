# Is there a way to have Reverse Drive Forward Drive and brake at the same time?

### Replies: 9 Views: 559

## \#1 Posted by: Toohat Posted at: 2018-08-28T17:29:57.377Z Reads: 111

```
I'm trying to have braking reversing and forward drive at the same time in my remote, but I cant figure out how to do it in BLDC tool and I dont really feel like messing around too much with the settings cuz i know some settings might break my system.
```

---
## \#2 Posted by: Toohat Posted at: 2018-08-28T17:41:08.104Z Reads: 104

```
And on the remote control when I apply a fraction of the throttle it goes way too fast too quick ![Capture|690x405](upload://p86XFtUPndBoh149jR4Wh3faTQI.JPG)
```

---
## \#3 Posted by: AutoItKing Posted at: 2018-08-28T17:44:35.271Z Reads: 96

```
Use Ackmaniac's firmware and VESC-Tool, it has what you want.
As for "too fast too quick", that's normal for current mode. This mode does not control speed but rather current. Think of it like a throttle in a car. The speed depends on the load.
```

---
## \#4 Posted by: Toohat Posted at: 2018-08-28T17:48:23.835Z Reads: 91

```
so I have to install the firmware and the tool for it to work?
```

---
## \#5 Posted by: AutoItKing Posted at: 2018-08-28T18:12:32.259Z Reads: 78

```
"Current" in the normal BLDC- or VESC-Tool will give you reverse and braking but it's a little unpredictable. Ackmaniac's implementation is better if you really need reverse. And yes, you will have to use his tool and firmware.
```

---
## \#6 Posted by: Toohat Posted at: 2018-08-28T18:15:06.928Z Reads: 73

```
I'm kinda scared I waited for 2 months for my focbox and i just got it yesterday and I dont want to break it with a firmware update so I will try the current mode you recommended thanks alot King
```

---
## \#7 Posted by: Toohat Posted at: 2018-08-28T18:27:13.812Z Reads: 65

```
Im moving all the buttons on my remote on current mode but no braking only reverse and forward
```

---
## \#8 Posted by: AutoItKing Posted at: 2018-08-28T18:40:14.342Z Reads: 57

```
Yep, that's what it does. Have you tried riding it? Going into reverse with some speed will brake first then go into reverse. Not the best implementation but it works.
```

---
## \#9 Posted by: Toohat Posted at: 2018-08-28T18:54:54.659Z Reads: 51

```
oh i see, thanks
```

---
