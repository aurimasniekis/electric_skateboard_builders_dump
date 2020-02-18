# Battery percentage reader?

### Replies: 23 Views: 3016

## \#1 Posted by: Tampaesk8er Posted at: 2017-03-01T02:32:56.164Z Reads: 271

```
I connected my battery percentage reader to the  VESC positive and negative wires but my reader still says 100% battery power, I ran out of power tonight while riding it. Does anyone know how to fix my issue?  
`<img src="/uploads/db1493/original/3X/e/3/e3a1ff1eb99e20a777c17fd2e4e7518a685f0b94.jpeg" width="669" height="499"><img src="/uploads/db1493/original/3X/2/1/21cd450acd2ab83edc7088dd245dc9f770c94f7c.jpeg" width="669" height="499">`
```

---
## \#2 Posted by: Tampaesk8er Posted at: 2017-03-01T02:35:07.976Z Reads: 268

```
I connected my battery percentage reader to the VESC positive and negative wires but my reader still says 100% battery power, I ran out of power tonight while riding it. Does anyone know how to fix my issue?

<img src="/uploads/db1493/original/3X/2/1/21cd450acd2ab83edc7088dd245dc9f770c94f7c.jpeg" width="669" height="499"><img src="/uploads/db1493/original/3X/e/3/e3a1ff1eb99e20a777c17fd2e4e7518a685f0b94.jpeg" width="669" height="499">
```

---
## \#3 Posted by: jmasta Posted at: 2017-03-01T03:03:10.845Z Reads: 255

```
Make sure your meter is set up for your battery. There should be a little button on the back to set the number of cells in your pack. (I can't remember if you have to hold the button while powering it on to access this setting)

For example, if the meter is displaying percentage based on a 6S battery when you are really running 10S, it will always show 100%.
```

---
## \#4 Posted by: Tampaesk8er Posted at: 2017-03-01T03:05:24.219Z Reads: 252

```
im running 2 3S 5000mah batteries. ill check it out, thank you.
```

---
## \#5 Posted by: barajabali Posted at: 2017-03-01T04:21:54.156Z Reads: 243

```
Hold the button on the back before you power everything up. Options Weill come up just go to 6 and then turn the system off and back on
```

---
## \#6 Posted by: Wilsonliang777 Posted at: 2017-03-01T05:38:43.656Z Reads: 232

```
I made the same mistake and did not set my battery reader to 24v.  It was only reading 12v.   The problem is most seller of this reader do not include a manual.
```

---
## \#7 Posted by: rwxr Posted at: 2017-03-01T06:58:03.915Z Reads: 221

```
See this thread:

http://www.electric-skateboard.builders/t/battery-indicator-baiway-ly5-settings/15942
```

---
## \#8 Posted by: Namasaki Posted at: 2017-03-01T08:32:22.450Z Reads: 211

```
<img src="/uploads/db1493/original/3X/8/a/8acef8dccc8e6e97f5d081f6b2fe2ef0cbfc845c.PNG" width="281" height="500">
```

---
## \#9 Posted by: Namasaki Posted at: 2017-03-01T08:39:25.031Z Reads: 195

```
How to get additional functions 

https://www.youtube.com/watch?v=py_LKc1Zt7w
```

---
## \#10 Posted by: Tampaesk8er Posted at: 2017-03-01T10:38:08.671Z Reads: 183

```
Mine doesnt have the button like this one has.<img src="/uploads/db1493/original/3X/a/b/abdc36faa491f0e4e5e7b82a54c660d003994553.jpeg" width="650" height="500">
```

---
## \#11 Posted by: rwxr Posted at: 2017-03-01T12:59:41.476Z Reads: 163

```
Show the back side
```

---
## \#12 Posted by: Namasaki Posted at: 2017-03-01T13:28:14.261Z Reads: 159

```
Mine didn't either. I bought some here and added it myself. 
uxcell 50pcs 6x6x4.3mm Momentary Tactile Tact Switch 4 Pin DIP Through-Hole https://www.amazon.com/dp/B0090VQK7C/ref=cm_sw_r_cp_api_rWSTybXHPZ4Z5
```

---
## \#13 Posted by: jmasta Posted at: 2017-03-01T16:21:54.356Z Reads: 152

```
If it doesn't have the programming switch on the back, you could just program it with a wire the same as with a momentary button.  Temporarily short the terminals shown in the video during power on; release; then short them again and again until you reach your desired setting (each short is the same as a button press)

 The soldered switch Namasaki posted is the best option though
```

---
## \#14 Posted by: Namasaki Posted at: 2017-03-01T16:30:36.012Z Reads: 148

```
I tried shorting the contacts with a wire but it didn't work.
```

---
## \#15 Posted by: jmasta Posted at: 2017-03-01T16:32:49.079Z Reads: 143

```
Hmm then why would a switch work? It's theoretically the same thing. No?
```

---
## \#16 Posted by: Namasaki Posted at: 2017-03-01T16:36:59.055Z Reads: 139

```
That's what I thought but I tried again and again with a wire and it didn't work. 
The switch doesn't connect all points together but connects 2 points on one side and 2 points on the other side at the same moment. It's near impossible to achieve this with 2 jumper wires.
Might as well just get and install the switch
```

---
## \#17 Posted by: jmasta Posted at: 2017-03-01T16:53:40.885Z Reads: 142

```
I trust ya!  Strange they don't include the switch by default

Mine has a single "K1" switch on the back. But it is definitely a different model than yours

<img src="/uploads/db1493/original/3X/7/c/7c0c730e840e007a7fda858ce228be6785074edc.jpg" width="690" height="465">
```

---
## \#18 Posted by: Luke Posted at: 2017-03-01T19:02:46.336Z Reads: 128

```
I have this lcd display. It works as described above :)
```

---
## \#19 Posted by: Mrmoonlight Posted at: 2017-03-01T19:09:39.319Z Reads: 129

```
That's the one I use. Got it off Ebay for cheap. Looks like the same hardware that's on the Enertion Space Cell except that  Enertion's doesn't have the white connector. The wires are soldered directly to the board.
```

---
## \#20 Posted by: Tampaesk8er Posted at: 2017-03-01T22:51:25.233Z Reads: 123

```
Heres a better pic. of mine, It has the 2 switches on back though (K+ and K-).  what sucks is that they only sell the buttons in bulk, all i need is one. Thank you all for sharing your knowledge with me, much appreciated, again i just learned something new. 



<img src="/uploads/db1493/original/3X/c/2/c25644a5b57dcf04fa37f87bd3a995b571dd126d.jpeg" width="669" height="499"><img src="/uploads/db1493/original/3X/a/5/a5a903240c95b61f90b1ba26f2b3ec1f6025a88b.jpeg" width="669" height="499">
```

---
## \#21 Posted by: Tampaesk8er Posted at: 2017-03-01T23:16:53.444Z Reads: 116

```
 Another question, in this diagram, is (Li6 - 6 strings) equal to 6 cells?

 <img src="/uploads/db1493/original/3X/1/8/1825b15bb3491367b0d07268173342079588a0ed.png" width="666" height="500">
```

---
## \#22 Posted by: mccloed Posted at: 2017-03-01T23:38:03.437Z Reads: 110

```
Yes. When it says "LI6" or "L6", this usually indicates 6 cells in series, or 6s.
```

---
## \#23 Posted by: Tampaesk8er Posted at: 2017-03-02T03:49:13.599Z Reads: 98

```
thank you.
```

---
