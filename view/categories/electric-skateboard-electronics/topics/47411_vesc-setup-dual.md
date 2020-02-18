# VESC Setup dual

### Replies: 57 Views: 2776

## \#1 Posted by: Ingvarjedi Posted at: 2018-02-25T14:59:17.466Z Reads: 360

```
Hello.
I have:
Two motors
https://hobbyking.com/ru_ru/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html

And two batteries in series 
https://hobbyking.com/ru_ru/turnigy-5000mah-6s-25c-battery.html

Two VESC from DIY
I have installed and connected two VESC CUN .
I set up the BLDC mode and both engines work when I press the gas without load.

But when I clamp my hand on the engine and press the gas, moto does not give any effort to scroll.

here are my settings![IMG_2284|666x500](upload://trmsOBxpA9Fg4UK60iEq8BE79U8.JPG)![IMG_2283|666x500](upload://fU5q07kFZxpzUvHIq5L47SWEL1S.JPG)![IMG_2285|666x500](upload://jIpR81ltV1lMOfwHCf6sF9r4pCc.JPG)![IMG_2282|666x500](upload://dcwwgV7emVcRuugSsHWWGZuDhc6.JPG)![IMG_2281|666x500](upload://9hNtdpBLvIyRxZWDuBYF579lOX9.JPG)![IMG_2286|666x500](upload://f6zJhv7fB7noOaenX7rJrwqvvDA.JPG)![IMG_2287|666x500](upload://4KAkt9jKdEGv3nTxn2Yo8QUOdDJ.JPG)![IMG_2288|666x500](upload://aXYnDcu3KipmFmgMeaGrJgMUy4r.JPG)![IMG_2292|666x500](upload://bKMZh2vLVUARlT62AFAFY96ltPT.JPG)![IMG_2289|666x500](upload://jP5UMt6GQYzn1kXFtPThGVQMPLE.JPG)![IMG_2290|666x500](upload://2FXOlGP2ThyylZXeesh1rgsGAuG.JPG)![IMG_2291|666x500](upload://tCUxzWtflTyef5kxjeqbXxIGRUW.JPG)
```

---
## \#2 Posted by: faithfulpuppy Posted at: 2018-02-25T15:05:27.100Z Reads: 290

```
What is your maximum current set to? Both battery Max and motor max
```

---
## \#3 Posted by: trampa Posted at: 2018-02-25T15:11:21.020Z Reads: 293

```
Hope this helps:

https://www.vesc-project.com/node/178

Frank
```

---
## \#4 Posted by: Ingvarjedi Posted at: 2018-02-25T15:26:17.531Z Reads: 294

```
Yes, I did everything according to the instructions.

The motors spin when the gas is pressed. But if I press the motor with my hand and press the gas, it does not spin, that is, my strength is greater than the effort given by the VESC.
```

---
## \#5 Posted by: Blitz Posted at: 2018-02-25T15:42:13.972Z Reads: 277

```
You have to push start uncensored motors to get them going.

Edit: Your motors are uncensored so they don't know what way to spin So you need to push them in the right direction for them to start, so there's no surprise that it dont spin, and please don't screw with your vesc settings LOL.
```

---
## \#7 Posted by: Ingvarjedi Posted at: 2018-02-25T16:03:12.454Z Reads: 254

```
![IMG_2294|375x500](upload://u4S6kT8LbEGkmLsgkZpxOXIdjUD.JPG)is selected - sensorless(uncensored)
```

---
## \#8 Posted by: Blitz Posted at: 2018-02-25T16:07:33.647Z Reads: 236

```
Everything is fine, What I'm trying to say is your motor does not have sensors It will not Start powerfully on its own hence why Your hand can hold it down. Do you still not Understand?
```

---
## \#9 Posted by: Ingvarjedi Posted at: 2018-02-25T16:17:27.618Z Reads: 230

```
I do not understand. I have ESC Racerstar, it gives a lot of power and I can not hold it in my hand.

May be changing StartUp Boost parameter, I increased it, it became more powerful?
```

---
## \#10 Posted by: Blitz Posted at: 2018-02-25T16:24:58.759Z Reads: 228

```
All I can say is When using Vesc and uncensored motors. you have to give it a small kick to get it going. Some people like a smooth start not 100% gas wheels up So Startup boost is for own preference and If your board rides OK don't worry about the wheel not spinning when you grip the motor It's normal.
```

