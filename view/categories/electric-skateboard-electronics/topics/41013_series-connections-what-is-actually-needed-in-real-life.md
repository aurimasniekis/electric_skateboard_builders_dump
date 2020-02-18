# Series connections - What is actually needed in real life

### Replies: 14 Views: 532

## \#1 Posted by: davidbonde Posted at: 2017-12-14T10:53:51.826Z Reads: 140

```
Something that I have still not completely wrapped my head around and fully understod is what is actually needed to make a safe serial connection between p groups. 

I have seen a lot of posts and theoretical calculations based on more or less theoretical assumptions. But every time I am still left with a certain amount of uncertainty.

So what are your guys real life experience. What have worked? What have not worked? What have been to little? What have been to overkill? Ect. 

To be more specific… I am soon to build a 10s5p pack with samsung 30Q cells. I have not yet decided about how I will do my series connection, and I am considering either Nickel strip only, busbar, or fleksible awg wire. Every method her own pros and cons. 

If we take the nickel only I have the possibility to stack strips. But how many is really needed… you know in real life, not just a theoretical calculation. I know that such calculation will be a great starting point, but one thing is calculation another is real life. 

On Endless Sphere I fund a chart done from real life testing, showing how much A a 7mm strip can safely handle which were about 7A cont.  But how does that compare to real life driving, with all the changing parameters that offers. 

I know this depends on a huge amount of factors like motor used, weight of driver, acceleration and the list go on. Thats maybe part of why I still are left with uncertainty after reading lots of posts. There properly is not a one answer fits all. 

And just for good reason…. this is not an attempt of skipping corners and being cheap. The easiest thing would be to just go overkill and be safe. This is an attempt of adding to my knowlege with some real life experience from your guys :)
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-12-14T11:42:18.347Z Reads: 122

```
The best design in the industry is the Tesla style fuse wire on each cell. It is more critical you're not over drawing current from cell than the voltage. I know the chart you are talking about is seen under the battery spot welding topic. I can only interpret it as the max amperage for chassis wiring meaning short distance. Stacking multiple nickel strips for current...I believe two or three is good enough, but it depends on the spot welder's capabilities. I rarely or don't see 4 nickel strips stacked.

Personally, my 10S5P 18650 Samsung 25R pack uses only a single nickel strips for series connections. I forgot the thickness. I used the paper insulator on the positive side in the plastic holders. The BMS is critical for the life span of the pack aside from building the pack.
```

---
## \#3 Posted by: davidbonde Posted at: 2017-12-14T11:48:17.225Z Reads: 118

```
Thanks this is just the feedback I want :) 
I take you haven't had any problem with your single nickel strip.
```

---
## \#4 Posted by: chuttney1 Posted at: 2017-12-14T12:03:06.917Z Reads: 112

```
I did the vinegar/salt test solution for authenticity of pure nickel all the way. To describe with those 18650 cell holders. I arranged it such that it flexes minimally, but hard to replace a bad cell if I had to. I got no problem with my pack cause I made sure those welds on each cell had 6 - 8 spots per terminal. If this is your first battery pack I suggest you make your pack a single layer if you can and you will have to take into account how much your board flexes in the middle to prevent the nickel strips from breaking from cell terminal if you forego the plastic cell holder and use other methods to hold the cells.

I think others here such as Longhairedboy can lend some suggestions on pack building as well as the many examples on Endless-sphere.
```

---
## \#5 Posted by: davidbonde Posted at: 2017-12-14T12:13:09.464Z Reads: 107

```
Thanks... this would be my second pack, and I slowly but surely gets more and more into the different possibilities thanks to feedback like yours. I gradually feel more and more confident in what I am about to do :)
```

---
## \#6 Posted by: chuttney1 Posted at: 2017-12-14T12:16:24.858Z Reads: 99

```
In that case find a way to make your pack easy to repair if you get a bad cell. A challenge for such a compact battery pack.
```

---
## \#7 Posted by: longhairedboy Posted at: 2017-12-14T12:23:33.497Z Reads: 97

```
i use 0.2mm x 10mm nickel in a single layer with additional nickel to bridge the cells within the P groups.
```

---
## \#8 Posted by: PXSS Posted at: 2017-12-14T12:25:40.871Z Reads: 94

```
I use 0.25mm thick copper in a single layer. 

<img src="/uploads/db1493/original/3X/5/0/50e1a8dcf7d4aa6243e6f5190c3797911ef48649.JPG" width="666" height="500">
```

---
## \#9 Posted by: davidbonde Posted at: 2017-12-14T12:33:39.905Z Reads: 88

```
Do you fold those up or are they kept this way?
```

---
## \#10 Posted by: davidbonde Posted at: 2017-12-14T12:35:18.474Z Reads: 86

```
Within the p group? Is that necessary?
```

---
## \#11 Posted by: PXSS Posted at: 2017-12-14T12:49:23.098Z Reads: 85

```
I keep them this way because my deck isn't large enough. I would need a 10in wide deck with at least 27in of wheelbase for 1310Wh of battery.
```

---
## \#12 Posted by: davidbonde Posted at: 2017-12-14T12:54:43.583Z Reads: 86

```
:) yes of course :) I see now that this is a huge pack :)
```

---
## \#13 Posted by: pshaw Posted at: 2017-12-14T17:31:24.367Z Reads: 73

```
I’m using .15mm thick single nickel strip for my 13s4p pack I’m building. 

I’m a bit weary of it but I assume the max I’ll pull through it is 90-100A. Maybe not even that much. 

One thing I’ve never seen is a post where anyone has a failed single nickel strip (due to heat) for a serial connection leading to board failure/ fires/ etc. 

So my thoughts is that everyone is going WAYYYY overkill and a single strip is fine.
```

---
## \#14 Posted by: davidbonde Posted at: 2017-12-14T18:15:56.679Z Reads: 70

```
Thats exactly what I am trying to get a little close on.
```

---
