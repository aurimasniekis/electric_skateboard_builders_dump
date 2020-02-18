# Unknown Hall error: 255

### Replies: 113 Views: 5448

## \#1 Posted by: bullrider12 Posted at: 2017-11-01T13:08:08.088Z Reads: 381

```
I recently got two Racerstars 200kv with 5 wire sensors. To make them work with the vesc I soldered a 6 pin jst to it.
Since the Temperatur signal is missing, I skipped this cable. 

I want To run both motors in hybrid mode, so I started a new motor detection.
Everything is fine expect the detection of the Hall Sensor.

It always shows me this message: unknown Hall error: 255.
I don't think I wired something wrong, that is why I'm even more angry that the Sensors not Working.

I already heard that running sensors in bldc hybrid mode is a hit or miss. But if it's a miss can it ever go to a hit? Or do I have to dismiss my sensors? 

I would be glad for any solution or advice! 
Thank you :slight_smile:
```

---
## \#2 Posted by: longhairedboy Posted at: 2017-11-01T13:12:04.623Z Reads: 353

```
if you have a volt meter you could check all your sensor wires for breaks, sometimes tiny wires with shit insulation can break inside the insulation with no outward indication of having done so. 

[quote="bullrider12, post:1, topic:37058"]
I already heard that running sensors in bldc hybrid mode is a hit or miss.
[/quote]

not to derail from your question but what does "hit or miss" mean exactly in regard to running BLDC hybrid?
```

---
## \#3 Posted by: rich Posted at: 2017-11-01T13:15:50.744Z Reads: 342

```
Did you try to swap motor cables and redo hall sensor detection? That worked for me. If the motor spins backwards then you have a "invert motor direction" button in vesc tool.
```

---
## \#4 Posted by: bullrider12 Posted at: 2017-11-01T13:19:01.980Z Reads: 335

```
thanks For your reply! 
Well that's probably something I need to do. 
I also tried detecting the Hall sensors in the foc tab and the results are quite good I think. At least there is no error message.

I read This (hit or miss) in another thread and I think it simply means that either your sensors work or they don't work with your vesc.
```

---
## \#5 Posted by: bullrider12 Posted at: 2017-11-01T13:20:59.786Z Reads: 314

```
Unfortunately I have those shitty mt60 connectors which only allows one configuration of the phase wires. 

But thank you for the advice, I will try that tonight :slight_smile:
```

---
## \#6 Posted by: Deckoz Posted at: 2017-11-01T13:42:05.056Z Reads: 305

```
I had something similar to this last night

One of my sensors must have died, checked all the wires continuity, they they're all(halls) and (temp) sending a base volt but I get 0's across the hall table now.  So from vesc to the sensor board all is good...so something on the sensor board must have gone bad.

Verified it wasn't the escs by using a different motor with sensors - which it detects. Motors probably have 1100 miles on them now. Shame the halls are epoxied to the windings, basically makes it unserviceable...ugh.
```

---
## \#7 Posted by: bullrider12 Posted at: 2017-11-01T18:04:55.906Z Reads: 299

```
Well, i switched 2 phase wires and checked all sensor wires, but it doesnt help at all. 

**VESC Terminal**
I tried to use the "param_detect" function in the vesc tool and it gives me this:

Cycle integrator limit: 116.06
Coupling factor: 771.16
Hall sensor detection failed:
-1, 5, -1, 4, 1, 6, 3, 4

**BLDC Motor Detection:**
Integrator limit: 115.89
BEMF Coupling: 863.54
Unknown hall error: 255

**FOC -Detect Hall Sensor**
<img src="/uploads/db1493/original/3X/c/c/cc961aa80f7c442501d98e25d5d48ec084ae89c6.PNG" width="690" height="110">

I'm pretty confused about the values written there as I dont know what they're meaning.
```

---
## \#8 Posted by: rich Posted at: 2017-11-03T18:40:25.691Z Reads: 271

```
Try to switch it again, there are 6 possible wire combinations, some motors doesn't work with all.

[quote="bullrider12, post:7, topic:37058"]
Unbenannt.PNG710x114 4.64 KB


I'm pretty confused about the values written there as I dont know what they're meaning.
[/quote]

In FOC the first and last number is always 255, this is no error, it's normal.
```

---
## \#9 Posted by: bullrider12 Posted at: 2017-11-03T18:42:34.256Z Reads: 260

```
Okay thank you! Im gonna try that.
The only thing is that i have mt60 connector, so wiring 6 combinations is a ton of work :smile:  
But let's do this!
```

---
## \#10 Posted by: rich Posted at: 2017-11-03T18:53:19.662Z Reads: 255

