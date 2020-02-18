# No lights on focbox and wont connect to laptop :(

### Replies: 96 Views: 2104

## \#1 Posted by: stormboard1 Posted at: 2018-04-11T11:17:16.429Z Reads: 188

```
so i finally got my eskate going and took it for a spin, then the board just stopped accelerating or responding to the remote. so iv it opened up now and theres no blue lights on the focbox ..the bt module is flashing..the remote reciever is flashing and connecting but the focbox has no blue lights and doesnt connect to the app on the laptop or show at all on the laptop. :frowning:
```

---
## \#2 Posted by: DeathCookies Posted at: 2018-04-11T11:19:53.910Z Reads: 186

```
Best way of getting help is providing as much Infos as you can. That also includes some Pictures of the Hardware to see if it is burned or sth. else ;)
```

---
## \#3 Posted by: stormboard1 Posted at: 2018-04-11T11:31:35.935Z Reads: 183

```
![image|375x500](upload://h3Vk346EI2snkR7tFUahjoJETvU.jpeg)![image|375x500](upload://jJPJUv93p6Zuac0c18DVdmSmmh.jpeg)![image|375x500](upload://39xPklxwdvxEwzwXX2aZd5bvKk9.jpeg)
```

---
## \#4 Posted by: TarzanHBK Posted at: 2018-04-11T11:41:40.905Z Reads: 168

```
You soldered the receiver directly to the Focbox. Cables might be shorted there and broke it.
```

---
## \#5 Posted by: stormboard1 Posted at: 2018-04-11T11:47:01.690Z Reads: 171

```
No the remote reciever came from enertion hotglued on beside the jst connectors if thats what you mean.. 

Anyway heres the internals..

![image|375x500](upload://3EGtpvFVt7kEOD7x4pr4lEl8X5u.jpeg)![image|375x500](upload://p8Ti3CeDttKHQAs3euVLCHCc5VA.jpeg)

![image|375x500](upload://qkRQ5dKn699xUcgaFi0JXOVnTQq.jpeg)
```

---
## \#6 Posted by: briman05 Posted at: 2018-04-11T11:55:01.536Z Reads: 158

```
What are those red and purple wires soldered to?
```

---
## \#7 Posted by: KTMinni Posted at: 2018-04-11T11:55:22.264Z Reads: 160

```
Check your battery voltage, and disassemble your focbox and take full pictures of it so we can see if something got fried or not.
```

---
## \#8 Posted by: stormboard1 Posted at: 2018-04-11T11:58:37.103Z Reads: 161

```
the red and blue wires are soldered to my charge port,loopkey,voltmeter etc. not to the focbox lol
```

---
## \#9 Posted by: CarlCollins Posted at: 2018-04-11T12:00:00.521Z Reads: 155

```
It would be most helpful if you share the information of your setup and what BLDC tool settings you were at.
```

---
## \#10 Posted by: CarlCollins Posted at: 2018-04-11T12:01:22.394Z Reads: 155

```
I think you've fried them or the Voltage is low for them
```

---
## \#11 Posted by: stormboard1 Posted at: 2018-04-11T12:04:41.485Z Reads: 152

```
just disassembled it and pics added..
battery voltage is 40.6 from the voltmeter
```

---
## \#12 Posted by: KTMinni Posted at: 2018-04-11T12:07:03.498Z Reads: 151

```
What's your battery setup?
```

---
## \#13 Posted by: stormboard1 Posted at: 2018-04-11T12:10:33.351Z Reads: 149

```
10s4p 30q battery, 6374 sensored motor singe drive.
i have the settings saved as i was guided throught he setup.ill find them think i was in.
fried what? how?
```

---
## \#14 Posted by: KTMinni Posted at: 2018-04-11T12:17:18.360Z Reads: 147

```
Your VESC(focbox) could have been fried from an amp spike or something of the like
```

---
## \#15 Posted by: CarlCollins Posted at: 2018-04-11T12:20:51.995Z Reads: 143

```
@stormboard1 Have you purchased the FOCBOXes from Enertion directly?
```

