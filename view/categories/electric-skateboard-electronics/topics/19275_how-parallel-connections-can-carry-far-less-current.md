# How parallel connections can carry far less current

### Replies: 40 Views: 3806

## \#1 Posted by: Hummie Posted at: 2017-03-18T22:43:01.881Z Reads: 289

```
<img src="/uploads/db1493/original/3X/1/f/1f20788422bc86ee2e3277ecbb68cf1de15541ef.JPG" width="690" height="445">
Let's start with the first pic in top left corner.  If this group of 12 cells are part of a 10s4p pack pulling 50amps, the connection between the fourth cell on the bottom and the third cell will have a total of 1.25 amps, the connection between the second cell and third will have 2.5, third and fourth cells will have 3.75 passing.   So we have ...about 1/40 the current passing through a parallel connector. @Ackmaniac @PXSS this is a common arrangement for a pack and even if we were to use another example from the four I posted the currents will be very similar.  What u think?
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-03-18T23:06:26.809Z Reads: 273

```
Each series pack has to provide the total current. The voltage gets added but not the current. So in the first picture the first 4 cells on the left have to produce 40A. The next pack also 40 amps and so on. Only the voltage gets multiplied from which each additional series connection.

Now I understand where your misunderstanding is coming from.
```

---
## \#3 Posted by: Hummie Posted at: 2017-03-18T23:18:41.142Z Reads: 263

```
Sorry yes ur right and forgot about that and will be 12.5 amps at the bottom, 25 next, then 37.5 amps would be flowing on that top left pic through the parallel connections.   the other examples of batteries above have more series connectors attached to the parallel connections and there will be no more than 25 flowing at most in the parallel connections
```

---
## \#4 Posted by: PXSS Posted at: 2017-03-19T00:52:12.036Z Reads: 249

```
I'm having a date with my gf. I will respond to this tonight at some point
```

---
## \#5 Posted by: Kaly Posted at: 2017-03-19T04:09:49.579Z Reads: 232

```
This is a great place to start getting some clarification on this topic ;-)

http://www.explainthatstuff.com/electricity.html
```

---
## \#6 Posted by: PXSS Posted at: 2017-03-19T11:11:23.785Z Reads: 219

```
@Hummie 
You don't seem to understand how parallel and series connections work. I recommend you do some reading on parallel and series circuits. 

The top left circuit is representative to some extent for electronic skateboard batteries. Most people make the parallel packs and then connect the end cell in series to the next group of parallel cells, just like in the top left drawing. 

I still don't get where you're getting your numbers from, it doesn't make much sense. Specially since you're not including equations. 

Here is the equation you should be using, which I also wrote in the previous thread. 
(N-1)/N * I = Max Strip Current
N = number of cells in parallel 
I = total current 

That will calculate the current flowing between the first and second cell in "parallel". The reason there is current flowing is because you need current to flow into cells 2, 3 and 4. It doesn't just appear there. 

Think about it this way, you have four pumps of water (batteries) running in parallel, they need to output 40 cubic feet per meter (Amps) of water(electricity) together. So each pump needs to provide 10cfm. You have a hose that can carry said volume to pump one but then you connect pump 1 to pump 2 with a dinky hose that can only carry 5cfm, then you connect another dinky hose from pump 2 to pump 3, and a third dinky hose from pump 3 to pump 4. 
Pump 4, although it can output 10cfm, is restricted by the dinky hose you attached to it. Pump 3 can also output 10cfm but now pumps 3 and 4 have to share a hose to pump 2 and then pumps 2, 3 and 4 have to share a dinky hose that can only handle 5cfm and try and put 30cfm through it. The result? The hose stretches and stresses and puts an extra strain in the pumps. It works but eventually you're going to overstrain the pumps and they will burn out. 

Now, same thing with batteries. You can use dinky nickel strips to connect them but you're going to generate heat and have unnecessary voltage sag which will cause your pack to fail sooner than later.
```

---
## \#7 Posted by: Tronik Posted at: 2017-03-19T13:28:20.461Z Reads: 199

```
Ever seen 500 9volt batteries connected?   On youtube and a guy turned a very large heavy metal wheel called Big Bethel,. .  9'vs in series
Series Doubles Voltage
 Parallel - ah