```
Your sensor and sensor port on the vesc is working in FOC so I guess it's a matter of phase wire assignment to get it detected in BLDC. If you have single 3.5mm bullets you could solder short patch cables for testing, they fit into MT60.

Or you give FOC a try (200kv is the upper limit), my motors perform really bad in hybrid BLDC but very good in FOC, no cogging at all. But it depends on the quality of the hardware, too (eg. Maytech doesn't run in FOC).
```

---
## \#11 Posted by: bigben Posted at: 2017-11-03T19:00:39.504Z Reads: 247

```
Which vesc firmware and tool are you using? I had problems with some versions of the vesc tool and firmware.
```

---
## \#12 Posted by: bullrider12 Posted at: 2017-11-03T19:06:13.112Z Reads: 250

```
I'm pretty scared to use FOC cause I cant afford to damage my vesc. I got one axle and one vanda vesc. 
My battery cables are also longer than 30cm. 

But I will test that 3.5mm bullets if i got some in my screw box.

Im using the latest vesc tool at the moment. Which version did you use?
```

---
## \#13 Posted by: bullrider12 Posted at: 2017-11-03T21:56:37.991Z Reads: 243

```
So I tried every combination the three phase wires can give me. None of them is working.
Anyone has an idea how I can check if the Sensor is working or not?
```

---
## \#14 Posted by: yaca Posted at: 2017-11-04T23:03:18.303Z Reads: 237

```
If you want to check your hall sensors from the motor you can connect the pos. and neg. wire of your sensorplug with 5 volts. You can also use a 1s battery. Then you take a voltmeter and connect it to the pos. wire and one of the sensor wires. Turn your motor slowly and it should show you +5 volts or 0 volts (or less if you use a 1s battery), it depends if it is a pos. or neg. magnet next to the sensor. Check all three sensor wires.
```

---
## \#15 Posted by: bullrider12 Posted at: 2017-11-04T23:32:59.382Z Reads: 223

```
Nice thank you! I'm gonna try that tomorrow :slight_smile:
```

---
## \#16 Posted by: bullrider12 Posted at: 2017-11-05T10:38:25.393Z Reads: 223

```
I tried it today.

Every sensor wire from H1 to H3 shows me either 5 volt or 0 volt. Depending on the pos or neg magnet next to the sensor like you said

So I assume that the sensor is fine and so are my wirings. 

But now I'm even more confused. What is the actual problem here?
```

---
## \#17 Posted by: scepterr Posted at: 2017-11-05T10:40:54.150Z Reads: 215

```
Can you you take pictures of the the sensor wires, splices, connectors
```

---
## \#18 Posted by: bullrider12 Posted at: 2017-11-05T10:58:21.734Z Reads: 225

```

Sure, I will do everything to make it work :smiley: 
<img src="/uploads/db1493/original/3X/5/5/55fdcf04da539a0bb416a5fde7886865077ce227.jpeg" width="281" height="500"><img src="/uploads/db1493/original/3X/4/0/408976d9ed3a3ed6568caa701160662a3a030d35.jpeg" width="375" height="500">

Left Foto: from motor to 6 pin connector
Right Foto: 6 pin connector

<img src="/uploads/db1493/original/3X/8/5/85d3b9cb06f5037ad66ec569c1051f7e6a9eba53.png" width="362" height="433">
```

---
## \#19 Posted by: scepterr Posted at: 2017-11-05T11:38:46.398Z Reads: 217

```
There's definitely something up with your wiring..it's giving me a headache looking at it...how many times is it split, theres an orange wire on the connector but I don't see it in the other pic. I only see 5 wires..

Also on vesc, with connector on the far side from you, left to right, it's gnd,h3,2,1,t,5v

You could ignore the white wire from the motor if there is no temp sensor which I'm sure there isnt
```

---
## \#20 Posted by: yaca Posted at: 2017-11-05T11:43:01.936Z Reads: 223

```
You have temp between H2 and H3 (actually H2 and H1). As scepterr said temp has to be next to +5V. I'm not sure about your pictures but if you have it connected like your drawing then it's wrong.

Edit: Hmm, on the pictures it seems you connected it the right way.
```

---
## \#21 Posted by: bullrider12 Posted at: 2017-11-05T12:07:57.375Z Reads: 215

```
sorry about the drawing. it's not that accurate regarding the position of the wires. It only shows which wires I connected.

you only see 5 wires becuase the motor sensor only has 5. I skipped the temp wire.
```

---
## \#22 Posted by: Martinsp Posted at: 2017-11-05T12:15:06.715Z Reads: 212

```
@bullrider12 
I am just curious if you have a wiring diagram for your motor hall sensors. Or something that is assigning the 5V, GND, H1, H2, H3 and possibly temp to the colors of the cables coming out of your motor. Or if you connected it just based on the colors. I am asking because often times manufacturers dont connect motors based on the regular normalization which is red=positive and black=negative. I have seen some motors that had the white as positive.
```

---
## \#23 Posted by: egzplicit Posted at: 2017-11-05T12:19:58.993Z Reads: 211