---
## \#16 Posted by: stormboard1 Posted at: 2018-04-11T12:28:32.688Z Reads: 143

```
yep 2 from you a few months back
```

---
## \#17 Posted by: CarlCollins Posted at: 2018-04-11T12:31:13.931Z Reads: 144

```
@stormboard1 you can contact Enertion Support for help. 
Email is support@enertionboards.com
We will provide you options if there is any hardware or software damages.
```

---
## \#18 Posted by: stormboard1 Posted at: 2018-04-11T12:34:54.060Z Reads: 143

```
what options?
```

---
## \#19 Posted by: briman05 Posted at: 2018-04-11T12:35:06.375Z Reads: 143

```
warranty on the focbox is 60 days it might be a candidate to sent to @JohnnyMeduse  for repair.
```

---
## \#20 Posted by: CarlCollins Posted at: 2018-04-11T12:37:42.486Z Reads: 145

```
Options about repair service or replacements 
Our tech team will examine the case and approve it
```

---
## \#21 Posted by: stormboard1 Posted at: 2018-04-11T12:39:00.130Z Reads: 137

```
i set the focbox up as instructed by well respected members on this forum and made sure to use safe and well within the limits of the focbox bldc not foc etc.. i double and triple checked everything and my board goes 500 yards and the focbox gives out..warranty or not thats just nuts i even push started the board and made sure it wasnt on fullcharge or going down hill..what more could i have done ..nothing looks fried ..i dont get this
```

---
## \#22 Posted by: DeathCookies Posted at: 2018-04-11T12:46:33.978Z Reads: 132

```
Maybe there was a foil over the mosfets and the heatsink?
```

---
## \#23 Posted by: stormboard1 Posted at: 2018-04-11T12:48:00.467Z Reads: 135

```
whats foil in this context?
```

---
## \#24 Posted by: TarzanHBK Posted at: 2018-04-11T12:52:25.963Z Reads: 138

```
Should not shorted this way only throttle down earlier because of bad heat dissipation.

@stormboard1 could you also provide a pic of the back of the Focbox? See if the DRV has some burnmarks.
And a pic of the heatsink with the pads to check if there is any foil left like @DeathCookies mentioned
```

---
## \#25 Posted by: briman05 Posted at: 2018-04-11T12:56:33.692Z Reads: 139

```
I have seen a focbox that has 2 joints soldered together.  I'm not saying that is what this case is but it has happened.
```

---
## \#26 Posted by: stormboard1 Posted at: 2018-04-11T13:05:24.986Z Reads: 135

```
yep no problem one second
```

---
## \#27 Posted by: stormboard1 Posted at: 2018-04-11T13:15:28.348Z Reads: 134

```
@TarzanHBK @CarlCollins 
Underside of the focbox
  
![image|375x500](upload://8QmIKlAT5TR5zRVip8OYDNJ84Rl.jpeg)![image|666x500](upload://2A2fnZzt6xp4oYyPBhl8L8PDeeZ.jpeg)![image|666x500](upload://fkbhnwlqL3Bq8fy4mqwrDNq4JYl.jpeg)
```

---
## \#28 Posted by: TarzanHBK Posted at: 2018-04-11T13:18:24.691Z Reads: 127

```
looks all good as far as i can tell from pictures.
Just start a chat with customer support at enertion.
```

---
## \#29 Posted by: CarlCollins Posted at: 2018-04-11T13:19:44.164Z Reads: 128

```
Everything looks good as pictures indicated.
I think tech team will help you with this. Please email us with all of these images and brief history about your issue.
```

---
## \#30 Posted by: stormboard1 Posted at: 2018-04-11T13:21:48.193Z Reads: 127

```
ok thanks will do it now
```

---
## \#31 Posted by: ARetardedPillow Posted at: 2018-04-11T13:23:02.114Z Reads: 129

```
I think the the sticker/padding on the case should be removed right?
```

---
## \#32 Posted by: BoostedBuilder Posted at: 2018-04-11T13:25:40.248Z Reads: 128

```
The white one? No its for heat dissipation.
```

