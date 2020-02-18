# FOCBOX DRV8302 Error

### Replies: 43 Views: 2243

## \#1 Posted by: ggalisky Posted at: 2018-04-24T00:14:55.840Z Reads: 212

```
Hello all,

I just had one of my motors stop spinning out of the blue and I found out that one of my FOCBOX's running BLDC just got the DRV8302 error out of nowhere. The other motor running the same settings is running fine. I have already contacted enertion support, but I wanted to see if the community had a faster solution. Attached is a photo of my error.
![16 PM|504x500](upload://iCk0ql5gNhH8XKv6YMRJK9ylq5x.png)
```

---
## \#2 Posted by: Ishayc Posted at: 2018-04-24T05:42:04.601Z Reads: 184

```
Where are you located? There are a few people here that can replace the DRV.

Check your motor phase wires and look for a short, that might cause the DRV to blow.
```

---
## \#3 Posted by: ThermalM16 Posted at: 2018-04-24T07:06:49.088Z Reads: 180

```
You can try reflashing the FW on it with either BLDC Tool or the newer VESC Tool. If that doesn't work, you'll likely need repairs. Depending on where you're located there are different options available for repair. If you're in the US, I'm the closest, but there are plenty of alternatives if you're in a different area.
```

---
## \#4 Posted by: moadymoad Posted at: 2018-04-24T09:10:42.758Z Reads: 174

```
Does reflashing ever work? My Tb vesc has drv but I can’t see any damage at all on the chip
```

---
## \#5 Posted by: CarlCollins Posted at: 2018-04-24T10:53:47.267Z Reads: 167

```
@ggalisky
Already answered you on the support ticket 
I think your FOCBOX is fried due to incorrect values.

_**1: Batt Max for 10s system will be maximum 30A and yours is 50A which is high for the 10s system.**_
_**2: ERPM value is also high, recommended value is 60000 and your is 100000 which is high**_
_**3: Input voltage recommended for FOCBOX is 50.4 maximum, your is 57 which is high.**_

Please provide the demanded images on the Support ticket
```

---
## \#6 Posted by: Acidfie Posted at: 2018-04-24T11:03:42.376Z Reads: 162

```
[quote="CarlCollins, post:5, topic:53288"]
3: Input voltage recommended for FOCBOX is 50.4 maximum, your is 57 which is high.
[/quote]

please elaborate what problem this setting can cause and why
```

---
## \#7 Posted by: CarlCollins Posted at: 2018-04-24T11:08:27.357Z Reads: 161

```
As per my knowledge and tech team, FOCBOX can handle maximum 60A continuous 
But due to difference in motor amps and battery amps, it has to be adjusted accordingly
for the 10s and 12s system, our tech team advised that voltage higher than 50.4 will make the system to produce extra heat. (if values are not adjusted accordingly)
50.4 is the recommended value by our tech team.

That's what I understand!
This guide is provided to set up your FOCBOX by our tech team
https://enertionboards.zendesk.com/hc/en-us/articles/115002858294-How-do-I-configure-my-Focbox-
```

---
## \#8 Posted by: Acidfie Posted at: 2018-04-24T11:36:20.572Z Reads: 156

```
AFAIK this can cause brake failures when motors are inducing higher voltage than 50.4V which can happen when rolling downhill.

i don't really know if i should trust your techteam right now.
```

---
## \#9 Posted by: CarlCollins Posted at: 2018-04-24T11:37:50.755Z Reads: 153

```
@Acidfie

If you know about **Bara Jabali** then I think you might trust our tech team 
As he is the head of tech team.
```

---
## \#10 Posted by: Acidfie Posted at: 2018-04-24T11:40:30.231Z Reads: 148

```
@barajabali could you please elaborate to me why the setting needs to be set at 50.4V? How do you prevent overvolting when going downhill?
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2018-04-24T12:43:08.201Z Reads: 143

```
[quote="CarlCollins, post:5, topic:53288"]
3: Input voltage recommended for FOCBOX is 50.4 maximum, your is 57 which is high.
[/quote]

@CarlCollins Max Input voltage **parameter** should stay at 57V or else your going to get a few none wanted error. The default parameter from Enertion is 57
```

---
## \#12 Posted by: CarlCollins Posted at: 2018-04-24T13:00:41.475Z Reads: 140

```
@JohnnyMeduse

I've advised as per the guide provided by Bara
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2018-04-24T13:02:15.677Z Reads: 138

```
His guide, provide the **physical maximum Voltage** that is warranty for working ... **not the parameter**
```

---
## \#14 Posted by: L3chef Posted at: 2018-04-24T13:03:07.184Z Reads: 135

```
Hmmmmm. Default has always been 57v. 
Could you pleasr double check this @CarlCollins
```

---
## \#15 Posted by: CarlCollins Posted at: 2018-04-24T13:03:33.802Z Reads: 132

```
Will confirm again with Bara
```

---
## \#16 Posted by: barajabali Posted at: 2018-04-24T13:32:07.327Z Reads: 133

