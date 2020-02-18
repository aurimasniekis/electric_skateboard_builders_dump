# To all Arduino knowers there - Help needed with diy cell meter

### Replies: 10 Views: 711

## \#1 Posted by: Okami Posted at: 2017-11-06T20:01:02.116Z Reads: 97

```
Hi there, Ive been recently struggling with this:

<img src="/uploads/db1493/original/3X/7/2/721305bf34a4aa7e4f20b91f00acdb4afa623c30.png" width="690" height="340">

What I would like to achieve is this:

https://www.electronify.org/basic-component-introduction/bar-graph-display

<img src="/uploads/db1493/original/3X/7/b/7bb23dedec4cfc4063d71d931b4bb5fbf1f7545b.png" width="611" height="332">

Where each bar corresponds to one cell group and also shows its voltage.

--

Extra question I had was this:

https://grabcad.com/library/kicad-bargraph-pcb-for-arduino-esp32-1

Where I could print these PCB's? I know it is not the one I need (would need to create a new one).. but I was wondering where do people order them, for example in count of 10?

EU Sources for pcb making would be nice.. as Thats where I reside ;)

---

Anyways, what I mean is - I would like to get extra help to achieve what I have showed in the pictures..

I want to sort of create my own cell meter but my arduino knowledge is lacking..

All I know for now, is that I can use LM3915 can make everything easier to output to leds of bar graph.

---

Then, using arduino I need to divide voltage for all cell groups I need.. as I remember there was something about dividing the voltage till it gets to 5v level, which the arduino can read.

So yeh, if anyone got that far, would be cool if you could confirm the steps which should be taken to create this.. Im still not sure what else I will need to program and get before programming and so on.
```

---
## \#2 Posted by: saul Posted at: 2017-11-07T04:28:36.212Z Reads: 67

```
still pushing on this i see lol.

for pcbs I use oshpark.com.
they are us, but they do int shipping too. just a longer wait. 

but whats wrong with the hk one? no way you can beat that price.
```

---
## \#3 Posted by: Okami Posted at: 2017-11-07T09:28:10.817Z Reads: 57

```
Well, I think the problem lies in the customization. 

The hobbyking module is nice, but for example, it does not allow more than 6cells in parallel, of course, it would be possible to connect next module.. but would be nice to make the desired led count etc before hand.

I also checked some other options.. so far the IDST module seems the best, but then again it doesnt have coulometer..

--

So yeh, probably need a few local people here who can help me out with this :D

Thanks for the interest non the less :D
```

---
## \#4 Posted by: Der6FingerJo Posted at: 2017-11-07T09:59:03.670Z Reads: 49

```
You are right about the Voltage Divider, for a 6S 25,2V LiPo Pack you would need a ratio of about 1:5.1 to safely get below 5V. 
Then you'd have to connect all cells via those resistors to the analog inputs of the arduino and read the individual voltages and also map them to their real values. By substracting the cell voltages you'll get a delta, which is your individual cell voltage.

As for displaying the Values, wouldn't an actual display be more efficient in this scenario? You could just hook it up and display the values of the cells or bars by programming the display. 
Instead, with a LED board like this you would need to do some sort of multiplexing to get it working just right, in addition to supplying power for all the LEDs using additional transistors (the smaller arduinos can only supply 200mA total).

So, my recommendation would be a simple OLED Display that is controlled via I2C. There are even colour OLEDs which could reproduce the bars exactly.
```

---
## \#5 Posted by: Okami Posted at: 2017-11-07T11:42:34.368Z Reads: 42

```
Yeh, thanks for summary. I have 16x 2 display lyinh around but i somehow never got to programming it.

I think i will just think about this.in the time to come,   the idea.about these little dots / bars just seemed to be good looking and sort of retro.

I guess.i just need.to rig up arduino and get to the point where.i get the needed.values / voltage levels, after that i can choose.which way i want to go to display it. 

Somehow the led graph idea seemed.simple, if i could use another chip which helps.with controlling the leds

--

Part of reason for this would be to have one more indicator to tell voltage level and also keep an eye on individual cells.
```

---
## \#6 Posted by: Kug3lis Posted at: 2017-11-07T14:55:45.199Z Reads: 34

```
It's not recommended to use voltage divider for measuring voltage of battery cell in multicell application. U will have really poor resolution because one cell is 3.7 and another is 35V.  At the moment I am working myself on small balancer which needs to measure each cell voltage.
```

---
## \#7 Posted by: Okami Posted at: 2017-11-07T16:07:27.018Z Reads: 31

```
Yes, ive heard about this also. So what is a better option to measure voltages which are higher?
```

---
## \#8 Posted by: deucesdown Posted at: 2017-11-07T16:56:11.206Z Reads: 30

```
Not sure if this helps, but I saw in a youtube video, haven't tried myself,

https://easyeda.com/

design a circuit and a pcb layout in a webapp, then order the finished pcb from them. Seemed incredibly cheap, like $2 to start?
```

---
## \#9 Posted by: saul Posted at: 2017-11-08T09:44:27.387Z Reads: 25

```
I started looking into this in more detail on a random night, he's right at a certain voltage the resistors would dissipate too much power. you'd need 1w+ resistors which are huge. and it becomes wasteful.

I started looking into optto isolators, I think its the way to go but at that point its basically the start of a full bms. which is not a bad thing, but it will take more time and work...

https://en.wikipedia.org/wiki/Opto-isolator
```

---
## \#10 Posted by: Okami Posted at: 2017-11-08T09:48:26.028Z Reads: 24

```
Thanks for info. Will try to take a look at it soon
```

---