---
## \#33 Posted by: CarlCollins Posted at: 2018-04-11T13:28:38.533Z Reads: 128

```
That's for heat dissipation, there is no issue with that
```

---
## \#34 Posted by: stormboard1 Posted at: 2018-04-11T14:20:28.387Z Reads: 117

```
sent the email just there to the email address you posted @CarlCollins  how long should this take ?
```

---
## \#35 Posted by: CarlCollins Posted at: 2018-04-11T18:29:28.349Z Reads: 114

```
You will get response within 24 hours
```

---
## \#36 Posted by: Acido Posted at: 2018-04-11T18:51:40.447Z Reads: 111

```
you checked the bms?
I fried my bms, reciever, vesc because a wrong wire connected on the bms...
```

---
## \#37 Posted by: CarlCollins Posted at: 2018-04-12T02:58:28.383Z Reads: 107

```
@stormboard1

Waiting for your response on the support ticket. 
Please check your email
```

---
## \#38 Posted by: stormboard1 Posted at: 2018-04-15T00:15:35.267Z Reads: 90

```
replied to the email and that address is correct yes
@CarlCollins
```

---
## \#39 Posted by: stormboard1 Posted at: 2018-04-19T23:46:31.399Z Reads: 86

```
okay so apparently something shorted as there is no blue light... i can see anything shorted and dont want this to happen again..also i only went like a few feet up the road i dont see what could have shorted ..if anyone has an idea what might have happened much appreciated
```

---
## \#40 Posted by: briman05 Posted at: 2018-04-20T01:26:39.452Z Reads: 82

```
What did Enertion have to say about that.
```

---
## \#41 Posted by: stormboard1 Posted at: 2018-04-20T01:48:44.750Z Reads: 83

```
"As per the tech team, your item is shorted and it's not a manufacturing defect.
So you have to buy the platinum warranty to get a replacement or repair freely (Warranty purchasable here: http://www.enertionboards.com/warranty/1yr-focbox-replacement-warranty/)
or you have the option to ship the faulty unit to our agent in US or Canada to get paid repair service 
Best,...."

i said it didnt make sense as it looked fine and how did it short..

"our tech agent said "Well if the blue led is off, something is shorting out the 5v"
So it does makes sense"
```

---
## \#42 Posted by: briman05 Posted at: 2018-04-20T02:08:38.847Z Reads: 80

```
I don’t think I have ever heard of a company with this short of a warranty period on a nice item from a manufacturer.
```

---
## \#43 Posted by: stormboard1 Posted at: 2018-04-20T02:17:45.751Z Reads: 81

```
exactly i cant get over how it went like a few feet up the road and blows..i had it set up right and cant see how it would have shorted ..seems like a cop out to me
```

---
## \#44 Posted by: psychotiller Posted at: 2018-04-20T02:22:58.020Z Reads: 79

```
I am doing a build right now for a customer using 4 brand new Focboxes and the same thing just happened to one of them. Plugged it in, connected to the bldc tool, hit read configuration and it went dead. Now, no lights, nothing. The other 3 are fine and went through detection perfectly.
```

---
## \#45 Posted by: Exiledd_Top Posted at: 2018-04-20T02:27:50.234Z Reads: 79

```
Is it the torque drive 4wd?
```

---
## \#46 Posted by: psychotiller Posted at: 2018-04-20T02:29:08.234Z Reads: 80

```
Yuuuup! Howard's probably not super stoked right now...3wheel drive is retarded.
```

---
## \#47 Posted by: Exiledd_Top Posted at: 2018-04-20T02:30:55.980Z Reads: 81

```
I got a loner focbox , u wana barrow it and use it and when the other gets fixed just give me that one ? My 4wd is out for 2-3 weeks no battery:( send it back to @barajabali amazing dude
```

---
## \#48 Posted by: psychotiller Posted at: 2018-04-20T02:31:50.889Z Reads: 82

```
I'm down!!! Do you need an enclosure for being so cool?
```

---
## \#49 Posted by: Scoo_B_SK8 Posted at: 2018-04-20T02:32:04.172Z Reads: 80

