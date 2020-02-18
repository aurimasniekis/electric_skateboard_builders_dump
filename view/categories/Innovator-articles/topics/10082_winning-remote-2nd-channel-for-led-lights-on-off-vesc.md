# Winning Remote 2nd Channel for LED Lights ON/OFF VESC

### Replies: 40 Views: 4670

## \#1 Posted by: Carvin_Ginger Posted at: 2016-09-24T14:53:11.672Z Reads: 542

```
Has anyone figured this out yet?

I have seen some posts where people want to do this.  It would be really cool if someone could give me some hints on getting this going :).
```

---
## \#2 Posted by: Pantologist Posted at: 2016-09-24T15:01:50.847Z Reads: 539

```
All you need is this. It just acts like a switch to complete the circuit you want to activate.

To turn the vesc on and off, you would to connect this to your BMS switch or anti spark switch power button. 

http://www.hobbyking.com/mobile/viewproduct.asp?idproduct=46040
```

---
## \#3 Posted by: Carvin_Ginger Posted at: 2016-09-24T15:03:46.759Z Reads: 526

```
That's great! Thanks @Pantologist
```

---
## \#4 Posted by: Blacksheep Posted at: 2016-09-24T22:12:06.693Z Reads: 494

```
@Pantologist have you done it ?
```

---
## \#5 Posted by: Pantologist Posted at: 2016-09-24T22:14:12.059Z Reads: 473

```
Nope. I sold my Winning Remote.

I believe some one used one. Not sure who. Someone else recommended it.
```

---
## \#6 Posted by: Blacksheep Posted at: 2016-09-24T22:16:02.711Z Reads: 468

```
I ordered one but still haven't plugged it
```

---
## \#7 Posted by: Pantologist Posted at: 2016-09-24T22:19:28.169Z Reads: 456

```
You need help setting it up?

Here's a decent video. Not sure which channel it is on the Winning. I never used mine.

https://youtu.be/R8WXRVb6Y7g
```

---
## \#8 Posted by: Carvin_Ginger Posted at: 2016-09-26T13:41:24.744Z Reads: 438

```
I want to set mine up with color changing LED (not strobe mode) and headlight.  Figured I would need 12 V battery supply separate and use that controller switch to complete the circuit from my winning remote.

Any suggestions on batteries, led's and headlights?  I did go thru the thread on this topic, but specifically I am trying to find how to rather than what products.

Does anyone power their lights from their main batteries?  Does it drain them pretty bad?  I have 8S 5000 mah currently.
```

---
## \#9 Posted by: Kasper Posted at: 2016-10-30T14:27:31.310Z Reads: 382

```
Hello everyone,

I've ordered a Turnigy on/off switch to control my headlight and taillight, and installed it into the second channel from my Winning reciever. I have a Winning remote and an Enertion Dual Raptor. Unfortunately the switch does not seem to work or the remote does not work. I assume that the switch is working so is it possible that the second channel is disabled somehow?
```

---
## \#10 Posted by: Baz_L Posted at: 2016-12-06T14:26:42.847Z Reads: 352

```
Bump! Anyone have any luck? Thinking of taking the plunge.
```

---
## \#11 Posted by: mccloed Posted at: 2016-12-06T17:17:42.221Z Reads: 332

```
Which Turnigy on/off switch did you get? Depending on the model you may have to hit the switch on the remote twice to turn on and twice to turn off.
```

---
## \#12 Posted by: psychotiller Posted at: 2016-12-06T18:20:05.504Z Reads: 326

```
Would this work with our new lights?
```

---
## \#13 Posted by: mccloed Posted at: 2016-12-06T18:58:52.562Z Reads: 312

```
Yup! :+1::punch::beers:
```

---
## \#14 Posted by: Kasper Posted at: 2016-12-06T19:41:45.525Z Reads: 316

```
Hi, thanks for the reply. In the meanwhile I found another way of installing the lights. I used the power from the vescs and installed a manual switch next to the power-switch from the board. Works great now, don'r even need a extra battery anymore for the lights.
```

---
## \#15 Posted by: Carvin_Ginger Posted at: 2017-02-01T02:08:15.181Z Reads: 317

```
Got it to work!

Turnigy Multistar Twin Output SBEC
https://hobbyking.com/en_us/turnigy-multistar-twin-output-5-10-amp-6-50v-sbec-for-lipoly.html

Turning Receivers Controlled Switch
https://hobbyking.com/en_us/turnigy-receiver-controlled-switch-1.html

Winning Remote (many stores)

VESC (Ollin Board Company ***only the best***)

8S Setup

https://youtu.be/kPWfGUbYBh8
```