---
## \#11 Posted by: Ingvarjedi Posted at: 2018-02-25T16:40:57.602Z Reads: 217

```
ok
why if I change the settings VESC and save them, then the parameters of the second VESC do not change?
```

---
## \#12 Posted by: Ingvarjedi Posted at: 2018-02-25T16:45:56.181Z Reads: 211

```

I added a boost from 0.010 to 0.115 this became more powerful, Hell, I still can hold the motor by hand :(((

Ok. he can not move my body weighing 96 kg
```

---
## \#13 Posted by: Blitz Posted at: 2018-02-25T16:48:59.187Z Reads: 210

```
Nice But be careful with Vesc settings If the Vesc pulls more amps that It can handle It could blow! So after changing this setting the board does not even start after a small push?
```

---
## \#14 Posted by: GrecoMan Posted at: 2018-02-25T16:51:42.212Z Reads: 207

```
the startup boost should not be higher than 0.05. please lower it if you want to keep your vescs.
```

---
## \#15 Posted by: Blitz Posted at: 2018-02-25T16:55:06.673Z Reads: 206

```
@Ingvarjedi Revert your settings Like @grecoman Said. Vesc's Is different don't expect the Startup to work the same as your esc OK?
```

---
## \#16 Posted by: Skitzor Posted at: 2018-02-25T16:55:21.742Z Reads: 199

```
That sounds like the traction control that's built in. Try disabling this and test once again.
```

---
## \#17 Posted by: Bensaida Posted at: 2018-02-25T16:56:37.710Z Reads: 195

```
this dude is gonna blow his VESCs and wonder what happened
```

---
## \#19 Posted by: Ingvarjedi Posted at: 2018-02-25T17:03:41.189Z Reads: 188

```
Where that?
```

---
## \#20 Posted by: Ingvarjedi Posted at: 2018-02-25T17:03:57.071Z Reads: 182

```
Hahahah may be))
```

---
## \#21 Posted by: Ingvarjedi Posted at: 2018-02-25T17:06:30.253Z Reads: 180

```
https://youtu.be/Nf_I4m9MHx4
```

---
## \#22 Posted by: GrecoMan Posted at: 2018-02-25T17:08:04.281Z Reads: 177

```
that’s not unusual... it’s an **UNSENSORED MOTOR, IT WILL NEED A PUSH START TO GET GOING**
```

---
## \#23 Posted by: Blitz Posted at: 2018-02-25T17:11:08.626Z Reads: 168

```
Its no use I said that like 3 times
```

---
## \#24 Posted by: Bensaida Posted at: 2018-02-25T17:17:10.820Z Reads: 165

```
oh but when i hold the motor it doesnt go? :P
```

---
## \#25 Posted by: Ingvarjedi Posted at: 2018-02-25T17:18:21.545Z Reads: 164

```
this is a feature vesc?
```

---
## \#26 Posted by: GrecoMan Posted at: 2018-02-25T17:18:51.047Z Reads: 163

```
no. the vesc will not push itself until it dies like other escs
```

---
## \#27 Posted by: Blitz Posted at: 2018-02-25T17:22:25.085Z Reads: 160

```
Look Man you can ether watch a few 1hour video guides or you can just Trust us, 

[quote="GrecoMan, post:22, topic:47411"]
it’s an UNSENSORED MOTOR, IT WILL NEED A PUSH START TO GET GOING
[/quote]
There are more expensive Motors with sensors but you dont have a sensored motor.
Vesc Is great with little drawbacks Its not perfect. You're original Question has been awnsered.
```

---
## \#28 Posted by: Colson003 Posted at: 2018-02-25T17:26:39.320Z Reads: 156

```
I’ll say it too, that is completely normal with sensorless motors. You could bump up your motor amps up to around 70 or 80 to help when you’re starting from a stop while riding the board.
```

---
## \#29 Posted by: Ingvarjedi Posted at: 2018-02-25T17:32:05.955Z Reads: 155

```

I began to understand, it means the truth.
Whoever see my screenshots and settings, maybe give a couple of tips
```

---
## \#30 Posted by: Blitz Posted at: 2018-02-25T18:00:46.040Z Reads: 154

```
whoa 70-80a Sounds Unsafe DUDE!

I would not even run a focbox over 50a Continuous.
```