```
That is awesome what you just offered!
```

---
## \#50 Posted by: briman05 Posted at: 2018-04-20T02:32:07.519Z Reads: 80

```
I am having a feeling that these are a product of them not having them at the beginning of there cyber Monday sale. Switching factories/ staffs. I think there may be more of a quality issue out there than they know.
```

---
## \#51 Posted by: Exiledd_Top Posted at: 2018-04-20T02:34:16.632Z Reads: 81

```
 I live in LA , maybe jerry can give it to u , or u can pick it up , only issue I can see that my focbox has xt90 and 4.5 bullet connectors.
```

---
## \#52 Posted by: Exiledd_Top Posted at: 2018-04-20T02:35:00.538Z Reads: 81

```
[quote="briman05, post:50, topic:51935"]
Switching factories/ staffs
[/quote]

They never switched factories for focbox is what I was told
```

---
## \#53 Posted by: psychotiller Posted at: 2018-04-20T02:37:27.001Z Reads: 79

```
I can switch the connectors. no big deal. i just ordered a new one from LHB, but it won't ship for a little while. I can cruise out to jerry's shop tomorrow I guess. do you need anything from the Psychotiller?
```

---
## \#54 Posted by: Exiledd_Top Posted at: 2018-04-20T02:40:08.212Z Reads: 78

```
I only work part time 2 days of the week with jerry high school student. (Saturday-sunday ) I can go drop it off today to jerry so you can go stop by his place Tommorow
```

---
## \#55 Posted by: psychotiller Posted at: 2018-04-20T02:41:23.931Z Reads: 79

```
You're the man Miguel!!!
```

---
## \#56 Posted by: Exiledd_Top Posted at: 2018-04-20T02:42:23.050Z Reads: 78

```
I don't really need anything am kinda set , your enclosure for the evo 4wd is still holding up really well after it flying 5 feet into the air lol.
```

---
## \#57 Posted by: stormboard1 Posted at: 2018-04-20T02:51:07.989Z Reads: 76

```
someone was saying that the phase wires are the biggest culprits but they were fully plugged and no wear etc..
```

---
## \#58 Posted by: psychotiller Posted at: 2018-04-20T03:00:42.969Z Reads: 75

```
The phase wires here are good and were plugged in properly to the motor as well.
```

---
## \#59 Posted by: briman05 Posted at: 2018-04-20T04:09:55.178Z Reads: 74

```
I think they rushed to get orders out at a semi reasonable time not like people just now getting them and they didn’t test them first. It would be interesting to see how many people got cyber Monday focbox and how many have died. I have 2  and I’m in the process of finishing ip my first build so hopefully mine work.
```

---
## \#60 Posted by: gravitycarve Posted at: 2018-04-20T04:25:07.622Z Reads: 71

```
I had one that died. Same story with support although the fet fried?
```

---
## \#61 Posted by: CarlCollins Posted at: 2018-04-20T09:47:36.420Z Reads: 67

```
FYI: All of the items have passed QC twice so we are confident that some of the FOCBOXes died due to user errors. Also, @stormboard1 Our tech agents wants the images of your setup wires and motor wires. 
Then we will provide you a detailed explanation about the cause of issue. :slight_smile:
```

---
## \#62 Posted by: briman05 Posted at: 2018-04-20T11:50:39.304Z Reads: 64

```
@CarlCollins I am saying that maybe the QC was lacking for the Cyber Monday focboxes because so far there are 3 that have died 2 with the same issues and 2 where people who have done multiple boards so they should know what they are doing. I know that when this sale went on Enertion went into the factory and cleaned house and fired everyone. Then had a whole new staff brought in. I don’t know about you but I have mistakenly hired people who lied a little on there resume from what they could really do so possibly this is the instance here. I would think the enertion would like to keep people backing them and keep customer satisfaction high by replacing or repairing these as people are still receiving there purchases from that day. The only place I have ever seen something where people pay and then wait 6 months to get their product is on a crowdfunding site.
```

