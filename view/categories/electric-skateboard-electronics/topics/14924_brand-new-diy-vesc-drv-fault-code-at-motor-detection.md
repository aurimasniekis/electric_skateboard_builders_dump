# Brand new Diy Vesc Drv fault code at motor detection

### Replies: 34 Views: 2882

## \#1 Posted by: Shogu12 Posted at: 2016-12-19T13:25:38.557Z Reads: 222

```
I just got 2 Vesc's from DIY and one setup pefectly fine but the other started flashing its red light after Foc motor detection  and would not spin up at all. It gave me the drv8302 fault code. I removed the heat shrink and noticed 2 bridged solder points on the drv could this be the issue? <img src="/uploads/db1493/original/3X/0/7/077024a644c27a9762956ec18984c58e214980bf.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/b/3/b3cf24f903929a62660206ddb1c2ad9eeeaeabf1.jpg" width="375" height="500">
```

---
## \#2 Posted by: coma0815 Posted at: 2016-12-19T13:36:14.731Z Reads: 204

```
My Vesc does also have these two bridges. It took me some research before powering it up the first time :grin: 
These two times two pins connected is not a problem. You can see the Pin Configuration here http://www.ti.com/lit/ds/symlink/drv8302.pdf on page 3.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2016-12-19T13:37:31.416Z Reads: 202

```
These bridge are totally normal.... maybe post some screen shoot of the bldc tool and more info about your supply.
```

---
## \#4 Posted by: Shogu12 Posted at: 2016-12-19T13:39:28.264Z Reads: 203

```
Well Im trying to figure out whatswrong with it I got it in the mail today and set it up like my other one but I never let the motor spin and is giving me a fault code. Diyelectricskateboards says they wont replace any vesc they sell on their site.... I inquired about an rma we shall see what happens.
```

---
## \#5 Posted by: Shogu12 Posted at: 2016-12-19T13:46:30.805Z Reads: 202

```
This is the non funtional vesc
<img src="/uploads/db1493/original/3X/e/7/e739e703858cecc0f6500da3d0b59e148922d903.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/b/a/ba92a7d18ebaf8eb57b08024865f7bec17bac606.jpg" width="374" height="500">
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-12-19T13:47:03.139Z Reads: 183

```
A lot can go wrong with a VESC, first if you don't properly isolate the motor lead prior to testing, and they touch once the power on, then you have a instant broken vesc. Also, if you run your motor without a proper motor detection, again it might broke your vesc. If you switch from foc to bldc in a improper way....
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2016-12-19T13:48:25.521Z Reads: 187

```
sorry...

thought the cutoff start was at 26... until I zoom in...
```

---
## \#8 Posted by: Shogu12 Posted at: 2016-12-19T13:51:27.916Z Reads: 188

```
This Vesv came out of the box and i ran the detection  just like on my 1st. With the same motor and heat shrunk leads.<img src="/uploads/db1493/original/3X/d/2/d260b2b34f9f62d67c76a54cca19b338fb395603.jpg" width="374" height="500"> this is the working one that was setup the same way. 
Is there a cheap fix ?since I doubt I will be getting  a refund...
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2016-12-19T13:52:58.827Z Reads: 181

```
This really look like a burn DRV... sorry for your lost 

If you have a air flow station and feel comfortable with soldering you can change the drv chip.
```

---
## \#10 Posted by: Shogu12 Posted at: 2016-12-19T13:58:15.864Z Reads: 180

```
I work for the Airforce and we have them at work but I dont know how I feel about  doing that though 😂 I'll see what Diy says if they refuse an rma I might have on of our avionics guys take a look at it.
```

---
## \#11 Posted by: Mark Posted at: 2016-12-19T14:15:32.190Z Reads: 175

```
Did you hook it up to a 12v power supply when you powered it for the first time?
```

---
## \#12 Posted by: Shogu12 Posted at: 2016-12-19T14:26:29.879Z Reads: 172

