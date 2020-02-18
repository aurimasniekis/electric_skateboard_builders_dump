# Almost no brakes in FOC. 12s3p 30Q battery - Flipsky 6.6 - Meepo HubMotors Style

### Replies: 106 Views: 1638

## \#1 Posted by: rey8801 Posted at: 2018-10-24T09:40:10.472Z Reads: 308

```
Hi guys! So basically I upgraded my battery from a 10s3p to 12s3p on my short board. I then changed from Maytech vesc to flipsky 6.6, Bestech D140 charge only BMS. I would first out with Diyeboard, meepo...hub motors. I used them in the past at 1-s with Maytech's vesc and I like them. Only concern was the speed, being actually 65Kv gives great torque but low speed. 
On both the vesc I am using @Ackmaniac's firmware, connect via CAN BUS. On the new Flipsky 6.6 I first tried BLDC sensorless but the motors really struggle to start even on bench testing, while was fine at 10s before. So I decide to move to FOC sensorless. Weird thing that I noticed, the motors spin in one direction during motor detection, and then they run in the opposite one on street. Is it normal for FOC detection? I repeated the detection like 20 times always the same. No reverse motor configuration enable in the VESC TOOL. Except for that, which doesn't happen in BLDC, FOC is really deadly silent. I have a weird behaviour when I engage gently the brakes on bench test https://www.youtube.com/watch?v=uybKdKPunB8. Basically they keep spinning really at low speed until I brake stronger (mainly the motor connect to the slave vesc).
Then I thought maybe it's only on bench test and I tried out on street...The accellaration is really smooth ecc...FOC does remove like 2-3 kmh, but the overall experience is better, bad news they do not brake! Really I was use to a really strong and reliable braking force with these motors at 10s and now that I move to 12s and new vesc they suck. I had to foot brake all the time, that would be expensive if I need to change one shoe every month :laughing:

Setting are basically the same as before:
![image|690x383](upload://6aP1YheTHcg4KCAhDF6Tx6ahkxH.png)  
![image|690x287](upload://5C16UWUWbgCg9HGLPreiCRmxfH4.png) 
![image|690x236](upload://cRYdZN5QrRMq1S12KHkiXOd7jdk.png) 
I was aalso thinking that maybe now 57V is too low since the battery is 50V fully charged but it doens't make any sense because it barely brakes at low speed too.

Do you guy have any idea way it sucks like that? am I missing something?

Thx thx

PS: @sayekim Hi man, I know you used meepo hubs at 12s, maybe you see the problem. Thx!
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-24T10:00:53.581Z Reads: 281

```
strange that it´s different behavior with the same settings.
I would set the bat min a bit more low like -10, but i think this shouldn´t be the issue.
did you make sure that your remote is calibrated right?
which mode you use, current no reverse with brakes?
```

---
## \#3 Posted by: rey8801 Posted at: 2018-10-24T10:03:11.292Z Reads: 278

```
I tried with two different remotes, Firefly adn Nano-x. Both well used in the past without problem.
I can lower the battery min but with dual vesc at -6A before I could really brakes strong. To me is more vesc related. Even a slightly better brake force would be still too low. They really do not brake.
Yes I am usign current no reverse with brakes. Watt limited with Ackmaniac firmware. Maybe it doesn't work well with VESC 6 hardware
```

---
## \#4 Posted by: Andy87 Posted at: 2018-10-24T10:04:38.726Z Reads: 264

```
did you tried it with the stock firmware?
```

---
## \#5 Posted by: sayekim Posted at: 2018-10-24T10:04:56.973Z Reads: 257

```
I think it is the esc too. Settings look fine and brakes were great on focboxes with 12s. 

Try the maytech with 12s if you haven’t already.
```

---
## \#6 Posted by: rey8801 Posted at: 2018-10-24T10:05:33.696Z Reads: 253

```
No didn't try it because I like the possibility of switching the modes by the app. But since doesn't work I can give it a try.
```

---
## \#7 Posted by: rey8801 Posted at: 2018-10-24T10:06:49.035Z Reads: 245

```
I am afraid the Meytech will fry instantly at 12s :laughing:
I think that a lot of people are using those ESC now. I hoep that I didn't get the only two faulty ones.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-10-24T10:08:37.917Z Reads: 239

```
it just would be one option i would consider. 
it´s not a big deal to flash the firmare back and forth.
```

---
## \#9 Posted by: sayekim Posted at: 2018-10-24T10:09:37.031Z Reads: 241

```
Oh yeah forgot about that there. 

But wasn’t that only for foc? Bldc was good for 12s on maytech. 

Get escapes or focboxes already and go belt drive. 
You will not believe how crazy 6374’s are.
```

