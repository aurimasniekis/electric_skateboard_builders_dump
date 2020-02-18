# Antennes in metal boxes - a long one

### Replies: 10 Views: 494

## \#1 Posted by: NilsS Posted at: 2017-05-03T21:29:18.449Z Reads: 92

```
Okay so Im using this ESC And reciver combo from China (Looks a little Scary, but i Will try it.) http://r.ebay.com/E9inxt And 7S7P 18650 Homemade pack.

Okay but my question is will the reciver work in a metal case? I know that metal blocks radio so really my question is: How many holes will I have to make in the box? Is it enough to do it just around the antenna? (I'm not worried about water since I'm spraying it with conformal coating)  My first thought was that I could extend the antenna, but that wouldn't work because of wavelength theory. And it would have to way to short or long. 
<img src="/uploads/db1493/original/3X/e/2/e2026273f71c61bff022b0dbdb4fe9b1f13f20e1.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/4/9/49230a056cc772e07d90658fb802d734a9fa742c.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/f/2/f24f51d73e69be4a3e29b4cf7f68b8905ddd5532.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/6/a/6afd496315ea06f3fd3b26b9b8b45f79a4f62a9e.JPG" width="666" height="500">
Any ideas for solutions or comments? 
Also under a 150a load that's 3A per cell? In my 7S7P pack?
```

---
## \#2 Posted by: smurf Posted at: 2017-05-04T02:58:35.753Z Reads: 65

```
Drill a hole through the deck. Put the antenna under the grip tape.
```

---
## \#3 Posted by: JohnA Posted at: 2017-05-04T04:16:31.919Z Reads: 57

```
A 150 amp load would actually be using 21.42 amps per cell. The 7s increases the voltage by adding in series, and the 7p is what boosts the amps the pack can deliver. So say it's using Samsung 25r with a max discharge rate of 20 amps continuous per cell. A 7s7p pack would be 25v and 140 amps.
```

---
## \#4 Posted by: NilsS Posted at: 2017-05-04T05:20:16.074Z Reads: 50

```
The antennna is a PCB antenna
```

---
## \#5 Posted by: NilsS Posted at: 2017-05-04T05:24:01.342Z Reads: 44

```
But Im using 18650s with Max discharge of 5.2A am i Fucked?
```

---
## \#6 Posted by: Print3r Posted at: 2017-05-04T06:43:51.901Z Reads: 40

```
I was about to say limit your amps but realised you are not using a vesc. Cells should never be pushed to their maximum - they produce a lot of heat and electric skateboards can't offer much ventilation (water ingress frying electronics then becomes a problem). Normally I would advise running the 18650s at 1/2 their max continuous rated current, but that gives you only 18.2A as a safe maximum. 

I would advise selling your stuff on ebay or using it as a portable charger for your new build. With electronics you always should spend a little more to be safe and plan ahead (especially if it is expensive)! Falling off a moving board isn't fun because the control system cut out or blasted full power unexpectedly, then you have to recover your board (which would be a pain if the remote didn't work and it just kept moving away). 

Sorry for the bad news, learn from it and it will be well-worth the money - you didn't try and overload them resulting in a fire.
```

---
## \#7 Posted by: NilsS Posted at: 2017-05-04T08:22:28.114Z Reads: 32

```
I used some old laptop batteries, that has a 0.1v higher maximum voltage per cell. I think it will be fine because my drone batterys draw 120a per cell (they are 1500mah) but are only rated for 60a and they work just fine, plus I'm light and do not weigh that much since I am a kid
```

---
## \#8 Posted by: Print3r Posted at: 2017-05-04T17:55:26.235Z Reads: 21

```
You are really over discharging your lipos, be careful - batteries contain a lot of power. I hope the best for your build, but none of your batteries will last long if you treat them like that. You will produce a lot of heat so after you have made 110% sure your battery connections are insulated those batteries will need some sort of heatsinking. I would love to know how much current you draw given your weight if it does work
```

---
## \#9 Posted by: treenutter Posted at: 2017-05-04T18:54:28.220Z Reads: 17

```
@NilsS an an unprotected ESC in a metal box adds the added risk of shorting something. Make sure you heat-shrink everything before you use this setup.
```

---
## \#10 Posted by: NilsS Posted at: 2017-05-05T05:51:17.413Z Reads: 11

```
Hi I am just a kid 55KG and I have seperat boxes for my ESC and batteries. I thought of buying a current limiter, but I couldn't find one that limits such a high voltage and current.
```

---