<img src="/uploads/db1493/original/3X/1/b/1b990a173c83b3cf36ca2fc527d53b8b02f448c2.jpg" width="318" height="159">

How about taking spare 36's and doubling down, if not triple to over 100v.  Power a 150# board. Im kinda scared.

<img src="/uploads/db1493/original/3X/1/b/1b990a173c83b3cf36ca2fc527d53b8b02f448c2.jpg" width="318" height="159">
```

---
## \#8 Posted by: SimosMCmuffin Posted at: 2017-03-19T13:50:33.600Z Reads: 197

```
I'm going to add my thoughts on this as well and I'm going to use my own self assembled 6S4P battery pack pictured below, to illustrate. 
<img src="/uploads/db1493/original/3X/2/3/23155fea0d73f35d045defb26bde8cc6c08d978a.jpg" width="690" height="459">


Here's an illustration of the battery (without balance leads):
<img src="/uploads/db1493/original/3X/0/4/048d9aaa4127378a8c851bdad379806445951e55.jpg" width="690" height="388">

Now, let's say we had a nice 40 Amps of current so we get an even 10 Amps flowing through each parallel cell.  Now the next picture has the wires/strips color coded so they show the current/heat/voltage sag in each segment of them.
<img src="/uploads/db1493/original/3X/4/f/4f743676acd7c2513d7b502c9f5cb407165a9626.jpg" width="690" height="388">

As can be seen the heat losses are better distributed across the parallel cell pack. I'll admit though that having one side heated by the resistive losses in the strip and the other side being cooler is still not ideal, but compared to the hummie's example where:
<img src="/uploads/db1493/original/3X/2/f/2f4c830c43a20f31aa70919456109897328c129f.jpg" width="690" height="163">

Now the most top cell is next to the hottest segments of the wire/strip and will heat up the most and will degrade the fastest of the parallel cells

EDIT: Added internal current flow indication to the cells.
```

---
## \#9 Posted by: PXSS Posted at: 2017-03-19T14:20:44.707Z Reads: 183

```
Thanks for the awesome diagram. That's what I've been trying to explain since yesterday.
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-03-19T14:24:05.796Z Reads: 185

```
@SimosMCmuffin  Could you please also make a drawing of my battery pack design. Would be great to visualize the advantages.

Edit: for @SimosMCmuffin Here in this post you find the pictures. Be aware that they will have parallel connections as well later on.
http://www.electric-skateboard.builders/t/laser-cut-plywood-deck-with-solderless-18650/19005/34?u=ackmaniac
```

---
## \#12 Posted by: SimosMCmuffin Posted at: 2017-03-19T14:44:48.053Z Reads: 184

```
<img src="/uploads/db1493/original/3X/1/0/10f7a1c0fa935ca9604afc1bb7a1187e306a7291.jpg" width="690" height="285">

Yes, it's a good setup as you actually have as many parallel wires as you have parallel cells, so you have minimal losses. And ideally you'll have 0 Amps flowing between the parallel cell connections.

PS. I didn't know how you were going to terminate the negative and positive ends so I went with my example, but you can tell me if you plan to do it another way, so I can update the illustration.

EDIT: Battery pack termination updated.
```

---
## \#13 Posted by: PXSS Posted at: 2017-03-19T14:47:06.178Z Reads: 181

```
I wouldn't say 0A on the parallel connections but close enough to it as long as your cells are balanced when you place them in the holders
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-03-19T14:48:11.119Z Reads: 177

```
Connect all 4 to one wire in the middle. So between cell 1 and 2 there is 10 Amps and from 2 to the main wire it is 20 A. Main wire to 3 is 20A and 3 to 4 10A.
```

---
## \#15 Posted by: SimosMCmuffin Posted at: 2017-03-19T14:48:47.442Z Reads: 174

```
Better hope they are pretty balanced before putting them in, or you'll have some power balancing happening otherwise :smile:

[quote="SimosMCmuffin, post:12, topic:19275"]
And ideally you'll have 0 Amps flowing between the parallel cell connections.
[/quote]
```

---
## \#16 Posted by: PXSS Posted at: 2017-03-19T15:07:11.138Z Reads: 159

```
Lol yup. That's how you make wires disappear ;)
```

---
## \#17 Posted by: SimosMCmuffin Posted at: 2017-03-19T15:13:22.699Z Reads: 164

```
I would rather lean on the: "That's how you vaporize Li-Ion cells internally" side of things. Wires should be able to handle the currents without escaping into the atmosphere, especially as you're plugging the cells one by one into the holders.
```

---
## \#18 Posted by: PXSS Posted at: 2017-03-19T15:23:59.199Z Reads: 167

```
I evaporated a holder in an experiment. The battery survived just fine. It had some health deterioration but if I remember correctly it was the equivalent of losses through 5 cycles
```

---
## \#19 Posted by: SimosMCmuffin Posted at: 2017-03-19T15:26:40.819Z Reads: 165

```
Did not assume the use of a holder. Did the holder have the spiral springy clip at the other end? That's what I would suspect to vanish in that case.
```

---
## \#20 Posted by: PXSS Posted at: 2017-03-19T15:48:23.401Z Reads: 161

```
The one posted on Ackmaniac's build. 
I've also evaporated Nickel tabs at around 18A although the spot welding job was sketch
```

---
## \#21 Posted by: Hummie Posted at: 2017-03-19T16:38:36.195Z Reads: 157

```
great pics Simon 
   And you've pulled out the "practically" zero current through the parallel connectors example I've been unable to come up with.   appreciate the help and the cool attitude.
if there's confusion about the numbers I posted for the current going through the strip, my first post was an electronics faux pas as I forgot only the voltages add here, but get to my second post and the numbers are spot on using a 50 amp draw as apposed to the 40 Simon is assuming.    

what are the risks to the cells in one of the poorly designed packs above?  Solely heat in some unlucky cells due to solely their connection having more heat?
```

---
## \#22 Posted by: SimosMCmuffin Posted at: 2017-03-19T17:10:25.875Z Reads: 152

```
[quote="Hummie, post:21, topic:19275"]
what are the risks to the cells in one of the poorly designed packs above?  Solely heat in some unlucky cells due to solely their connection having more heat?
[/quote]


It's pretty much just about where the heat is generated. 

And then there is how many ways you can have the current flow to the next series cell pack, AKA do you have single or multiple parallel wires or double thickness for example for the high current segments to minimize the losses in the high current segments.
```

---
## \#23 Posted by: PXSS Posted at: 2017-03-20T05:18:58.550Z Reads: 134

```
Plus voltage drop on the higher resistance strips, (smaller strip = higher resistance) which affects overall performance by a little I would believe. Not enough to be an issue by itself but if you were already having voltage sag issues, they would only be exacerbated by it.
```

---
## \#24 Posted by: Hummie Posted at: 2017-03-20T05:37:46.544Z Reads: 132

```
I think the resistance of a cell is typically less than these nickel connectors, can the connection resistances all be added and, maybe through extrapolating using the cell's own resistance and sag graph, the sag of the pack can be revealed...and it would be much more than the simple cells?   Sag would be an ohms equation incorporating the resistance of the cells and connections?
```

---
## \#25 Posted by: PXSS Posted at: 2017-03-20T05:45:13.505Z Reads: 130

```
They can be added. It's a little more complicated than that though as internal resistance of cells change depending on their state of charge and temperature. It is very complex to try to model
```

---
## \#26 Posted by: SimosMCmuffin Posted at: 2017-03-20T08:06:58.770Z Reads: 130

```
Here's an article for modeling li-ion internal resistance under different conditions, just to get an idea what all kinds of things are going on in the cell.

https://www.google.fi/url?sa=t&rct=j&q=&esrc=s&source=web&cd=3&cad=rja&uact=8&ved=0ahUKEwjx8bfdzuTSAhVTGsAKHXM5BVgQFggmMAI&url=http%3A%2F%2Fwww.evs24.org%2Fwevajournal%2Fphp%2Fdownload.php%3Ff%3Dvol3%2FWEVJ3-5340444.pdf&usg=AFQjCNHYPJBZVaGonLKhrVaaNZYqTxpUTQ&sig2=EK1cVf9jXB6mJ6JABd2V9w
```

---
## \#27 Posted by: PB1 Posted at: 2017-03-20T12:14:34.832Z Reads: 134

```
Interesting discussion. 