---
## \#10 Posted by: sofu Posted at: 2018-10-24T10:15:44.797Z Reads: 235

```
The motor detection spinning one way but running spinning another thing on the flipsky vescs is a known issue. It's a bit strange but just flip your wires and keep it in mind. Weak and a bit weird braking behavior on the flipsky seems to also be a thing. Maybe it has to do with their components choice...
```

---
## \#11 Posted by: rey8801 Posted at: 2018-10-24T10:36:49.838Z Reads: 226

```
Well really they almost don't brake it's impossible to use them like that. If that is the case they are totally trash. How can I ride without brakes.
```

---
## \#12 Posted by: rey8801 Posted at: 2018-10-24T10:37:55.242Z Reads: 223

```
Yeh I know I now got 6384 motors for my next project. Crazy big. Belt drive is not my thing I really don't like the sound and the style too.
```

---
## \#13 Posted by: rey8801 Posted at: 2018-10-24T10:39:57.599Z Reads: 215

```
I will try. If that is the braking force I get you can basicaly throw the in the garbage. Better that you test them to because if that is the case we should all together ask Flipsky to fix them or refund us because it's impossible to use it. I don't understand how many people said that they are good.
```

---
## \#14 Posted by: sayekim Posted at: 2018-10-24T10:46:33.728Z Reads: 206

```
I don’t mind the sound. Besides in foc they aren’t that loud. 
I only went hub because I thought to stay stealthy to avoid authorities. 
Now riding full gear and going to many group rides that point is kind of mute now.
```

---
## \#15 Posted by: Andy87 Posted at: 2018-10-24T10:50:01.228Z Reads: 202

```
if i would have a case and the time i would through them on and test them.
without brakes they definitly useless!
did you check your fault log? maybe something cut off your break force.
```

---
## \#16 Posted by: rey8801 Posted at: 2018-10-24T10:53:13.356Z Reads: 194

```
I will check the error but at really low speed I don't see how that can be the case. I hope the original firmware will help but also @sofu specified that they have less braking force. She is testing the dual 6.6. I really don't understand why all the people that used the single 6.6 don't say that. I didn't read anything about it.
```

---
## \#17 Posted by: rey8801 Posted at: 2018-10-24T10:54:16.318Z Reads: 189

```
You can use duct tape for a test. Just saying because the more we wait the less pressure we can put on them. These are expensive garbage if that is the case :laughing:
```

---
## \#18 Posted by: rey8801 Posted at: 2018-10-24T10:55:34.952Z Reads: 195

```
In Belgium Esk8 is ok. I just don't like the bulky rear truck with belts ecc... I know that you get the best performance out of it. I will think about in case, but so far hub motors satisfied my needs.
```

---
## \#19 Posted by: sofu Posted at: 2018-10-24T10:55:51.257Z Reads: 191

```
Out of curiosity, what're your settings at? So far I've tested them on raptor 2 hubs and direct drives and results have been a bit mixed... I've yet to test them on a belt drive though so I can't say for sure if it is actually the vesc...
```

---
## \#20 Posted by: rey8801 Posted at: 2018-10-24T11:05:04.625Z Reads: 188

```
I posted them in the first post https://www.electric-skateboard.builders/t/almost-no-brakes-in-foc-12s3p-30q-battery-flipsky-6-6-meepo-hubmotors-style/72170?u=rey8801
```

---
## \#21 Posted by: Andy87 Posted at: 2018-10-24T11:05:29.252Z Reads: 176

```
i need time on the weekend. at the moment it´s already dark when i come home.
but i asked a friend here who is using the dual for quite a while.
will report back as soon as i have a feedback.
```

---
## \#22 Posted by: rey8801 Posted at: 2018-10-24T11:05:53.639Z Reads: 176

```
thxs man :wink:
```

---
## \#23 Posted by: hiboute Posted at: 2018-10-24T11:06:32.318Z Reads: 180

```
i have also two flipsky 6.6 
I though also that the brakes were too soft at speed. My parameters were -6 for batt min. I've changed it to -10, and now it is great.
```

---
## \#24 Posted by: rey8801 Posted at: 2018-10-24T11:08:15.774Z Reads: 178

```
yeh but you have to deal with your battery. I always used in the past -6A, so -12A from dual vescs back to the battery. For 3p 30Q I think it's the safe one. At the moment the brakes are not there, really I need to foot brake everytime. If I push them all the way down they almost loose all the power. Before at 10s with same setting, same motors, Maytech vescs, I could almost slide!
Are you using them at 10s or 12s? FOC or BLDC?
```

---
## \#25 Posted by: sofu Posted at: 2018-10-24T11:10:42.998Z Reads: 172

```
Oops I totally forgot that... Yeah I would maybe try -60 motor and -10 battery and see if that makes it better? I personally run -60/-15 on a 10s4p on focboxes/vesc-xs which is on the extreme side but it's working great
```

