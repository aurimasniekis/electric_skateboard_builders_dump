# Best ESC for mountain boards?

### Replies: 24 Views: 3306

## \#1 Posted by: theviith Posted at: 2017-02-17T04:35:33.992Z Reads: 308

```
Does anyone know any good ESCs for trampa mountain board running on 12s 9000mah?

Thanks in advance,
```

---
## \#2 Posted by: barajabali Posted at: 2017-02-17T04:36:50.505Z Reads: 313

```
Vesc-x speaking from my personal experience.

The ollin vesc is also robust enough to handle mountain boards. 

Trampas working on the v6, beta is out soon. 

Fvt ESC's are okay but kinda scary 

Anything else will fail
```

---
## \#3 Posted by: Nowind Posted at: 2017-02-17T06:30:58.943Z Reads: 298

```
Actually using Robbe Roxxy 9120 OPTO with additional Cap Bank from YGE.

<img src="/uploads/db1493/original/3X/7/2/72de2acb05c04374f7cb30870008f984b9471396.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/c/1/c1c499c5ec6416759b442e6d543d89b63477f587.JPG" width="666" height="500">


This combination works good at the moment, without Capbank i burned 2 of the Roxxys.
They are extremely powerfull compared to a VESC 4, but not that smooth !

Also IMO its important with most ESC and in every case with the Roxxy that you make sure to protect them agains dust and debris and vibrations. Im using some thick foam rubber under a UK Box : 

<img src="/uploads/db1493/original/3X/0/9/09fc898816aeb64928419ab2e42f661aec89ab70.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/f/9/f907153e75497af378566e477ff19d09fe1ff30e.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/1/e/1e856808d558a95025849a18115b5c106dc6ae96.JPG" width="666" height="500">

After my expierence its the by far better way to use some velcro and foam rubber to mount this ESC´s then to direct fix them without damping. Other RC-ESC like HW Max6 handles this good, but Roxxy dont.
Also its more easy to maintenace the truck or use the adjusters with a easy removable Box :wink:
```

---
## \#4 Posted by: okp Posted at: 2017-02-17T06:40:20.379Z Reads: 275

```
a dumb question, but is there a way to remove this "bike braking" noise with non VESC ESCs? Where does this comes from?

Thanks!
```

---
## \#5 Posted by: Duffman Posted at: 2017-02-17T07:17:30.566Z Reads: 273

```
Some RC ESCs brake by shorting the motor coils. To make this controllable they do it with PWM. So what you hear is the PWMed shorting of the regenerated motor current. Others may regenerate to the battery, but with low PWM frequency which is in the hearable spectrum.

As long as you can't change the PWM frequency or the complete software of the 'non VESC ESC' you can't change the noise it makes...
```

---
## \#6 Posted by: Nowind Posted at: 2017-02-17T08:51:54.614Z Reads: 260

```
Its weired... depends on combination of used motors also. Hobbywing Max6 with Sk3 the Brakesound is horrible... with Alien HEV alot better.
In generall the Roxxy is the silents Rc Esc i tested so far....
```

---
## \#7 Posted by: Okami Posted at: 2017-02-17T09:32:28.591Z Reads: 251

```
@Duffman @Kaly  How about fvt / maytech 12s escs? Are they loud when braking? My fvt 6s is silent when braking, paired with sk3'.
```

---
## \#8 Posted by: monkey32 Posted at: 2017-02-17T16:59:32.422Z Reads: 237

```
Anyone tried torqueboard ESC on a mountain rig?
```

---
## \#9 Posted by: Kaly Posted at: 2017-02-17T18:38:12.504Z Reads: 227

```
I still have the TB ESC 2 years latter. Pretty robust esc. 

@okami the FVT esc makes a noise but to me is not a biggy. I have always like a auditory feed back from the board.  After getting to know your setup, you can tell if things are ok just by the sound.
```

---
## \#10 Posted by: Okami Posted at: 2017-02-17T18:40:20.620Z Reads: 223

```
@Kaly Do you know anyone who has made a video if it? At least I think I havent heard the sound in the videos I've watched of you riding.. but im also not sure which esc's in which video u use :slight_smile:

So if you have ''recorded'' the braking sound of 12s fvt esc.. that would be nice :)
```

