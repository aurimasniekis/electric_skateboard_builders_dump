# Devin&rsquo;s VESC Settings Calculator (for 2.16 - 2.18 firmware)

### Replies: 40 Views: 1947

## \#1 Posted by: evoheyax Posted at: 2017-07-29T04:52:27.941Z Reads: 303

```
So I know a lot of you have your opinions about Devin. Love or hate the guy, the formulas he has come up with, whether correct or not, tend to yield positive results. I have yet hear anyone try his formulas, and complain that they had bad settings.

Maybe gearing has an effect? IDK, I have only tried these formulas with hub motors (hummies and carvons), both with amazing results.

The idea is to create a constant wattage at all rpm. This gives a predictable (smooth) acceleration and braking, while increasing low rpm torque in many situations.

Now, you could run the firmware by @Ackmaniac, which implements watt control. Result's might be even better then this formula, but you do need to change your firmware, which if done incorrectly, could fry your VESC.

For the faint of heart or those looking for a simple solution, this calculator should yield interesting results. Here's the [calculator](http://www.vescstatus.com/setcalc).

Just an FYI, I am not affiliated with Devin in any way, and have posted this out of my desire to help others, and not at the request of Devin. This was my idea to create, and I was not influenced by anyone but myself into creating it. Please do not argue about Devin here.

Please post your results! The hope is either to confirm or debunk his formulas.

*** WARNING: USE AT YOUR OWN RISK! WE ARE NOT RESPONSIBLE FOR ANY DAMAGE TO YOUR VESC OR MOTORS BY USING THESE FORMULAS! KNOW THE WATTAGE LIMITS OF YOUR MOTOR OR YOU WILL FRY YOUR MOTOR (THIS FORMULA DOES NOT KNOW THE LIMIT OF YOUR MOTOR). KNOW THE MAX BATTERY REGEN AMPS YOUR CELLS CAN DO OR YOU WILL DESTROY YOUR BATTERY! YOU HAVE BEEN WARNED! ***
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-29T04:59:20.375Z Reads: 280

```
Just curious, why do you suggest people change their min/max voltage, not sure what the benefit of this is and it may mislead people about needing to set it. I always see newbies adjust this to their batteries voltage, then wonder why they're board shuts off when they brake.

Also, I tried li-ion 10s4p with .08 resistance, 8 motor min, and 3200w and I get this

<img src="/uploads/db1493/original/3X/f/d/fd3621ad21f60e6c16477ea9b682275b63c77c89.png" width="690" height="227">
```

---
## \#3 Posted by: evoheyax Posted at: 2017-07-29T05:05:19.213Z Reads: 263

```
Weird... could you highlight the upper left corner of your screen and sedn me the error? It's a php error, that I am not getting when trying your settings.
```

---
## \#4 Posted by: evoheyax Posted at: 2017-07-29T05:07:06.599Z Reads: 255

```
For the battery settings, I am just giving advice of new users in case they need advice on what settings to set. These are generic, and not perfect, but they will protect your batteries. Since I have the data I need already, I figure why not...
```

---
## \#5 Posted by: Jinra Posted at: 2017-07-29T05:07:23.858Z Reads: 243

```
No error, It goes straight to this.

<img src="/uploads/db1493/original/3X/9/6/964a3d34496309c859ca0043e6654e42201e120d.png" width="416" height="500">
```

---
## \#6 Posted by: evoheyax Posted at: 2017-07-29T05:08:26.263Z Reads: 221

```
Highlight the upper right corner, there is an error... You can't see it cause its black font on black background. But if you click above the home and drag up to the top of the page, you'll see the error.
```

---
## \#7 Posted by: Jinra Posted at: 2017-07-29T05:08:57.372Z Reads: 215

```
Haha..

> 
Notice: Undefined variable: motor2MaxWatts in /home/lukebelz/vescstatus.com/app/models/setcalc.php on line 76

> Notice: Undefined variable: motor2MaxWatts in /home/lukebelz/vescstatus.com/app/models/setcalc.php on line 76

