# A Mechanical BMS - Just an Idea

### Replies: 16 Views: 865

## \#1 Posted by: Monte Posted at: 2017-08-26T15:00:03.851Z Reads: 160

```
Hi,
So today i had the idea of an *Mechanical* BMS. The cells would be connected via (many) switches to change to complete pack from an 10S4P into an 1S40P. This way, the complete pack would balance itself.
I made a simple 2S1P and connected them via 3 switches to change tha pack into 1S2P. But for this i already needed 3 switches, For more cells, the 'switch count' would get higher 
exponentially. Thats a problem of course.
So here is my Question: Is there some kind of 'multi switch' to change many poles at once to make it simpler and safer? Safer would be more important here ;)
Here is a simple way to do this:
<img src="/uploads/db1493/original/3X/8/5/851caaf94d337903fd180bb8fb46edc8d6233c87.png" width="500" height="500">
I know it looks weird :/
```

---
## \#2 Posted by: Monte Posted at: 2017-08-26T15:05:16.372Z Reads: 154

```
I made this with old crappy laptop cells and 5 cent switches from China :P
<img src="/uploads/db1493/original/3X/b/9/b98d823899cc5dcfde4c04e51269e6d3a4774d9c.JPG" width="690" height="460">
```

---
## \#3 Posted by: FredSaberhagen Posted at: 2017-08-26T16:04:16.310Z Reads: 148

```
Kind of a cool idea.  I think the safety factor would be a "break before make" so you don't short everything. Also add a resistor into each path to control your rate of current balancing.

The big problem to think about is this:what happens in your scenario if you have a dead cell at 0v?
```

---
## \#4 Posted by: Namasaki Posted at: 2017-08-26T16:51:33.817Z Reads: 143

```
What's the point?
An electronic bms does everything your trying to do and much more with greater convenience and comes in a tidy, small and lightweight package. 
Technology should move forward not backwards. 
Your going backwards
Sorry if that sounds mean or rude but the truth isn't always kind.
```

---
## \#5 Posted by: Monte Posted at: 2017-08-26T18:20:48.779Z Reads: 130

```
@Namasaki 
The point im trying to acomplish here is to share my Idea. Nothing more. Just a project to waste some time. Im bored :D
But if the ppl help me, (As i said, i know the parts, but i cant find them bc i dont know its names) this could be a 5$ Bms.
```

---
## \#6 Posted by: Monte Posted at: 2017-08-26T18:23:16.497Z Reads: 122

```
Sorry i took a nap :P Resistors sounds good. What Ohm would be the best?
I was thinking about an Volt drop alarm. I saw that somewhere on Hobbyking. And 1S stuff is the cheapest right?^^
```

---
## \#7 Posted by: Namasaki Posted at: 2017-08-26T19:25:47.004Z Reads: 112

```
I had hope that I could shock you back to reality. 
Since that didn't work. 
The switches your using will not handle the high voltage and current of an Eboard with a full size battery.  The explosive arc that will happen inside them when you switch them will burn them up. 
If you are determined to try this, then please wear protection clothing and a face shield and keep a fire extinguisher handy.
```

---
## \#8 Posted by: FredSaberhagen Posted at: 2017-08-26T20:10:18.789Z Reads: 104

```
Well a resistor would help with that.   Pick around 500 ohms.  Keep it in the  <10mA that way
```

---
## \#9 Posted by: Vanarian Posted at: 2017-08-26T20:23:14.767Z Reads: 104

```
Here comes Vanarian, defender of silly ideas!

Actually you could use  automotive relays coupled with fuses instead of your switch (which are truly not good) 

There are plenty able to carry your power levels and you can control them with arduino. Bulky but  I like that.

That's not going backwards, that's thinking out  of the box. You can have 10 ideas and only one useful in the lot to succeed.  Way to go, keep us updated!
```

---
## \#10 Posted by: JdogAwesome Posted at: 2017-08-26T21:53:42.064Z Reads: 88

```
I do have to agree with @Namasaki here, it's pretty impractical, but I think it's always a good idea to thing outside the box!  First off using mechanical switches or relays is going to be crazy bulky and dumb so I think maybe MOSFET's in some sort of configuration would be the only way to do it. Other than that, yeah a normal BMS is gonna be a lot easier and practical though why not!
```

---
## \#11 Posted by: Monte Posted at: 2017-08-27T10:31:48.571Z Reads: 68

```
Well, this small switches are just for testing. I know that this tiny guys cant handle 36V with 40 AMP and much more.
```

---
## \#12 Posted by: Monte Posted at: 2017-08-27T10:37:35.948Z Reads: 64

```
Whoa, i dindnt think(ed?) about relays. Good idea :relaxed:
But why should i need a Arduino with that? The Relays i know start to work ar 12V. If i build a Step down converter into it i can control them all with one switch. THat sounds even more complicated with more cables but i would love to try it with old Laptop Cells :P The problem with this would be the costs of the Relays, i would need much more than 10 relays. And they cost around 12 bucks for a (Qualitative) good one. :/
```

---
## \#13 Posted by: goldenHusky Posted at: 2017-08-27T11:54:48.876Z Reads: 54

```
I would get some logic level mosfets and an arduino nano
```

---
## \#14 Posted by: Namasaki Posted at: 2017-08-27T13:34:42.364Z Reads: 45

```
Using old laptop cells for a little science project is one thing.  
Powering  an Eboard with them is a whole other matter. 
This has been discussed time and time again. 
They are normally  not capable of handling high current drain and could turn your board into a rolling bon fire
Better keep your fire extinguisher handy
```

---
## \#15 Posted by: Monte Posted at: 2017-08-27T17:58:11.521Z Reads: 33

```
Yeah i wouldnt use them for an Board. Untill i get to that point its a long way i guess. :D
I got here more than 100 cells i didnt testet. If i get to the point where this Idea might work, i would use this cells in a large pack. like 10S8P or something. (Would be a bit op i guess but whatever)
```

---
## \#16 Posted by: smurf Posted at: 2017-08-27T18:28:03.236Z Reads: 29

```
This is how I balanced all my batteries in parallel

https://www.instagram.com/p/BUpRI3eFWo1/
```

---