---
## \#26 Posted by: rey8801 Posted at: 2018-10-24T11:11:42.112Z Reads: 169

```
-15 on each vesc? I though that for 30Q cell is 4A each cells, so 4p = 16A. You are using almost the double
```

---
## \#27 Posted by: Andy87 Posted at: 2018-10-24T11:13:01.816Z Reads: 169

```
you not gonna do a downhill break for 1hour. think with -10 on both you still on the safe site with 3p.
```

---
## \#28 Posted by: Andy87 Posted at: 2018-10-24T11:14:34.732Z Reads: 166

```
this ratings for a full charge cycle from 2.5-4.2V.
i don´t think you brake longer than 1 minute constant.
```

---
## \#29 Posted by: rey8801 Posted at: 2018-10-24T11:14:41.479Z Reads: 161

```
True that is for short term, like 5 sec max brakes. I will try to increase them but it still means that they suck because with my previous Meytech vescs, that everyone said that they were trash, they actually always worked and never have problem. With -6A each vesc I could always brake really strong no matter the motor I used.
```

---
## \#30 Posted by: sofu Posted at: 2018-10-24T11:17:52.876Z Reads: 161

```
Yeah but you're not going to be doing 30A constant all the time on recharge. For me it only ever hits that once in a blue moon. Just nice in emergency situations that I've run into once or twice... which is once or twice too many tbh
```

---
## \#31 Posted by: rey8801 Posted at: 2018-10-24T11:19:16.033Z Reads: 164

```
ok I will start to increase it. Still not clear why they handle so badly the regenerative current compare to my older Maytech vescs. Fine we'll see it. Thx for the help.
```

---
## \#32 Posted by: Andy87 Posted at: 2018-10-24T11:28:28.623Z Reads: 163

```
ok so now it´s one to one...
the guy i asked run dual fesc 6.6 and was running before maytech 4.12
same settings, only maytech in bldc and fesc 6.6 in foc.
he says the breaks now more strong than they where with maytech before.
:thinking:
he run a dual belt drive by the way 6355 or something like this, idk exactly.
```

---
## \#33 Posted by: rey8801 Posted at: 2018-10-24T11:32:52.665Z Reads: 156

```
I would like to be 2 - 0 for him :smirk: Maybe ask him his setting and battery. So we can understand better. Did he move to FOC because he likes more than BLDC or for other reason? Because in my case I had to do it. In BLDC the motors were rattling really really bad at low speed, meaning that even if you are almost close to stop and you would accelerate they will trough you off the board since they rattle instead of spinning. Also this aspect not present with previous Vescs. Could be that just using sensor motors would avoid this behaviour.

@sofu do you mind check the video in the first post. Is that a normal behaviour in FOC? If I brake gently after spinning, the motors, mainly one keeps spinning.
```

---
## \#34 Posted by: Andy87 Posted at: 2018-10-24T11:36:51.124Z Reads: 150

```
10s 4p and he changed to foc because he wanted.
don´t think he tried bldc with the dual fesc.
other settings i don´t know yet.
```

---
## \#35 Posted by: pat.speed Posted at: 2018-10-24T11:41:10.029Z Reads: 157

```
I’m thinking maybe the flipsky components aren’t as efficient or something and that causes losses in the breaking regen. The lower regen would mean your brakes are not strong or even non existent. That would make sense but I really don’t know enough about electronics to say that’s what is wrong, do you have a bt module to check how many amps are being used in regen.

Edit: maybe even a faulty current checker (idk what the proper word is rn, I’m tired af) that is giving off a in correct reading of the current you are pulling. Example you are getting regen of 1a but the vesc thinks it’s 6a and is not letting any more go to the batt. Idk I’m just throwing out random ideas, mostly based on someone’s claims that flipsky use cheaper components to bring down costs
```

---
## \#36 Posted by: rey8801 Posted at: 2018-10-24T11:42:25.179Z Reads: 149

```
Yes I do. Next time I will log the ride. This morning I was too angry for the fact that I had to foot brake for the whole city...so annoying :joy:
```

---
## \#37 Posted by: Amonada Posted at: 2018-10-24T12:02:15.824Z Reads: 148

```
You said you changed your battery from 10s3p to12s3p. Does the new battery have a BMS?
```

---
## \#38 Posted by: sofu Posted at: 2018-10-24T12:02:16.925Z Reads: 152

```
Actually this is not normal behavior at all... I am a bit concerned 🤣
```

---
## \#39 Posted by: rey8801 Posted at: 2018-10-24T12:02:41.003Z Reads: 151

```
YEs I wrote in the first post charge only Bestech D140.
```