---
## \#31 Posted by: Blitz Posted at: 2018-02-25T18:03:17.883Z Reads: 152

```
Tip 1 

[quote="GrecoMan, post:14, topic:47411"]
startup boost should not be higher than 0.05.
[/quote]
Did you Lower it?

Tip 2 Be very careful with vesc settings don't tinker or joke around You could blow them up!

Tip 3 read your Comments on this topic twice and think about what people are trying to tell you.
```

---
## \#32 Posted by: mmaner Posted at: 2018-02-25T18:12:11.222Z Reads: 148

```
I run my FocBoxes at 80amp burst, no problem.
```

---
## \#33 Posted by: Blitz Posted at: 2018-02-25T18:13:24.108Z Reads: 146

```
Burst I understand but what colson wrote could be read differently 

[quote="Colson003, post:28, topic:47411"]
70 or 80
[/quote]
```

---
## \#34 Posted by: GrecoMan Posted at: 2018-02-25T18:13:37.490Z Reads: 148

```
I ran my TB vescs at 120a motor max...
 
i run my upgraded enertions at 120a motor max
```

---
## \#35 Posted by: Blitz Posted at: 2018-02-25T18:14:07.063Z Reads: 149

```
Again I'm talking about "Continuous Current" are we one the same page here?
```

---
## \#36 Posted by: GrecoMan Posted at: 2018-02-25T18:15:37.924Z Reads: 148

```
dude he didn’t say constant 🤣

you don’t understand the relationship between batt max and motor max. the vesc will never pull more than the batt max. you could have motor max at 120a and batt max at 20a, it would never pull above 20a. the motor max just mainly sets your low speed torque
```

---
## \#37 Posted by: Blitz Posted at: 2018-02-25T18:17:10.894Z Reads: 148

```
I understand but you need to be more clear, because @Ingvarjedi could change the wrong setting.
and he has proven to have low understanding of vesc's
```

---
## \#38 Posted by: GrecoMan Posted at: 2018-02-25T18:18:11.013Z Reads: 147

```
I said the exact name of the setting that he could change...
```

---
## \#39 Posted by: Blitz Posted at: 2018-02-25T18:28:50.023Z Reads: 144

```
@grecoman thanks for explaining this, I will remember when programming my vesc think twice take a break think again then Finnish :joy:
```

---
## \#40 Posted by: FredrikHems Posted at: 2018-02-25T18:35:43.478Z Reads: 150

```
[quote="GrecoMan, post:34, topic:47411"]
I ran my TB vescs at 120a motor max…
[/quote] 

And how did that go? :joy: 
6 vesc’s later.. :joy:
```

---
## \#41 Posted by: pennyboard Posted at: 2018-02-25T18:37:16.568Z Reads: 151

```
Are you talking continuous current in this case or burst? 
Cause when I log data on my VESC and look at it, motor max is at about 80Amp and battery max is at 40Amp. If pulled 50 or 60 Amps at times, for bursts. I believe the capacitors on the VESC provide the extra current for short bursts but once they get depleted of charge, max continuous current is dictated by battery max settings.
```

---
## \#42 Posted by: pennyboard Posted at: 2018-02-25T18:38:09.952Z Reads: 151

```
I’ve been running mine at 80 amps for about 6 months, no problems
```

---
## \#43 Posted by: FredrikHems Posted at: 2018-02-25T18:41:33.759Z Reads: 144

```
I know many do 80 without problems.
The reason i quoted Greco is because I know he have gone thru a «couple» og vescs :wink:
```

---
## \#44 Posted by: GrecoMan Posted at: 2018-02-25T18:44:39.224Z Reads: 140

```
lol. I know the exact reason why every single one of my vescs blew, and that was not it 😉

i can even list them if you want 🤣
```

---
## \#45 Posted by: FredrikHems Posted at: 2018-02-25T18:45:39.172Z Reads: 136

```
I guess alot of drv’s
```

---
## \#46 Posted by: GrecoMan Posted at: 2018-02-25T18:46:22.000Z Reads: 134

```
was the motor pulling 50-60a it was that the BATTERY current? it’s totally normal for the motor current to be higher than the battery current. unless i’m mistaken, the large caps on the vesc are to smooth out voltage ripples, but you could totally be right.
```

---
## \#47 Posted by: GrecoMan Posted at: 2018-02-25T18:46:34.498Z Reads: 134