```
What do you need me to confirm? @JohnnyMeduse is correct. 57v, or else your voltage spikes could cause errors and cutoffs

The 50.4v is for the physical battery voltage. That’s the voltage of a fully charged 12s battery.
```

---
## \#17 Posted by: CarlCollins Posted at: 2018-04-24T13:42:54.751Z Reads: 129

```
@barajabali
The Voltage, you've confirmed it already. thank you
```

---
## \#18 Posted by: SeanHacker Posted at: 2018-04-24T13:50:54.516Z Reads: 128

```
@CarlCollins You should really consider letting the guys that KNOW what they are talking about deal with these issues. Your posts are getting ridiculous and I can see why some are reluctant to trust your team. 

_**"If you know about Bara Jabali then I think you might trust our tech team**_
_**As he is the head of tech team"**_

This ^^^ is about the only thing I can trust from your posts so far.
```

---
## \#19 Posted by: CarlCollins Posted at: 2018-04-24T13:54:36.688Z Reads: 126

```
@SeanHacker

Thank you so much for your feedback which wasn't required actually :slight_smile:
```

---
## \#20 Posted by: SeanHacker Posted at: 2018-04-24T13:55:17.594Z Reads: 124

```
You're welcome. Seems to me your feedback wasn't required either dude. ;)
```

---
## \#21 Posted by: CarlCollins Posted at: 2018-04-24T13:56:12.713Z Reads: 123

```
Replied to your comment only man ;)
```

---
## \#22 Posted by: SeanHacker Posted at: 2018-04-24T13:57:19.382Z Reads: 124

```
![double-awesome-memes-com-16229475|494x500](upload://roJpPzA4gUw8URGLDdDJNBkb3bq.png)
```

---
## \#23 Posted by: Mathias Posted at: 2018-04-24T14:14:58.270Z Reads: 120

```
50.4 V max voltage would effectively mean FOCBOX can't run 12s, which is nonsense. You can't set it so close to your battery voltage without risking frequent cutouts, which are probably most likely during braking at high speeds. I really hope that's a misunderstanding, and I hope nobody actually uses this setting!
```

---
## \#24 Posted by: ggalisky Posted at: 2018-04-24T14:37:03.121Z Reads: 122

```
@CarlCollins 
https://enertionboards.zendesk.com/hc/en-us/articles/115000605073-Erpm-limits-on-the-Focbox-

Doesn't this show that the ERPM limit is 100,000. So if 60,000 is less than 100,000, shouldn't I be fine?

http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/

On this page isn't the focbox rated for 60A?

and since my system is 10s isnt it not possible for my pack to produce more than 42v? Wouldnt that keep me under the 50.4v limit?

If anyone else can help me understand why my FOCBOX is fried let me know. 

Also, if I wanted to have a go at replacing the DRV8302 chip myself if enertion doesn't cover this under warranty, which it looks like they may not, what tools do I need for SMD? Solder paste, heat gun, soldering iron?
![52 PM|690x380](upload://bsYUpRiyskNBlxIRl9QecB7ShqB.png)![03 PM|690x378](upload://5tnRsjJVUKtrdYLUpLMS4YEkdlO.png)![18 PM|690x375](upload://pvFTxlAA8ImWPybEuu5kJ5uQLDH.png)![45 PM|690x377](upload://t5EkLFLoFIUJcAXaahnbaZ6igKg.png)

Thanks!
```

---
## \#25 Posted by: barajabali Posted at: 2018-04-24T15:23:11.457Z Reads: 109

```
[quote="barajabali, post:16, topic:53288, full:true"]
What do you need me to confirm? @JohnnyMeduse is correct. 57v, or else your voltage spikes could cause errors and cutoffs

The 50.4v is for the physical battery voltage. That’s the voltage of a fully charged 12s battery.
[/quote]
It is just a misunderstanding guys. @CarlCollins is just trying to do his job by trying to answer questions on the forum (which he isnt really required to do) cut him some slack.
```

---
## \#26 Posted by: Mathias Posted at: 2018-04-24T15:32:31.545Z Reads: 108

```
I think we all appreciate that he is active and communicating. I didn't mean to crap all over that. It's still important to point out that this is a setting that might be dangerous to 12s riders. 

Any safety relevant issue is worth discussing to death...
```

---
## \#27 Posted by: barajabali Posted at: 2018-04-24T15:34:11.167Z Reads: 105

```
Thats why he tagged me to confirm. Which is the right thing to do
```

---
## \#28 Posted by: Acidfie Posted at: 2018-04-24T16:25:06.785Z Reads: 105

```
@barajabali thanks for clarification of this issue.

[quote="CarlCollins, post:9, topic:53288"]
If you know about Bara Jabali then I think you might trust our tech team

As he is the head of tech team.
[/quote]

and maybe know you know why i doubt this in the first time.
```

---
## \#29 Posted by: ggalisky Posted at: 2018-04-24T20:08:20.700Z Reads: 102

```
Wait guys can we focus on the issue at hand? I know entertion support is a fun topic, but can anyone tell me if my settings exceeded the specs of the focbox? Thanks
```