```

I’ve used the 140kv variant of this motor and redid the hall plug and it worked fine both in bldc hybrid and FOC. 

Double check the temp pin on vesc (usually it’s next to the 5v) and make sure you skip that.
```

---
## \#24 Posted by: bullrider12 Posted at: 2017-11-05T12:35:59.396Z Reads: 216

```
@Martinsp
This is the wiring schematic.  
<img src="/uploads/db1493/original/3X/c/8/c88a1fcb14ced0a1afd62c888bd587c4a495ea5b.PNG" width="217" height="168"> 

@egzplicit 
on the vesc connector the +5V is the green wire. 
So according to this picture, it goes to the outer side of the connector. Am I right?
<img src="/uploads/db1493/original/3X/2/7/2786ab40ca11f2c118f55ce463a84088d80f4191.png" width="294" height="500">


**I added a hopefully proper schematic of my wiring. :slight_smile:**
<img src="/uploads/db1493/original/3X/8/5/85d3b9cb06f5037ad66ec569c1051f7e6a9eba53.png" width="362" height="433">
```

---
## \#25 Posted by: Martinsp Posted at: 2017-11-05T12:45:45.480Z Reads: 195

```
That looks like it is correctly wired, and yes the 5V is near the hole in the PCB/corner of the PCB.

What you should do is: while the board is off unplug the sensor connector and connect external power supply of some kind (5V) to the hall sensor connector plug (phase wires dont matter now, you can leave them plugged in to the VESC) according to your connection to 5V and GND. **No power should go to the hall signal output (yellow white blue).** that would destroy the halls. Now connect a multimeter GND/black probe to negative of the powersupply and positive into one of the three hall sensor outputs, be carefull not to short anything (yellow, white or blue) and see what you get when you rotate the motor very slowly. You might have different values than me but important is that the values are not fluctuating when you are not rotating the motor. What I get is 0.00V in one position and when I rotate the motor a little bit (rotate it just enough that there is the next magnet facing the hall sensor) I get 0.12V. Try this with all of the three sensor wires (yellow white blue) and report back with the results.
If you have any more questions feel free to ask.
```

---
## \#26 Posted by: yaca Posted at: 2017-11-05T13:12:32.158Z Reads: 182

```
Hmm, he already did the hall sensor test today. And why it should be 0.12 volt? I tested it and it is 5 or 0 volts between positve wire and sensor wire or 5 or 0 volts between minus and sensor wire. depends which magnet pole is next to the sensor.
```

---
## \#27 Posted by: bullrider12 Posted at: 2017-11-05T13:14:21.365Z Reads: 179

```
I did this with the vesc turned on and I got either 5 or 0 volts.

@yaca
you already answered to this :smiley:
```

---
## \#28 Posted by: Martinsp Posted at: 2017-11-05T13:17:27.502Z Reads: 176

```
I missed the fact that he did the test, sorry.

It depends on what sensors you use, I used just some random sensors I had at that time so they are not very commonly used. The VESC works perfectly fine however. I said that you/he might get different values, It all depends on the halls used. The important part is that you/he should not get values jumping around/fluctuating because that might make the ESC do bad things (cogging etc.) due to incorrect readings.
```

---
## \#29 Posted by: bullrider12 Posted at: 2017-11-05T13:18:32.005Z Reads: 168

```
Okay I see what you did there. The values aren't jumping around. they are pretty constant :slight_smile:
```

---
## \#30 Posted by: Martinsp Posted at: 2017-11-05T13:27:18.177Z Reads: 171

```
I thought this would be the case since the hall detection in FOC worked, just wanted to make sure it is not wiring issue.
I had some random bad detections using the 3.1FW. So try doing the detection a couple more times maybe it will register it. Also make sure that the low dutycycle marked as "D:" is as low as you can get it. Click the ? in the VESC-tool for additional information.
```

---
## \#31 Posted by: bullrider12 Posted at: 2017-11-05T13:32:03.288Z Reads: 174

```
 Where can I find this?
I got another question regarding the combination of the phase wires. Do I have to detect and apply the new settings before trying another combination?
```

---
## \#32 Posted by: Martinsp Posted at: 2017-11-05T13:41:19.709Z Reads: 174

```
<img src="/uploads/db1493/original/3X/9/b/9b5ba8a748748edf74e6f2134d50f21732611364.png" width="690" height="440">

With the VESC combination of the phase wires does not matter while doing detection since the VESC detects the table. Once you apply and set the VESC up to work in hybrid/sensored mode you can not swap the phase wires without doing detection again.
```

---
## \#33 Posted by: bullrider12 Posted at: 2017-11-05T13:44:24.868Z Reads: 167

```
Okay, because my method was to do a motor detection and see if the hall sensors are detected. Once it fails, i switched two phase wires and did another detection and so on.
```