---
## \#40 Posted by: rey8801 Posted at: 2018-10-24T12:03:43.867Z Reads: 155

```
I tried different remotes, receiver, CAN bus ecc...
Always the same. I hope that with increasing the braking currents it will help.
```

---
## \#41 Posted by: rey8801 Posted at: 2018-10-24T12:05:57.079Z Reads: 147

```
Maybe better to ask directly to Flipsky. @BarbaraZ when you have time do you mind read the first post of this thread? Check the video and settings and maybe ask to your technicians about it. These are 2 brand new Flipsky 6.6 form the EU group buy of like last month. They basically don't have brakes at the setting reported. Same setting used before with another vesc without problem. Thank you!
```

---
## \#42 Posted by: Sender Posted at: 2018-10-24T12:08:34.859Z Reads: 146

```
I am also curious what the telemetry data says about what regen you are hitting.  It might be a simple bump in settings to get you to the same place.  Annoying, but maybe not too big of a deal.

I run regen breaking pretty damn high too though.  On 6p 30q I have -20 per vesc...  i would try -10 per on your setup to see how it is.
```

---
## \#43 Posted by: rey8801 Posted at: 2018-10-24T12:10:11.913Z Reads: 142

```
yeh I already made the new mode. I will try this evening and see it. I also not sure why the motors keep spinning while I gently brake after acceleration. You can find the video in the first post. Maybe is due to the lower setting.
```

---
## \#44 Posted by: Sender Posted at: 2018-10-24T12:11:44.195Z Reads: 139

```
Yeah, just watched the video. That does seem weird.
```

---
## \#45 Posted by: sofu Posted at: 2018-10-24T12:11:48.566Z Reads: 138

```
This is two separate 6.6s connected via canbus right? Out of curiosity, can you screenshot every page for your app settings general and app settings ppm for both vescs and put in an imgur album or something? The low brake motor issue concerns me...
```

---
## \#46 Posted by: rey8801 Posted at: 2018-10-24T12:12:43.558Z Reads: 135

```
ahahahah great :joy:
```

---
## \#47 Posted by: rey8801 Posted at: 2018-10-24T12:15:42.846Z Reads: 134

```
Yep connect by canbus. I will do ti this evening when I can reach the board. Dind't save them. I guess they should be right although is true that the motor connected to the slave vesc is the one that most of the time keeps spinning. I think the setting are ok but I will post it later.
```

---
## \#48 Posted by: Andy87 Posted at: 2018-10-24T12:29:12.662Z Reads: 137

```
Got answer from that guy.
60/-60 43/-10 are his settings.
```

---
## \#49 Posted by: rey8801 Posted at: 2018-10-24T12:34:50.805Z Reads: 137

```
ok higher as well. I will try to increase them.
```

---
## \#50 Posted by: mackann Posted at: 2018-10-24T12:52:16.739Z Reads: 136

```
I use 4x flipsky single vesc, the brakes is very very strong, i cant remember the exakt setting i have atm but i remember i did have to lower it because it was to strong, way more then my raptor 2. But i gues the 4wd helps abit to. I also run them in foc.
But it looks like you have a very low battery current max regen, try raise it.
Is it high speed brake or low speed brake that are weak?
```

---
## \#51 Posted by: rey8801 Posted at: 2018-10-24T12:54:02.528Z Reads: 134

```
I would say both acutally. They are really not comparable to before. I went a bit faster let say 30kmh only twice becasue after the first time I had to foot brake before a cross...Was early in the morning, that woke me up really fast though :grin:

BTW Congrats for the new shop! looking good...thinking about get an EVO style deck from you :wink:
```

---
## \#52 Posted by: mackann Posted at: 2018-10-24T12:58:17.328Z Reads: 137

```
Ok, i have done some brake test with them, at 70 km/h they was so strong i almost fell off (but maby it is because im used to the low brake power on the raptor 2 when going high speed) so after some tuning to lower them it work good, at 5-15 km/h they are still to strong, gonna test more tonight :smiley:
```

---
## \#53 Posted by: Ixf Posted at: 2018-10-24T13:04:38.352Z Reads: 134

```
Following.. This is really interesting.. I helped 2 friends back in taiwan build separate boards.  One is based off vesc 6 (the trampa version) one is based off focboxes.  Same gear ratio and tires.  The one on the 6 is havingreally soft brakes... I wonder if its the 6 vs 4 design?  

I have flipsky 6.6 dual on my diy and focboxes on my kaly,  The kaly def brakes harder on the same setting and ratio but it has bigger motors so probably not a good 1 to 1 test.
```

---
## \#54 Posted by: rey8801 Posted at: 2018-10-24T13:19:37.045Z Reads: 137