```
Yeah I used my bench powersupply.
```

---
## \#13 Posted by: rpn314 Posted at: 2016-12-19T18:53:15.990Z Reads: 160

```
Where are you located? One of us with a hot air station is probably nearby as well. If you're Utah I'd be happy to take a look at it for you.
```

---
## \#14 Posted by: sl33py Posted at: 2016-12-19T19:05:21.870Z Reads: 159

```
[quote="rpn314, post:13, topic:14924, full:true"]
Where are you located? One of us with a hot air station is probably nearby as well. If you're Utah I'd be happy to take a look at it for you.
[/quote]


@shogu12 - same here if you are in the Seattle area i could take a look.
```

---
## \#15 Posted by: Shogu12 Posted at: 2016-12-19T21:28:35.238Z Reads: 151

```
@rpn314 @sl33py Really nice gestures  but I'm stationed in Korea.
```

---
## \#16 Posted by: Eboosted Posted at: 2016-12-20T06:07:59.865Z Reads: 144

```
I got 4 VESCs from DIY, I'm starting to get really nervous before even connecting them,  here are some recommendations I gather from other posts:

1. Connect them first with power supply instead of directly to the battery at 12V

2. Run motor detection first

3. Do not try to connect it FOC at least for now, but if you go ahead, reboot VESC after writting settings and read again to confirm correct settings have been written correctly

Anything else we should all be aware of?
```

---
## \#17 Posted by: Shogu12 Posted at: 2016-12-20T07:14:27.259Z Reads: 140

```
So I bought 2 one is working great and the other wouldn't detect the same motor to start with. I went through  paypal buyer protection and they said if no tampering was done they would issue  a refund. I had to make it clear  that the removed heatshrink  cant count as tampering.
```

---
## \#18 Posted by: Shogu12 Posted at: 2016-12-22T22:52:48.604Z Reads: 137

```
I recently  purchased a 3rd vesc from diy so I can ride my dual setup while the broken one is being sent back. I've read up on it and decided to upgrade all my vesc's with a bigger c18 capacitor. And will be doing so for all Vesc's  for my fellow airmen here in Korea. Apparently it solves issues so now I'll receive vesc>test on bench power supply>run motor detection > upgrade c18. Incase its bad when I get it and will have to be returned.
```

---
## \#19 Posted by: Shogu12 Posted at: 2016-12-24T04:48:49.404Z Reads: 131

```
So my 2nd Vesc just died( I assume) while riding. I heard some crackling from inside my cover I'll update once I'm home.
```

---
## \#20 Posted by: Eboosted Posted at: 2016-12-24T05:51:52.951Z Reads: 129

```
Damn! so both VESC are bad nnow?

Did you ever find what happened with the first one?
```

---
## \#21 Posted by: Shogu12 Posted at: 2016-12-24T06:07:05.381Z Reads: 124

```
I just hooked it up and it has drv8302 fault. Been riding it for a week with no issues. Since this one worked there's no chance of replacing  it so I'm  gonna order some drv's and reflow soldering  station. The problem is I'm  gearing up to build 80 close to identical boards and if these  vesc's keep breaking I cant do that since I'll  have people 500$ out and no way to guarantee  a working product.
```

---
## \#22 Posted by: Shogu12 Posted at: 2016-12-24T06:08:03.840Z Reads: 121

```
The first one was basically  DOA and I sent it back to DIY. My 3rd will arrive in a week or so.
```

---
## \#23 Posted by: Shogu12 Posted at: 2017-01-04T08:13:24.824Z Reads: 114

```
Update: Today I was refunded for the broken Vesc from diy.
```

---
## \#24 Posted by: Martinsp Posted at: 2017-01-04T17:45:03.221Z Reads: 112