---
## \#30 Posted by: SeanHacker Posted at: 2018-04-24T20:15:38.660Z Reads: 104

```
You're settings look fine. 

Tell us your setup. Is it a dual or single? Looks like you have a 10S battery? What type of motors and KV? What type of batteries are you using? Just reading around the forum it looks as though quite a few FOCBoxes are burning up right now. Maybe QC was rushed?
```

---
## \#31 Posted by: ggalisky Posted at: 2018-04-24T20:23:35.053Z Reads: 99

```
10s4p samsung 30Q, torqueboards 190kv 6355, dual
```

---
## \#32 Posted by: SeanHacker Posted at: 2018-04-24T21:17:23.599Z Reads: 93

```
I have two builds with the same exact setup. I also have another same just with Samsung 25R's. You're settings are perfectly fine and even conservative. You can actually run 40A Batt Max each and be fine. I run at 30A to be safe and for longevity. Here's my settings. Been using the same for a couple years now. 

Motor Max= 70A
Motor Min= -55A
Batt Max= 30A
Batt Min= -10A

Min ERPM= -60000.00
Max ERPM= 60000.00  <----- This is what might've killed it here

Battery cutoff start= 30.00V
Battery cutoff end= 28.00V

I got all these settings for my setup from the man himself @Ackmaniac. Been running like a dream for a while now. Tons of power, range, ect...
```

---
## \#33 Posted by: ThermalM16 Posted at: 2018-04-24T22:47:35.135Z Reads: 82

```
The DRV can be blown and have no visible damage. Reflashing can fix software issues. I haven't seen a DRV error caused by a software issue before, but it's the first step in diagnosing a problem when you don't have test equipment on hand.
```

---
## \#34 Posted by: ggalisky Posted at: 2018-04-24T23:56:55.649Z Reads: 82

```
@SeanHacker

This is from enertions website: https://enertionboards.zendesk.com/hc/en-us/articles/115000605073-Erpm-limits-on-the-Focbox-
 
  Eric Wilson
6 months ago Updated
Follow
Well there's a myth going around that it is 60K ERPM which is fine. We've tested it to 100k ERPM.

Wouldn't this mean I'm within the specs outlined by enertion? Or is it less robust than advertised? So confused.
```

---
## \#35 Posted by: ggalisky Posted at: 2018-04-24T23:59:10.132Z Reads: 78

```
![IMG_6691|500x500](upload://x5iUgG1UqO5kjqiQtxzcRfN08Tz.JPG)![IMG_6690|500x500](upload://auk3CttaQiHfQPzalZRAdq7BXZO.JPG)
```

---
## \#36 Posted by: b264 Posted at: 2018-04-25T00:06:40.174Z Reads: 76

```
Motor Min and Batt Min need to be negative, not positive.  I'm not sure how this is even working.
```

---
## \#37 Posted by: RedEagle Posted at: 2018-04-25T00:08:07.012Z Reads: 76

```
You are well within spec. But 60k is the limit the community has set. Most of us run into a plethora of issues above 60k.

Although the FOCBOX has upgraded components it is still a vesc4 at heart based upon the design of the vesc5. 

Vesc6 solves most of the limitations of the vesc4 design. Vesc4's have a mixed rate of success. 

The ones I never have seen fail are @chaka 's. 
I'm lucky to run maytechs without issues so far.
```

---
## \#38 Posted by: SeanHacker Posted at: 2018-04-25T01:10:29.355Z Reads: 76

```
You my friend caught me slipping on my "-". Edited as soon as I could. Thanks dude.
```

---
## \#39 Posted by: ggalisky Posted at: 2018-04-27T14:21:52.610Z Reads: 66

```
> Hi,
> 
> If your board works for 100 miles that means the issue is not from the factory,
> 100 miles is a lot of time for something go wrong.
> So it's not a manufacturing defect, you need to purchase the platinum warranty to get replacement or repair.
> Kind regards
> Eric Wilson
> Enertion Support
```

---
## \#40 Posted by: TehAtheist Posted at: 2018-04-27T14:27:43.064Z Reads: 66

```
I had DRV8302 issue on my VESC 4.12 recently, it appears to have been resolved by reflashing the firmware (or updating from 3.37 to 3.38). But haven't had time to test my board intensively, but really seems to be fixed now.
Obviously, I had no permanent  issues, just loss of power and an error for a second during rides.
```

---
## \#41 Posted by: ggalisky Posted at: 2018-04-27T14:46:13.495Z Reads: 65

```
I guess FOCBOXs are rated for 100 miles run within spec, how laughable. I have another focbox that has run with canbus with this one for all 100 of those miles and doesn't have any issues. I will never by an enertion product again. Time to learn SMD.
```

---
## \#42 Posted by: ggalisky Posted at: 2018-04-27T14:51:43.940Z Reads: 67

```
Does anyone know how to reflash a focbox? Where can I download the firmware?
```

---
## \#43 Posted by: RedEagle Posted at: 2018-04-27T17:47:17.156Z Reads: 62

```
https://www.electric-skateboard.builders/t/vesc-project-com-is-online-public-vesc-tool-download/32268
```

---
