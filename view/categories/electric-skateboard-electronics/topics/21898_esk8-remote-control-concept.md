# Esk8 Remote control concept

### Replies: 21 Views: 1947

## \#1 Posted by: baxter Posted at: 2017-04-27T12:20:06.254Z Reads: 247

```
So here is a concept design for an electric skateboard remote control. I have no experience with designing electronics, nor do I have a 3D printer or awesome CAD skills, so bear with me as I describe my design to the community.

This design would rely on a spring loaded slide potentiometer and an 18650 cell as the power source, although you could get away with most other cylindrical cells (e.g. a 16340).  There would be an interlock button to prevent unintended acceleration. I have tried to keep a minimalist approach, but as I am no electronics guru, I will leave this design to those in the community who are technically minded and can make it a reality. 

As a thumb based remote control, it's a little different to what you might be used to, but it is meant to be a simply operated by being held within a closed fist, and moving your thumb toward your index finger to accelerate, and away to slow down and brake.  So basically, you push the plunger down to go faster; and lift it up to slow down and brake. Here is a crude diagram.

<img src="/uploads/db1493/original/3X/d/5/d59efbe7e2331b60c622da67ff7dc13b4da0edfa.png" width="403" height="483">

Obviously, it would need to be a little longer to fit in an 18650 cell, and the loop at the top a little larger to put your thumb in, but I hope you get the idea.  Not sure if the guts of the existing remotes would be able to be inside this one, but would be cool to have another cost effective option to what can be currently be obtained commercially.  

What do you suggest as a name for the design?

What do you guys think?
```

---
## \#2 Posted by: Tomer Posted at: 2017-04-27T12:27:01.831Z Reads: 222

```
I don't dig this mechanism. 
In my opinion braking in this method is not very convenient and you don't have much preciseness.

Thanks for sharing though.
```

---
## \#3 Posted by: KTMinni Posted at: 2017-04-27T14:03:56.667Z Reads: 207

```
My only gripe with it is the remote design does not easily allow it to be ergonomic.  Also releasing the trigger too fast could result in a brake if you aren't careful due to the nature of springs that aren't designed for controllers.
```

---
## \#4 Posted by: saul Posted at: 2017-04-28T07:36:14.838Z Reads: 173

```
it look too threatening. you can't ride around a city with that! too much like a deadman switch.
```

---
## \#5 Posted by: Okami Posted at: 2017-04-28T12:18:29.938Z Reads: 162

```
yeh I will also join the numbers who dont really get the design or think it is not super practical..

In my understanding, a ''sliding potentiometer (trigger) would still be better as you would have a grip under the remote to keep the remote 'leveled'..

With this design it looks like there would be just too much free play!

It might work of course.. but Im still not sure what kind of componenets would be needed, to make it super smooth and not ''jerky''.
```

---
## \#6 Posted by: baxter Posted at: 2017-04-28T12:38:38.725Z Reads: 154

```
The potentiometer would be held at neutral by two springs, one which allow upwards movement, and another for downward movement.  This is no different to a trigger style potentiometer, which is held at zero throttle by default.  This is no different to the method used by a gt2b (or any of its mods), except the potentiometer is linear.

<img src="/uploads/db1493/original/3X/6/f/6f736dd90c63ed7e43ebb6d7f54479e65e6634df.png" width="479" height="347">

My design seeks to use a push/pull mechanism as opposed to using rotation around an axle. That is all.
```

---
## \#7 Posted by: Okami Posted at: 2017-04-28T12:41:43.613Z Reads: 143

```
Yeh, im imagining something like this:

<img src="/uploads/db1493/original/3X/1/a/1ae1b60b56a1fbd99b86e1e4f9d9da27d5b245b2.jpg" width="250" height="188">

But with ''vertical'' lever, not horizontal..

Also it would need to work both ways, so maybe the initial resting position would be in the middle, like some ''slider remotes'' have it.

--

''Crude'' updated image:

<img src="/uploads/db1493/original/3X/e/c/ec49f58d7c2ea76c7710a4bd66fc982301d2d490.jpg" width="441" height="440">
```

---
## \#8 Posted by: ThomasLefort Posted at: 2017-04-28T13:11:22.123Z Reads: 133

```
Why not :-) It need to be test because the main problem is the reliability of the brake. But I would change the linear potentiometer by a Velostat. It mesure the pressure, it is precise and it can be really small. But it's not easy to make
```

---
## \#9 Posted by: Okami Posted at: 2017-04-28T13:16:29.137Z Reads: 138

```
[quote="ThomasLefort, post:8, topic:21898"]
Velostat
[/quote]

How does it work?

All I find on net, is something like this:
<img src="/uploads/db1493/original/3X/c/d/cdfaa2480191026140e246daa577f1d166b301e0.jpg" width="500" height="375">

I assume it is a fabric/material which stretches and then gives some sort of electrical output?
```

---
## \#10 Posted by: ThomasLefort Posted at: 2017-04-28T13:24:30.048Z Reads: 131

```
Yes. You can put 1 layer of materiel (adhesive tape or neoprene), 1 wire, some layer of Velostat , 1 wire, 1 layer of material. And when there is a pressure on the Velostat, it resistance change. It is precise. With adhesive tape, you can only put positive pressure. But if you put it between Neoprene you can mesure positive and negative pressure.

And the mesure occur across the layers. So it can be really small. Their is Velostat that you can sew on gloves for exemple to remotely control the board with the pressure of the fingers.
```

---
## \#11 Posted by: Okami Posted at: 2017-04-28T13:36:07.827Z Reads: 119