---
## \#34 Posted by: egzplicit Posted at: 2017-11-05T13:45:18.966Z Reads: 164

```
@bullrider12 you don’t neee to match the colours of the hall sensors, they can be in any order as long as you don’t plug one in the temperature slot. The diagram looks good but don’t bother matching the order because it doesn’t matter. Detection will figure out the order on its own.
```

---
## \#35 Posted by: bullrider12 Posted at: 2017-11-05T13:46:29.510Z Reads: 168

```
@egzplicit
yeah I thought so too, but I wanted it to look good in my eyes that's why I wired yellow to yellow and white to white and so on ^^
```

---
## \#36 Posted by: bullrider12 Posted at: 2017-11-05T14:02:22.747Z Reads: 169

```
@Martinsp 
I tried to adjust the low duty cycle from 0,01 to 0,05 and got the same failure.
```

---
## \#37 Posted by: Martinsp Posted at: 2017-11-05T14:03:47.686Z Reads: 167

```
it still displays the error message?
```

---
## \#38 Posted by: bullrider12 Posted at: 2017-11-05T14:11:34.498Z Reads: 171

```
yeah sadly. It shows me Unknown Hall Error :255

If I do the param_detect in the vesc Terminal it gives me following results:
Cycle integrator limit: 118.39
Coupling factor: 859.43
Hall sensor detection failed:
-1, 3, 5, 4, -1, 2, 1, -1

Maybe we can do something with those values.
```

---
## \#39 Posted by: Martinsp Posted at: 2017-11-05T14:13:57.432Z Reads: 172

```
Have you ever used a different FW successfully with hall sensors? Because I think that -1 is an incorrect value, the rest seem correct.
```

---
## \#40 Posted by: bullrider12 Posted at: 2017-11-05T14:18:55.132Z Reads: 168

```
No I never had a hall sensor in previous FW. I thought it could be a FW issue too, but now I need to know which FW i can use to test.

I mean besides the outer -1, there are 5 values that seems to be correct. I got only 5 wires so I assume that the -1 in the middle is the temp wire. So in my opinion it should work ^^
```

---
## \#41 Posted by: bullrider12 Posted at: 2017-11-05T14:22:07.352Z Reads: 165

```
<img src="/uploads/db1493/original/3X/7/a/7a8a66be76a938a4123f68a5f959cabd7db5b7ce.PNG" width="690" height="374">

I dont know how much this picture helps in finding the problem. But i dont want to miss a tiniest hint.
```

---
## \#42 Posted by: Martinsp Posted at: 2017-11-05T14:22:31.989Z Reads: 158

```
Hall detection does not use the temperature at all. It is in the connector just because it comes from the motor if you have a temp sensor in there. The temp sensor is not part of the detection in any way. 

What HW are you using? I would try 2.54 from @Ackmaniac.
```

---
## \#43 Posted by: bullrider12 Posted at: 2017-11-05T14:23:51.043Z Reads: 148

```
Oh okay. I see. 

I'm using 4.12 HW and will give that 2.54 FW a try.
```

---
## \#44 Posted by: bullrider12 Posted at: 2017-11-05T14:35:28.491Z Reads: 154

```
Didn't work.
Damn I'm tired of this sensor. Thought it would be easy to implement it to my system. I guess I just have to stay with sensorless setup for a while.
```

---
## \#45 Posted by: Martinsp Posted at: 2017-11-05T14:50:28.059Z Reads: 153

```
Man that sucks.. usually it is easy but there seems to me something wrong regarding the hardware. :/ Does it happen with this motor on more than one VESC? Or does the VESC work with sensors with any other motor?
```

---
## \#46 Posted by: bullrider12 Posted at: 2017-11-05T15:00:29.042Z Reads: 151

```
I got two of them for a dual setup. None of them is working with a sensor.
Since I dont have other motors with hall sensors, i can test this option. 

What if other sensored motors would work? Are my sensors not compatible with the vesc? I doubt that cause other people are pretty succesful in setting this motor up...
```

---
## \#47 Posted by: Martinsp Posted at: 2017-11-05T15:17:03.560Z Reads: 146

```
Hmm okay I doubt that this is going to be a problem but this is unfortunately the last idea I have :/ Measure from one of the pins of the hall sensor connector to resistors R8 R9 or R10. Each pin should be connected to one of the resistors. You should measure between the connector and one side of the resistor a direct short and on the other side of the resistor you should have 10 kΩ.
```

---
## \#48 Posted by: bullrider12 Posted at: 2017-11-05T16:12:36.553Z Reads: 148

```
Thank you mate, i will try that in the next few days :slight_smile:
```

---
## \#49 Posted by: bullrider12 Posted at: 2017-11-09T20:46:20.529Z Reads: 149

```
Just a quick question:

If I want to measure the hall sensor voltages, do I have to measure 5+ and H1, H2, H3 or GND and H1, H2, H3?
```

