# 2 vesc , 1 motor

### Replies: 22 Views: 1542

## \#1 Posted by: almogu Posted at: 2017-11-02T19:52:28.345Z Reads: 239

```
hello good, I'm almogu skate electric Spain. my doubt, since I did not find information, is if it is possible to connect 2 vesc to a single motor, I suppose that by the port can bus. but I do not know if someone did it or tried it since both vesc could be affected when passing the current from one to the other by not being well synchronized.
```

---
## \#2 Posted by: psychotiller Posted at: 2017-11-02T19:53:47.947Z Reads: 239

```
Why would you connect 2 speed controllers to 1 motor?
```

---
## \#3 Posted by: Surfer Posted at: 2017-11-02T20:01:32.871Z Reads: 235

```
I believe he means the another way around, 2 motors 1 vesc. Eso no se puede hacer amigo!
```

---
## \#4 Posted by: Hummie Posted at: 2017-11-02T20:10:59.915Z Reads: 225

```
you can put two esc on a motor if you really wanted to, likely a very big motor that would need more power than one. dont know the details on synching them but on vedder's site you could find out. i think you maybe could make it a 6 phase motor if you rewind it as well and that would be ideal
```

---
## \#5 Posted by: Acido Posted at: 2017-11-02T20:13:46.597Z Reads: 213

```
Dont see a scenario where that is needed, and think that dual is cheaper
```

---
## \#6 Posted by: Hummie Posted at: 2017-11-02T20:18:15.311Z Reads: 210

```
if you have a really big motor and want to run it on vescs and get more amps into the motor than a single vesc would put out.   On a bike or something bigger than a board probably
```

---
## \#7 Posted by: almogu Posted at: 2017-11-02T20:30:03.481Z Reads: 197

```
My skate has a big 36v 25A engine. It is not small like yours, these are the first engines that were mounted on the skates. If I put two VESC, I would have more power, since I had a lap and it fell short on the slopes. I have configured the VESC to 50A of delivery to the engine and the battery is 30A and it is enough to 60A. I think the VESC are designed for high revving engines, not for power.

<img src="/uploads/db1493/original/3X/1/2/1202776c67dcfcf0463eba24a00f0e19c2022ed9.jpg" width="666" height="500">
```

---
## \#8 Posted by: ShutterShock Posted at: 2017-11-02T20:49:36.890Z Reads: 179

```
First of all *cough* it is a motor not and engine :joy:

The motors most people use are just as powerful as the one on your board.  Many of them are 50.4V and 80A compatible.  So maybe you just need to do some adjustments in your BLDC tool to make it run better :slight_smile:
```

---
## \#10 Posted by: Mikenopolis Posted at: 2017-11-02T22:14:08.940Z Reads: 156

```
[quote="monkey32, post:9, topic:37205"]
try giving him an answer in Spanish. Fuck man
[/quote]

*sigh* ....we are ALL just keyboard warriors now and then aren't we? @ShutterShock's comment was correcting @almogu's terminology. Your comment basically consist of three profanities and ended with you agreeing with what Ryan said anyway.

And is someone really a dumbass because they only speak English or smart because they speak two? I speak three and still dumb as hell.
```

---
## \#11 Posted by: Hummie Posted at: 2017-11-02T23:05:39.324Z Reads: 140

```
can definitely do higher than 50 motor amps, if that's what you're saying you are doing Im not sure.     i haven't had a problem at 100.    you can access a lot more power increasing the motor amps.  its a different animal.  the battery amps more so happen at higher speed so its not a true 100 amps being sucks from the battery.
```

---
## \#12 Posted by: krloz Posted at: 2017-11-02T23:12:56.198Z Reads: 132

```
Yo creo que eso es peligroso para los vescs. Una sincronización tan perfecta no creo que sea viable y el chip que se encarga de sincronizar los fet es tremendamente delicado.  Como dicen investiga a ver porque igual no lo tienes bien configurado.  Sino me suena que había por el mundo una variante del vesc pero optimizada para mucha más potencia diseñada para bicis y karts.
Come on guys. Being nice is free and gets you good karma :wink:
```