```
For braking this sounds like a good solution.. more pressure applied, stronger brake :slight_smile:
```

---
## \#12 Posted by: KTMinni Posted at: 2017-04-28T13:43:33.948Z Reads: 120

```
Interesting idea...  I feel like a glove with that technology would make it seem like you're using the force to control your board.
```

---
## \#13 Posted by: darkkevind Posted at: 2017-04-28T20:24:26.117Z Reads: 115

```
Kinda reminds me of my wife's tampon! :slight_frown:

No offense!
```

---
## \#14 Posted by: Okami Posted at: 2017-04-28T20:36:07.858Z Reads: 115

```
[quote="darkkevind, post:13, topic:21898"]
Kinda reminds me of my wife's tampon! :slight_frown:
[/quote]

You nailed it ! :D

@baxter Can you make another 3d model so people understand better?

It looks like current design is already made in some kind of software..so keep up, if you want to find someone who builds it, the design needs to be way more refined ;)
```

---
## \#15 Posted by: baxter Posted at: 2017-05-14T03:57:48.086Z Reads: 117

```
Okay,  to better illustrate the concept I was going for, a google search picked up a couple of existing items which might explain better as to what I had in mind. The cylindrical form factor was an idea I got from a medical research pipette:

 (the top half obviously):
<img src="/uploads/db1493/original/3X/d/7/d79a4d699143414e9489a0d210b8f59d0a4b7cc3.jpg" width="143" height="279">


Similarly, imagine a slot car controller had a loop at the top for your thumb (for braking), a wireless transmitter and a self contained a power source)  :slight_smile: 
<img src="/uploads/db1493/original/3X/6/b/6bc148984c0118960264b376ef98d8c2a4224f16.jpg" width="301" height="500">
<img src="/uploads/db1493/original/3X/d/0/d0c6392d9ede262ebefe22645cfcf365ebe1a98f.jpg" width="289" height="250">
<img src="/uploads/db1493/original/3X/5/2/520448851950ef99729e45f468ce7fafd374462f.jpg" width="425" height="500">
<img src="/uploads/db1493/original/3X/7/6/76909c65b9844202ca65b9ace70d3bbe1de3708d.jpg" width="458" height="500">

Does that make more sense?
```

---
## \#16 Posted by: Okami Posted at: 2017-05-14T18:37:38.621Z Reads: 97

```
damn, just build it yourself man.. ure the one with the concept in the mind and can even find pics like that :d why the laziness then.. we will help with electronics or whatever if you need.. though u seem to know a lot about resistance and that velo band or what.. so is the design the only obstacle?..

there are a few programs which seem to be very simple to work with.. if you wanna realize it.. just invest some hours into it, so others can maybe jump in on your concept once u have a rough shape in 3d model
```

---
## \#17 Posted by: baxter Posted at: 2017-05-15T12:56:55.299Z Reads: 97

```
Actually I have no design experience whatsoever. I don't have a clue how to make a circuit board or how a velostat works. I don't have a 3D printer or even how to wrangle electric pixies - its just Lego to me. While I might know what some parts are called I wouldn't know what I would need, let alone how to put them together from scratch. Nonetheless, I think the design has merit.

In light of these shortcomings, and with the fervour that I have seen the community adopt these designs, I think the slot car remote style could be popular if some enterprising individual(s) wanted to make their own remote controller, they can take this idea and run with it if they want.
```

---
## \#18 Posted by: Okami Posted at: 2017-05-15T14:18:48.799Z Reads: 98

```
Ok I get your point now haha :D so you are not so keen to develop the design. u just thought to share it, in case anyone was interested.. sorry for bashing you.. since I was checking what @lox897 is doing with vesc remote.. that I got a bit pissy that nobody is going to make your design and we dont even know how it works.. in the first place.. 

But yeh aftershowing the last pictures, the concept is a lot more clear now.. though, without testing it is super hard to tell whenever such system is effectial from the ergonomics perspective..

Like now, only recently i found out that thumbwheel remotes work better for precision and are not as ''harsh'' as trigger style remotes.. perhaps would have got thumbwheel remote, instead of trigger style one..

Or someone just should make the conversion for mini remote to thumbwheel remote more comfortable.
```

---
## \#19 Posted by: Okami Posted at: 2017-05-25T17:25:00.948Z Reads: 80

```
@baxter u might wanna see this

<img src="/uploads/db1493/original/3X/0/0/004bd957bd46a2e4faaa7ffb9a6d05b8ea037ba5.png" width="690" height="413">

Video:
https://www.youtube.com/watch?v=UdnfIuVak_U
Though.. the connection is shit.. but I really liked the concept and whole style for a second lol

--

I also see u asked for a name for this mechanism (the one you @baxter developed as concept) -  maybe call it 'Grenade control'' or the 'Push/Pull''mechanism.
```

---
## \#20 Posted by: wmj259 Posted at: 2017-05-26T00:48:27.674Z Reads: 69

```
If you can make drawings and dimensions I can CAD it up for you no problem.
```

---
## \#21 Posted by: baxter Posted at: 2017-05-26T13:07:40.800Z Reads: 61

```
Yeah that remote is funky design.  While it is a trigger remote, the throttle looks like it works on a slide mechanism. Not sure how you'd progressively apply the brakes with that remote. The fact that it didn't work properly doesn't help its cause.  

Some people like the trigger, some people like the thumbwheel, this is would be yet another option to control your speed. 

Grenade Control - sounds cool! But to be fair, the person who makes it get to name it!
```

---