```
For what can I say my 4.12 vescs were way better in braking than these 6.6 I will get telemetry data to compare it. This morning I was really surprise to be honest.
```

---
## \#55 Posted by: Ackmaniac Posted at: 2018-10-24T14:29:17.509Z Reads: 131

```
Just check the voltage in the realtime data that it matches roughly the voltage you measure with a multimeter. Can be that they messed up the resistor for the sensor. 
And also check that your battery isn't overcharged. Because in that that case the voltage during regen would raise rapidly.
```

---
## \#56 Posted by: rey8801 Posted at: 2018-10-24T14:34:54.306Z Reads: 129

```
The battery was at 49.4V from external volt meter which matches the multimeter. The vesc reads 47.9V, I see from your app, that's unfrotunatelly a know issue for flipsky vesc 6.6. I think it's really a probelm of this vesc 6.6. I do not knwo why others didn't notice before. About the weird behaviour you can see in the video in the first post I have no idea actually.
```

---
## \#57 Posted by: Ackmaniac Posted at: 2018-10-24T14:44:31.573Z Reads: 133

```
When you see the realtime data with the app do you see the masters data or the slaves data? Because the master would be important here.

And a difference of about 3 % in voltage looks like they used cheap 5% tolerance resistors.
```

---
## \#58 Posted by: rey8801 Posted at: 2018-10-24T14:46:28.607Z Reads: 133

```
I see the slave unfortunately because I have the model attached to it. Master UART I used for Firefly remote. I can use it with out the uart and place there the module if needed.
The different in voltage yes, I think is reported somewhere that they use a voltage sensor with bigger tolerance. Really stupid to save money on something so visible
```

---
## \#59 Posted by: Ackmaniac Posted at: 2018-10-24T14:48:00.893Z Reads: 136

```
You can see the master via the app as well, you have to go in the settings of the app and enable CAN and select the ControllerId of the master. Please also make sure you **disabled** "Send status via CAN" in the masters VESC settings,
```

---
## \#60 Posted by: rey8801 Posted at: 2018-10-24T14:49:13.698Z Reads: 132

```
ah ok didn't know. so mine is already set like that
I thought that in that way I would visualised still the slave, but make modification also on hte master. So no definitely I see the master data on the app.
```

---
## \#61 Posted by: Ackmaniac Posted at: 2018-10-24T14:52:13.972Z Reads: 120

```
Ok then when you use the app then try to only see the data of the slave when you ride. Because it can be too much for the master to provide the realtime data to the remote and the app at the same time. When you only capture the data of the slave it is no problem.
Don't think that this is your problem but it is worth a try.
```

---
## \#62 Posted by: Ackmaniac Posted at: 2018-10-24T14:53:34.371Z Reads: 118

```
And you should also check the data when you brake. Because maybe the Firefly ESC sees too high current at low currents. Easy to do with the app by using the video function.

BTW maybe you can make a video with the app and provide it here. By that i could tell you much better what is going on in detail. That's what the feature is there for.
```

---
## \#63 Posted by: rey8801 Posted at: 2018-10-24T14:54:32.719Z Reads: 113

```
Sorry I am not following. So I have to disable the option "connect by CAN to ID 0"? But if I do that I won't be able to change the modes afterwards, right?
In the past I had the module connected to the slave too with vesc 4.12 and didn't have this problem. I think it's really the VESC.
```

---
## \#64 Posted by: Ackmaniac Posted at: 2018-10-24T14:56:46.807Z Reads: 114

```
Sadly i don't know in which frequence the remote is capturing the realtime data. So it could cause issues. But that is easy to test by just simply doing a ride without the app. If the issue is still there then that is not the root cause.
```

---
## \#65 Posted by: rey8801 Posted at: 2018-10-24T14:59:05.903Z Reads: 118

```
the receiver uses 115200 baud rate. or well the receiver is sending at 115200, while the remote itself is 9600. To be able to receive data on the remote display I need to set it at 115200 at the master UART level. I had the same behaviour also with the nano x remote, if that can helps.
```

---
## \#66 Posted by: visnu777 Posted at: 2018-10-24T15:06:04.119Z Reads: 114

```
Have you tried it without the Bluetooth module?
Really strange...
```

---
## \#67 Posted by: rey8801 Posted at: 2018-10-24T15:07:59.509Z Reads: 118

```
no the bluetooth module was always connected but I do not understand why it can be a problem with the module. I will try all the combination possible.
```

---
## \#68 Posted by: Ackmaniac Posted at: 2018-10-24T15:22:03.396Z Reads: 116

```
The Bluetooth module can only be a issue if it asks the master for the realtimedata and the remote does the same as well. Baudrates do not matter. BUt if the Nano X had the same behavior then it isn't the root cause. 
I guess the ESC detects the wrong data but that can be clarified with a video where we can see the realtime data.
```