---
## \#50 Posted by: Martinsp Posted at: 2017-11-09T22:43:19.396Z Reads: 146

```
Measure the voltage of the hall signal (H1 H2 H3)with the black probe on GND
```

---
## \#51 Posted by: bullrider12 Posted at: 2017-11-09T22:45:33.929Z Reads: 146

```
Okay, I tried that too, but ground to H1 H2 or H3 is not giving me any results. 
But if I use the 5V pin and measure it with H1 H2 H3 i get either 0 or 5 volts.
```

---
## \#52 Posted by: bullrider12 Posted at: 2017-11-09T22:48:20.508Z Reads: 148

```
I'm have the bad feeling that they soldered something wrong in this 200 kv batch ^^

Two other guys are having the same problem too. So maybe there is something wrong with the motors :blush: 
@kylepls @vishal_tejwani
```

---
## \#53 Posted by: bullrider12 Posted at: 2017-11-09T22:55:15.267Z Reads: 145

```
@Martinsp
What is the worst thing that can happen if I change gnd and 5v
```

---
## \#54 Posted by: egzplicit Posted at: 2017-11-09T22:59:48.080Z Reads: 146

```
That’s a shame. I’ll take one of my motor out in a week and I will test my hall sensors to see if I get 5v between GND and H1/H2/H3 if that helps.

I don’t know the electronics in a hall sensor but I assume it will fry it if you reverse polarity.
```

---
## \#55 Posted by: bullrider12 Posted at: 2017-11-09T23:07:17.376Z Reads: 151

```
That would be nice :slight_smile:
Thank you!
```

---
## \#56 Posted by: Martinsp Posted at: 2017-11-09T23:07:28.775Z Reads: 150

```
Do not reverse the polarity of the power supply (power input to the halls). I was talking about the position of your measuring probes not where you connect the power.
```

---
## \#57 Posted by: egzplicit Posted at: 2017-11-09T23:09:05.371Z Reads: 150

```
Why would he get readings between 5v and H wires instead of GND and H? So weird...
```

---
## \#58 Posted by: Martinsp Posted at: 2017-11-09T23:10:36.588Z Reads: 147

```
I dont really think that that is possible. You should get at least something... is there a chance you had your probes not connected properly?
```

---
## \#59 Posted by: bullrider12 Posted at: 2017-11-09T23:39:23.693Z Reads: 149

```
I will try again tomorrow, but I'm pretty sure I did it right.

Since I don't have an external power source I connected the gnd and 5v from sensor to the vesc and pulled out the sensor wires from the jst connector. Don't worry I made sure they don't touch each other :slight_smile: 

Then I connected one probe to gnd and the other one to (h1 h2 h3) and got 0 volts. Even if I turned the motor by hand.

After that I tried it with 5v and (h1 h2 h3) and instantly got 5v. Turning the motor to next magnet gave me 0 volt and so on.

Let me try it again tomorrow.
```

---
## \#60 Posted by: yaca Posted at: 2017-11-10T00:10:23.069Z Reads: 151

```
Usually I measured my hall sensors with a 1s lipo battery and I got  the same volts between + and H and also between gnd and H, 0 / 4 volts, just the opposite way (depends on the magnet pole).
Now first time I measurd directly at the sensor plug (focbox) when the vesc is on. I don't know what that means but I measured strange values. Between + and H I get 5,13 / 1,54 volts and between gnd and H I get  3,62 / 0,03 volts. Anybody knows if this values are normal?
```

---
## \#61 Posted by: Martinsp Posted at: 2017-11-10T00:19:01.153Z Reads: 150

```
That is very strange behavior. :thinking:
Try this @bullrider12 measure between 5V and H(does not matter which one) and rotate the motor by hand slowly to a point where you get 0V on your meter. Now without moving the motor connect the meter instead of 5V to GND and you should be getting those 5V. Because you are using different "side" (5V being one side and GND the other) as a reference so where you get 5V against 5V you should get 0V against GND and vice versa.

@yaca the exact values may be different because of the saturation curve of the hall sensors used. But this is my theory with your case: When you get 5,13 against 5V (as I explained in previous part of this reply) it is normal that you get low value against GND. the VESC was supplying 5,16V (5.13+0.03) at that time it seems like, which is correct. The same goes for 3.62+1,54=5.16 It is OK, you are just referencing the voltage against a different part of the supply. If your VESC works/recognizes the sensors you are good.
```

---
## \#62 Posted by: bullrider12 Posted at: 2017-11-10T08:19:52.145Z Reads: 146

```
Tried this again with same results.
5v/H = 5.15/0 volt
Gnd/H= 0 volt

I got two motors/two vescs and measured this on both with the Results above... 
so what does this actually mean for me.
```

---
## \#63 Posted by: bullrider12 Posted at: 2017-11-17T16:20:26.716Z Reads: 145