---
## \#16 Posted by: Carvin_Ginger Posted at: 2017-02-01T02:10:45.057Z Reads: 306

```
If you post a wiring diagram I can help.  It also maybe that you need to remove one of the caps on the Turnigy Reciever Controlled Switch. It has two small black caps and one is removed.

Send me a pic or something.
```

---
## \#17 Posted by: ACIN Posted at: 2017-02-01T02:43:24.733Z Reads: 302

```
Man I have been looking for something like this for ages!
If you could do just a mini guide with the wiring, which lights you used etc. on how you got this to work I (and probably many others) would be very thankful!

So this works as long as you have a remote with an additional switch function and a matching receiver?
Also, do you have any idea how I can make the red taillights I'm looking to install flash brighter when I'm breaking like a bike/car?
```

---
## \#18 Posted by: Carvin_Ginger Posted at: 2017-02-01T04:12:30.855Z Reads: 300

```
I haven't worked on the brake lights, not really interested.

The on/off switch is pretty straight forward.  Just plug the channel into the remote receiver and break the positive wire to the thing you want to power.  It took a little messing Around with the caps on the switch, but trial and error worked.

The twin output is needed to convert the 42v of the batteries to 5v and 12v.  Those LEDs are using 5V, I'll be using the 12V on front and rear lights.

I'll post a wiring diagram. But honestly, just this one YouTube video did the trick.

https://m.youtube.com/watch?v=qGZakWwZUYQ
```

---
## \#19 Posted by: a-3zo Posted at: 2017-03-14T19:33:49.710Z Reads: 278

```
Hi.
I have got the same remot trying to switch my lights with the 2nd channel switch. But it doesnt work. Have tried the turnigy r/c switch, the efla600 and many others. No function. Does anybody have an wiring diagram or a guide how to connect the whole circuit?
The 2nd channel functionality was the main reason for buying that remote... you are my last hope...

PS: sorry for my bad english... im from Germany.
```

---
## \#20 Posted by: a-3zo Posted at: 2017-03-17T07:40:08.302Z Reads: 263

```
Hi. Just tried the wiring like in the video (s)...
Still doesnt work :frowning:
Somebody help, please.
```

---
## \#21 Posted by: ralphy Posted at: 2017-03-28T21:30:06.770Z Reads: 236

```
COOL Im going to do that!
```

---
## \#22 Posted by: stchase24 Posted at: 2017-08-26T21:53:39.009Z Reads: 199

```
Did you ever get it to work? My channel 2 switch on the winning remote doesn't seem to work for the lights I bought. 

My other remote does work with the lights though.
```

---
## \#23 Posted by: Ishayc Posted at: 2017-08-26T22:13:00.694Z Reads: 192

```
I have tried 2 winning remote controls and the 2nd channel didn't work. On a different remote control it worked perfectly.
```

---
## \#24 Posted by: stchase24 Posted at: 2017-08-26T22:44:09.299Z Reads: 192

```
Same here. Must be a faulty remote. I was able to sort of get it to work by holding down the pair button and flipping the channel switch up and down 4 or 5 times. It resets when you power off the board though.

What remote are you using now?
```

---
## \#25 Posted by: Carvin_Ginger Posted at: 2017-08-26T23:33:13.153Z Reads: 186

```
Hey guys!  I am super late updating this.  On the receiver that connects to the lights there are 2 removable tabs.  You have to remove one to get it to work.  There should be a small image included with the packaging.

Post a pic of the receiver connected to the lights.

Also, bear in mind there are voltage requirements and the receiver has to be grounded.

Post a pic so I can see.  These are very specific.
```

---
## \#26 Posted by: Ishayc Posted at: 2017-08-27T06:40:04.193Z Reads: 174

```
I'm using this one -
https://m.aliexpress.com/s/item/32607181070.html?trace=storeDetail2msiteDetail
```

---
## \#27 Posted by: Ishayc Posted at: 2017-08-27T06:41:13.012Z Reads: 171

```
Tried removing the tabs in any possible combination, it just refused to work with the winning remote.
```

---
## \#28 Posted by: Carvin_Ginger Posted at: 2017-08-27T12:50:22.447Z Reads: 167

```
The real issue is the wiring. Post a wiring diagram (hand sketch) of what you did.
```

---
## \#29 Posted by: stchase24 Posted at: 2017-08-28T00:13:55.182Z Reads: 166