> Notice: Undefined variable: motor2MaxWatts in /home/lukebelz/vescstatus.com/app/models/setcalc.php on line 77

> Notice: Undefined variable: motor2MaxWatts in /home/lukebelz/vescstatus.com/app/models/setcalc.php on line 78
```

---
## \#8 Posted by: evoheyax Posted at: 2017-07-29T05:10:25.276Z Reads: 204

```
Error should be fixed, might still be other bugs. It's hard to catch everything.
```

---
## \#9 Posted by: Jinra Posted at: 2017-07-29T05:11:54.683Z Reads: 205

```
FYI on the motor min

<img src="/uploads/db1493/original/3X/2/9/299ebfeac9bceff9dc8e19a75280a9b42396bbf0.png" width="690" height="204">
```

---
## \#10 Posted by: evoheyax Posted at: 2017-07-29T05:13:07.313Z Reads: 198

```
danm, I thought I tested it more throughly than this, haha.
```

---
## \#11 Posted by: evoheyax Posted at: 2017-07-29T05:15:27.189Z Reads: 196

```
Ah, put a positive number for the regen battery amps and try again. It looks like you put -8, not 8.

I have updated the calculator page to be more clear, but I will also add code to convert what's inputted into positive numbers just in case.

Thanks for all the help debugging.
```

---
## \#12 Posted by: Jinra Posted at: 2017-07-29T05:18:45.698Z Reads: 187

```
You might want to throw in some kind of limiter for the code for li-ion users since 18650's are typically limited to 20A/cell max. Putting 50 motor min spat out -43A battery min (regen)... lol

Also, when putting .08 resistance, it gives me a notice that the resistance is .16 (2x)
```

---
## \#13 Posted by: evoheyax Posted at: 2017-07-29T05:21:42.641Z Reads: 182

```
Shit, that's wrong, it should be a battery min your putting in, not motor min. Need to fix the label. The instructions are correct, and it calculates it correctly, just wrong label.
```

---
## \#14 Posted by: evoheyax Posted at: 2017-07-29T05:23:29.982Z Reads: 176

```
From what Devin told me, when you measure the resistance in the FOC detection, it's half of what the real resistance is (the firmware multiples the FOC number by 2 when using it, but stores it at half of the real resistance).
```

---
## \#15 Posted by: Jinra Posted at: 2017-07-29T05:25:20.565Z Reads: 166

```
How is motor min calculated? Also based on resistance?
```

---
## \#16 Posted by: evoheyax Posted at: 2017-07-29T05:29:16.192Z Reads: 167

```
Yes, it's all on the same formula. Until yesterday, I had never tried to apply it to motor min before. Using the battery min multiplied by the voltage at 2/3rds of the voltage range (assuming that's about average, will give slightly better performance at higher voltage, which is more likely I think for most people). That gives us a wattage, which can then be used in the other formula, to back track the motor min.

Tried with hummies and the carvons (both 2wd drive, since the each have a broken motor), and brakes are buttery smooth.

I will add a warning about using too high for li-ion packs. Thanks for the advice!
```

---
## \#17 Posted by: sprocket12 Posted at: 2017-07-29T06:49:27.941Z Reads: 160

```
Just remember we are starting to use bigger 26650's too. These can go higher as in 30A or more. 

I know, most all lie on the c rating but I'm pretty sure some will do 30.
```

---
## \#18 Posted by: darkkevind Posted at: 2017-07-29T07:14:58.852Z Reads: 168

```
How do I know what my desired wattage is? Never come across this value before.

Also, good tool but on Samsung browser it doesn't work well where there's a big black box covering up most of the form once you fill in a value...

Put in a value, keyboard comes up and your footer comes up too...
<img src="/uploads/db1493/original/3X/7/2/728f69da51a60598e977440a61eeec5567eca550.png" width="281" height="500">

Next value and then closed the keyboard, form's covered up by something...

