# How many additional caps for 12s vesc for long wires

### Replies: 18 Views: 1435

## \#1 Posted by: ieatflys Posted at: 2017-05-01T22:01:06.154Z Reads: 164

```
Hello there.... im building a mountainboard using the torqueboards vesc (x4) and implementing a 6374 motor at 190kv on 12s.....  there will be two vesc off of each length of positive and negative power wires that go to the front and rear of the board.

My power wires are undoubtfully going to be long and i have read in many places that i will need to add capacitors across the leads near the vesc to help make up for the battery cable length.

My question is.... is there a rule of thumb to follow for how many capacitors to add per length of battery wire? My battery will be going through a pcb a switch or two and then battery wire then be vesc... should i be counting my diy pcb as battery wires? Im assuming so.  Can i use one capacitor bsnk for the length of wire that power both vesc? Or do i need to double it since there are 2 vesc pulling power through the same wire?? My electrical experience is telling me no but i figured id ask anyway....

If i may ask while i am here as well. My 190kv motors on 12s will come close the the erpm limit... what is the actual limit? And is there a way to set the erpm limit so i do not exceed it?

Thank you all much!
```

---
## \#2 Posted by: Jebe Posted at: 2017-05-01T22:19:29.937Z Reads: 152

```
You can restrict the erpm limit with the BLDC tool. the default is 100k. Limit this to 60k
```

---
## \#3 Posted by: ieatflys Posted at: 2017-05-01T22:51:24.604Z Reads: 147

```
So if i set it to say 58k i should be good right?
```

---
## \#4 Posted by: Jebe Posted at: 2017-05-01T22:59:04.159Z Reads: 147

```
check out this thread. explains motor selection and erpm really well
https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#5 Posted by: JohnA Posted at: 2017-05-01T22:59:40.472Z Reads: 140

```
"As a rule of thumb, for every 4inch/10cm extra length/distance between battery and ESC, add an 220uF extra capacitance near the controller (electrolytic condensators, voltage the same as the capacitors already installed, low ESR type)" 

Information is from: (they go over everything you could want to know about caps) https://www.rcgroups.com/forums/showthread.php?952523-too-long-battery-wires-will-kill-ESC-over-time-precautions-solutions-workarounds
```

---
## \#6 Posted by: ieatflys Posted at: 2017-05-01T23:02:34.749Z Reads: 131

```
Ok awsome i will do that!!! Thank you guys very much i couldnt find any official details only discussion about it!! What sort of an esr rating would be considered low enough? And should i consider any of my tracing befor the power wires on my pcb as power wire length as well?
```

---
## \#7 Posted by: ieatflys Posted at: 2017-05-01T23:10:58.812Z Reads: 134

```
One additional question for you all.... would it not be better to lengthen my motor wires?? I have read many places this is bad in foc sensored opperation and should be avoided. Especially when the wires will be about 1.5 to 2 foot longer than normal...  would it not be wise to stick with the more capacitors option?
```

---
## \#8 Posted by: Jebe Posted at: 2017-05-01T23:20:38.730Z Reads: 127

```
idk - don't use foc. BLDC sounds bad ass
```

---
## \#9 Posted by: ieatflys Posted at: 2017-05-01T23:23:14.047Z Reads: 126

```
As much as i like the sound i need to be able to use sensors for my setup... and ither way i need to add caps so i dont kill my vesc
```

---
## \#10 Posted by: Jinra Posted at: 2017-05-02T00:34:29.631Z Reads: 116

```
You can use sensors with BLDC, I do it for both my boards.
```

---
## \#11 Posted by: ieatflys Posted at: 2017-05-02T01:12:12.753Z Reads: 111

```
Thats fantastic!!! My batteries need to come in the mail so i can start really playing with these. I will more thssn likely be running sensored bldc!!  Whats the point of foc? Other than being quiet isnt it unreliable and unefficient
```

---
## \#12 Posted by: Jinra Posted at: 2017-05-02T01:15:27.562Z Reads: 110

```
It's unreliable, but quiet. I'm a fan of the BLDC hum anyway.
```

---
## \#13 Posted by: ieatflys Posted at: 2017-05-02T01:20:23.715Z Reads: 108

```
Me as well i will be running that route... however i still need to get a cap bank togeather so i dont blow stuff up
```

---
## \#14 Posted by: saul Posted at: 2017-05-02T06:13:08.242Z Reads: 101

```
190kv on 12s and mtb wheels is going to be stupid fast.

149kv or lower is what you really want. the torque would be awesome! and no worries of erpm limits.
```

---
## \#15 Posted by: ieatflys Posted at: 2017-05-02T06:19:03.643Z Reads: 102

```
Everything is already bought and here in the mail besides caps batteries and trucks....  this is my fith build judt my first with vesc....  its geared high so im cruising at sbout 60 to 80 percent wich is the general efficiency range of motors.... the torque will be just fine with 4 sensored motors on 12s haha
```

---
## \#16 Posted by: ieatflys Posted at: 2017-05-02T06:43:45.968Z Reads: 98

```
So since i am running 2 esc off of the same power wires should i be adding 440uf i stead of 220uf per 4 inches?   Also  do i need to be tskijg current into account like they were mentioning in the post or am i fine going the 220 of 440 uf route?

@JohnA
```

---
## \#17 Posted by: JohnA Posted at: 2017-05-02T09:20:17.119Z Reads: 91

```
@ieatflys I've heard people saying that when you combine 2 ESC's you can merge the caps and be fine with the 220uF per 4 inches. But if you have the room, adding closer to 440uF won't hurt anything and just make the system more robust. From what I understand the Esr value is more important then the uF for this application. We just want it to smooth the voltage ripples out.
```

---
## \#18 Posted by: ieatflys Posted at: 2017-05-02T17:58:01.175Z Reads: 78

```
Fantastic. Thanks @JohnA
```

---