---
## \#63 Posted by: CarlCollins Posted at: 2018-04-20T11:52:46.700Z Reads: 64

```
@briman05

We understand and we are currently doing it.
If someone faces issue due to Manufacturing defects ,we will replace the item :slight_smile:

Customer's Satisfaction is the main priority
```

---
## \#64 Posted by: briman05 Posted at: 2018-04-20T11:59:35.455Z Reads: 62

```
@CarlCollins But 3 have died by 3 different people. One is @psychotiller who has done a lot more boards then the others havenso maybe there is something that is going on. If customer satisfaction is the main priority then these focboxes should be repaired for free. Because these 2 don’t sound like a DVR failure. Plus I’m pretty sure @psychotiller knows how to wire up a board and not blow a focboxes this isn’t his first time. Anything can happen and people can say it’s user error just like UPS not paying insurance money because they say the item was properly packaged I deal with it every day at my job.
```

---
## \#65 Posted by: CarlCollins Posted at: 2018-04-20T12:03:19.776Z Reads: 60

```
@briman05

Our Tech team always inspect the case thoroughly and then provide their remarks about it. 
So if they have contacted Support and their issues identified as User error then there is not doubt that our Tech team inspected it twice.

All of us are humans and doing minor mistakes is part of the human nature.
It might be from our side or from customer side
But double inspection reduces the possibility of error
```

---
## \#66 Posted by: SeanHacker Posted at: 2018-04-20T12:06:43.020Z Reads: 57

```
It's pretty cool how so many FOCBoxes passed QC twice when a ton of them still had the thermal tape plastic still on them. Great QC process guys.
```

---
## \#67 Posted by: Scoo_B_SK8 Posted at: 2018-04-20T12:16:43.566Z Reads: 61

```
[quote="briman05, post:64, topic:51935"]
@psychotiller knows how to wire up a board
[/quote]

from even reading it sounds like he already had 3 focboxs detected on a 4WD setup and on the 4th one... poof.  Can't think of a reason anyone would set one foc different from the other 3 on a 4WD (<==just noting my observation & 2cents).
```

---
## \#68 Posted by: Acidfie Posted at: 2018-04-20T12:16:58.382Z Reads: 62

```
going to hook in here;

@SeanHacker is absolutely right, no offense towards enertion but these thermal pads are really questionable.

If @stormboard1 maybe could post some pictures here from his setup (phase wires and wiring and transition of the phase wires out of the enclosure) would help a lot!
```

---
## \#69 Posted by: briman05 Posted at: 2018-04-20T12:40:45.787Z Reads: 58

```
Yes everyone is human so if everyone is human then maybe there should be a one time repair where if it blows you ask for a pictures of set up with focbox apart  plus a picture of bdlc settings to explain what is wrong to the person so they know in future builds but say we are all humans so this time its on us and repair it. Then if the person doesnt learn and blows it again its on them.  Also QC is just a visual inspection it is not a test throw those things on a pre built board with the same settings as previous tested ones and pull the trigger a few times hard and brake hard then send it out.  It may sound like alot but this way it will be tested and known to work when it left.  And I know it will take alot more time doing this but I know of one focbox that had a bridge of solder between 2 spots and it caused it to fail so how did that one get through QC twice without someone catching it?
```

---
## \#70 Posted by: CarlCollins Posted at: 2018-04-20T12:51:03.088Z Reads: 55

```
@briman05

I totally understand what you are saying and I agree with it.
That's we re-advised our QC department to perform leveled tests on the unit before shipment.
not all of the FOCBOXes has that thermal pad film left on. 
Only those which were manufactured initially by the new team.

and I think we already got his BLDC tool settings via support email or he must have been mentioned that he was using default settings.

That's why we advised that if anyone facing manufacturing defects with the items, we will replace it for you
```

---
## \#71 Posted by: briman05 Posted at: 2018-04-20T12:57:12.352Z Reads: 55

```
I still feel like there should be a one time fix to show that everyone is human.  Maybe that is something you could bring up to Jason.  I know we live in a corporate world but the corporation shouldn't come before customers.
```

