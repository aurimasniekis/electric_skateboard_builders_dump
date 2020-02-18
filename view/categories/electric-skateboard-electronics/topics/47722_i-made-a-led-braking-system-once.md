# I made a LED braking system once

### Replies: 34 Views: 1943

## \#1 Posted by: LunarKim Posted at: 2018-02-28T01:11:32.060Z Reads: 353

```
https://youtu.be/w369Y7ochqQ

I would like to let me know if you have any good LED patterns.

Of course the module was made by a friend. I just put the receiver on.

https://www.electric-skateboard.builders/t/braking-signal-system/45770?u=lunarkim
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2018-02-28T01:13:43.317Z Reads: 327

```
How did you make this?
```

---
## \#3 Posted by: ZackoryCramer Posted at: 2018-02-28T01:13:57.296Z Reads: 318

```
I saw a short clip of the carvon esk8's with lights lighting up when the board is turning towards the corresponding side.
```

---
## \#4 Posted by: LunarKim Posted at: 2018-02-28T02:03:30.477Z Reads: 301

```
A friend with a knowledge of electronics made me. It's plugged into the receiver.
```

---
## \#5 Posted by: ARetardedPillow Posted at: 2018-02-28T02:10:30.914Z Reads: 293

```
Does he have a tutorial for it? I really want to know how this works :grin:
```

---
## \#6 Posted by: ZackoryCramer Posted at: 2018-02-28T03:12:48.686Z Reads: 286

```
You can use an Arduino as an add-on between the receiver and Vesc. The Arduino can read the ppm(I assume) input and determine what state the vesc is in.
```

---
## \#7 Posted by: Scoo_B_SK8 Posted at: 2018-02-28T03:31:15.900Z Reads: 267

```
solidgeek just put a snip of code that might help.  I did similar with different style remote but pretty much map the throttle, anything idle (val) blink led and brake(Val) led on.  On analog stick you can even incorporate turn signals, but sure a 3 way switch would work too
```

---
## \#8 Posted by: laurnts Posted at: 2018-02-28T03:39:34.462Z Reads: 259

```
@LunarKim How about selling two of it for me :smiley:
```

---
## \#9 Posted by: PartyPoison Posted at: 2018-02-28T05:16:29.933Z Reads: 250

```
This might help you on making those brake lights, Done by @Nowind on his carver  https://www.electric-skateboard.builders/t/trampa-street-carver-nowind-build-history/15192/101?u=partypoison
```

---
## \#10 Posted by: eb1925 Posted at: 2018-02-28T05:47:32.132Z Reads: 242

```
This is some next level shit man! He should make these to sell, I'd buy haha.
```

---
## \#11 Posted by: AntiPusher Posted at: 2018-02-28T05:59:36.520Z Reads: 229

```
These Look Awesome!!!!!!!!!!!!!!!!
```

---
## \#12 Posted by: Slak Posted at: 2018-02-28T10:04:53.108Z Reads: 218

```
And what do you do if there is a problem with the Arduino ? You can't use your esk8 then because your PWM signal does not reach the VESC anymore ?

I really really think it's a bad idea to put some electronic (thus potential problems thus less safety for you) between the receiver and the VESC but it's just maybe me. I did LED braking system on my build and I have nothing between VESC and receiver. There is at least to different ways to achieve that, can you find them ?

PS : I said "between the receiver and Vesc" because it's what you stated, meaning PPM is going to Arduino only and Arduino transfers it to VESC next. Is this what you think of (because my answer is based on that ;) )
```

---
## \#13 Posted by: LunarKim Posted at: 2018-02-28T13:49:43.946Z Reads: 202

```
It is connected to the receiver in parallel using a Y-cable. And a friend told me that the module of the LED braking system is not Arduino.

