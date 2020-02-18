# Bypassing bms Idea

### Replies: 18 Views: 722

## \#1 Posted by: pat.speed Posted at: 2017-10-01T07:05:33.064Z Reads: 156

```
I'm not quite sure how this would work but it would be very helpful for people that bypass there bms. So normally if you bypass the bms you have no control over how much the batteries get discharged but by adding a simple led we should be able to fix this. So basically all you need to do is connect an led or light or any other thing to the output of the small discharge only bms. Now what will happen is that led will stay turned on as long as your cells are charged but when they drop down to the low cut off on the bms it will turn off the led and viola you know that the batteries are flat. In my mind this should work but I haven't actually tried it. If anyone has a spare bms that can try this for me that would be great as this could help lots of people

Good day
```

---
## \#2 Posted by: pat.speed Posted at: 2017-10-01T07:07:36.628Z Reads: 155

```
Just realised the led will actually blow up from the voltage we run at but a small ubec could be added first to drop the voltage down
```

---
## \#3 Posted by: scepterr Posted at: 2017-10-01T07:08:45.125Z Reads: 150

```
And the idea for some people is to not have the BMS be able to shut off the vesc
```

---
## \#4 Posted by: pat.speed Posted at: 2017-10-01T07:10:51.617Z Reads: 150

```
Yes and this will solve this for them. It would even be possible to add a more complex circuit that activates a buzzer or something to let you know
```

---
## \#5 Posted by: scepterr Posted at: 2017-10-01T07:12:21.123Z Reads: 142

```
[quote="pat.speed, post:1, topic:34448"]
Now what will happen is that led will stay turned on as long as your cells are charged but when the drop down to the low cut off on the bms **it will turn off the esc** a viola you know that batteries are flat.
[/quote]
The idea is to bypass that shut off ability
You don't want anything being able to turn off the ESC other than a fuse or the ESC itself.
```

---
## \#6 Posted by: pat.speed Posted at: 2017-10-01T07:13:33.707Z Reads: 131

```
Ahh sorry typo that was meant to be led
```

---
## \#7 Posted by: scepterr Posted at: 2017-10-01T07:14:18.823Z Reads: 126

```
3 letters and so much confusion lol
```

---
## \#8 Posted by: pat.speed Posted at: 2017-10-01T07:15:16.505Z Reads: 119

```
Haha yeah I was wondering what you meant in the first post
```

---
## \#9 Posted by: PXSS Posted at: 2017-10-01T07:16:05.956Z Reads: 115

```
He meant turn off the led. 

This is possible, you would need a voltage divider to get only between 2v and 5v to the led.
```

---
## \#10 Posted by: pat.speed Posted at: 2017-10-01T07:16:34.081Z Reads: 111

```
Yeah or a Bec circuit that drops the voltage down to 5v
```

---
## \#11 Posted by: PXSS Posted at: 2017-10-01T07:16:59.400Z Reads: 102

```
Simple resistor in line would work
```

---
## \#12 Posted by: pat.speed Posted at: 2017-10-01T07:17:38.059Z Reads: 102

```
Yes or even a small voltage regulator they cost a dollar for like 5 on ebay
```

---
## \#13 Posted by: pat.speed Posted at: 2017-10-02T06:26:27.861Z Reads: 87

```
Anyone able to test this for me?
```

---
## \#14 Posted by: Martinsp Posted at: 2017-10-02T07:11:46.720Z Reads: 81

```
Yes it would absolutely work. You would need a resistor in series with the led that would limit the current and thus prevent the led from blowing up. So say for example you would need a 42 kilo ohm resistor to limit the led current to 1mA @42V
```

---
## \#15 Posted by: Crossfire Posted at: 2017-10-02T07:42:49.871Z Reads: 85

```
I have 2x 5S4P packs in series for 10S4P 30Q lions. I could easily put a lipo checker with buzzer on balance leads. So it will beep at preset voltage.

https://hobbyking.com/en_us/hobbykingtm-lipo-voltage-checker-2s-8s.html?___store=en_us

That way I could monitor 8 cells out of 10 for example.
```

---
## \#16 Posted by: pat.speed Posted at: 2017-10-02T07:53:50.906Z Reads: 82

```
I have that checker too but it is quite inaccurate and you have to disconnect it every time you finish so it doesn't drain the batteries
```

---
## \#17 Posted by: Crossfire Posted at: 2017-10-02T08:05:18.099Z Reads: 80

```
I have a BT module hooked to my focbox so I can monitor parameters without looking under the board. That's accurate enough for me anyway.
```

---
## \#18 Posted by: pat.speed Posted at: 2019-03-02T01:39:06.908Z Reads: 27

```
Hey guys wanted to update this thread, I feel as though this could be very useful to a lot of members now as more people use charge only bms modules. So the idea is that you wire up the bms normally for charge only but then add a led or similar connected to the bms output, this way the led stays lit when the board is powered but when reaching LVC it will turn off without cutting the power to the board. 

In my case I’ve got it set up with my led display showing battery percentage, this way I don’t need a resistor inline with the led and I can see my voltage percent too.
```

---