<img src="/uploads/db1493/original/3X/6/b/6b7df82da4fcb8ef27311780c9305ade1934ef4f.png" width="281" height="500">
```

---
## \#19 Posted by: Smorto Posted at: 2017-07-29T14:48:37.113Z Reads: 150

```
<img src="/uploads/db1493/original/3X/3/7/37590f312f8199ba789803f21d1c84c2a6b53000.png" width="297" height="62">

I thought these values were supposed to stay at 8 and 57?
```

---
## \#20 Posted by: evoheyax Posted at: 2017-07-29T15:39:22.818Z Reads: 153

```
God no. Even if you have a bms, you don't want to rely on your bms to stop you from over discharging, because theres no cutoff strategy like the VESC has. This means your bms can (and its happened to people before) through you off your board at speed. You want a gradual loss of power that forces you to slow down, not an immediate ejection.

Just a warning, this app is not phone friendly.
```

---
## \#21 Posted by: evoheyax Posted at: 2017-07-29T15:55:34.620Z Reads: 147

```
First of, sorry, this website is not good for the phone, was not meant for it. sorry.

On the topic of calculating watts, watts = amps * voltage, For amps, that's battery amps. So if you have an idea of how many battery amps you want to draw (since you know the limit of battery I'd hope), and for voltage, I suggest 2/3 of your voltage range. For me, my range is 50.4 to 39.6 and that difference multiplied by 2/3 and added to the min (39.6) gives me my voltage at about 2/3 the range, which is 46.8. If you multiply that by your designed battery amps, you know your watts. But heres the kicker... You need to know what the max watts your motor can do. It's pretty normal for companies to state it when you buy the motor, because other wise, you could easily burn up your motor.

That's the mathy way of figuring it out. The other way is good old trial and error. If you feel your board is too weak and you haven't hit the limit of 120 motor amps for the VESC 4 or 6, or 300 amps for the FOCBOX, raise your wattage and recalculate. If your battery can do the battery amps that are associated with 120 motor amps, that's using the full potential of your VESC 4 or VESC 6 and getting the most power. But your battery needs to handle the battery amps and your motor needs to be able to handle the wattage with the motor amps (wattage for motor amps is calculated differently then the formula above).

The key with these formulas is to keep a ratio between motor and battery amps. This is not a simple 1:1  or 2:1 ratio, and once you have once side of the equation, you need to solve the other. So once you have battery amps correctly (both positive and regen) for the power you want and that your battery can do, and your motor wattage is not too high for the motor, your good.
```

---
## \#22 Posted by: Smorto Posted at: 2017-07-29T16:00:31.817Z Reads: 136

```
No I'm not talking about the battery cutoff start and end, I am talking about the max and min input voltage. I burned my very first vesc by changing one of these values. I was saved by the good people that @chaka employs.
```

---
## \#23 Posted by: evoheyax Posted at: 2017-07-29T16:08:02.676Z Reads: 134

```
I've never heard of such a thing before. I have 8 chaka VESCs, also set them like this, and never had an issue.

The max doesn't matter, you can leave it at 57. In fact, if you look at my number, I add 0.1*numberInSeries to that number, to give you breathing room in case you over charge your battery. The VESC doesn't help limit your battery from going too high, so it really doesn't matter. The min though should be the same as your cutoff end.

I can't see why changing this number could mess anything up (even if you set it horribly wrong).

