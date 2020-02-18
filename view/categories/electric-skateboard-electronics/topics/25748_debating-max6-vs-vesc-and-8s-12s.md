# Debating max6 vs vesc and 8s/12s

### Replies: 23 Views: 1886

## \#1 Posted by: lunasicc Posted at: 2017-06-20T04:18:25.429Z Reads: 174

```
im going to be building a holypro mtb in the near future. i was pretty set on running a 12s for power, while the vesc6 does look good, its currently out of stock and hasnt been out long for people to give proper advice on it.(not to mention the crazy price). and it seems like all the other 12s compatible escs arent the greatest, im not interested in any reliability issues. now im second guessing it and thinking about running dual max6's with 8s for now(not to mention its a tried and trued setup) and probably more user friendly. im just thinking it might not have the power i want. im 75kg and basically want to be able to top out atleast 30mph while still having sufficient torque on a 5:1 gear setup.

should i wait and go 12s later? or just commit and buy dual vesc6's?
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-06-20T10:26:11.752Z Reads: 168

```
I wanna start my mountainboard setup soon too and was asking the same question.
@Nowind video of his 8s max6 setup is the reason i´m going this route over the vesc.
Cheaper, lighter, much more robust, waterproof, cool housing from Nowind available, much more punch than the vesc.
https://www.youtube.com/watch?v=dSswwaDubS8
```

---
## \#3 Posted by: jga Posted at: 2017-06-20T10:53:14.018Z Reads: 159

```
I was thinking myself of buying the Max6 instead of a VESC as it seems to deliver quite good. I have seen it at £125 in UK which is pretty decent. And the anti-spark is included, which saves you a few more £ as well.
Look for the posts of @Idea, he has an 8S set up on a MTB and he sells the motor mount. If I remember correctly he was reaching quite impressive speed with 8S.
```

---
## \#4 Posted by: Minim Posted at: 2017-06-20T20:40:03.465Z Reads: 147

```
Can you set a amp limit in the max6/8 to not kill the batteries?
```

---
## \#5 Posted by: gee Posted at: 2017-06-20T21:24:43.985Z Reads: 142

```
bruh did you just do a wheelie in the video??
```

---
## \#6 Posted by: Smorto Posted at: 2017-06-20T22:33:26.659Z Reads: 135

```
Hate to nitpick but thats a manual :joy:/
```

---
## \#7 Posted by: lunasicc Posted at: 2017-06-21T03:30:08.955Z Reads: 131

```
yeah ive seen that video. honestly looks like it has a good amount of power.its just hard to judge from videos! but this will not have more punch than 12s on vescs like you mentioned...lol
```

---
## \#8 Posted by: benwong Posted at: 2017-06-21T03:52:18.736Z Reads: 126

```
I believe MAX6 can pump a good power. I have Trampa MTB setup too, using Trampa motor 136KV, i wish can use MAX6 with 8s but i loss some top speed with this low KV motor from esk8 calculation, so i end up go for FVT 12s sleeping lion ESC which @Idea Tom test it with improve firmware. But I just fried my ESC last week due to wrong remote wire connection and sent back to FVT for repair. Haven try out yet. 

Estimated next week will get my ESC and go for run.
```

---
## \#9 Posted by: lunasicc Posted at: 2017-06-21T04:50:12.301Z Reads: 124

```
i guess what im really looking for is people that have gone the 8s route and switched to 12s. do alot of you guys just stick with it and find that its plenty of power? or do you end up wanting a faster setup? having the option to be able to do 65kmh if i wanted sometimes would be nice. i just think 8s with 190k motors on a mtb wont be enough and i might get tired of it:laughing:
```

---
## \#10 Posted by: Minim Posted at: 2017-06-21T05:01:34.519Z Reads: 122

```
they even have a max8 esc for more amps so these can deliver lots of power. I have one on a 1/5 RC car but I can't find anywhere to limit the amps. Wouldn't this kill our battery packs pulling way to much amps from it?
```

---
## \#11 Posted by: TarzanHBK Posted at: 2017-06-21T06:32:27.227Z Reads: 116

```
That´s @nowind not me in the video ;)

@minim no you have to get some really good batteries that are able to deliver some juice.