```
**Update**

I finally got my sensored setup working. I'm not using the stock sensors from my motors cause it seems like there is broken cable somewhere. Since I don't want to open up my motor I tried to build an external hall sensor after this tutorial: http://www.instructables.com/id/How-to-Add-External-Hall-Sensors-to-a-Turnigy-SK3-/

Thank you for that tutorial btw. @danielz :slight_smile:

It was a pain in the ass to solder those tiny parts, but in the end it all worked out :slight_smile: 

Thanks to everyone who participated in this problem!
```

---
## \#64 Posted by: danielz Posted at: 2017-11-17T16:35:01.993Z Reads: 139

```
Excellent, they are tricky to solder, i broke the legs off on my first attempt lol
```

---
## \#65 Posted by: briman05 Posted at: 2017-12-23T03:49:58.446Z Reads: 138

```
Could this issue be because of the orange cable which would be the temp sensor is not soldered to a line thus creating a second grounded pin. If you popped that pin out it could correct the problem
```

---
## \#66 Posted by: Luuke Posted at: 2018-01-18T17:45:20.212Z Reads: 141

```
I have also problems with the Hall sensor detection of my Motor as well (maytech 6374 170KV).
VESC is a Focbox.
I can measure 0V or 3.3 V on all 3 lines (orange, brown and green) depending on motorposition.
VCC is 5.1V
Yellow one ist temp sensor. I can see roomtemperature in the VESC tool.
I tried higher currents as well. Rotor is spinning.

Do i need 5V signal level for the halls?
Then I have to lower the trigger level....
![34|312x500](upload://piuy2ThdoPetCOsP4fkWNRrXMNo.jpg)
```

---
## \#67 Posted by: Martinsp Posted at: 2018-01-18T19:29:29.312Z Reads: 132

```
That is odd... do you get any numbers? Or just fail with no values for the sensors detected?
```

---
## \#68 Posted by: Luuke Posted at: 2018-01-18T20:04:48.600Z Reads: 132

```
No values, just error :(
```

---
## \#69 Posted by: Martinsp Posted at: 2018-01-18T20:06:33.963Z Reads: 133

```
In both BLDC and FOC? BLDC si said to be a hit or miss with some hall sensors
```

---
## \#70 Posted by: Luuke Posted at: 2018-01-18T20:15:24.396Z Reads: 134

```
Just tried foc
```

---
## \#71 Posted by: Martinsp Posted at: 2018-01-18T20:20:24.590Z Reads: 131

```
with the same result?
```

---
## \#72 Posted by: Luuke Posted at: 2018-01-19T14:45:23.789Z Reads: 137

```
This are the results for BLDC & FOC.
Both failed!
![HALL_BLDC|690x376](upload://jEuljxPg03IEp7Lsom31kDgyxGD.JPG)![HALL_FOC|690x380](upload://w5QvfHEb5M8nB4Mu6tLBEj4h6we.jpg)
```

---
## \#73 Posted by: louwii Posted at: 2018-01-21T08:43:21.202Z Reads: 131

```
I'm joining in.

I did the motor detection in BLDC and FOC with sensors. It fails in BLDC mode, the hall table is exactly like the one @Luuke has in BLDC.
However, in FOC mode, the sensor detection went fine, I got proper values in the table.

Is that normal ? I'm quite bothered as I'm using a Torqueboard Vesc for now on a 10S battery, I don't really want to run FOC as it seems that those VESC don't really like it...
```

---
## \#74 Posted by: scepterr Posted at: 2018-01-21T10:01:13.276Z Reads: 131

```
@louwii What motor is this on?

Also, @Luuke I'm pretty certain your motor doesn't have a temp sensor unless you added one, I would verify wire order, the vesc, focbox have an internal temp sensor that always shows temp
```

---
## \#75 Posted by: louwii Posted at: 2018-01-21T20:13:24.970Z Reads: 128

```
That's on a build kit board motor, that I bought used from a forum member.
```

---
## \#76 Posted by: scepterr Posted at: 2018-01-21T20:15:15.587Z Reads: 127

```
Can you take a pic of the connector
```

---
## \#77 Posted by: briman05 Posted at: 2018-01-22T00:12:41.977Z Reads: 128

```
@Luuke I would take out your temp sensor wire if your motor has no temp sensor. It is basically acting as a second ground. Try taking it out and redo it. You can not have to grounds in your wiring.
```

---
## \#78 Posted by: Luuke Posted at: 2018-01-22T06:41:03.624Z Reads: 126

```
I have a temperature sensor!
Value is around 1.7 volt, which is correct for ambient temperatur.
I also measured the three pins of the halls. They seem to be OK as well.
```

---
## \#79 Posted by: scepterr Posted at: 2018-01-22T06:48:06.343Z Reads: 125

```
I'm not familiar with a maytech model that comes with temp sensor, do you have a link?
```