---
## \#72 Posted by: CarlCollins Posted at: 2018-04-20T12:59:37.443Z Reads: 56

```
@briman05

Already advised, Logistics, production, and Jason about it :slight_smile:
```

---
## \#73 Posted by: Scoo_B_SK8 Posted at: 2018-04-20T13:31:47.763Z Reads: 56

```
businesses would go under if they tailored to that... don't get me wrong, as a consumer it sounds awesome, but there is far to much human error.  Also that is why they offer warranties.  i think the focboxs have 60days from factory if i'm not mistaken, and a Platinum you can purchase.

different example; im a paint contractor and if i came back to  all my clients who put a nail hole in a wall, i'd be a full time sucker not making a dime (i even offer 30days, but am pretty lenient on that even)

also... i keep reading stuff like this but never hear the conclusion.  (denied replacement or got replacement).
```

---
## \#74 Posted by: sk8l8r Posted at: 2018-04-20T13:50:13.972Z Reads: 58

```
I'll be honest here I'm/was about to order to order some foc's for my first VESC build I feel I'm heading into a world of pain if a builder as experienced as @psychotiller has these 'user problems' I'm totally screwed :(
```

---
## \#75 Posted by: Scoo_B_SK8 Posted at: 2018-04-20T14:02:27.228Z Reads: 62

```
there are way more working foc's than the 4 or 5 lately that have gone down
```

---
## \#76 Posted by: psychotiller Posted at: 2018-04-20T14:04:43.879Z Reads: 62

```
Yup. 3 worked. On the 4th, doing exactly the same process, I hit connect and it connected, then read configuration, Then it went dead. no poof, no smoke, nothing. So, i'm just sending it out to Johnny Meduse. He'll tell me where the fuck up was and I'll be sure to share it here.

-For the record I didn't even contact Enertion about this because I know how a standardized customer service process works. (or Doesn't)

Pay the $45 repair cost and move on.
```

---
## \#77 Posted by: briman05 Posted at: 2018-04-20T14:37:34.167Z Reads: 60

```
Well painting and electronics are 2 different things I understand where you are coming from but also that 60 day warranty is only on manufacturing defects. They could say anything can be a user defect as if they pass the 2 QC inspections they can say the user must have tried to fix the issue themselves. Yes 100% there are more working Focs than not working Focs but with the several recent ones that were all bought from the Cyber Monday sale you have to question the workmanship. I’m glad that @JohnnyMeduse is out there to fix issues that we have because he will definitely fix any issues so we don’t have to send it back to the manufacturers which normally takes a lot longer.  It would be interesting to hear everyone’s outcome of repair or replacement that is outside of a Configuration issue.
```

---
## \#78 Posted by: Scoo_B_SK8 Posted at: 2018-04-20T15:23:28.750Z Reads: 57

```
Here’s the part I’m not understanding; 
If people are just now getting cyber Monday focbox’s, how are those different from ones purchased & received within the last month.  I would think they are all coming from same factory just that cyber Monday boxes purchased have priority to get out to customers who have paid 1/2yr ago vs. those who have paid 30days ago but same focbox’s all around.

I get that you have part shortages during production but if parts are substituted than are you really getting what you paid for and therefore grounds for a return?????
```

---
## \#80 Posted by: briman05 Posted at: 2018-04-20T15:38:37.829Z Reads: 54

```
We wouldn’t be able to know that correct as that is part of the manufacturing process. Is there something to look for in the Focbox that is as consumers could look for.
```

---
## \#81 Posted by: briman05 Posted at: 2018-04-20T15:44:58.751Z Reads: 53

```
They started delivering all the ones that they had in stock when the new group of workers came in went out first and then they have been fulfilling the rest as they are done. But a lot of people had purchased multiple items such as nano-x or chargers. The nano-x with focbox went out towards end of December and January. But there was a issue with the chargers taking a long time to manufacture so people who ordered the charger and focboxes there order was held up because of the charger. And everyone’s order was held up by “money clip gate” but there are some people didn’t get the clip in there order. So the money clip was basically an excuse for the delay.
```

