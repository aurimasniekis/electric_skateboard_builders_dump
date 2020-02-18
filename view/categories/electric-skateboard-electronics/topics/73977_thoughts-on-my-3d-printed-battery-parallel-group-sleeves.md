# Thoughts on my 3D printed battery parallel group sleeves?

### Replies: 14 Views: 472

## \#1 Posted by: niuva Posted at: 2018-11-08T22:40:45.411Z Reads: 155

```
Ever since I got into building electric skateboards I've had a soft spot for 'modular' batteries, especially trying to keep things under 99wh. Now that the new Focbox Unity is soon coming out, I thought that it would be a great time to build a new board. Previously I've gone with NESE modules for modularity, but those things aren't really plug and play but instead require a solid ten minutes of unscrewing to get the pack apart, plus they add quite a bit of extra bulk. So here is my possible solution, on which I'd really like some feedback on and would like to hear your thoughts, especially from more experienced battery builders than I, before I start spotwelding stuff up.

So basically what I've got so far are 10 'sleeves' that fit seven 18650 cells in parallel that will be connected to each other via 5.5mm bullet connectors (for fast disassembly) to form 10S7P. This 'design' also also leaves me with a hollow canal between the two groups to run my wiring in, on the bottom of the enclosure. Each pack shall have a BMS balance connector and obviously two dangly bullet connectors originating from each side of the pack.
![image|666x500](upload://wbI4EY4MVdAhbXzH1lL8FB8drZK.jpeg) 

Would said 3D printed sleeves (ABS) still require the typical treatment of fishpaper around them, or would the tight fit of the 3D printed sleeve do the job? Obviously I'd still insulate the positive ends of each cell with those circly fishpaper bits before spot welding them together.
Why 3D printed sleeves you might ask? Well, to make the battery look less like a DIY C4 pack of explosives and more elegant and neat.

![IMG_6769|666x500](upload://1waSgZ8WBNHSYEGFZhk0RfwbBG0.jpeg)

Wires would come out under the end caps of each pack. 5.5mm bullet connectors with 14AWG wire.
 ![IMG_7621|666x500](upload://7N3bVa8vonw8jWgEvOKIknzidsc.jpeg)
 ![IMG_1412|666x500](upload://e4UIzuieV2sWttKi9Oc0jxQgjlv.jpeg)
```

---
## \#2 Posted by: brenternet Posted at: 2018-11-08T22:55:05.465Z Reads: 144

```
I like the idea. Once the balance leads and wiring is run though how will this be modular out of interest? Surely it will just become a sleeved permanent pack?
```

---
## \#3 Posted by: niuva Posted at: 2018-11-08T22:59:37.331Z Reads: 141

```
I'm thinking that each parallel group will be a completely individual unit. Something that I can quickly disassemble in a matter of minutes into 10 packs of >99WH groups for transport.
That's the plan at least - unless someone smarter than me comes in and tells me that that is a bad and a dumb plan! :)
```

---
## \#4 Posted by: skatardude10 Posted at: 2018-11-09T00:16:06.311Z Reads: 123

```
I love it!!! I'd personally feel more comfortable with something like nylon since it doesn't crack as easy as ABS, but that's just me being nit picky, I have a feeling this is going to work out *amazingly*. It all looks so sexy already, can't wait to see it all wired up. Great idea btw!
```

---
## \#5 Posted by: niuva Posted at: 2018-11-09T00:21:02.375Z Reads: 118

```
I usually acetone vapour smooth my ABS prints, so there is really no chance for these to really split. Bonds the layers nicely together. :+1:

If anyone is interested, I can share the STL files for these.
Also, what if I'd stick a TP4056 module on each pack for easy individual group charging via USB when they are not connected up in series - because why not?  :thinking:
![image|468x500](upload://e4YmkcP1d0W3Sk4bPFFWIVLzcF8.jpeg)
```