---
## \#80 Posted by: louwii Posted at: 2018-01-22T07:08:14.883Z Reads: 130

```
![IMG_20180121_225154|375x500](upload://ym5QaJ6nfFWewKr3tWQYfffpJrh.jpg)

There you go. I believe the missing wire is for temperature.
```

---
## \#81 Posted by: scepterr Posted at: 2018-01-22T07:12:11.742Z Reads: 128

```
Yeah the connector and wire order is fine, hmmm
I would make sure that when you plug it into the vesc the wires are fully seated in the connector sockets, I've seen sometimes they get pushed up a bit and cause isssues
```

---
## \#82 Posted by: louwii Posted at: 2018-01-22T07:17:10.697Z Reads: 127

```
I really don't get why it would work on FOC but not BLDC. I'm just stumped. DIY is nice but sometimes, debugging stuff is painful. I wish it was as easy as debugging software :sweat_smile:

Can I just use the hall table found in FOC and put them manually in BLDC ?

I'll try to do those steps http://www.electric-skateboard.builders/t/unknown-hall-error-255/37058/61?u=louwii tomorrow and see if there's something unusual.
```

---
## \#83 Posted by: scepterr Posted at: 2018-01-22T07:18:37.259Z Reads: 132

```
The values are different you can't swap them, and the FOC sensor test is different, I've seen that happen before where bldc doesn't detect and FOC does
```

---
## \#84 Posted by: Luke23 Posted at: 2018-03-18T10:46:20.690Z Reads: 127

```
Hello guys 👋 
Did you already solved the 255 Hall Sensor Problem ? 
I had the same Error Code 255 under Bldc Sensor detection with one of my 90mm Maytech Hubs. 
Under the foc detection the sensors worked fine, realy unexplainable for me.
Now it works. I only switched two of the three   cables from the motor. Now the motor was spinning backwards and I set the value of invert motor detection on true that the motor can spin in the right direction.
Everything is fine now and I‘m running in Bldc Hybrid Mode now.
Hope this helps someone, nearly got mad about this problem 😉
```

---
## \#85 Posted by: Mikenopolis Posted at: 2018-05-09T18:57:49.056Z Reads: 117

```
Ok I’m confused. I’m having that “unknown hall error: 255” problem

I have two motors from @scepterr  One detected fine. And another gives this error. Wires are the same on both. Any ideas?

![image|666x500](upload://uFfcIzaNvG2lHoX9E0h73r3R8DK.jpeg)
```

---
## \#86 Posted by: briman05 Posted at: 2018-05-09T19:33:05.255Z Reads: 112

```
Maybe try it in Foc.  I had a hall sensor failure on my motors one worked on the bldc tool then switched to ack's tool and neither worked and I thought I screwed up my focboxes or motors.  Put it in Foc and both motor sensors picked up first try
```

---
## \#87 Posted by: Mikenopolis Posted at: 2018-05-09T19:50:41.901Z Reads: 113

```
My pack is 12s. Fried a FocBox last time around. Not gonna mix 12s and FOC for now. I just closed everything up and running sensorless BLDC for now. 

I always kick off so I guess it’s not much of an issue. 

I also finished reinstalling my CarvOn Raptor this morning in Sensored FOC with zero issues. Makes me wonder if it’s the motor or sensor itself
```

---
## \#88 Posted by: banjaxxed Posted at: 2018-05-10T06:50:11.610Z Reads: 114

```
Try the increasing the duty, that worked for me on maytech hubs I'm playing with, I was getting the same error, I got so frustrated with the detection I started using the wizard to wipe config & start again, it's actually dammed good.

I had to go really high with the duty, maybe something about the type of sensors maytech use![image|690x414](upload://erZBeYMAJJpFLXifcUR17BMGDOR.png)
```

---
## \#89 Posted by: amazingdave Posted at: 2018-05-10T14:51:40.310Z Reads: 106

```
How high did you have to go? I’m having no luck detecting a dark matter motor.... also on 12s so don’t want to risk foc.
```

---
## \#90 Posted by: banjaxxed Posted at: 2018-05-10T14:52:24.527Z Reads: 106

```
0.14 per screen
```

---
## \#91 Posted by: Mikenopolis Posted at: 2018-05-10T15:18:54.104Z Reads: 107

```
I tried. Went all the way up to .20!

The other motor worked at .10 I’m really thinking the sensor is the problem
```

---
## \#92 Posted by: Blasto Posted at: 2018-05-10T15:26:37.542Z Reads: 107

```
Try the foc sensor detection, it will give you a more detailed hall table
```

---
## \#93 Posted by: Bjork3n Posted at: 2018-05-10T15:31:38.999Z Reads: 108

```
Try a shorter usb cable, it worked for me. 
Had the exact same issue
```

---
## \#94 Posted by: banjaxxed Posted at: 2018-05-10T16:46:40.715Z Reads: 109