After various discussions with myself and others, this is also how I built my 10s5p battery pack. Directly welded the taps of the "serial cells" so I have 5 individual rows, then added a cross bar in order to be able to balance the pack. 
From the "termination cross bar" I even have two individual, parallel connections to my VESCs.

Main reason was to reduce the current flow in the wires. 

I think building a pack as in post 12 is slightly more effort and more difficult, however it has advantages: 
- reduced current in the connections
- if done properly the pack has some flex
- it's even possible to extend the pack, e.g. from 4p to 5p. 

Disadvantage: 
- pack is less solid
- less variations for pack layout
```

---
## \#28 Posted by: SimosMCmuffin Posted at: 2017-03-20T12:49:40.252Z Reads: 129

```
Can you post a picture of your pack? I'm just wondering how the whole construction looks like.
```

---
## \#29 Posted by: PB1 Posted at: 2017-03-20T21:54:54.796Z Reads: 133

```
Sure, it's all VERY DIY, no fancy tools. I was going to document all of it in a build log - but what the hell, I will never get around doing it anyway. So here you go. 

Started with hot-glueing 5 cells, then another 5. Then spot-welded those taps. Note, my cells came with pre-welded taps in z-form
<img src="/uploads/db1493/original/3X/0/e/0e1c8746be292aa32d1765f02c594ca4e77dbdc4.jpg" width="666" height="500">

In the back my DIY spot welder. Don't do this at home if you don't know exactly what you're doing. I don't recommend it, but it worked. To the right a small 2s5p pack with the cross bar. 
<img src="/uploads/db1493/original/3X/f/b/fbb59eed9f9f7f30c0ee2eb844238b544febc0ba.jpg" width="666" height="500">

Test layout on the board, no soldiering yet. 
<img src="/uploads/db1493/original/3X/2/d/2d7373ffa528e2f66f851344342633914e9f025e.jpg" width="375" height="500">

Soldering the balance wires. 
<img src="/uploads/db1493/original/3X/c/b/cb836aec9811eed4bf9afc0722b56959435d606f.jpg" width="375" height="500">

Then I added two AWG 10 wires with plugs to connect the two 5s5p packs plus two AWG 10 terminals to two VESCs. Tape and shrink wrap. 
The two 5s5p packs are pretty flexible, enough for a medium flex board.
```

---
## \#30 Posted by: SimosMCmuffin Posted at: 2017-03-20T22:52:15.726Z Reads: 126

```
Ok, your pack construction was a bit different from what I had in mind :smile:

Here's my own DIY spot welding setup:
<img src="/uploads/db1493/original/3X/5/2/5206b75756187b8696f7f1ed13705042e5fbd306.jpg" width="333" height="500">

Decided one day that I needed to spot weld a pack together so checked around online for good platform and then saw this on my usual check for new articles on hackaday: http://hackaday.com/2016/03/22/arduino-nano-runs-battery-spot-welder/ and coupled my own version of it together with components off of my shelf. Hella ghetto I admit, but it gives a configurable double short circuiting pulse for the battery triggered with a dead simple foot switch.

Anywhoo, I thought you would have done your battery pack welding like this:

<img src="/uploads/db1493/original/3X/9/d/9dd40aa450bf508b5df29511361978081c5c3f6f.jpg" width="458" height="499">
First weld ready 5P packs from both side with strips.

<img src="/uploads/db1493/original/3X/9/e/9e815b2492438e276212cc00f05c4974fe3d3f19.jpg" width="481" height="499">
Then add the parallel strips while the parallel cells are oriented like this. Orange arrow shows the connection logic.

<img src="/uploads/db1493/original/3X/9/9/99dd67ec01e0782914a2db0a18c51a0877d39f0a.jpg" width="690" height="304">
<img src="/uploads/db1493/original/3X/d/5/d5f0d831cd7231b38326b0cf3678902c31374f5c.jpg" width="690" height="287">

Then just fold the pack out (The bends are over emphasized on the lower pic for illustration purposes). Recommend adding the balance leads before doing that though.
```

---
## \#31 Posted by: PB1 Posted at: 2017-03-21T11:40:43.418Z Reads: 119

```
Ghetto style rulz :grin:

Different process, same result. 