```
Hey guys,

Is there anyone who can help me? I got the same DRV8302 fault on my maytech VESC but at first it went away and was spinning the motor again until i tried to change direction (bench test only not on skateboard) and now after i tried to reupload 2.18 FW it does not spin the motor anymore at all. The chip has no obvious damege to it :/ do you think that changing the DRV will solve it? BTW i built one VESC and it s running awesome for a couple of months (5 maybe) and for the last few weeks in FOC too with sensorless, I used the same configuration on the bought maytech one and it immediately gave me the drv error. Can you help me please? :( 

thanks in advance :)
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2017-01-04T18:03:45.976Z Reads: 108

```
The issue on this tread where concerning a vesc from diy (or @torqueboards witch is a other vendor) ... I suggest to maybe start your onw tread and post some picture of your serup and screenshoot of your parameter in the bldc tools. It should be easier to help you, and less confusion for new people. 😉

As for your question, yes changing the drv will probably solve your problem, but I can't garanty you for how long, since It hard to see if they are using low grade parts... 🤔unlike the one you build.
```

---
## \#26 Posted by: Martinsp Posted at: 2017-01-04T18:09:20.309Z Reads: 111

```
Thank you, I registered just a moment ago and have not really figured out how to create a new thread :D Thank you anyway :) I am not going to replace it right now how ever because i messaged them what has happened to me, it should be covered by their one year warranty but then again... it is china :D 

as far as the components go, I checked that and all of the ones that have writing on them seem to be the ones i used and the ones in the Benjamins VESC BOM so i hope the passive components are not junk.   

BTW do you think that a broken piece of the inductor coil core (the grey thing that holds the copper) could be the problem for some reason?
```

---
## \#27 Posted by: SORRENTINO Posted at: 2017-01-04T18:11:47.949Z Reads: 105

```
Some one need to design an ESC without a drv!!
```

---
## \#28 Posted by: Shogu12 Posted at: 2017-01-08T03:18:32.992Z Reads: 99

```
Today my drv's and cap's arrived I'll update once the soldering station and tools get here.
```

---
## \#29 Posted by: Shogu12 Posted at: 2017-01-12T09:24:48.947Z Reads: 88

```
Happy to announce  that I replaced the drv on one of my vescs and it works again. Also I added a 2nd cap at c18 on all 3 of my Vesc's, it seems c26 was meant to be there but wasnt delivered that way. Kinda proud it worked to be honest. <img src="/uploads/db1493/original/3X/4/8/488e7c6578615a122e621a496dd8ef42e4b18999.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/9/b/9bad905d773017a4ecc4a48fd152d99ec2e6c8c5.jpg" width="374" height="500"><img src="/uploads/db1493/original/3X/7/7/771f8205d7ddbb217a2090e840e7ce3337f90054.jpg" width="375" height="500">
```

---
## \#30 Posted by: Pedrodemio Posted at: 2017-01-12T11:27:47.945Z Reads: 80

```
I have one coming, this thread got me worried
```

---
## \#31 Posted by: Shogu12 Posted at: 2017-01-12T11:47:47.780Z Reads: 78

```
My new 2 work fine. I upgraded them to ride foc.
```

---
## \#32 Posted by: Pedrodemio Posted at: 2017-01-12T12:08:29.176Z Reads: 78

```
Nice, I tried FOC a long time ago on the first firmware, when the new one arrive I will test again on the one I already have
```

---
## \#33 Posted by: Shogu12 Posted at: 2017-01-12T12:10:48.953Z Reads: 77

```
Check if they have the two caps at c26 and c18 if not dont do it.
```

---
## \#34 Posted by: Maxid Posted at: 2017-01-12T13:24:48.736Z Reads: 71

```
Looks to me that you did not add a second capacitor to c18 but rather you added c26. It also looks like you bridged them together - not sure what that will do to the VESC.

C26 was added in the BOM for v4.12
http://www.electric-skateboard.builders/t/vesc-capicators-problem/10949/18?u=maxid
```

---