---
## \#83 Posted by: briman05 Posted at: 2018-04-20T15:47:02.168Z Reads: 51

```
I’m not sure if I would know what a cold joint would look like compared to a proper joint.
```

---
## \#85 Posted by: ThermalM16 Posted at: 2018-04-20T16:43:50.416Z Reads: 50

```
@stormboard1 I know this is kind of late, but sometimes the BT module can kill a VESC. I had a 4.12 that came to me for repairs, and if I recall, something on the 3.3V rail died, but the lights on the BT module still came on. I'm not sure if that's the issue or not, but it's something to look into possibly.

I'll go into a little detail about that blue light real quick. So the blue light is hooked up to the 3.3V rail. The 3.3V rail is powered by a 5V rail. This 5V rail is created/powered by the DRV. So if the DRV is dead, there is no 5V, and therefore no 3.3V. In a different case, the 3.3V rail will be dead but the DRV is okay. I think you mentioned you still had lights coming on on your BT module. So most likely, the BT module is powered by the 5V rail, which is intact, and the 3.3V rail was killed by something. That something could be any number of things, but it's almost always from a short, or something to that extent.
 
In regard to repairs, I do Enertion's FOCBOX repairs in the US. It looks like they deemed it as an issue not caused by a manufacturing defect, so it won't be covered by them, but in any case, if you're interested in getting a repair, I'll see what I can do. 

@Deckoz @briman05  You probably won't be able to spot a bad joint by looking at the PCB. All of the ones that really matter and can cause serious issues are a bit harder to inspect. The DirectFETs have a total of 9 joints under them, and the other main joints to inspect would be those on the DRV and MCU. 

Hopefully that helps explain some stuff
```

---
## \#87 Posted by: briman05 Posted at: 2018-04-20T17:03:42.606Z Reads: 49

```
[quote="ThermalM16, post:85, topic:51935"]
So most likely, the BT module is powered by the 5V rail, which is intact, and the 3.3V rail was killed by something. That something could be any number of things, but it’s almost always from a short, or something to that extent.
[/quote]

So let’s say it wasn’t the BT module that killed the Focbox and it shorted would you deem that a manufacturing problem yourself even after the tech that @stormboard1 spoke to said it was user error. What would happen then.
```

---
## \#88 Posted by: ThermalM16 Posted at: 2018-04-20T17:05:50.979Z Reads: 47

```
If the large ground pad on the bottom of the DRV isn't connected then yes, the magic smoke will escape. This is also another pad you can't visually inspect. What I meant was you'd need to inspect their individual pins under a scope to verify everything is working as it should. I remember on the very first MCU I replaced, I somehow bridged two pins and it wouldn't let me flash a new FW on it with my ST Link. After way too much time, I looked at it under my scope and sure enough there was a tiny string of solder, no thicker than a hair bridging two of the pads that was practically hidden behind the pins of the MCU. Point being is that not everyone knows what to look for, and it can be a bit involved. 

I'm not sure if replying to you is a good idea or not lol. Either you'll be like yeah thanks for the info, that was informative, I'm sure other forum members will get something from that, or you'll be like let me try to show everyone my knowledge of esk8 and all of its subjects is greater than that of anyone else on the forum
```

---
## \#90 Posted by: ThermalM16 Posted at: 2018-04-20T17:15:52.693Z Reads: 47

```
So it all depends, and my answer is that I wouldn't know without looking at it. The other techs that would have looked at it have been doing this for longer than me, so I'd be inclined to stand behind their decision. 

If the issue was caused by an issue with the FOCBOX itself then yes, it would be covered, but from their inspection, it wasn't.
```

---
## \#91 Posted by: ThermalM16 Posted at: 2018-04-20T17:22:50.111Z Reads: 47

```
Hey, I don't mean any offense, but the way you type comes off kind of condescending. Adding the ... and winky face make it seem that way. I don't have any way of telling your tone of voice over the forum, so it can make certain ways of expressing yourself via text a bit harder to interpret.

 I've seen other posts where you go at it with other people. I just don't want to get caught up in pointless arguments on here. I come here for the build porn, chill people, and more than anything else, to learn more than what I already know.
```