```
I bought these lights: http://www.ebay.com/itm/YY-MADMAX-LOSI-5IVE-T-5T-FRONT-AND-REAR-LIGHT-SET-ALUMINUM-RED-BRIGHT-WHITE/362076200674?_trkparms=aid%3D222007%26algo%3DSIM.MBE%26ao%3D1%26asc%3D41376%26meid%3D9d12bf15ec544035af9ac4f473ebaad6%26pid%3D100011%26rk%3D2%26rkt%3D12%26sd%3D382126887167&_trksid=p2047675.c100011.m1850

They literally plug right into the winning receiver or any other receiver's channel 2 or 3 port. I just can't seem to get the channel 2 switch to work on the winning remote. It works fine with my other receiver though. I'm using the same receiver that @Ishayc is using in his link above.
```

---
## \#30 Posted by: Carvin_Ginger Posted at: 2017-08-28T00:55:59.292Z Reads: 163

```
You need this:

https://hobbyking.com/en_us/turnigy-receiver-controlled-switch-1.html

As I mentioned above.  I guess this week I will make a VERY detailed walk through.
```

---
## \#31 Posted by: Ishayc Posted at: 2017-08-28T06:10:09.363Z Reads: 156

```
The wiring should be fine since it's running and working with a different remote control.
I'm guessing it's an issue with the 2nd channel on the winning remote.
```

---
## \#32 Posted by: Hummie Posted at: 2017-08-28T06:42:51.700Z Reads: 156

```
how hard and how dangerous would it be to have a switch to turn the board on or off from remote?
```

---
## \#33 Posted by: Carvin_Ginger Posted at: 2017-08-28T13:45:18.032Z Reads: 151

```
1.  You need power going to the receiver for it to work.  If you are using the remote to turn it on that means that the VESC is on already.

2.  The switch is rated at 10A/30V.  Your board should be a lot higher than that.

3.  You don't want to use this two power it on/off.  It will burn out fairly quickly an become dangerous.
```

---
## \#34 Posted by: hornet90 Posted at: 2017-09-24T07:26:38.848Z Reads: 136

```
If you have a bms with on off switch like bestech it should work to turn on and off board
```

---
## \#35 Posted by: Grolletje Posted at: 2018-03-11T18:07:41.895Z Reads: 106

```
I know this thread is dead, but I have trouble doing this too.

While diagosing the problem I found out the the switch on my remote replied really weird in ppm frequencies. I tried this by plugging the VESC into channel 2, then used the BLDC tool to check the freqency. the frequency difffers from 18 ms to 68 ms while using the switch, but often it stays at like 42 ms. It seems that there is no real high or low. 

the frequency is very high too, the remote in channel 1 uses from 1 to 2 ms
```

---
## \#36 Posted by: bevilacqua Posted at: 2018-03-11T22:11:55.568Z Reads: 103

```
I managed to make it work on a rc car type reciever-switch [amazon]. But i had to flick the button on and off about 5 times to tur them on, and 3 times to turn them off. 

I generally wouldn’t recommend this remote because of signal rellyability issues, far mor important that being able to turn on and off the lights.
```

---
## \#37 Posted by: GhettoFab.rictation Posted at: 2018-03-12T10:20:43.135Z Reads: 96

```
Doesn't sound appealing
```

---
## \#38 Posted by: Hatman30 Posted at: 2018-07-25T20:44:22.335Z Reads: 66

```
I found with the nano X remote there was a four second pause. Also the negative and outside connection need to be swapped and the bottom two pins on the RC switch bridged to make it work .
```

---
## \#39 Posted by: Panda_eskate_fpv Posted at: 2018-10-16T01:58:43.370Z Reads: 47

```
Can you please post pics on what needs to be done I have a nano x remote and want to use channel 2 to turn my lights on
```

---
## \#40 Posted by: Hardy312 Posted at: 2018-11-09T02:59:48.659Z Reads: 42

```
I had the same problem,  but I figured it out for the turnigy controal switch working with the nano x and the torque boards v2 remote..  on the turnigy servo cable that is brown red and yellow before you connect it into channel 2 of the nano reciever you must cut the yellow and red , strip the wire and reverse them and solder..  

The turnight has a 30v max and has to have a common negative with lights and reciever. Because of the 30v max I have the controal switch breaking the 29.6v ballance lead off of my 10s lipo setup that than supply's power to a dc dc converter tieing into my lights.. hopefully that's helpful
```

---