---
## \#11 Posted by: monkey32 Posted at: 2017-02-17T19:09:25.720Z Reads: 216

```
Good to hear ........I got a deal on two used .....Planing on throwing them on the Trampa when I part up
```

---
## \#12 Posted by: okp Posted at: 2017-02-17T20:25:53.674Z Reads: 207

```
can people post videos of the noise while braking ? that would help ! cause to me; the noise break is really a no go for a mountainboard.
```

---
## \#13 Posted by: Okami Posted at: 2017-02-17T21:17:02.411Z Reads: 197

```
I think these Toro Esc's does make some nasty sounds.. at least I remember a thing or two I heard about them long time ago on this forum..

@lowGuido Can you tell your experience - which are the most noisy car esc's u have used?
```

---
## \#14 Posted by: tann Posted at: 2017-02-18T01:21:35.823Z Reads: 191

```
Do you still sell those remotes Kaly? I can not figure out how to PM.
```

---
## \#15 Posted by: lowGuido Posted at: 2017-02-18T02:15:48.454Z Reads: 184

```
Toro were louder than most. The hobby king ones weren't too bad.
Its only car escs that make the noise.
```

---
## \#16 Posted by: Schulerbible Posted at: 2017-05-28T13:26:33.694Z Reads: 152

```
Is there a valid reason why a standard VESC would not work for a mountain board? I am looking into a 10s3p or maybe 10s4p battery pack which powers up two 6374 motors.
```

---
## \#17 Posted by: Mikeomania12 Posted at: 2017-05-28T13:37:01.914Z Reads: 155

```
Toro sounds like train brakes
```

---
## \#18 Posted by: Mikeomania12 Posted at: 2017-05-28T13:39:09.894Z Reads: 160

```
https://youtu.be/xSYDCbZolnA end of video I have maytec 12s on my trampa. I can say brakes r almost silent. Ppl don't hear me coming into interactions or about to pass then. A little tricky to get used to after having the skyrc Toro on my other boards.
```

---
## \#19 Posted by: telnoi Posted at: 2018-03-19T10:55:35.846Z Reads: 110

```
Looking to build a board (on a semi budget) for my wife.
Considering the Hobbywing MAX6 V3.

How is the breaking of that ESC? Don't care as much about sound/good if people hear us coming ;). Is it progressive and related to the PPM signal/can you precisely control the brake force?
```

---
## \#20 Posted by: Nowind Posted at: 2018-03-20T06:40:36.456Z Reads: 104

```
The Brake of the MAX6 is very good IMO.
Good to control and also adjustable.
Only downside is the noise.
```

---
## \#21 Posted by: PredatorBoards Posted at: 2018-04-30T14:02:41.218Z Reads: 88

```
Which ESC of all the bunch here have the best throttle and brakes? I'm not looking for VESC levels of smoothness, but I am looking for something tolerable for semi-precise riding in the city.

Planning to pull a @MoeStooge and shove an inrunner onto one of my boards.
```

---
## \#22 Posted by: MoeStooge Posted at: 2018-04-30T14:23:33.595Z Reads: 84

```
Hands down for me it's the Mamba XL-X. 3.2 miles of hard 35+mph braking while passing gravity downhillers has solidified this esc as my Go too.   Data  logging is excellent and programming features set it apart.. 128deg farenheit was top temp for the 3.2mile uphill with average speed over 30mph.. all on 8s. You can pull punch, power and fully adj throttle and brake curves..
```

---
## \#23 Posted by: PredatorBoards Posted at: 2018-04-30T14:41:07.991Z Reads: 79

```
Interesting. I'm building a technical/sliding eboard as opposed to my usual 'race' setups. This means creating a lightweight build with all of the weight located in the front (makes it much easier to control the tail in a slide).

I'll likely start with a 6S1P setup that can output 100A. Motor of choice is the Goolrc 4092 using the same 9T/72T pinion gear configuration you have. Choice of wheels are Orangatang Kegels or AHMYO Akashas. How well will this setup keep up with say a 'standard' dual 5065 10S setup? Acceleration and Throttle control wise.
```

---
## \#24 Posted by: MoeStooge Posted at: 2018-04-30T18:16:24.264Z Reads: 70

```
Motor for motor it will smoke it.
```

---