Remember, my cells already had z-tags. Really like your process otherwise
```

---
## \#32 Posted by: SimosMCmuffin Posted at: 2017-03-21T11:44:29.798Z Reads: 119

```
Yea I didn't expect the z-tags, so that's why I thought it was going to be different, but hey, you make due with what you have.
```

---
## \#33 Posted by: Ackmaniac Posted at: 2017-03-21T16:33:18.019Z Reads: 120

```
I am not a pro when it comes to electromechanics so i have a silly question for the pros.
I would be interested if the current in these u turns create a inductance like it happens in the motor or does that only happen when it is a circle

<img src="/uploads/db1493/original/3X/0/d/0dcb5e454ca398a9541be70d4a43864a8ebe429b.jpg" width="440" height="282">
```

---
## \#34 Posted by: Maxid Posted at: 2017-03-21T16:53:17.245Z Reads: 118

```
Can't be much with just half a turn
http://www.66pacific.com/calculators/coil-inductance-calculator.aspx
```

---
## \#35 Posted by: Hummie Posted at: 2017-03-21T18:46:54.437Z Reads: 114

```
I'm no pro but everything has inductance and capacitance to some degree. The inductance profuced being determined by the length and width of wire with shorter and fatter making less inductance.  Maybe put the multimeter on inductance and check the whole pack

I think the coils of a motor or any conductor will reinforce the field so if you simply add a turn or loop to the battery wires it will increase. As u say.  U can cut down the inductance by putting the plus and minus wires beside each other cancelling each other.  the closer the better
```

---
## \#36 Posted by: PB1 Posted at: 2017-03-21T19:28:42.482Z Reads: 112

```
@Ackmaniac, yes, there is a little bit of inductance once the initial current flows or if the current changes direction. 

Then you can really neglect it in this DC part of the whole circuit. Don't think that e.g. recuperation has a large effect.

Edit:DC part of the whole circuit
```

---
## \#37 Posted by: Hummie Posted at: 2017-03-21T19:30:35.949Z Reads: 115

```
I read long wires have caused problems with foc program
```

---
## \#38 Posted by: SimosMCmuffin Posted at: 2017-03-21T20:24:26.237Z Reads: 111

```
Here's a link to Vedder's VESC6 analysis video with timecode pointing to the part where he demonstrates the wires inductance depending if it's a big loop vs. both wires running parallel next to each other: https://youtu.be/x6lPdI9OVQg?t=13m4s

So technically yes. You would have extra inductance in your pack if you were to leave the parallel strips on such a round bend, but in reality you would push them pretty much together with a sharp bend and then the strips would be parallel and next to each other and you also have 5 parallel strips (in the case of the picture you pointed to), which would drop the total inductance caused by them to a 1/5.
```

---
## \#39 Posted by: Randyc1 Posted at: 2017-04-20T15:44:37.225Z Reads: 96

```
In your diagram where the wires are Red will also augment  their resistance correct ?
...Will their Higher  resistance at red points change the way Current flows through the Pack  ?

Will More current flow through batteries where heat is less  ( not 10A on each cell) ??<img src="/uploads/db1493/original/3X/3/e/3e06fd34dc9ba3423dd69b66c62111d4cecb071f.jpg" width="640" height="360">
```

---
## \#40 Posted by: Hummie Posted at: 2017-04-20T15:50:13.423Z Reads: 96

```
i dont think the resistance of the red will increase much at all, it will get warmer and increase resistance slightly assuming that it's not under specd and not getiting significantly hotter.  I think the current from each cell should stay pretty much the same  assuming the wiring will have only slight variations in its resistance at different points.   I think more so the red will show increased heat and that is not good for cells and deteriorate them and will maybe unbalance cells over time.

maybe where the heat is less, so around the green area, the resistance will be a bit lower, so a bit less currrent will have to come from the branch of that paralleled cell to equal the rest,  so the cells will not have to put out as much compared to the other paralleled cells with more resistance in their paralleled branch, and that will also keep them in better shape and unbalance the pack as well.
```

---
## \#41 Posted by: Battosaii Posted at: 2018-10-15T14:47:53.994Z Reads: 39

```
I have a similar battery build set up but not sure if I should use tabs like you or 12 gauge wires for the connection.
```

---
