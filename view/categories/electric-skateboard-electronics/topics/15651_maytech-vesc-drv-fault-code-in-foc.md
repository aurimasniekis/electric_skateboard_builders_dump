# Maytech VESC DRV fault code in FOC

### Replies: 19 Views: 2104

## \#1 Posted by: Martinsp Posted at: 2017-01-04T18:24:01.874Z Reads: 225

```
Hey guys,

Is there anyone who can help me? I got the DRV8302 fault on my maytech VESC but at first it went away and was spinning the motor again until i tried to change direction (bench test only not on skateboard) and now after i tried to reupload 2.18 FW it does not spin the motor anymore at all. The chip has no obvious damege to it :confused: do you think that changing the DRV will solve it? BTW i built one VESC and it s running awesome for a couple of months (5 maybe) and for the last few weeks in FOC too with sensorless, I used the same configuration on the bought maytech one and it immediately gave me the drv error. Can you help me please? :frowning:

thanks in advance :slight_smile:
```

---
## \#2 Posted by: wmj259 Posted at: 2017-01-04T19:16:25.918Z Reads: 219

```
From what I read the maytech sensors **weren't** originally built with FOC in mind.
http://www.electric-skateboard.builders/t/maytech-vesc-in-foc/15603/8?u=wmj259
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2017-01-04T19:25:02.626Z Reads: 203

```
As for your question, yes changing the drv will probably solve your problem, but I can't garanty you for how long, since It hard to see if they are using low grade parts... :thinking: unlike the one you build.

And yes I'm referring to passive component, as lower voltage  or lower capacitive values... 

@wmj259 I'm sorry but I don't think they have FOC in mind... since they clearly don't recommand to use it... It is not that you can't (any vesc can) it's just that you need to be more careful and know what you are doiing.  Also, The only VESC on the market right that as been design with FOC in mind, is the VESC-X from Enertion.
```

---
## \#4 Posted by: wmj259 Posted at: 2017-01-04T19:25:34.912Z Reads: 191

```
That is what I meant to say, sorry typo.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-01-04T19:26:34.947Z Reads: 190

```
No problem... 😅
```

---
## \#6 Posted by: Martinsp Posted at: 2017-01-04T19:43:47.518Z Reads: 181

```
Thanks, and do you know which components to check? Or which components does the FOC affect? Or "at least" where i could find complete schematics? or something like that?
```

---
## \#7 Posted by: Martinsp Posted at: 2017-01-04T19:49:42.536Z Reads: 176

```
I have looked at the website i bought it from here is the link http://www.michobby.com/product/vedder-vesc-speed-controller/ and what they say is that quote: "All of the hardware is ready for sensorless field-oriented control (FOC)" and "Sensored and sensorless FOC wich auto-detection of all motor parameters is implemented since FW 2.3" it is listed as features which of course does not prove that the components are the same ones but at least that is something that they cant blame me for because they dont say it is not suitable for what i have been trying to use it for. If i understand it correctly that is.
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-01-04T19:51:54.685Z Reads: 170

```
You can find the complete schematic and bom on vedder site

http://vedder.se/

You need to check if they use the latest bom... (the easier way, is to look for c26, if it's there then you have the 4.12 bom, if not it might be the 4.10 bom)
```

---
## \#9 Posted by: Martinsp Posted at: 2017-01-04T19:57:15.425Z Reads: 160

```
The C26 is there it looks exactly like my genuine 4.12 as far as design goes.

I didnt say it before but FOC detection worked and gave me similar numbers as the genuine one so i assume that it should be ok with FOC is that correct?
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-01-04T20:02:55.833Z Reads: 152

```
Yes, It should work as your older one.
```

---
## \#11 Posted by: Martinsp Posted at: 2017-01-04T20:06:06.860Z Reads: 149

```
maybe a silly question but I want to be sure as you seem to have more experience than i do, does your last answer mean that the foc should be fine with the maytech vesc? I am asking because I dont wanto to damage more DRVs than it is necessary :D
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2017-01-04T20:11:09.791Z Reads: 139

```
Yes, it will work, but just be careful, and don't copy paste your older configuration, and if it was in bldc before, maybe reprogramme the firmware (that should reset all the parameter to the default ones) and then you can follow the step by step configuration for foc
```

---
## \#13 Posted by: Martinsp Posted at: 2017-01-04T20:14:53.569Z Reads: 131

```
By saying same configuration i meant that the voltage and amperage limits were the same, I did the motor configuration separately. 
Do you mean like just reupload (flash) the FW? 
When i saw that "yes it will work..." you made my day :D fingers crossed that you are right :D
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2017-01-04T20:18:40.177Z Reads: 122

```
Yes Re-Upload the firware
```

---
## \#15 Posted by: Martinsp Posted at: 2017-01-04T20:20:35.157Z Reads: 123

```
Thanks a lot :) may the odds be ever in your favor :D (hope you know hunger games otherwise it would sound weird :smiley: )
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2017-01-04T20:23:25.990Z Reads: 119

```
Hahaha, that could sond weird 😂
```

---
## \#17 Posted by: Sarky1 Posted at: 2017-01-05T17:02:47.463Z Reads: 107

```
Hey Martinsp, 

Keep me posted with your findings as I'm thinking about running foc on my maytech dual ves 12s setup
```

---
## \#18 Posted by: Martinsp Posted at: 2017-01-05T18:48:08.695Z Reads: 104

```
Hey,
well I have no idea about 12s systems because i run 10s so that might make a difference because some peopla are having problems if they dont match kv to voltage. I am not going to repair it myself however because they replied to my emails saying that i can send it back to them and the service will be coverd by warranty except the shipping to them which from Slovakia is 18 euros 1st class so not that big of a deal because it means that i wont have to do anything to the vesc so i get to keep the warranty in case something else happens. Cause i am pretty sure that they would not be happy if i removed the clear heatshrink. I know that it doesnt do anything to the vesc but it is just enough for the company to blame you for messing with it...

but if you have bought in the last year it should be covered by warranty so i would not be afraid  to try foc... I guess on one at first so that if it screws up for some reason you dont have to be pushing your board :D
```

---
## \#19 Posted by: Martinsp Posted at: 2017-01-05T18:54:18.167Z Reads: 99

```
The customer service is nice after all, I thought they are not replying for some reason until I told them that i will report an issue on paypal but that WAS NOT true in the end.. it turned out that they had new years holiday. :) 

so if the person that i spoke to is reading this i am sorry i just was not sure because i have bad experience with chinese market mostly from aliexpress where the seller does not reply to normal messages until you talk about refunds and stuff... 

Quality wise I cant tell so far because it might have been just a faulty unit or something even though they say that they test each VESC before shipping. The thing is taht the motor detection worked just fine so if they just try to run a detection and call it a test if the motor spins then I cant really blame them for lying... 

anyway.. hope you will have better luck than me :D if you try it let me know please :)
```

---