---
## \#69 Posted by: rey8801 Posted at: 2018-10-24T15:24:02.464Z Reads: 115

```
ok I will make it and post it. I hope on bench test is gonna be fine otherwise I will crash trying to make it :joy:
```

---
## \#70 Posted by: Ackmaniac Posted at: 2018-10-24T15:42:50.323Z Reads: 113

```
No need to do crazy rides. Just simply do full brakes where it acts weird and let us know at whichsecond of the video you did so.
```

---
## \#71 Posted by: lockeboss Posted at: 2018-10-24T15:43:44.288Z Reads: 111

```
before one of my flipsky vesc broke i had one motor which brakes and one which doesnt.i think the master didnt if i rember correct.

but i didnt find something about this behavior either
```

---
## \#72 Posted by: rey8801 Posted at: 2018-10-24T15:51:21.360Z Reads: 111

```
Damn I unpacked them like 2 days ago. They both brakes but in case of gently brakes the slave in my case is keeping spinning like that . Only in FOC not in BLDC though.
```

---
## \#73 Posted by: rey8801 Posted at: 2018-10-24T15:53:16.621Z Reads: 112

```
yeh but when I rode it this morning you can not feel that behaviour. The brakes are just really weak. the only way to see this behaviour is during bench testing.
```

---
## \#74 Posted by: Ackmaniac Posted at: 2018-10-24T15:54:14.219Z Reads: 113

```
Is "Send status via CAN" active on the slave?
```

---
## \#75 Posted by: rey8801 Posted at: 2018-10-24T16:00:53.648Z Reads: 118

```
I think yes since the bluetooth works and I can change the modes on both the vesc, but to be honest I do not remember. I will check this evening. I write down all the different tests I need to do it. Thanks for the help
```

---
## \#76 Posted by: rey8801 Posted at: 2018-10-24T19:28:56.121Z Reads: 118

```
Ok so here the video after increasing the motor min and the battery min. It definetely does the trick now the brakes are ok
https://youtu.be/9e3FvLftF2A
Do you see something weird? One thing I am not sure is the duty that never reach 0 even when I engage the braking. In this case still bluetooth connected to the slave and then connect by CAN to ID 0 enable. So we are looking to the master data. Tried afterward and the weird behavior still there but when you ride you don't notice it. 


Then remove the connect to CAN ID 0 in the app to se slave data e see what happen and here the master motor now keep acceleration when I am braking.
https://youtu.be/iufUbrMm3uU
Probably the second test doesn't tell anything. Should I simply remove the Bluetooth signal from the slave and see if that helps? Or also remove the UART signal from the master VESC for the remote.


And to answer to your other question send status over can is active at the slave side.

Real voltage at the end of the ride was 48.7V.

Here a bit of telemetry data from this morinig https://www.dropbox.com/s/zbsxn1yym6lv13a/2018-10-25_10-01-47_Avenger_X_esc_Data.csv?dl=0
https://gct-hp.de/VDLA/

Screenshot of the results
![vescmonitor|281x500](upload://3GpCLZpyDuSMnqpcFidvPxUKWbp.png)

I see that the regenerative current didn't exceed -10A so seems ok.
```

---
## \#77 Posted by: rey8801 Posted at: 2018-10-24T19:39:21.686Z Reads: 115

```
Hi! So here the screenshots:
Master:

![image|690x245](upload://fdnQfMxfvRZkMGVyE4j4EeO8XUU.png) 
![image|690x277](upload://evdvyBAdWA2BScDaJanz2rGBuWc.png) 
![image|690x273](upload://kiOBKi71KZohZ5Jqr4zmGyPRqXt.png) 

Slave (bluetooth connected)
![image|690x327](upload://62TzwHTnfsHPJQbdWgS2ql1Rx5V.png) 

Do you see something weird?
Anyhow tired to rise the setting and indeed now it brakes again -60A/-11A did the trick! Thx
The weird behaviour still there.
```

---
## \#78 Posted by: sofu Posted at: 2018-10-24T21:37:39.017Z Reads: 104

```
If the "master motor still spinning on low brake" issue is still present, try swapping "Send CAN status" for both vescs. Master should have True and slave should have False. Then also turn off traction control. To be honest everything looks fine and your motor shouldn't be spinning at low brake... it should be stopped, but see if that helps?
```

---
## \#79 Posted by: rey8801 Posted at: 2018-10-24T21:41:32.024Z Reads: 108

```
Well based on what I know if you use @Ackmaniac firmware and the Bluetooth is connected to the slave then the slave vesc has to be with send status over CAN active while master not.
For the spinning during brakes is either the motor connected to the slave or both together.
```