---
## \#6 Posted by: Fiori Posted at: 2018-11-09T00:38:24.119Z Reads: 107

```
As someone who 3d prints everything in sight, I love this idea. 

However, I really cant see how you would connect these together and still keep them so close to each other. If you want multiple separate packs you are going to have to have multiple BMS too.  

The space for connectors and such seems small, but I feel like as builds progress they take up more room than you think. 

I'll be following this project for sure.
```

---
## \#7 Posted by: niuva Posted at: 2018-11-09T01:20:36.857Z Reads: 106

```
Quick mockup in 3D to visualize what I have in my head regarding the connection and wiring scheme. Larger Yellow blobs are supposed to be[5.5mm bullet connectors](https://www.gator-rc.com/media/catalog/product/cache/3/image/512x512/9df78eab33525d08d6e5fb8d27136e95/p/u/pu5.52pc.jpg).   Something in this ballpark..

[Using generic 2pin RC JST connectors for balance connectors.](https://www.cordlessrenovations.com/wp-content/uploads/2013/06/CR-CN5.jpg)
![image|690x281](upload://4U9ckxqEoDp49nEFtS25GcZCSzS.jpeg)

Single module of 7P would look something like this:
![image|631x500](upload://mLD2b9pWeC0okpKUVb4STjSKVGK.jpeg)
```

---
## \#8 Posted by: danile Posted at: 2018-11-09T01:41:59.523Z Reads: 101

```
Such a cool idea!
Good luck with this!
```

---
## \#9 Posted by: marsrover001 Posted at: 2018-11-09T02:15:50.084Z Reads: 96

```
Love it. I've got a 12s7p now that would have benefited from this idea. In builds where space is tight it might be an issue. Maybe link 2 packs side by side(one print)? Needs more printer build area but could be the difference between fitting and not.
```

---
## \#10 Posted by: MoustacheMonkey Posted at: 2018-11-09T08:33:13.506Z Reads: 86

```
Damn, this looks nice! I would love to see how you solder those series connections to keep this as compact as possible! I think you'll need more space between the packs than showed on the 3D mock-up though.
```

---
## \#11 Posted by: niuva Posted at: 2018-11-09T16:13:18.103Z Reads: 78

```
I can easily fit a 2P pack on my printer, but the reasoning why I went with smaller 1P was the goal of keeping each pack under 99WH for transport / air travel. One 30Q cell is aprox 11WH and with seven cells in one parallel group would end up around 77WH _(right?)_ - well below the limit that I'm aiming for with these packs.

I'm still waiting for someone to come in and slap this idea out of my head. I refuse to believe that everyone so far likes it and thinks it's a good plan - otherwise I'm moving forward with this. :smiley:
```

---
## \#12 Posted by: deucesdown Posted at: 2018-11-09T18:00:36.600Z Reads: 62

```
I guess it begs the question, what does the printed enclosure give you that glue and tape don't?

In contrast NESE is no-solder no-spotweld.

Thought provoking and interesting for sure.

Oh add a thermistor per pack if you're accessorizing :)
```

---
## \#13 Posted by: briman05 Posted at: 2018-11-09T21:45:32.771Z Reads: 54

```
I really like the look of that nice and clean. My only question is are you going to heat shrink them when the packs are all built?
```

---
## \#14 Posted by: niuva Posted at: 2019-02-27T16:53:39.492Z Reads: 37

```
Project has been on hold for a while, but managed to finish my 10 7P packs of batteries. Snow is starting to melt in Finland and soon will be able to stick them in my new build.

Skipped the dumb idea of sticking a TP4056 module on each pack. Charging a pack took several days. :smiley:  Quite satisfied with the look so far. My biggest issue with a traditional 'tape em' up' look was purely the aesthetics. Tired of having my batteries look like C4 Explosives.
![image|666x500](upload://sndFMkMiPKHCJiwdHKi7vAuXbtv.jpeg)
```

---