@lunasicc this 8s setup is able to deliver more power than a 12s Vesc setup. Do the math:
8S with max6: 8 x 3,6V x 150A =4320W
12S with Vesc: 12 x 3,6V x 50A =2160W
So yes pretty much twice the power on the paper ;)
You need higher Amp ESCs on 12S to get even more power.
If you wanna go faster, take a higher KV motor. But I haven´t seen someone going over 60km/h with a eMTB.

@Minim the max8 is only a 6s ESC. And yes, you´re able to kill weaker batteries with normal ESC without Amp regulation.
```

---
## \#12 Posted by: benwong Posted at: 2017-06-21T07:16:25.375Z Reads: 105

```
@TarzanHBK If using 12s 120A ESC means can have 5000+W? 
Higher volt, less amp draw and lower volt, higher amp be draw right?
```

---
## \#13 Posted by: TarzanHBK Posted at: 2017-06-21T07:25:11.907Z Reads: 103

```
On the paper yes, not sure what this ESC is able to deliver in real world.
That´s correct
```

---
## \#14 Posted by: lunasicc Posted at: 2017-06-21T07:32:53.267Z Reads: 107

```
a vesc6 is higher than 50 amp.. there are many more knowledgable people than me on here, but what i do know for sure is a 12s will destroy a 8s in everything. assuming you have the esc's and battery to support it. and people have gotten to 40 mph/65kph on a emtb. done with a 12s and 200kv motors lol.
```

---
## \#15 Posted by: Minim Posted at: 2017-06-21T07:38:11.926Z Reads: 103

```
I ment Max5 sorry, That one is rated at 200A 8S. It's very tempting to go this way instead of expensive and unstable VESC knowing how good the hobbywing ESCs are. I use them on my big 6S multirotor hexa also with great results. On my 1/5scale car I drive it in snow, mud, rain and everything without problems :)
```

---
## \#16 Posted by: TarzanHBK Posted at: 2017-06-21T07:38:39.962Z Reads: 103

```
Sure when Vesc 6 is finally in the shelves why not. 

Do you have a link to a video with someone doing over 60 kph?

You asked for advice, so if you wanna wait for the Vesc 6 and want to spend the money on it, go for it. Should be a good pick for a MTB.
If you wanna save some moneys and want a proven, nice punshy board, consider the 8s setup.
Have fun building and tell us what route you went.
```

---
## \#17 Posted by: Nowind Posted at: 2017-06-21T09:34:26.316Z Reads: 102

```
[quote="lunasicc, post:14, topic:25748"]
, but what i do know for sure is a 12s will destroy a 8s in everything.
[/quote]

Thats just not true :wink:

A normal Vesc 4 on 12S, even with 100a motorcurrent dont delievers the torque of a 8S Max6 with High-C rated Lipos... and on 100A they tend to die.... again a normal unmodified Vesc4
```

---
## \#18 Posted by: Minim Posted at: 2017-06-21T09:42:29.195Z Reads: 101

```
Is there any negative about the max6 besides the lack of amp limit?
```

---
## \#19 Posted by: Nowind Posted at: 2017-06-21T11:15:03.329Z Reads: 96

```
The Brake sound is annoying...
```

---
## \#20 Posted by: Minim Posted at: 2017-06-21T14:58:50.236Z Reads: 84

```
How is the accleration? can it be set so that its massive with full throttle but still possible to accelerste gently with part throttle or do you need to reprogram it if you want to cruise?
```

---
## \#21 Posted by: lunasicc Posted at: 2017-06-22T04:41:40.179Z Reads: 82

```
Interesting. I'm just thinking about running max6 now. And maybe upgrading later. Maybe once a couple cheaper vesc6 options are out. And btw. I'd like to purchase your direct drive setup that you produce and sell. Should I pm you or would email be better??
```

---
## \#22 Posted by: Nowind Posted at: 2017-06-22T05:17:49.536Z Reads: 83

```
@Minim 

Max6 is the oldschool stuff ... Rough and not good adjustable
Vesc is the fancy stuff... like a new uptodate car... with ABS, EPS, Apps, Sensors

With MAX6 you can build strong and light Setups wich are great for freestyle stuff... you will never have to worrie about heat, water or dirt... even mounting is so simple... countersunk the Truck screws and velcro them to the tip... done

@lunasicc
Best is you send me an email : jens@e-toxx.com

Cheers
```

---
## \#23 Posted by: lunasicc Posted at: 2017-06-23T05:10:04.982Z Reads: 78

```
sounds good, thank you!
```

---