```
Same here, detection happened but there was a complaint about one of the values, time for the multimeter compadre
```

---
## \#95 Posted by: banjaxxed Posted at: 2018-05-10T16:47:23.274Z Reads: 108

```
Fraid not, his other one using the same cable was fine
```

---
## \#96 Posted by: Mikenopolis Posted at: 2018-05-10T17:07:08.744Z Reads: 107

```
So what do I do with the multimeter. Just check each wire’s voltage?

Definitely not the wire length since I setup three out of four motors. Swapped vesc as well so it more likely the motor or sensor. 

@scepterr when you get get better, let me know in PM If you have any suggestions
```

---
## \#97 Posted by: Bjork3n Posted at: 2018-05-10T17:23:59.564Z Reads: 102

```
That was the same case for me. One box had no issues but the other did not like the long usb.

Most likely we had different issues.
```

---
## \#98 Posted by: banjaxxed Posted at: 2018-05-10T17:27:17.516Z Reads: 104

```
I'm going to use @Martinsp's method to zero in on the problem sensor/wire
 http://www.electric-skateboard.builders/t/unknown-hall-error-255/37058/61?u=banjaxxed
```

---
## \#99 Posted by: TarzanHBK Posted at: 2018-05-13T10:56:32.752Z Reads: 105

```
How does your motor act while detection?
```

---
## \#100 Posted by: Esk8t.nz Posted at: 2018-05-15T12:11:10.867Z Reads: 109

```
Just got the dreaded unknown hall error 255..
What was the fix for this besides risking run foc.. 😂😂
```

---
## \#101 Posted by: Esk8t.nz Posted at: 2018-05-16T07:26:24.701Z Reads: 110

```
so you just changed your phase wires and it fixed your 255 error?
```

---
## \#102 Posted by: Luke23 Posted at: 2018-05-17T17:57:53.827Z Reads: 111

```
Yes, for me it worked with switching two motor wires and invert the motor spinning direction. 
It makes no sense at all but now it works ;)
Hope you fix it also.

http://www.electric-skateboard.builders/t/unknown-hall-error-255/37058/84?u=luke23
```

---
## \#103 Posted by: Esk8t.nz Posted at: 2018-05-18T12:01:53.836Z Reads: 108

```
Thnx.. got it sorted.. dectected and running in bldc hybrid..
```

---
## \#104 Posted by: Mikenopolis Posted at: 2018-05-18T16:52:30.148Z Reads: 107

```
congrats.

you what you swap two wires, then detected in the opposite directions, then inverted motor direction in app?

OR

did you swap two wires, inverted direction THEN detect?
```

---
## \#105 Posted by: Esk8t.nz Posted at: 2018-05-19T05:24:16.903Z Reads: 103

```
![20180518_195937|690x335](upload://5S13JTW4DrT4Cf1Q5eKaNgXDOCx.jpg)

I bumped up the D value.. and switch phase wires arnd in difrent combinations then out of no where it detected.. haha..
```

---
## \#106 Posted by: Esk8t.nz Posted at: 2018-05-19T05:25:15.737Z Reads: 101

```
Hopefully yoy can sort yours..
```

---
## \#107 Posted by: Mikenopolis Posted at: 2018-05-19T05:33:33.449Z Reads: 101

```
I changed the duty value all the to.20 before I gave up. I'll live with sensorless for now. Really tired to opening it up these past two weeks lol
```

---
## \#108 Posted by: banjaxxed Posted at: 2018-05-20T08:49:14.945Z Reads: 99

```
Cheap slutty sensors love the 'D' 😂
```

---
## \#109 Posted by: Blacksheep Posted at: 2018-05-20T15:50:47.898Z Reads: 97

```
I get this error with my torqueboard hubs but I don’t have sensor ?
```

---
## \#110 Posted by: banjaxxed Posted at: 2018-05-20T18:33:15.651Z Reads: 96

```
There's no reason to run hall sensor detection if you don't have sensors
```

---
## \#111 Posted by: Blacksheep Posted at: 2018-05-20T22:34:00.107Z Reads: 95

```
No I just run motor detection
```

---
## \#112 Posted by: OKI Posted at: 2018-05-23T09:32:11.169Z Reads: 94

```
Detection results:
Integrator limit: 121.98
BEMF Coupling: 676.60
Unknown hall error: 254

Hello;
Have problems detect sensor hall motor maytech please help.
```

---
## \#114 Posted by: PaleRider Posted at: 2019-09-15T21:06:02.289Z Reads: 20

```
[quote="Blacksheep, post:109, topic:37058, full:true"]
I get this error with my torqueboard hubs but I don’t have sensor ?
[/quote]


Same here: motors running unsensored, show "unknow hall error 255" during motor detection.
Everything seems to run fine.
Is there a problem to fix, or I could just forget about it?
```

---