![20180228_224108|666x500](upload://8bqDtU4yR31bxlJcmnY3gxc3R0a.jpg)

I have drawn the connection structure.

![20180228_211821|374x500](upload://6zgDXBbshvl2aGnDhaiTPWRvfzw.jpg)![20180228_211732|374x500](upload://kHnM9htVfGSmI36XWrhzGx8cVEz.jpg)

It is a LED braking system module made by a friend.
```

---
## \#14 Posted by: SkaterBoy58 Posted at: 2018-02-28T14:01:14.627Z Reads: 191

```
do you have a circuit diagram of the pcb?
Cheers
```

---
## \#15 Posted by: Slak Posted at: 2018-02-28T14:07:41.319Z Reads: 189

```
Hey Lunar, it is one of the solution to do it. I guessed it was done like this but @ZackoryCramer said "between the receiver and Vesc" so I added my post-scriptum to be sure he was aware it was not "between" but "in parallel".

Nice job from your friend. Don't know if you can easily change thresholds or colors but even the capa is here (to protect) and it's even smaller than an arduino pro mini, good point !
```

---
## \#16 Posted by: LunarKim Posted at: 2018-02-28T14:29:57.070Z Reads: 184

```
I saw four wires on this PCB and plug the LED pattern into the USB connection.
```

---
## \#17 Posted by: LunarKim Posted at: 2018-02-28T14:31:49.080Z Reads: 180

```
This PCB was made by the idea of ​​a friend. I am an excellent guy who wants to learn.
```

---
## \#18 Posted by: rene Posted at: 2018-02-28T14:43:02.605Z Reads: 186

```
[quote="LunarKim, post:17, topic:47722"]
This PCB was made by the idea of ​​a friend.
[/quote]

Could you ask your friend to share some details about the PCB - I would like to use this. Had the same Idea using an Arduino - but why to invent the wheel, a second time.
```

---
## \#19 Posted by: LunarKim Posted at: 2018-02-28T14:46:07.681Z Reads: 185

```
Okay. I'll ask him.
```

---
## \#20 Posted by: LunarKim Posted at: 2018-03-01T10:01:23.868Z Reads: 173

```
https://youtu.be/jwIbPcdw8mY

My E-longboard.
```

---
## \#21 Posted by: linsus Posted at: 2018-03-01T15:30:31.371Z Reads: 160

```
There is code to do the same light control within the 4.xx VESC somewhere.. 
Ben had it on his board for a while. Think he even had turninglights controlled by left and right on the nrf nun-chuck.
```

---
## \#22 Posted by: Scoo_B_SK8 Posted at: 2018-03-01T15:41:16.959Z Reads: 159

```
i would think Ben had the settings in his nRF24 remote.
 this is snippet of code used to control driving lights with nun-chuck style.
could easily add too to get additional lights/reaction

//*************************--LIGHTS--*************************
//Throttle 
Throttle_PWM = analogRead(Throttle_in);
if((Throttle_PWM) < 100){
digitalWrite(Throttle_out, LED_ON);
}
else{
digitalWrite(Throttle_out, LED_OFF); 
}


//L_Signal 
Signal_PWM = analogRead(Signal_in);
if((Signal_PWM) > 100){ 
  
  if (timeElapsed > interval_Blink){        
      ledState = !ledState;         // toggle the state from HIGH to LOW to HIGH to LOW ... 
      digitalWrite(L_Signal_out, ledState);
      timeElapsed = 0;              // reset the counter to 0 so the counting starts over...
}
}
//R_Signal
else if((Signal_PWM) < -100){

if (timeElapsed > interval_Blink){        
      ledState = !ledState;         // toggle the state from HIGH to LOW to HIGH to LOW ... 
      digitalWrite(R_Signal_out, ledState);
      timeElapsed = 0;              // reset the counter to 0 so the counting starts over...
}
}
else{ 
digitalWrite(L_Signal_out, LED_OFF); 
digitalWrite(R_Signal_out, LED_OFF);
} 
//********************************************************************
```

---
## \#23 Posted by: linsus Posted at: 2018-03-01T16:08:54.648Z Reads: 143

```
Yeah, you're right. 
I never saw what was inbetween the VESC and the LEDs though. Was some led standard stripes and probably a LED driver that has a stepdown from the battery. 

Thinking of implementing something similiar.
```

---
## \#24 Posted by: Scoo_B_SK8 Posted at: 2018-03-01T16:32:33.557Z Reads: 140

```
50/50 smd led strip only needs 12v.  There are other options too.
```

---
## \#25 Posted by: Jammeslu Posted at: 2018-03-01T18:25:33.332Z Reads: 136

```
Could someone make a plug and play kit for these controlled light thing?
```

---
## \#26 Posted by: rene Posted at: 2018-03-07T09:48:00.853Z Reads: 124

```
Did you got an answer from you friend?
```

---
## \#27 Posted by: LunarKim Posted at: 2018-03-10T00:26:23.849Z Reads: 126

```
Sorry, man. He rejected the material.
```

---
## \#28 Posted by: LunarKim Posted at: 2018-03-10T00:26:47.928Z Reads: 126

```
https://youtu.be/RMWd57jnhbE
```

---
## \#29 Posted by: LunarKim Posted at: 2018-03-13T14:00:29.499Z Reads: 118

```
https://youtu.be/NUG-L9nxhh8
```

---
## \#30 Posted by: StarLoad Posted at: 2018-03-19T22:46:31.551Z Reads: 107

```
Good guy~~!
```

---
## \#31 Posted by: LunarKim Posted at: 2018-03-20T14:36:24.366Z Reads: 104

```
https://youtu.be/QQxUm87Ye_c
☺
```

---
## \#32 Posted by: LunarKim Posted at: 2018-06-17T13:40:09.456Z Reads: 77

```
![20180616_001540|666x500](upload://3IyPqYTDDwWBPbRSATHuizIimpy.jpg)

This time I made my own brake module without the help of my friend who made the brake module.
I used the Arduino nano.

https://youtu.be/UuyO-4L-XTI
```

---
## \#33 Posted by: LunarKim Posted at: 2018-06-17T13:43:31.507Z Reads: 78

```
https://youtu.be/S_N9nbEXpeg
```

---
## \#34 Posted by: LunarKim Posted at: 2018-06-19T15:00:27.344Z Reads: 62

```
https://youtu.be/c5jQANTvjwM
```

---
