# Wiring trouble with VESC

### Replies: 17 Views: 1232

## \#1 Posted by: TSThunder Posted at: 2017-07-07T04:50:22.398Z Reads: 68

```
So I am planning to use DIY Electric's VESC, but their VESC's power input uses a XT90 female connector. The problem is that the batteries I am using has 5.5mm bullet connectors, and I want to use a loop key instead of DIY's $60 trashy power switch. 

So basically I can't use a 5.5mm to XT90 connector for my battery-->VESC connection because connecting the power source to the VESC can be dangerous, and I still want to use a loop key.

Help would be very appreciated

Batteries: [https://hobbyking.com/en_us/turnigy-5000mah-5s-30c-lipo-pack.html](https://hobbyking.com/en_us/turnigy-5000mah-5s-30c-lipo-pack.html)
```

---
## \#2 Posted by: psychotiller Posted at: 2017-07-07T04:57:37.565Z Reads: 63

```
Connecting the vesc to a power source isn't dangerous...

What you should do, if you don't want to solder an xt90 male end to your battery leads is cut the connector off of the vesc and solder on 5.5mm bullets.  Either way, you still have to connect the battery. Same dillemma, same danger.

Then you can use the xt90 to make a loop key and solder it into the negative battery lead (between the battery and the vesc.
```

---
## \#3 Posted by: TSThunder Posted at: 2017-07-07T05:02:03.919Z Reads: 57

```
Are you sure? I thought that not having an anti-spark is dangerous.
```

---
## \#4 Posted by: psychotiller Posted at: 2017-07-07T05:05:25.846Z Reads: 57

```
I suppose it would be dangerous if you live in a dynamite shed. Or douse yourself in gasoline before you plug your board in? It's just a spark otherwise. If you use xt90 anti spark plugs your dynamite shed will also work.
```

---
## \#5 Posted by: TSThunder Posted at: 2017-07-07T05:10:11.592Z Reads: 51

```
Haha, I was just pretty concerned because I read that if you connect you batteries directly into your VESC, then it would end up frying up the VESC
```

---
## \#6 Posted by: psychotiller Posted at: 2017-07-07T05:14:30.476Z Reads: 51

```
Huh? Where did you read that? You have to plug them in to use them right? Apparently the vesc is even more fragile than we thought. I know lately there has been alot of back and forth about it's durability, but really, there are only a couple of things you need to worry about. 
The erpm limit 
and not getting too carried away with settings before you understand what they do.
Oh! And don't say VESC I heard
```

---
## \#7 Posted by: TSThunder Posted at: 2017-07-07T05:38:28.213Z Reads: 52

```
I heard it from one of my lasts posts here: http://www.electric-skateboard.builders/t/lipo-battery-safety-question/26707/7?u=tsthunder
```

---
## \#8 Posted by: sl33py Posted at: 2017-07-07T05:43:27.696Z Reads: 51

```
A few of us cavemen have used with and without anti-spark of any kind for years.  

You'll be fine.

Yes it will spark.  Yes it will slowly wear away the contacts, but easy to swap if so.  The higher the voltage the bigger the spark - not a huge deal.

If you douse yourself in gasoline i think you'd still need to hump the board as you plug it in to ignite - or maybe a fierce hug at least...

XT-90 anti-spark loop key is super simple and will work.  Soldering heavy gauge wires does take a hotter iron and some practice to make it look nice.

I have an old "how-to" you are welcome to peruse and hope it helps!
https://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204

GL!
```

---
## \#9 Posted by: psychotiller Posted at: 2017-07-07T05:44:33.451Z Reads: 46

```
Ahhhh yeah, they were talking about the sparks eventually destroying the connection in whatever plugs you choose.  They did mention a few lines down that you would just need to replace your plugs every few months if you lived with the spark. They didn't say it would destroy your vesc. :smiley:

You'll be alright.  Make sure you read everything you can on setting up your vescs. Don't do guesswork.
```

---
## \#10 Posted by: ShutterShock Posted at: 2017-07-07T05:44:42.952Z Reads: 43

```
I'm not quite sure you interpreted what I was saying there correctly @TSThunder

My intention was to warn against the sparks that could be experienced in the high voltage situations, however, further down in that post, someone else further educated both myself, and.. well I assume you read the rest.  I was not completely correct in what I was saying, however it is still a _good idea_ to use an antispark within your system to promote the longevity as a whole. 

Futhermore, see where @evoheyax corrected me, a few posts down

@sl33py :joy:  :joy:  sl33py is correct as well
```

---
## \#11 Posted by: psychotiller Posted at: 2017-07-07T05:46:22.523Z Reads: 41

```
[quote="sl33py, post:8, topic:26964"]
If you douse yourself in gasoline i think you'd still need to hump the board as you plug it in to ignite - or maybe a fierce hug at least...
[/quote]

Bahaha! @sl33py I just pee'd a little
```

---
## \#12 Posted by: TSThunder Posted at: 2017-07-07T05:48:32.750Z Reads: 35

```
My bad! I misinterpreted what you said in post
```

---
## \#13 Posted by: TSThunder Posted at: 2017-07-07T05:50:58.856Z Reads: 35

```
Thanks! I guess I went through the trouble of researching on/off switches and anti-spark plugs for nothing. I am just gonna plug it into the VESC raw now :)
```

---
## \#14 Posted by: psychotiller Posted at: 2017-07-07T06:09:25.166Z Reads: 33

```
No lube?!? No nothing?!?
```

---
## \#15 Posted by: sl33py Posted at: 2017-07-07T06:12:06.527Z Reads: 33

```
Not for nothing i assure you.  You'll eventually get tired of swapping plugs/connectors and make an anti-spark loop key.

Or get a "fancy" anti-spark switch...  But until then - keep reading, asking questions and soaking up the goodness.

Most importantly - go RIDE and have fun!

[quote="psychotiller, post:14, topic:26964, full:true"]
No lube?!? No nothing?!?
[/quote]

A *fierce* hug...:smirk:
```

---
## \#16 Posted by: Namasaki Posted at: 2017-07-07T06:21:27.795Z Reads: 33

```
This thread has been most entertaining.
Maybe vescs should come with this label:

<img src="/uploads/db1493/original/3X/f/6/f60bbd03d9a71288fa809e6f8845cec09a6026b7.jpg" width="500" height="500">
```

---
## \#17 Posted by: wafflejock Posted at: 2017-07-07T06:29:04.556Z Reads: 29

```
Yeah I dunno when I was using the 2 6S multistar packs in series for a 12S with the DIY VESC it was blowing up the XT-90s I had like every other time or every third time I'd plug in to the point the connector would be totally charred and not very trustworthy (and just not connecting eventually).  Didn't harm anything in the process just gave me a good jump the first few times I did it but pretty much immediately ordered an antispark.  Downgraded to 10S and doesn't seem nearly as bad but I keep using the anti-spark cause it's already there and like to have the fail safe.
```

---
