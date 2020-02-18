# How to charge your phone off your esk8

### Replies: 23 Views: 1147

## \#1 Posted by: lowGuido Posted at: 2017-09-10T20:46:28.826Z Reads: 220

```
no one likes a dead phone, and when you are riding around ontop of a box of juice it makes sense to install a small buck converter to charge your phone/gopro/headlights/other when you need it.
https://www.youtube.com/watch?v=4yYXNMzDFDg
```

---
## \#2 Posted by: jmasta Posted at: 2017-09-10T21:10:29.086Z Reads: 209

```
Keep in mind that this might not work with iPhones. I guess they have some type of resistor for verification 

I built a USB charger from a cheap 5V BEC, powered by my 12V rail. Worked for everything but iPhones 6 and up.  So I had to replace it with a USB charger meant to be installed in a car; read the reviews to find one that works with iPhone
```

---
## \#3 Posted by: Jinra Posted at: 2017-09-10T21:11:54.611Z Reads: 202

```
Where is your 12v rail?
```

---
## \#4 Posted by: jmasta Posted at: 2017-09-10T21:14:54.553Z Reads: 195

```
It's a 12V 3A BEC that accepts full 12S voltage. It powers headlights, tail lights, LED on the push button switch, VESC fan, and USB charger. Basically the 5V charger gets stepped down twice
```

---
## \#5 Posted by: cwazy1 Posted at: 2017-09-10T21:15:28.943Z Reads: 192

```
is there a retrofit way of using my phone to charge my board when it runs out of juice?
```

---
## \#6 Posted by: jmasta Posted at: 2017-09-10T21:21:25.289Z Reads: 182

```
Yeah it could be done, technically, with a step up converter. But it wouldn't be pretty and it wouldn't get you very far.  Your skate battery is probably 50x the watt-hours of your phone.  Don't be fooled the high mAh number. Your phone operates at 1S voltage 

You'd be better off saving your phone battery and  calling an Uber...
```

---
## \#7 Posted by: cwazy1 Posted at: 2017-09-11T00:10:03.753Z Reads: 158

```
haha I was being sarcastic. But good response to my question anyways!
```

---
## \#8 Posted by: Nordle Posted at: 2017-09-11T06:29:09.050Z Reads: 143

```
Haha, but you never know on this forum if its sarcasm or serious..
```

---
## \#9 Posted by: cwazy1 Posted at: 2017-09-11T06:29:49.816Z Reads: 142

```
thats what makes it exciting :)
```

---
## \#10 Posted by: lowGuido Posted at: 2017-09-11T08:10:03.766Z Reads: 133

```
[quote="jmasta, post:2, topic:32816"]
Keep in mind that this might not work with iPhones.
[/quote]

Im not sure if you actually watched the video but im using it to charge an iPhone 6
```

---
## \#11 Posted by: jmasta Posted at: 2017-09-11T08:24:38.862Z Reads: 125

```
Couldn't tell what version it was. The one I built worked with my old iPhone but not the newer ones
```

---
## \#12 Posted by: Gynpe Posted at: 2017-09-11T11:01:37.207Z Reads: 112

```
If the configuration of my battery is 37V which it is, can I do this or will I cook my phone, usb charger and something else?
```

---
## \#13 Posted by: lox897 Posted at: 2017-09-11T11:01:57.584Z Reads: 108

```
Nice video @lowGuido

I have a weird attraction to watching you solder :joy:
```

---
## \#14 Posted by: lox897 Posted at: 2017-09-11T11:04:44.504Z Reads: 110

```
It's a step-down converter. Imagine you're on a staircase and at the very top is the highest voltage, the lowest step is the voltage you want to step down to. Any of the steps in between can still step down to the lowest step. So the answer to your question is yes, but you will need a step down converter which can handle that voltage. A 50v maximum would work fine.
```

---
## \#15 Posted by: lowGuido Posted at: 2017-09-11T11:54:34.625Z Reads: 106

```
@lox897 you should watch the drift trike video. XT60's for days.
```

---
## \#16 Posted by: lowGuido Posted at: 2017-09-11T11:55:42.012Z Reads: 110

```
@Gynpe yeah you can. the buck converter will lower the voltage.
```

---
## \#17 Posted by: pjotr47 Posted at: 2017-09-11T14:24:37.399Z Reads: 101

```
I want to step down a 10s battery what converter can i use?

The 10s is with a BMS but when i set my BMS off there is a voltage of 3volt. The last time that i used a stepdown converter, it starts smoke when i put the BMS of something with the 3v. I want to go to 12volt
```

---
## \#18 Posted by: themegak Posted at: 2017-09-11T14:33:27.976Z Reads: 99

```
Apple is full of shite with their "think differently" tag line and screwing their customers with crap like this at every turn.  Such an evil empire.
```

---
## \#19 Posted by: krloz Posted at: 2017-09-11T14:40:23.912Z Reads: 97

```
I didn't understand your second paragraph but this one takes up to 60v input

https://m.banggood.com/DC-DC-Step-Down-Module-Large-Power-Regulator-Converter-7V-60V-Input-5A5V-Output-p-1096156.html?rmmds=search
```

---
## \#20 Posted by: pjotr47 Posted at: 2017-09-11T14:53:27.186Z Reads: 98

```
Sorry English is not my first language ;) 
The most step down have a input limit. I had used a step down converter but when i set the BMS off, the converter starts smoking because 3volt was to low as input voltage. Now i search a solution.
I hope the picture can help
<img src="/uploads/db1493/original/3X/4/4/44b2b60000ea8d89f819d76076ce5e0489c8f904.png" width="480" height="360">
```

---
## \#21 Posted by: krloz Posted at: 2017-09-11T15:09:28.952Z Reads: 93

```
O ok. Now I understood. Not English native either.  
A step down converter smoking because of a low input id's very weird. Normally they will drop voltage and give something below the input voltage.  Or nothing at all. 
I have mine after a loop key so when it is off it gets 0v. So can't say
```

---
## \#22 Posted by: Blacksheep Posted at: 2017-09-12T14:15:01.907Z Reads: 76

```
Do you disconnect your esc when you charge your battery?
```

---
## \#23 Posted by: mmaner Posted at: 2017-09-12T14:58:05.890Z Reads: 73

```
I've got one of these on my 6s board, but I don't ever use it other than to show people that I can :slight_smile:

http://www.ebay.com/itm/121705400285?ul_noapp=true
```

---