---
## \#80 Posted by: rey8801 Posted at: 2018-10-24T22:00:01.493Z Reads: 109

```
@Ackmaniac I was also thinking at maybe connect the Bluetooth to the master VESC and move only the UART cable from the receiver to the slave vesc. The remote has a ppm signal part that would be on the master and the real data would take from the slave. In this way the master won't have to deal with double data transferring but only through the Bluetooth.
```

---
## \#81 Posted by: Ackmaniac Posted at: 2018-10-25T21:29:45.898Z Reads: 98

```
That the master still accelerates is really strange. 
Can you try to enable "Max dir switch ERPM enabled".
This way you have to release the throttle and brake again to start going backwards.
That's what i use all the time so maybe there is a mistake in the code when it is not activated. But what also looks strange is that your motor wants to go backwards at the beginning in the video when you accelerated.
```

---
## \#82 Posted by: rey8801 Posted at: 2018-10-25T21:31:38.592Z Reads: 97

```
but I am using current no rev with brakes. I don't use reverse
```

---
## \#83 Posted by: Ackmaniac Posted at: 2018-10-25T21:34:26.812Z Reads: 100

```
That makes it even more strange. Can you post the rest of your settings? Exspecially the ones which you changed.
```

---
## \#84 Posted by: rey8801 Posted at: 2018-10-25T21:35:01.119Z Reads: 98

```
do you mean the motor setting?
```

---
## \#85 Posted by: Ackmaniac Posted at: 2018-10-25T21:40:11.710Z Reads: 94

```
Yes, and a video where you connect to the master with the app while doing the same bench test would be very helpful.
```

---
## \#86 Posted by: rey8801 Posted at: 2018-10-25T21:45:37.355Z Reads: 93

```
Wait what do you mean connect to the master with the app? Do you mean I need to put the bluetooth module connected to the master? or is it ok leave it connected to the slave and activate connect to CAN ID 0?
```

---
## \#87 Posted by: Ackmaniac Posted at: 2018-10-25T21:47:04.445Z Reads: 94

```
It's ok to leave it at the slave. Only need to see the data of the master when it accelerates during braking. because the slave doesn't move but master does.
```

---
## \#88 Posted by: rey8801 Posted at: 2018-10-25T21:47:54.133Z Reads: 91

```
Ah ok, in the first video is actually the slave that moves. Other times is both. I will make the video.
```

---
## \#89 Posted by: Ackmaniac Posted at: 2018-10-25T21:49:54.481Z Reads: 92

```
[quote="rey8801, post:76, topic:72170"]
Then remove the connect to CAN ID 0 in the app to se slave data e see what happen and here the master motor now keep acceleration when I am braking.
[/quote]

So was it the master or the slave that started to move when you braked in the video where the board was on the bench? And does it do that each time or only sometimes?
```

---
## \#90 Posted by: rey8801 Posted at: 2018-10-25T21:57:17.725Z Reads: 88

```
So in the first one is the slave https://www.youtube.com/watch?v=uybKdKPunB8
in the second one https://www.youtube.com/watch?v=iufUbrMm3uU I removed connect to CAN ID 0 to have data from the slave and in that case is the master that keeps spinning.
When I ride is like the first case. They always do it on bench test, sometimes one, sometimes only the slave. I will make the video connected to the master like the first situation but with the telemetry.
```

---
## \#91 Posted by: Ackmaniac Posted at: 2018-10-25T22:11:35.759Z Reads: 87

```
Please also check if you get a clean signal from the remote when you brake by looking at the PPM signal in the tool.
And you can also check the realtime data with the tool and maybe make a video of it.
Something funny is going on which can be a noisy throttle signal or a ESC that detects wrong sensor values.
Never seen that before and did different tests with my board(s) and don't have any issues at all. No matter what i try.
```

---
## \#92 Posted by: rey8801 Posted at: 2018-10-25T22:15:29.093Z Reads: 89

```
well I used 2  different remotes and receivers with same result. Same remotes were used with 4.12 vescs and no probelm. It's only with the flipsky 6.6 that I saw it.
The motors at the moment are sensorless
```

---
## \#93 Posted by: Ackmaniac Posted at: 2018-10-25T22:19:07.940Z Reads: 88

```
Seems that the flipsky 6.6 hardware doesn't work that well with the VESC 6 software. Maybe someone with a original VESC 6 who uses a PPM remote and my firmware can verify that that issue doesn't exist.
```

---
## \#94 Posted by: rey8801 Posted at: 2018-10-25T22:22:37.444Z Reads: 90

```
yes others suggested to try the original firmware since they do not have that issue. Although I would like to keep having the possibility to swap modes and modify throttle curves. So far it's fine while riding it.
```

---
## \#95 Posted by: Ackmaniac Posted at: 2018-10-25T22:26:40.288Z Reads: 90