---
## \#94 Posted by: ThermalM16 Posted at: 2018-04-20T17:33:11.515Z Reads: 46

```
@Scoo_B_SK8 What nonsense?

@Deckoz See, I took the winky face as sarcasm. Now I know that's not what you meant. Not sure why you deleted all of your replies though

Now that this thread is horribly derailed, hopefully my previous explanation will help out with explaining some general VESC issues
```

---
## \#97 Posted by: briman05 Posted at: 2018-04-20T17:43:23.290Z Reads: 45

```
To get this back on topic. The thing I would like to know is that since I'm sure @stormboard1 shared pictures with the techs but they are not seeing it first hand and pictures can only be blown up so close but let say for the sake of reasoning if this Focbox was sent to you and you examined it under a scope and you found a solder bridge would it then be replace/fixed and then  be deemed manufacturing defect and covered under the warranty even though the initial assessment was user error and not covered.
```

---
## \#98 Posted by: briman05 Posted at: 2018-04-20T17:46:17.866Z Reads: 44

```
Also I will always back @Deckoz because his knowledge and everyones knowledge on here is extremely important to the forum.  Recently @Deckoz possibly saved me from making a huge problem when I go to set up my board in bldc tool so I owe him that much.
```

---
## \#99 Posted by: Deckoz Posted at: 2018-04-20T17:49:40.331Z Reads: 42

```
It's fine let's just drop it and stay on topic...
```

---
## \#100 Posted by: Scoo_B_SK8 Posted at: 2018-04-20T17:51:51.423Z Reads: 44

```
@Deckoz you should leave that oven flow bit up tho
```

---
## \#101 Posted by: Deckoz Posted at: 2018-04-20T17:55:33.584Z Reads: 43

```
Deleted to many posts can't edit anything for 24 hrs so it'll be gone before I can edit anything.
```

---
## \#102 Posted by: ThermalM16 Posted at: 2018-04-20T17:59:40.615Z Reads: 44

```
I'll be honest with you @briman05 I would be inclined to say it was in fact a manufacturing defect if I saw something to that extent. At the end of the day it's up to Enertion to make the call, I don't make any decisions based on whether or not something should be covered under warranty. They will let me know I have a FOCBOX inbound for repair and how to contact the customer. 

Honestly, from everything I've seen since I've been on board with them, they're a pretty awesome company. I also don't get paid to talk on the forum and defend them, I'm just here because I have some extra time today and I figured I'd try to help out. I can understand why they won't warranty everything. A lot of the time these issues are user error, and it definitely puts them in a tricky spot. On one hand you want to warranty it and have a happy customer, but on the other hand, its not cheap at all and they don't have an unlimited source of money. Keep in mind they have to pay for shipping, for the repair, for parts, and anything else along the way.
```

---
## \#103 Posted by: briman05 Posted at: 2018-04-20T18:09:24.126Z Reads: 43

```
I 100% agree with you as the company I work full time for does that and warranties everything but main boards as those are subject to user error and generally go back when someone pulls the plug and the unit is still powered on.  This this thread has start today I have seen 2 other posts about bad focboxes.  I'm not trying to start something but it seems rather odd that in the past week there have been several bad foc that have come to light on this forum.
```

---
## \#104 Posted by: Deckoz Posted at: 2018-04-20T18:19:48.097Z Reads: 45

```
http://www.electric-skateboard.builders/t/focbox-unity-dual-motor/52706/84?u=deckoz

Looks like Enertion already knows it's an issue.
```

---
## \#105 Posted by: JohnnyMeduse Posted at: 2018-04-20T18:24:47.305Z Reads: 44

```
Hummm... It think you got me wrong here, that not the same thing.

And as I said, THEY ARE TESTED before shipping.

And this not only an Issue that concern Only Enertion, but everyone that is using directfet.

EDIT: Also the Issue on this thread are probably more over the 5V which mean that it is most likely a blown TVS Diode on DRV, Or 3,3V and It is a Can That have blow.
```

---