```
lots of shorted things

i’ve blown fets, melted traces, etc
```

---
## \#48 Posted by: pennyboard Posted at: 2018-02-26T01:14:07.752Z Reads: 119

```
Motor was pulling 60 Amps with motor max set to 80 Amps. 
Battery was pulling 30 Amps, with battery max set to 40 Amps
```

---
## \#49 Posted by: GrecoMan Posted at: 2018-02-26T01:23:01.381Z Reads: 118

```
yea. that’s normal. the motor will always pull more than will be drawn from the battery. hence the reason it’s safe to run 120a motor max and 25a batt max (like I do). the motor can be pulling 120a, but the amperage that’s actually pulled from the battery will never go above 25a
```

---
## \#50 Posted by: Ingvarjedi Posted at: 2018-02-26T05:18:57.506Z Reads: 116

```
I'm right?

![Plan|238x499](upload://6icNYeHO6vkFVaPmXUq8yc17ULc.png)
```

---
## \#51 Posted by: Ingvarjedi Posted at: 2018-02-26T18:21:45.584Z Reads: 111

```
Can I use the FOC mode for VESC 4?
are there any restrictions and security settings?
```

---
## \#52 Posted by: Blasto Posted at: 2018-02-26T18:26:17.148Z Reads: 112

```
![image|238x499](upload://MFBNkQe4O2eq6QCP1PqBkuVZno.png)
```

---
## \#53 Posted by: b264 Posted at: 2018-02-26T18:29:17.796Z Reads: 105

```
It's probably better to put the loop key on the negative line but electrically it makes no difference.  BMSs switch the negative lines and positives get tied together

It can just be less confusing is all.  Electrically it makes no difference
```

---
## \#54 Posted by: Ingvarjedi Posted at: 2018-02-26T18:39:49.971Z Reads: 108

```
Thank you. I was mistaken when I was drawing, I meant what you did))
```

---
## \#55 Posted by: ShutterShock Posted at: 2018-02-26T18:53:52.454Z Reads: 107

```
Please keep in mind that to configure the settings on the second vesc you will need to plug in the usb cable into the second vesc and program that by itself too.

They do not transfer settings between each other
```

---
## \#56 Posted by: Esk8board4life Posted at: 2018-07-20T00:52:20.218Z Reads: 83

```
Hey guys I was wondering, so I’m going to run a dual motor setup... does that mean I set my battery max to 40a and each motor max to 20a? Also for regen max battery -30a and each motor regen max -15a? Is this correct pls help. Also how to I connect the two via canbus using slave and id0 and id1. Helppppppp!
```

---
## \#57 Posted by: Esk8board4life Posted at: 2018-07-20T00:56:31.250Z Reads: 85

```
Also... as long as the motor max is higher than battery... it doesn’t really matter. Like the battery will only give the motor 30a even if it’s set at like 40 or 50. Right?
```

---
## \#58 Posted by: Andy87 Posted at: 2018-07-20T12:46:38.372Z Reads: 83

```
the battery max depends on your battery.
if you run dual than div. that to 2 and you have your bat max current.
The same with bat min current (but this you can set a bit higher as you usually just break for a short time and will not charge const. with 20A for example).
The motor max you can theoretical set to any value.
But usually it´s around 60-80A per motor.
The motor min just set to 40A per vesc and than look how you like your breaks. if too less set it up, if too strong set it down.

your vesc will not draw more amps from the battery than your max battery setting.
But the vesc can put out more amps than you set your battery amps.
if your motor needs more amps, the vesc will just regulate that by put down the voltage which on your motor. P=U*I more I less U as the Battery Power always stay the same.
Hope that made it more clear, not more complicated :sweat_smile:

Dual set up:
Yes can bus than one as master "0" one as  slave "1" and activate, sent data via can bus or something like this.
You could also connect your vescs with a Y-split cable of the remote, than you don´t have to set any master or slave.
```

---
## \#59 Posted by: trampa Posted at: 2018-07-20T12:58:06.834Z Reads: 74

```
If you run a dual, you need to cut the values for the battery in half since each ESC pulls/pushes Amps and having two ESCs your battery sees twice the values you enter.
You need to understand the relation between the different values, which you can read in the post below.

https://www.electric-skateboard.builders/t/vesc-6-cooling-and-max-current/61944/9?u=trampa
```

---