```
Maybe you can give the original firmware a try to see if that fixes the issue. Then i can try to find the root cause in the differences of the software which only belongs to the different hardware.
So if you have the time that would be great. I don't have any vesc 6 or clone myself.
```

---
## \#96 Posted by: rey8801 Posted at: 2018-10-25T22:35:19.215Z Reads: 94

```
Ok I will try. No problem.
Here the video you asked. Be prepared something new. Now the salve motor (closer to the camera) was try to spin in the other direction and when it does that the master clogs and even if you accellarate does not go faster. Anyhow the old behavior is still there but as you can see didn't happen always this time. It is a bit random. More towards the end you will see it.

Data from Master, FOC sensorless. 

https://youtu.be/jnuTEz7jxSY
```

---
## \#97 Posted by: ElectricCoast Posted at: 2018-11-17T04:41:03.742Z Reads: 78

```
Hey guys did you ever fix the problem @rey8801?  I have soft brakes on my 2 separate flipsky 6.6's.
```

---
## \#98 Posted by: rey8801 Posted at: 2018-11-17T06:59:28.829Z Reads: 76

```
Hi! Yes both me and @Winflysolved it by increasing the setting. So basicaly I had motor max 50, moto min - 50 and Batt max 25 and min - 6. I went to - 60 motor max and - 11 battery min. I guess some components is different on these vesc thst make them to handle regenerative braking differently. You can go evenper, as long you check your telentry data and see thst you are not sending back too much current.
```

---
## \#99 Posted by: tsmash Posted at: 2019-02-16T23:39:40.371Z Reads: 67

```
I have similar problems to those described above my Flipsky Vesc 6.6. I have two of these that each exhibit strange behavior in FOC mode.  Here's what I've discovered.  Note these issues are only present in FOC mode.

1) If I run the motor config wizard, then the VESC performs just fine (brakes as it should, with smooth, strong braking force).  That is...until I turn the vesc off and back on again.
2) If I turn the vesc off and then back on, the behavior gets weird.  I have one Flipsky 6.6 vesc that continues to run at a lower speed when the brakes are applied (i.e., it won't stop), and second Flipsky 6.6 that slowly comes to a stop with virtually no braking force at all.
3)  If I then re-run the motor wizard, then both vesc's run just as they should again...until I reboot the vesc.

This seems to be a bug in the FLIPSKY hardware.  There's no reason why re-booting the vesc should change the configuration or behavior.

UPDATE:  One of my esc's is defective, and FLIPSKY customer service was super responsive and immediately shipped me a new one.  With my other (good) esc: after reading @rey8801's comments, I was able to get the braking force at the level I want (even after the re-boot).  I had to crank my settings WAY up though (motor max current brake = -100, batt max current brake = -30, which seems kind of insane for a 6355 190kv motor).  The behavior is still different after the re-boot (not sure why that is), however with these settings my FLIPSKY 6.6 is braking just fine (after reboot), and performing quite well.
```

---
## \#100 Posted by: rey8801 Posted at: 2019-02-16T23:41:38.333Z Reads: 65

```
I had point 2 as well but only with no load. Once I ride them no problem whatsoever.
```

---
## \#101 Posted by: tsmash Posted at: 2019-02-16T23:43:48.344Z Reads: 62

```
So...you got the bakes to be strong again just by cranking up the setting?  Did you notice a difference in behavior before and after you reboot?
```

---
## \#102 Posted by: rey8801 Posted at: 2019-02-16T23:46:09.023Z Reads: 62

```
after rebooting no changes. I was using Ackmaniac firmware though. Concerning the brakes I had to increase them and then they were ok. Still not really strong brakes compare for instance to Focbox unity that with lower value I get really good braking force.
```

---
## \#103 Posted by: tsmash Posted at: 2019-02-16T23:47:38.360Z Reads: 60

```
So Ackmaniac works with the 6.6?  Didn't realize it could be used!  Are you using the Watt control mode?  

Thanks!
```

---
## \#104 Posted by: rey8801 Posted at: 2019-02-16T23:48:43.226Z Reads: 61

```
yes it does and yes watt control mode.
```

---
## \#105 Posted by: tsmash Posted at: 2019-02-16T23:49:55.091Z Reads: 60

```
Dope!  Will give it a try.
```

---
## \#106 Posted by: Eboosted Posted at: 2019-03-03T05:05:38.696Z Reads: 56

```
I didn't read the whole thread but on foc you need to increase battery min a lot more as the algorithm to calculate actual braking current is different than in BLDC, if you have used - 6A in the past you need you use - 9A on each vesc , try that for a 12s3p battery, it won't hurt the battery at all, all my batteries are still working after many years
```

---