---
## \#13 Posted by: ShutterShock Posted at: 2017-11-03T01:17:16.309Z Reads: 126

```
Thanks Mike, I agree I wasn't trying to be a dick, just slight sarcasm lol. Sometimes people just don't know so why not provide correct information.
```

---
## \#14 Posted by: ShutterShock Posted at: 2017-11-03T01:23:03.676Z Reads: 115

```
No need to get aggressive, I was just playing around. Thanks.
```

---
## \#15 Posted by: Eboosted Posted at: 2017-11-03T05:20:14.931Z Reads: 105

```
@almogu te sugiero hacer un upgrade de motor, consíguete un 6374 o un 6384, no son tan caros, reusa tu VESC.

Dime que VESC y que batería usas y te ayudo a configurarlo para que le saques máximo provecho.

En que parte de España estas? @tueboard puede darte una mano con este tema también! 

Suerte y bienvenido al foro!
```

---
## \#16 Posted by: MysticalDork Posted at: 2017-11-03T05:34:15.246Z Reads: 102

```
@almogu If you want more power than a 4.12 vesc can give, it would be easier to just buy a more powerful vesc with upgraded components that can handle more power, like a FOCBOX, vesc6, Ollin v1.1, etc. There are a couple others as well but I can't remember the names. They can all give much more power in a single vesc. 

I think multiple vesc with 1 motor **could** be done, but it's more work than it's worth.

You'd be surprised how much power the "little" BLDC motors have. If you can't get enough out of that big old clunker motor, I think it would be a good idea to upgrade to a 6374 or 6384 like eboosted suggests.
```

---
## \#17 Posted by: monkey32 Posted at: 2017-11-03T06:20:36.176Z Reads: 97

```
Appologies gents.....my tirade was venting some personal stuff.....didn't take the comment as it as intended. I was a dick. 

@ShutterShock - sorry brother no harsh feels nor words.
```

---
## \#18 Posted by: krloz Posted at: 2017-11-03T07:33:35.735Z Reads: 91

```
Hell yeah!! Good karma for everyone XD
```

---
## \#19 Posted by: ShutterShock Posted at: 2017-11-03T17:40:48.005Z Reads: 78

```
No problem. All good here
```

---
## \#20 Posted by: krloz Posted at: 2017-11-03T20:47:25.501Z Reads: 70

```
So what do we conclude on the 2 vescs one motor issue. 
A parte me he dado cuenta de que sí tu motor está limitado a 36v y 25A tu problema no está en los vescs qué cualquiera puede con 42v y 50A sino en tu motor.  Mis motores no son gran cosa y comen hasta 60A a 42v
```

---
## \#21 Posted by: MysticalDork Posted at: 2017-11-03T21:00:27.968Z Reads: 65

```
Yep. Go with a brushless motor, they're very powerful.
```

---
## \#22 Posted by: almogu Posted at: 2017-11-05T07:53:57.562Z Reads: 52

```
Thank you all for the comments. I will consider the idea of ​​changing the engine but before I will review the optimal configuration to try to get the engine to give me more. before having these pieces of wheels, I went with some longboard and ran well and hard. I have more than 8 years in the world of electric skateboarding and we started a group of people to move the theme of electric skateboarding in Spain. With respect, tueboard, just started and only with homemade skate and with what you see on the Internet not by knowledge.
```

---
## \#23 Posted by: Surfer Posted at: 2017-11-05T08:52:48.545Z Reads: 42

```
Oh yes you have so much knowledge, @tueboard ? Nah! he is only looking in internet, he doesn't have any knowledge, he only owns couple electric e-sk8 websites,  and he only has so many different electric skates, and yes a lot more knowledge than you about modern skates. You still stuck with 40 kilos skate from the last decade. Yes with respect.
```

---
