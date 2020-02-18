# The ultimate 18650 battery pack – serial then parallel or parallel then serial?

### Replies: 11 Views: 6089

## \#1 Posted by: PB1 Posted at: 2016-05-17T16:53:37.991Z Reads: 250

```
Had an interesting private discussion with another forum member triggered by my [post](http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/22?u=pb1) in the diagram thread. 

Which is the **proper way** to build a big pack out of 18650 cells? First parallel (e.g. 4 cells) and then serial (e.g. 10 4p packs) for a total pack of 4P10S – or first serial (e.g. 10 cells) and then parallel (e.g. 4 packs) to get 10S4P???? 

Most people seem to go the parallel and then serial path and this path has many advantages. 

However in order to build the ultimate flexible big pack I see many advantages in building 5S1P packs, then serial two of them into 10S1P, then parallel them to 10S4P  

Assumption: no BMS

What do you think? Pro’s and con’s? Does it matter?
```

---
## \#2 Posted by: barajabali Posted at: 2016-05-17T16:57:51.067Z Reads: 243

```
I do the parrellel then serial like most do.

It doesn't make sense in my head which cells the 10 balancing leads would go to on the serial than Parallel...
You need to balance each serial connection 1s,2s,3s individually I don't understand how you would balance them if you built the pack serial than parallel.

Proper way for a 10s4p is to make (10) 4 parallel packs. Then serial all of them together.
```

---
## \#3 Posted by: Jinra Posted at: 2016-05-17T17:03:45.600Z Reads: 233

```
I've asked this before and was pointed to a big endless sphere discussion which ultimately ending up with saying series-to-parallel was bad. I don't have a link to the post so I can't tell you exactly why.

My thoughts are that since you're putting a bunch (lets so 10s like you said) in series you'll need to connect balance cables to all 10 of the leads PLUS +10 for each pack in parallel. It's more efficient to just parallel anything you have, then series them once.
```

---
## \#4 Posted by: delta_19 Posted at: 2016-05-17T20:01:35.796Z Reads: 192

```
i remember that thread, i think something about the huge current/voltage difference from going one cell to one cell vs. going 10 to 10 was bad and could damage things.
```

---
## \#5 Posted by: Ulfberht Posted at: 2016-05-17T20:11:01.342Z Reads: 188

```
The way I visualize it is: Parallel connections make a "Cell" then you wire those in series to get up to the voltage you are looking to run at. 10s3p would be 10 packs of 3 batteries.
```

---
## \#6 Posted by: PB1 Posted at: 2016-05-17T20:20:30.925Z Reads: 175

```
Ok, agreed to all that was said above ... however ... :-) 

I still see some advantages going serial and then parallel. 
Modular - you can start with xSyP and then increase both in Voltage and capacity. 
Maintenance - you **can** check each cell and possibly replace a bad one, can't do that in one big parallel pack. 

Of course the packs have to have the same voltage before you parallel them. 

I'm doing this with 4 5S LiPos btw, gives me a nice 10S2P pack. Either bulk charging them to 42V or balance charging them indivually. 

Has anybody tried? Any other supporters?
```

---
## \#7 Posted by: lox897 Posted at: 2016-05-17T20:23:32.489Z Reads: 155

```
Check out this thread: https://endless-sphere.com/forums/viewtopic.php?f=35&t=72026

Go to the bottom of page 1 and the start of page 2.
```

---
## \#8 Posted by: PB1 Posted at: 2016-05-17T20:30:06.581Z Reads: 148

```
ok, thanks for the link. 
One guy says do it this way, the other guy says do it the other way round.
```

---
## \#9 Posted by: lox897 Posted at: 2016-05-17T20:31:40.380Z Reads: 145

```
@chaka says to do parallel and then series. @chaka builds lots of packs so I'd do what he says. Parallel and then series. Or you could do series then parallel, for science?
```

---
## \#10 Posted by: JTAG Posted at: 2016-05-17T23:09:42.713Z Reads: 143

```
You will always need to balance charge. And when you do; you need the balance leads. Using balance leads is only practical when de batteries are first parallel than series.
```

---
## \#11 Posted by: seanpain4 Posted at: 2016-05-18T05:41:22.783Z Reads: 128

```
You will need to balance them. 

It also depends how you are making your battery. If they are all adjacent to each other in one big pack like below, then it won't matter what order it is done in, as they will all be next to each other. 

<img src="/uploads/db1493/original/2X/f/f48d65fecb6a274a3b40e7d214c106d985590a41.png" width="327" height="250">

But what i am doing for my build, is having 6 packs of 13 cells in parallel, then i will wire them all in series. I will also have a set of smaller leads running out so i can balance charge all of them properly.
```

---