Make sure you are on 2.18 firmware, it is the best for not having any firmware issues (at least that I know of, and I've been spending long days all week in the neck deep in the firmware code).
```

---
## \#24 Posted by: Smorto Posted at: 2017-07-29T17:29:45.616Z Reads: 126

```
I don't know man, all I know is I have heard many people tell other people not to change it and it ended up badly for me.
```

---
## \#25 Posted by: Jinra Posted at: 2017-07-29T17:31:25.040Z Reads: 129

```
he's just suggesting it as a backup for the battery cutoff I suppose, though the battery cutoff itself is enough in my opinion you can leave the minimum input voltage at 8 volts.
```

---
## \#26 Posted by: evoheyax Posted at: 2017-07-29T18:35:25.059Z Reads: 124

```
You can do either.

That was likely an issue with a particular firmware. There are no known issues with the 2.18 firmware. Vedder does some "weird" stuff with data. If you look at his code, what hes stores in the VESC, and the value you see on your screen are quite different. Many are mutiplied by 1000 or divided by 1000, some divided by 2. Likely, in some version, he messed this up (this happened for the acceleration multiplier in a firmware version). It's easy. Look how many little mistakes I made, even after testing for almost a day and refining this calculator.
```

---
## \#27 Posted by: evoheyax Posted at: 2017-08-01T17:42:15.476Z Reads: 112

```
Does anyone have results they'd like to share?
```

---
## \#28 Posted by: Ackmaniac Posted at: 2017-08-01T19:46:35.640Z Reads: 106

```
Set Battery max to 57V. This value isn't meant to protect the Battery. It is there to protect the VESC from Overvoltage. For example when the BMS shuts down. If you give the VESC more than 60V it will get damaged.
The VESC will shut down immediately when it reaches that Voltage under breaking. So really don't set it lower.

And be aware that the higher you go with motor max the more sensitive you throttle will be. Because in current control you regulate directly the motor amps.
So if you had motor max at 40A and gave 25% throttle you told the VESC to output 10A to the motor. 
If you raise your motor max to 100A and still want only the power as before (10A) then you reach that now already at 10% throttle.
```

---
## \#29 Posted by: TranxFu Posted at: 2017-08-01T21:41:20.439Z Reads: 109

```
I'm getting this... Don't think I should apply those onto my settings however. :grimacing:

<img src="/uploads/db1493/original/3X/8/3/8346dfcb0e3a9850751beefad94484aafe94198f.png" width="651" height="500">
```

---
## \#30 Posted by: Jinra Posted at: 2017-08-01T21:50:15.968Z Reads: 107

```
Yea.. I still personally believe devin's math makes no sense, but then again it was hard enough to understand what the hell he was trying to say. Not sure why it's saying max watts possible is 504 watts.. that makes no sense to me.
```

---
## \#31 Posted by: Ackmaniac Posted at: 2017-08-02T01:20:14.524Z Reads: 101

```
Lol. With these settings in the picture and current control you have more or less a on/off switch. In Watt control it would be controllable but the calculator is recommended for firmware version 2.18. So at like 1/2 max speed you can only use 1/6 of the throttle. Everything above that results in full power. 
And a Motor Min of -120 is also like a on/off switch at breaking. Not as bad as acceleration but not nice.

And the recommended max and min input voltage is simply dangerous. Shows again that Devin doesn't even test his stuff by himself.
```

---
## \#32 Posted by: evoheyax Posted at: 2017-08-02T05:39:27.043Z Reads: 92

```
What are you concerned about with regards to those numbers?

Try it and see.

I have tested numbers like these on different motors without any issues and they always work fine.
```

---
## \#33 Posted by: evoheyax Posted at: 2017-08-02T05:42:30.813Z Reads: 91

```
Basically, Devins formula is simple: you need a ratio between motor amps and battery amps. His logic is you can create even wattage by basically setting the battery and motor wattage to the same through these formulas. Personally, I don't think this is the best thing, but it's food for thought. It's seems like everyones to afraid to try something different.

The max watts is because of the 120 amp limit of the VESC 4 and 6. The FOCBOX can supposedly do 300, thus, you can put more watts through the FOCBOX.
```

---
## \#34 Posted by: evoheyax Posted at: 2017-08-02T05:44:05.735Z Reads: 89

```
[quote="Ackmaniac, post:31, topic:29020"]
And the recommended max and min input voltage is simply dangerous
[/quote]


What's dangerous about it?
```

---
## \#35 Posted by: Jinra Posted at: 2017-08-02T05:55:06.117Z Reads: 88

```
I don't get why 120a at 10s voltage is max 500~Watts. Also wouldn't ackmaniacs fw essentially do exactly what you said (even wattage)?
```

---
## \#36 Posted by: Ackmaniac Posted at: 2017-08-02T06:59:23.887Z Reads: 90

```
When These limits are reached the VESC throws immediately an over or undervoltage fault and shuts down for 3 seconds. Its not cool to loose brakes for 3 seconds when you need them.
```

---
## \#37 Posted by: evoheyax Posted at: 2017-08-02T15:15:15.421Z Reads: 84

```
It's hard to actually hit 120 motor amps with battery settings like this. battery watts = voltage * battery amps. To achieve the same motor watts, you would need to be at the same voltage used to calculate battery watts. Not likely, so you'll pull 115 or so most likely, not the 120. And you only pull that at the beginning of your acceleration. The rest of the time, you'll pull way less than 120.

This is why I said before your watt control mode is likely a better alternative. But I will be trying both watt control mode and these settings after I rewind hummies motors this week.

@Jinra the idea is on the battery side, theres watts (battery watts) and on the motor side, theirs watts (motor watts). His theory is if they are the same, you get a constant wattage through out the acceleration and braking curve.

Motor watts = (motor amps)^2 * Resistance.
Battery watts = voltage * battery amps

So together, you get (motor amps)^2 * Resistance = voltage * battery amps. So if you want to figure out one (battery or motor amps), plug in the other.

Yes, you can do more watts, but to do more watts while keeping this battery watts and motor watts ratio equal, means your stuck with the VESC's limit, which is 120 motor amps.

If youe maxing out at 120 battery and motor amps like above, but want a higher battery amp (regen or regular), you can raise the battery amps. It[s just your going to start losing this formula and won't have as smooth of an acceleration and/or braking, depending on which battery amp limit you change.

I used to pull 85 battery amps total between 4 vescs, for over 4000 watts (from the battery side). However, It was wasted, sitting in the VESC, and not getting to the motor. Now, I pull 40 battery amps instead, for a bit over 2000 watts total. I feel slightly more or the same power under my feet, but I'm wasting way less power (as a result, I was able to do 9 miles instead of 5 the other day).

You can look at this, call them crazy, as everyone did when Devin was here, or try them and prove Devin wrong.

I'm not trying to say Devin is some saint. Just that everyone should be open minded. I know a lot of you have beef with him, but that's between you and him. I'm just the messenger that tried his math, and had success. I want to find out if this formula and good or not, which is why I made this calculator. Try it, and tell me how it went. That's all I ask. And when you getting cogging and horrible performance, then we know the formula doesn't hold. But maybe it does hold? You'll never know until you try.
```

---
## \#38 Posted by: TranxFu Posted at: 2017-08-03T13:45:03.556Z Reads: 73

```
[quote="evoheyax, post:32, topic:29020"]
What are you concerned about with regards to those numbers?
[/quote]

I'm just bothered by applying 10A for battery max / min. Doesn't that limit my overall power output tremendously ?
```

---
## \#39 Posted by: evoheyax Posted at: 2017-08-03T15:22:34.264Z Reads: 73

```
In a number sense, yes. But, The power is on the motor side really. Put more than 10a on the battery side and your wasting energy. I use to set my motors to 80 motor amps and 20 battery amps (per motor). Now, I do 120 motor and 12 battery, and I have the same, if not better acceleration, but I consume less energy in the process.
```

---
## \#40 Posted by: Jinra Posted at: 2017-08-03T15:42:55.639Z Reads: 73

```
With your calculator you're limiting potential energy by a ton. With 10A battery on 10s, you're capping your potential draw to 360w of power. You can set motor max to 120, but when would you ever utilize that, you only have 360w to work with. While 3v @ 120a would equate to 360w, you can't ever have 3v duty cycle and draw 120a due to the way current control works. At 18v (50% duty) you can only draw 20 amps of current in the motor.

With 40/80 battery/motor config, you would get 1440w of **available** power. At 18v on this setup, you can draw up to 80A! This is double the available power for acceleration.

If you're claiming better/same acceleration and performance, you should post a video. Do a 20 yard sprint on flats with the two configs. One doing 40a battery 80a motor, and the other doing your 10a battery and 120a motor.
```

---
