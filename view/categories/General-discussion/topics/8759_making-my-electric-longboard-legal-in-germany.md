# Making my electric longboard legal in Germany

### Replies: 92 Views: 8152

## \#1 Posted by: Ackmaniac Posted at: 2016-09-01T10:49:56.948Z Reads: 572

```
My plan is to find a way to make my longboards legal in Germany.
For that I studied which vehicles are already legal that are powered by an electric motor. And I came across the “Smart Ped” kick push scooter.
As a couple of you know you would need a license plate for electric vehicles which go faster than 6 km/h and accelerate on their own. 
So the “Smart Ped” doesn’t accelerate. It only holds the speed like a cruise control. And also the motor has a max power output of 250 Watt and max speed of 25 km/h.
So I was thinking about the same behavior for my electric longboard. You would have to push on your own but it could hold the speed with 250 watt and stops giving power above 25 km/h.

So is started to look in the code of the Vesc and finally found a way to program this by changing the firmware. 
I made the first test runs and still need to do some fine adjustments but it looks very promising, only the 
max speed settings are not yet included.

So the behavior is as described:

* No acceleration
- When the trigger is pulled the board tries to keep the speed
-	Power of the motor is limited to 250 watts (limited by software, so any motor is fine)
-	When the board can’t keep the speed (up hill) then the board will only try to keep the actual speed:
e.g. before hill 20 km/h,  on top of the hill 15 km/h because 250 watts was not enough so you would continue rolling with 15 km/h on the flat. To be faster you need to push again and pull the trigger again
-	when the trigger is not touched then it rolls freely
-	full brake power available (saferthan a non-powered board)
-	above 25 km/h the motor can’t be activated

Does anybody see a reason why this shouldn’t be legal then. Because “Smart Ped” kick push scooter does the same thing and it is allowed. But maybe I missed something.
```

---
## \#2 Posted by: E-Boarding Posted at: 2016-09-01T10:58:54.846Z Reads: 515

```
a asked the mellow guys a few months ago if they can do exact this behavier but got no useful respond, keep going, I would try this aswell but have no idea how to change the VESC that way.

btw. you can set max rpm in the VESC
```

---
## \#3 Posted by: Ackmaniac Posted at: 2016-09-01T11:04:43.872Z Reads: 499

```
You can't do it by settings in the BLDC tool. (Not yet :grin:)
You have to change the code in the firmware which isn't so easy. 
Maybe later on a new section can be implemented in the BLDC-TOOL (maybe app settings) to choose and adjust this behavior.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-09-01T11:19:39.572Z Reads: 475

```
[quote="Ackmaniac, post:1, topic:8759"]
Power of the motor is limited to 250 watts (limited by software, so any motor is fine)
[/quote]

I dont think that it will work that way...

Lets explain it with an example:
If an eboard can go faster than 6km/h it needs insurance and so on. You are not allowed to drive with it even if you change the max speed on the software side. That is because you could go faster if you remove the software "lock". 

I think you have to use a 250W motor otherwise you could potentially use more wattage and thus it is not legal.
```

---
## \#5 Posted by: Ackmaniac Posted at: 2016-09-01T11:32:26.220Z Reads: 434

```
By my studies it is only important that the power on the shaft gives max 250 Watts in average (whatever average means here, so small pikes are allowed). 
Also a motor can't be regulated because then you could power it with a higher voltage battery and it would give again more power. And there is no law for the battery. So the regulation must be on the output power. Not the power the motor might can produce.

And you only need insurance when it accelerates to more than 6 km/h. But my modifications doesn't allow that. It only keeps the speed, so it is only a assistance. E-bikes till 25 km/h and 250 watts are also only allowed because they assist you when you push the peddle instead of accelerating on their own. And they need no insurance.
The "Smart Ped" does the same, and it is legal.
```

---
## \#6 Posted by: Maxid Posted at: 2016-09-01T11:45:25.510Z Reads: 412

```
you are wrong - an e-bike is basically limited to exactly this behavior.
Only thing that needs to also be implemented:
As far as I know the vehicle is not allowed to "hold" the speed but needs to slow down if there is no constant "push" by the user. That is why you have to keep peddaling on a bike and do these awkward pushes on the scooter.
```

---
## \#7 Posted by: Ackmaniac Posted at: 2016-09-01T12:15:33.672Z Reads: 383

```
The "Smart Ped" keeps the speed for 500 seconds and then needs another push. I think something like this can easily be implemented. But good that you mentioned. 
In reality you would never notice because i think you won't keep the same speed for 8 minutes constantly without a speed change. But do you know where i can find more details about that?
```

---
## \#8 Posted by: Maxid Posted at: 2016-09-01T13:51:56.500Z Reads: 385

```
http://www.gesetze-im-internet.de/stvg/__1.html

> (1) Kraftfahrzeuge und ihre Anhänger, die auf öffentlichen Straßen in Betrieb gesetzt werden sollen, müssen von der zuständigen Behörde (Zulassungsbehörde) zum Verkehr zugelassen sein. Die Zulassung erfolgt auf Antrag des Verfügungsberechtigten des Fahrzeugs bei Vorliegen einer Betriebserlaubnis, Einzelgenehmigung oder EG-Typgenehmigung durch Zuteilung eines amtlichen Kennzeichens.
> (2) Als Kraftfahrzeuge im Sinne dieses Gesetzes gelten Landfahrzeuge, die durch Maschinenkraft bewegt werden, ohne an Bahngleise gebunden zu sein.
> (3) Keine Kraftfahrzeuge im Sinne dieses Gesetzes sind Landfahrzeuge, die durch Muskelkraft fortbewegt werden und mit einem elektromotorischen Hilfsantrieb mit einer Nenndauerleistung von höchstens 0,25 kW ausgestattet sind, dessen Unterstützung sich mit zunehmender Fahrzeuggeschwindigkeit progressiv verringert und
> 1.
> beim Erreichen einer Geschwindigkeit von 25 km/h oder früher,
> 2.
> wenn der Fahrer im Treten einhält,
> unterbrochen wird. Satz 1 gilt auch dann, soweit die in Satz 1 bezeichneten Fahrzeuge zusätzlich über eine elektromotorische Anfahr- oder Schiebehilfe verfügen, die eine Beschleunigung des Fahrzeuges auf eine Geschwindigkeit von bis zu 6 km/h, auch ohne gleichzeitiges Treten des Fahrers, ermöglicht. Für Fahrzeuge im Sinne der Sätze 1 und 2 sind die Vorschriften über Fahrräder anzuwenden.

Especially 3 is the interesting part

Also interesting regarding the 250W motor:
http://www.pedelecforum.de/wiki/doku.php?id=e-motor:nenndauerleistung
explaining how that number is measured.

Oh and btw:
I am highly interested in this project. Please go forward with this and publish the firmware once you have a working version. This will make my life a lot easier (and calm down the lady at home). In theory you could even incorporate the remote to switch between the "legal" mode and the one for private properties ;)
```

---
## \#9 Posted by: Ackmaniac Posted at: 2016-09-01T14:54:09.206Z Reads: 350

```
You are right.
"It has to stop powering when the driver stops pedeling"
But when it comes to the "Smart Ped" that only could mean to stop assisting the  acceleration and not to shut off the power completely. I guess we would need a lawyer to make that point 100% clear. 
I also tried to find more details about the "Smart Ped" and how they made it legal but most pages simply say because it doesn't accelerate.
```

---
## \#10 Posted by: michaeld33 Posted at: 2016-09-01T14:56:38.285Z Reads: 341

```
Just FYI, this project has already been attempted/compleated in some form by the respected butthole himself. @lowGuido
Not identical. But very similar.

https://www.youtube.com/watch?v=jzwtTf7k4yQ
```

---
## \#11 Posted by: Ackmaniac Posted at: 2016-09-01T15:27:51.447Z Reads: 326

```
He uses the cruise control of the nunchuck. Nice idea.

Sadly that doesn't cover all the regulations.

For example he has not the limitation of 250 watts.
And if there is a hill that slows him down he would accelerate again on the flat to the previous speed.

He also doesn't have brakes. (No regulation but very nice to have)

One more thing i had to think about. When the law says that it also has to stop powering at 25 km/h then all the ebikes are illegal. Because they don't stop powering at that speed. They only don't assist you for more than 25 km/h. So if you only can push it to 20 km/h with your muscels then it would support you till 25 km/h. But it lets you stay on that speed and doesn't shut off directly.
Which brings us back to the point where we need to find out how they managed to make the "Smart Ped" legal.
```

---
## \#12 Posted by: Maxid Posted at: 2016-09-01T15:38:04.736Z Reads: 310

```
[quote="Ackmaniac, post:11, topic:8759, full:true"]
One more thing i had to think about. When the law says that it also has to stop powering at 25 km/h then all the ebikes are illegal. Because they don't stop powering at that speed. They only don't assist you for more than 25 km/h. So if you only can push it to 20 km/h with your muscels then it would support you till 25 km/h. But it lets you stay on that speed and doesn't shut off directly.
Which brings us back to the point where we need to find out how they managed to make the "Smart Ped" legal.
[/quote]
They stop supporting your peddaling at 25km/h. If you are not able to get to 25km/h even with the support they will not go to 25 by themselves. Why should this be illegal. I don't get what you are saying here.
```

---
## \#13 Posted by: E-Boarding Posted at: 2016-09-01T17:07:46.172Z Reads: 275

```
Is it allowed to multiply the power of your push by factor x?
I thought the Scrooser worked that way, but I'm not sure.
```

---
## \#14 Posted by: Ackmaniac Posted at: 2016-09-01T21:49:34.147Z Reads: 275

```
I had a quick look and on the actual website they say that the standard Scrooser is only allowed on private property. So it seems that it is not sure that also the "Smart Ped" is really allowed. But then it would be strange that they advertise with that feature.

Anyway, i will try to copy the behavior of it.

Maybe somebody of the forum can help us with the question if it is allowed or not.
Maybe with some bundled research we can find a way to make our hobby legal for Germany and a couple of other countries.
```

---
## \#15 Posted by: lowGuido Posted at: 2016-09-02T01:22:31.075Z Reads: 269

```
[quote="Ackmaniac, post:11, topic:8759"]
And if there is a hill that slows him down he would accelerate again on the flat to the previous speed.
[/quote]

Im not sure i undestand this statement?
```

---
## \#16 Posted by: dude Posted at: 2016-09-02T02:02:22.250Z Reads: 261

```
I think the board needs to keep the reduced speed (reduced from the hill) until u accelerate by pushing ... else it would count as accelerating on it's own which would be not allowed.
```

---
## \#17 Posted by: cantstopme Posted at: 2016-09-02T02:13:10.071Z Reads: 262

```
that wont help you at all. it doesnt matter what private measures you take to limit the power or functionality of the board, b/c they will argue that you could switch those off at any point. Only thing that matters here is its native specs. If your board comes with more power and is built for higher speed than allowed it's illegal.
```

---
## \#18 Posted by: Ackmaniac Posted at: 2016-09-02T06:35:26.095Z Reads: 251

```
As i mentioned earlier. The power is not the problem. The only thing that matters when it comes to watts is that that the motor doesn't provide more than 250 watts in average. Even if the motor could produce 5000 watts by the specs.
```

---
## \#19 Posted by: lowGuido Posted at: 2016-09-02T12:04:08.143Z Reads: 248

```
My board does that. It will never accelerate faster than you push it.

Infact that in my mind is the biggest downside.
```

---
## \#20 Posted by: Maxid Posted at: 2016-09-02T12:22:39.890Z Reads: 247

```
Not true according to this:
http://www.pedelecforum.de/wiki/doku.php?id=e-motor:nenndauerleistung
```

---
## \#21 Posted by: dude Posted at: 2016-09-02T12:32:35.429Z Reads: 236

```
Unsure ... it says the amount of energy the drive system can output, not only the engine. If drive system = power source + controller + motor it would allow a more powerful motor if the controller limits the output ... right? I hate laws ;)

see section "1.2. Messung" ... that looks like a test of the engine power inside the complete system ... not on it's own
```

---
## \#22 Posted by: Maxid Posted at: 2016-09-02T12:42:41.007Z Reads: 234

```
as far as I know the motor needs to be tested with the S1 standard:
> 2.2. S1 Dauerbetrieb

> Betrieb mit konstantem Belastungszustand, dessen Dauer ausreicht, den thermischen Beharrungszustand zu erreichen.

which means the temperature the motor produces is the crucial point. An SK3 will probably not reach the "thermischen Beharrungszustand" with just 250W (if you don't supply just 1V ;))
```

---
## \#23 Posted by: dude Posted at: 2016-09-02T12:59:28.764Z Reads: 223

```
does "thermischen Beharrungszustand" not only mean that you need to use it until the temperature of the motor stays constant?

In the 2.2 section you quoted there is a link to this thread:
http://www.pedelecforum.de/forum/index.php?threads/legalisierung-eines-500w-motors-%C3%BCber-begrenzung-des-batteriestroms.8462/
especially this post:
http://www.pedelecforum.de/forum/index.php?threads/legalisierung-eines-500w-motors-%C3%BCber-begrenzung-des-batteriestroms.8462/page-2#post-109683
There is not that much about the legal things of the 250W limit, but they seem to interpret the limit as average of typical use with temporal spikes allowed.
```

---
## \#24 Posted by: Ackmaniac Posted at: 2016-09-02T13:01:17.072Z Reads: 227

```
As i sayed earlier. A motor that produces 250 watts at 24V would produce around 375 watts at 36V. And the battery is not regulated. So you only can limit it by the power output.
The bigger problem we have is if it is allowed to keep the actual speed with the motor or not.

The "Smart Ped" keeps the speed for 500 seconds with a miaximum of 250 watts. And they advertise that it is allowed in Germany. So they are lying or they found way. But i also could not find any more detailed infomation about it. 
I just thought that i can do that as well so started modifying the vesc firmware with a innocent feeling.:innocent:

BTW , can sombedoy who has a sensored motor tell me if the motor gives a more stable rpm signal than a unsesored motor with the VESC.
```

---
## \#25 Posted by: dude Posted at: 2016-09-02T13:09:37.631Z Reads: 214

```
:D legal in germany can also mean that you are allowed to drive it in your driveway ... or did they advertise something more specific?

for keeping the speed or slowing down the assistive force over time ... maybe we find some other devices which fall under this regulation and answer the question on this way.
```

---
## \#26 Posted by: dude Posted at: 2016-09-02T13:30:54.533Z Reads: 216

```
Ok i found it ... Der Tagesspiegel writes:
> nach Angaben seines Erfinders darf es legal auf der Straße und auf dem Radweg fahren

I don't expect any reply ... but i'll ask them directly on which legal base this is allowed on german roads ... maybe it works :)
```

---
## \#27 Posted by: Ackmaniac Posted at: 2016-09-02T13:37:04.653Z Reads: 208

```
Awesome. Thank's for the help.
```

---
## \#28 Posted by: dude Posted at: 2016-09-02T13:47:52.460Z Reads: 204

```
It's in my own interest ;) I planned to make my build as stealth as possible ... but the motor is sooo big ... it will not be stealth at all. Someone got an insurance for his board, but that does not cover all legal problems and i think he was just lucky to meet the right insurance guy at the right time ^^ And come on ... a number plate on a skateboard? So your possible solution is the only way for me to maybe not have to think about a 1500€ fine all the time.
```

---
## \#29 Posted by: Hummie Posted at: 2016-09-02T14:25:44.891Z Reads: 206

```
Wow that's a huge fine. 

And that's a strange law which it seems is still not understood

How about you just limit the erpm on the vesc or the max amps to the motor?  limiting the amps to the motor would be a true way to limit the power.  limit the erpm to just go slower and satisfy the police
In USA there are a lot of people riding boards and bikes that are illegal and no one knows and the cops don't care.  With a 250watt limit, they will never be able to truly test a 250watt output and neither will you and ur basing it on the input of course so you're sure to have a bit of wiggle room.
```

---
## \#30 Posted by: kampfhahn Posted at: 2016-09-02T15:37:23.860Z Reads: 198

```
You could also try to get an insurance and leave the licence plate at home because riding without a licence plate is just a baby delict (fine 60 €) compared to riding without an insurance.
```

---
## \#31 Posted by: cantstopme Posted at: 2016-09-02T16:39:02.702Z Reads: 199

```
the law in Austria is a bit more relaxed and declares e-scooters up to 600w and 25km/h max as bicycles, so you don't need a plate or insurance for them. Problem is that definition only covers 2-wheeled vehicles and they say nothing about Eboards. The legal situation is just unclear atm. I bought a board with low-wattage motors (500w total), top speed is alot higher tho, so it's illegal aswell. I just accept being an outlaw then and try to avoid confrontations with police.
```

---
## \#32 Posted by: dude Posted at: 2016-09-02T17:12:23.415Z Reads: 205

```
[quote="Hummie, post:29, topic:8759"]
limiting the amps to the motor would be a true way to limit the power.  limit the erpm to just go slower and satisfy the police
[/quote]

yes that seems to work but it's only one part of the legal problems.

[quote="kampfhahn, post:30, topic:8759, full:true"]
You could also try to get an insurance and leave the licence plate at home because riding without a licence plate is just a baby delict (fine 60 €) compared to riding without an insurance.
[/quote]

nice ... didn't know that it's still insured without licence plate ... so with much effort to find an insurance company which would make a special agreement like Cantholz84 got ( http://www.elektro-skateboard.de/forum/showpost.php?p=39239&postcount=94 ) this would be an emergency solution ^^ but lets hope that the ideas in this thread work out, that would be less difficult. I think even if we find out that the only assisting board with an average of 250W output may be legal but the laws are not specific enough it should stop some law enforcements from opening a case.
```

---
## \#33 Posted by: Chrisi-MUC Posted at: 2016-09-02T21:29:44.036Z Reads: 197

```
Quite new to esk8 (no practical experience atm, but I've read hour the last days), but I hope this information helps a little bit to get this topic further. 
This Guy sells a so called "Gasgriff-Freischalter" which detects if the biker is pedalling or not (and other things to upgrade to an ebike) It's also quite interesting to read about pseudo pedalling, which means the biker only has to keep the Pedal rotating, the engine gives the power. 
Seems as many upgrade bicyclists are also in a grey zone...
http://www.groetech.de/index.php?main_page=product_info&cPath

Max. speed 25km/h: I think a software limit would be ok, as long If you keep it. You have always the possibility to cheat afterwards. Same with the good old Mofa. You Can drive it as built by the manufacturer or tune/manipulation it to higher power/speed afterwards...

Max. Power: dunno if there is a offroad mode for some e mountain bikes, but 2 weeks ago my collegues saw an 120kg guy riding his e-fatbike offroad uphill with at least 20km/h, where they struggled with their mountainbikes with 6km/h. Must have consumed more than 250W during this time.
Maybe there is also a possibility to make a software based powercouter/averager in VESC?

@dude thanks for the link with the license plate story.
```

---
## \#34 Posted by: dude Posted at: 2016-09-03T10:11:05.945Z Reads: 187

```
Got an answer from the FlyKly company who made the Smart Ped. But until now the only information i've got is that in difference to e-skateboards they don't accelerate and that makes them legal. I asked pretty detailed but the answer was a bit short ;) Ok they have many target countries so they can not have everything ready. Will let you know when i get some more insight from them.
```

---
## \#35 Posted by: Chrisi-MUC Posted at: 2016-09-03T22:16:21.318Z Reads: 181

```
some additional information, which you may have read before:

Some information about vehicle classification in Germany/EU:
https://www.google.it/url?sa=t&source=web&rct=j&url=http://www.dekra.de/fileadmin/lokationdata/niederlassung_chemnitz/niederlassung_chemnitz/dokumente/2014-06-26_Verkehrssymposium_2014_Grohmann_v3.pdf&ved=0ahUKEwih5P7TnPPOAhVmOpoKHQgGBSAQFggbMAA&usg=AFQjCNFFcyA24QQ4Nb0AtHJu-XhHMonZ2Q

The more I read something about  it, a esk8 could slso be a "elektronische Mobilitaetshilfe", which is in the class of powered vehicles, but limited to only 20km/h...

https://www.gesetze-im-internet.de/mobhv/BJNR209710009.html

Maybe the ADAC (Automotive Club in Germany) legal department could also help with this topic:
https://www.google.it/url?sa=t&source=web&rct=j&url=https://www.adac.de/_mmm/pdf/fi_elektronische_mobilitaetshilfen_sp_0214_38557.pdf&ved=0ahUKEwjjt4-8h_TOAhWGBZoKHZINDh8QFggjMAQ&usg=AFQjCNHwlvJlvraz7Wns0pu3MJgQpuUuuw
```

---
## \#36 Posted by: dude Posted at: 2016-09-04T16:30:28.566Z Reads: 174

```
Did not get any more details from FlyKly. Their findings seem to result in the same like ours.

- not accelerating
- max 250W in average
- max. 25km/h

And if i understand them correctly ... they think that the maximum amount of time you are allowed to keep that speed is 500 sec.

I will not try to get more from them, they don't seem to have the time for this or they just didn't research this stuff in detail ... no idea ...
They also wrote they wanna get an official certification ... but who knows on what priority they have this and how long that could take ... so better not wait for anything there.
```

---
## \#37 Posted by: Maxid Posted at: 2016-09-04T17:40:13.468Z Reads: 172

```
500s is a seemingly very large number. That is 8min of cruising and should me more than enough for us. 

Seems like this could in fact be done - i'd be so happy if we could make this legal. Just telling that security guard at work that he can no longer prohibit me from riding would me an amazing feeling.
```

---
## \#38 Posted by: Ackmaniac Posted at: 2016-09-04T18:29:18.440Z Reads: 180

```
I came pretty far with the software. Feels quite good at the moment and i try to make the carving feel as natural possible. Only problem is that the rpm's differ alot when you carve.
Hopefully we can find out if this setup without acceleration is allowed.

Funny thing is that it makes even fun to ride that way. You get the feeling againof doing some sport because you have to push to the speed you want. And another positive side effect is that my average wh consumption of 10 Wh/km came down to around 5 Wh/km. 

And during testing with other settings i  found out that it is really relaxing to cruise with max 750 watt power.
```

---
## \#39 Posted by: Monte Posted at: 2016-09-04T18:40:37.691Z Reads: 191

```
Wäre es nicht einfacher nen 250w motor zu benutzen der einfach unterstützend ist? Also so das wenn man Voll gas gibt man trz. lansgamer wird. Einfach damit man länger ausrollt. (rpm und Amp einfach runterregeln das der motor nicht mehr kann als 25kmh)
Wenn man dann noch Cruise controll benutzt mit mit einem schalter der im board als druckplatte/trittschalter fungiert müsst das doch dem gesetz gerecht werden oder?
In meiner stadt gibt es ein Straßen verkehrsamt. Wenn ich da mal vorbei komme und zeit hab werd ich einfach mal reingehen und versuchen da mal nachzufragen ob das so legal ist bzw wie man das ganze legal machen kann.
```

---
## \#40 Posted by: Maxid Posted at: 2016-09-06T08:41:10.981Z Reads: 181

```
Is there anything we can do to help? I am really looking forward to this and can not wait to try it.
```

---
## \#41 Posted by: Ackmaniac Posted at: 2016-09-06T09:23:46.763Z Reads: 167

```
I will do some more testing this evening.
At the momenti am trying to figure out the efficiency of our motors. Because then i can add this to the calculation. Should mean that at a efficiency of 90%, 250 watts send to the motor would only be 225 watts on the shaft. So we can add 10% more power. But i can't find excact figures for my SK3 6374 - 192kv or Enertion 6355.
```

---
## \#42 Posted by: Maxid Posted at: 2016-09-06T09:31:01.820Z Reads: 161

```
I'd just go with the theoretical 250W since you will never be able to cover every available setup we have. Some have hub motors, some a tighter belt than others.
Did you see this: http://rideside.at/blog/2016/sind-e-scooter-fur-die-strase-zugelassen/
Apparently not even escooters are allowed on German streets?
```

---
## \#43 Posted by: Ackmaniac Posted at: 2016-09-06T09:37:35.986Z Reads: 170

```
I think there is no brushless motor which achieves more than 95% efficency. Maybe somebody has detailed number for our kind of motors. 

I also read that there is a scooter manufactor in Germany who created a commitee for a new law for light electric vehicles. 
https://www.my-egret.com/de/content/wo-darf-ich-meinen-egret-roller-fahren-32
Hopefully he can achieve something.
```

---
## \#44 Posted by: dude Posted at: 2016-09-06T10:02:56.359Z Reads: 169

```
@Maxid Yes in the default configuration only segways and e-bikes are allowed here ^^

@Ackmaniac You plan to limit the motor to 250W max or are u going for the in average on an typical trip thing? ... I think the average would be 250W on 0° climb ... so as an non universal approach (different for every board and person{weight / motor / voltage}) you could measure at what rpm your motor uses 250W and limit the rpm, this would also solve your rpm problem? Yes thats no solution for your efficiency question ... i have no idea what difference 5% make and if the 5% more make sense on a 25km/h limit.
```

---
## \#45 Posted by: Ackmaniac Posted at: 2016-09-07T10:45:28.244Z Reads: 167

```
I calculate with a efficiency of 90% for now. Means 250 Watt / 0,9 eficiency = 277,77 Watt. And you really can feel the difference when you go up a hill between 277 and 250.

Problems i have at the moment is the duty cycle control of the speed in the BLDC mode. In FOC the speed mode is current control.
I tried to soften it already but i am not happy with the result. Because it feels good when you drive in a staight line. But when you carve it brakes and gives power all the time which doesn't feel good. I softened that already but it is still not perfect.
So i will try to change the BLDC control of the speed to current control instead of duty cycle.
But not sure if i can achieve the results i want.
```

---
## \#46 Posted by: austin54 Posted at: 2016-09-07T16:18:15.521Z Reads: 165

```
Beside the technical issues I would like to come back to the legal part.

I think none of us has the legal background, which is needed to get this clarified. If it would be only a technical issue, we would already have several commercial boards available which are be compliant to EU laws.

So I suggest to collect money to fund professional consulting from a lawyer so that the community knows exactly what we need to do to leaglise our boards. This could speed up the process. If we just wait until our politicians do something we will wait forever. 

We don"t have a lobby in Germany. But with money we could change this. 

Currently I don"t know how we could organise this. Also I don"t know a consulting company which could guide us through the law jungle and do the lobby work.
```

---
## \#48 Posted by: dude Posted at: 2016-09-07T16:56:49.639Z Reads: 163

```
Successful lobbying is $$$$$$ ... nothing for individuals :D :'(

I think we researched what we could (without prof. help). Let's keep the illusion that our interpretation of the law is correct ;) I expect it's enough to convince the critical policemen that it's likely legal.

You can buy boards in germany ... they just won't tell you that they are not legal on public roads and the normal buyer will not research if it is ... so maybe the problem for the manufacturers is not big enough to make compliant editions for problematic countries. So that there are no legal ones must not mean that it is not legally possible.
```

---
## \#49 Posted by: Ackmaniac Posted at: 2016-09-07T18:30:36.022Z Reads: 162

```
I managed to get the current control in BLDC mode running for speed control. And i can tell you that it is so smooth. So much better than duty cycle. Sometimes you can't tell if the motor assists or your costing. Only the android app that i wrote to see the live statistics tells me the truth.
After some more testing I need to tell vedder about that. Can't imagine a reason why this shouldn't be adopted for speed control in BLDC. And in current control it is very easy to switch off the power of the motor and coast when you go slightly faster than the speed control allows. Because i don't want breaking when I carve.

BTW, as i wrote earlier, a company tries already to change the law for light electric vehicles in the EU. And they hope to have a result by the end of the year. They also replied to a mail i wrote them and told that it is still in progress and that they are optimistic.
https://www.my-egret.com/de/content/wo-darf-ich-meinen-egret-roller-fahren-32
```

---
## \#50 Posted by: kampfhahn Posted at: 2016-09-08T06:32:54.675Z Reads: 151

```
Related: http://www.zeit.de/hamburg/politik-wirtschaft/2015-08/faltbare-elektro-roller-markteinfuehrung-hamburg-buerokratie-huerden

I hope that this workgroup in brussels doesn´t only fight for their scooters to be classified als "PLEVs" but electric vehicles of any kind (electric skateboards, hoverboards (hate them btw), scooters...)
```

---
## \#51 Posted by: Chrisi-MUC Posted at: 2016-09-08T20:05:34.085Z Reads: 171

```
This is the link to the DIN working group: http://www.din.de/de/mitwirken/normenausschuesse/nasport/europaeische-gremien/wdc-grem:din21:191006031

A preview of the DIN could be available here (when released for public): http://www.din.de/de/mitwirken/normenausschuesse/nasport/entwuerfe/74966!search-na?state=H4sIAAAAAAAAAE2LsQrCMBRFf0XunKGu2SqKuEhBncThNXlGMTX6XjKU0n83S8Htnns4E6hPBw_7LjEaUNFAPW8pl2H5fHod5Q_O44cXvJPjrLDTbPB4Zu1YOgpVrxuDb2EZYQEDKZGV85JpkrqvaC-nfbvZrTyrw80gCA_KkV21zfwDYnqN6ZwAAAA&pageNum=0

specific DIN project site (did someone already link this?)
http://www.din.de/de/mitwirken/normenausschuesse/nasport/projekte/wdc-proj:din21:191486964
Maybe the specific DIN contact person could give some information.

First I was bit irritated about "nicht für den öffentlichen Straßenverkehr..." but the specific DIN project is for "Nicht-Typ zugelassene leicht motorisierte Fahrzeuge für den Transport von Personen und Gütern und damit verbundene Einrichtungen - Persönliche leichte Elektrofahrzeuge (PLEV) - Sicherheitstechnische Anforderungen und Prüfverfahren". - sounds good. but limeted to 25km/h.
```

---
## \#52 Posted by: maddash1337 Posted at: 2016-09-10T16:22:26.239Z Reads: 176

```
Hey there I guess you read a lot about the law. 
What would happen if I build an eboard limited to 4 or 6 km/h? Would it be street legal? Because there are also those kid cars with e motor ....
```

---
## \#53 Posted by: austin54 Posted at: 2016-09-22T20:41:47.386Z Reads: 149

```
Any news regarding your project?

I would be interested in your BLCD settings. Could you share them with us?

I would be also interested in which remote control you use? I tested a wireless Nunchuck with cruise control, but had problems with outages. Currently I have  a nano remote 2,4ghz, but no cruise control.
```

---
## \#54 Posted by: E-Boarding Posted at: 2016-09-24T06:46:12.488Z Reads: 146

```
A board limited to 6km would be legal, it doesn't count as KFZ.

I would also be interested in the firmware and would like to try this.
```

---
## \#55 Posted by: Ackmaniac Posted at: 2016-09-24T09:33:34.364Z Reads: 144

```
I will create a firmware and vesc-tool mod once Vesc-tool (new Bldc-tool)  is out.
The problem is that it seems that even with that modification it is not allowed. If you reduce the max speed to 6 km/h than it could be allowed. Better than nothing. At least you have breaks. (to have a reason why you have motors) 

And you can cheat by changing the mode by some other device and every time you switch the board off on it is back to 6 km/h.

I hope that the guys from the scooter company can achieve law changes till next summer.

BTW: would it be allowed to have a board which provides multiple modes as long as you run it on the streets in the legal mode? Than that would be the solution.
```

---
## \#56 Posted by: DeathCookies Posted at: 2016-09-24T10:10:03.804Z Reads: 139

```
You cannot make a legal Skateboard that **could** ride more than 6km/h and **limit** the speed to 6km/h. This is because you could probably drive faster and no one can Control it. Just when the Skateboard it self cannot drive faster than 6km/h (mechanical not Software limit) it would be allowed. Thats how it is! E. G. You could reduce the voltage / Gear ratio that it can only drive max 6kmh.
```

---
## \#57 Posted by: E-Boarding Posted at: 2016-09-24T10:32:31.560Z Reads: 140

```
[quote="Ackmaniac, post:55, topic:8759"]
The problem is that it seems that even with that modification it is not allowed.
[/quote]

why?
Up 6km/h with motor only and up to 25km when you push to accelerate should be ok. I would like to try that and test how the police react.
```

---
## \#58 Posted by: TarzanHBK Posted at: 2016-09-24T12:26:26.480Z Reads: 150

```
my experience here at the wonderful Saarland (South West Germany if you don´t know - study some maps..Jesus..:monkey:):

-rushing at the bike path with about 32km/h next to a main street, two policemen saw me and one like hit the other and was like "dude, look at that!!" - i just kept going and nothing else happend :smiley:

-the other time was down a pedestrial/bike way down at the Saar (our local beautiful river - you still didn´t look at a map, don´t you?), a police woman stopped my friend on my board and was like: 
"no you can´t drive that here, how fast does that go?" -hmm about 20km/h?! 
"that´s too fast, you can´t drive that without a moped license! so get off!"
and he had to grab it and walk a few blocs away from that strage ladywithoutaplan :smiley:
```

---
## \#59 Posted by: kampfhahn Posted at: 2016-09-24T14:36:24.813Z Reads: 147

```
Interesting. Moped (A1) license for a 4-wheel vehicle :slight_smile:  I´m sure that was her first incident with an esk8 so far.
```

---
## \#60 Posted by: TarzanHBK Posted at: 2016-09-26T08:16:29.121Z Reads: 145

```
seemed so, she was like "better i say something stupid then say nothing and blaming myself"
:monkey:
```

---
## \#61 Posted by: SirDiff Posted at: 2016-09-26T19:16:54.373Z Reads: 143

```
I don't know if this can help in any way, but i was checking how's the esk8 situation in Italy, and found some interesting things. 1st: normal skateboards seem to be legal in private zones only, not even bike lanes. The same goes for roller skates and non motorized scooters. 
2nd: bikes can go up to 25 km/h with a motor helping you, as expected
3rd, the most interesting: Segway somehow managed to get a law just for themselves: you can use those up to 6km/h on sidewalks and 20 km/h on bike lanes, that's because they don't need a push (so they are not "gait accelerators", that's the word they use, i think) and they're not a bike or a moped. So, there's officially nothing different between a segway and an esk8, since they don't seem to count the number of wheels to define the type of vehicle.
```

---
## \#62 Posted by: E-Boarding Posted at: 2016-09-26T19:25:06.535Z Reads: 140

```
In germany there is an exact definition what a segway is and this doesn't fit skateboards :frowning: 

1.   zweispuriges Kraftfahrzeug mit zwei parallel angeordneten Rädern mit integrierter elektronischer Balance-,Antriebs-, Lenk- und Verzögerungstechnik,
2.   eine Gesamtbreite von nicht mehr als 0,7 m,
3.   eine Plattform als Standfläche für einen Fahrer,
4.   eine lenkerähnliche Haltestange, über die der Fahrer durch Schwerpunktverlagerung die Beschleunigungoder Abbremsung sowie die Lenkung beeinflusst,
5.   entspricht den Anforderungen der Richtlinie 72/245/EWG des Rates vom 20. Juni 1972 zur Angleichungder Rechtsvorschriften der Mitgliedstaaten über von Fahrzeugen verursachte Funkstörungen(elektromagnetische Verträglichkeit) (ABl. L 152 vom 6.7.1972, S. 15), die zuletzt durch die Richtlinie2006/96/EG (ABl. L 363 vom 20.12.2006, S. 81) geändert worden ist, in der jeweils geltenden Fassung,
6.   eine Anzeige für den Energievorrat.
```

---
## \#63 Posted by: SirDiff Posted at: 2016-09-26T19:32:35.200Z Reads: 144

```
In Italy (i'm not surprised, that's how they do things down here :unamused: ) they had to specify on segway's site why that's even legal, writing this "Il Ministero chiarisce, inoltre, che Segway PT non rientra tra gli acceleratori di andatura di cui ai commi 8 e 9 dell’art. 190 del CdS in quanto trattasi di mezzo non funzionante a propulsione esclusivamente muscolare.
", so they don't write a definition, just "they are not something you can't use". I'm building my first esk8, if they stop me and ask questions, I'm just gonna tell them about this segway thing, they don't even know esk8s exist here
```

---
## \#64 Posted by: elkick Posted at: 2016-10-07T11:42:37.379Z Reads: 147

```
Seems we are getting support from Federal Council. It requests the German Government to legalize electric mobility vehicles within German law (page 3 and 4):

http://www.bundesrat.de/SharedDocs/drucksachen/2016/0301-0400/332-16(B).pdf?__blob=publicationFile&v=1

Whatever they will do for restrictions (they are quite good at those!), at least it's moving into the right direction.
```

---
## \#65 Posted by: Ackmaniac Posted at: 2016-10-07T12:08:22.667Z Reads: 149

```
Seems that they will decide something soon. But who knows what "asap" means for politicians.
But lets pray that they give us a possibility to drive our boards legally.

> Vor diesem Hintergrund wird eine Regelung durch den
> Verordnungsgeber schnellstmöglich für erforderlich und umsetzbar erachtet,
> auch um zu verhindern, dass immer mehr nicht zugelassene Kraftfahrzeuge
> sowohl auf Fuß- und Radwegen als auch auf Straßen unterwegs sind
```

---
## \#66 Posted by: dude Posted at: 2016-10-07T12:14:10.872Z Reads: 144

```
niiiice! and it seems as they don't see this vehicles as a problem that must be regulated. they see it as useful stuff that should be legalized. let's hope the resulting laws are not only for the big players but also for us diy guys.
```

---
## \#67 Posted by: Maxid Posted at: 2016-10-07T12:38:09.711Z Reads: 145

```
I just don't like the "beziehungsweise sogar 35 km/h" - that sounds like they don't like the speeds these things are capable of. I don't see how they will allow a 40-50km/h board to be legal.
```

---
## \#68 Posted by: dude Posted at: 2016-10-07T12:55:58.602Z Reads: 146

```
i would expect that the limit is 25km/h ... for me that would be ok. for everything above i would prefer some sort of age restriction and insurance. think about many stupid kids with 50km/h e-boards ;) not funny ^^ and many vehicles are just not safe at those speeds ... for example a hoverboard with 25km/h would be stupid.
```

---
## \#69 Posted by: TarzanHBK Posted at: 2016-10-10T10:39:35.970Z Reads: 145

```
these are some great news! i´d love to tell my grandchildren later that i wasn´t able to drive legal in the streets, but then the huge community changed something :slight_smile:
```

---
## \#70 Posted by: maddash1337 Posted at: 2016-10-16T16:10:29.332Z Reads: 138

```
@Ackmaniac thank you for this infromation - please keep us updated.
I would love to hear it becomes legal - even if the speed limit is 25km/h.
```

---
## \#71 Posted by: azevedo Posted at: 2016-10-19T18:31:12.628Z Reads: 144

```
Hello 

My first post. I'm from Portugal and here it seems we have a 250 W limit to e-bikes, because esk8 are rarity there is no information available.

I am investing time and money on this subject so I will ask for a definitive answer from my lawyer.

Would be great to have a way to comply esk8 with the law.

Keep doing this research.

TY
```

---
## \#72 Posted by: Chrisi-MUC Posted at: 2016-10-22T17:06:30.995Z Reads: 146

```
I really really really really really like it
```

---
## \#73 Posted by: Wubbalubbadubdub Posted at: 2017-03-15T20:16:15.897Z Reads: 134

```
I live in Sindelfingen and work in Boblingen (suburbs of Stuttgart in Baden Wurttemburg). I have a two hub motor setup, only one of which is currently working. When I get the second motor working, I plan to use it to go to/from work when the weather is nice. 

Have there been any developments regarding the legalization issue or the BLDC tool workaround? I plan on using my esk8 within the restrictions imposed by german law (at least when I am visible on the sidewalk and not on the bike trail away from police. If I buy ackmaniac's tool and use the android app, can I use it to set my board to within acceptable limits? If I am stopped during my usual commute there really is no way for the polizei to know my board's capabilities, and so if they see me abiding by the law the there is no reason for them to investigate further.
```

---
## \#74 Posted by: kampfhahn Posted at: 2017-03-15T22:22:50.883Z Reads: 135

```
Don´t know if you can temporarily or permanently change the topspeed-affecting values like "Max ERPM" with @Ackmaniac s app but i´m pretty sure that taking out your smartphone right before you stop for a police check would make the cops very suspicious.

Greetings from the Ländle
```

---
## \#75 Posted by: Ackmaniac Posted at: 2017-03-15T22:37:59.244Z Reads: 136

```
Yes you can limit the top speed. And you can select a new mode with the app which doesn't get stored on the VESC. So next time you switch off the board and switch it back on it is in the standard mode.
Just think about it :stuck_out_tongue_winking_eye:
```

---
## \#76 Posted by: Wubbalubbadubdub Posted at: 2017-03-16T17:48:05.858Z Reads: 127

```
I dont think i will ever be pulled over on the bike lane I plan in going down, because it is well off the road.I still don't plan on going terribky fast up or down it.

 I want to use the app to make the board act legally for the portion of my ride that I will be on a sidewalk. That way I dont have to watch my speed or look out for polizei because I know the board will only go so fast. I need to get a speedometer as well I suppose.
```

---
## \#77 Posted by: Wubbalubbadubdub Posted at: 2017-03-16T17:49:37.833Z Reads: 133

```
Ok so the only issue I can see is that I have two VESCs for two motors. Do I just order two bluetooth receivers? How does that work?
```

---
## \#78 Posted by: Ackmaniac Posted at: 2017-03-16T18:05:14.506Z Reads: 133

```
With my firmware the master updates all slaves in the system automatically. But only by the app. Not by the BLDC-tool
```

---
## \#79 Posted by: E-Boarding Posted at: 2017-03-16T19:46:23.668Z Reads: 134

```
I've done the same, it works well with dual setup.
My VESC is limited to 6 km/h but when the police stops you riding like 20 km/h, good luck telling them the max speed was 6 km/h :expressionless:
```

---
## \#80 Posted by: Ackmaniac Posted at: 2017-03-16T19:52:08.999Z Reads: 137

```
When you limit it to 6 km/h i also would set the motor max and battery max really low. Just tell them you use the motors for braking and that they are too weak to move a human faster. I guess the average police man doesn't know that much about brushless motors.
And if they test it they can't proof you wrong.
```

---
## \#81 Posted by: Wubbalubbadubdub Posted at: 2017-03-16T19:57:40.373Z Reads: 139

```
that is exactly what i thought! Unless they demand I open it up or know the specs, then there is no way to tell
```

---
## \#82 Posted by: Witya Posted at: 2017-08-03T19:25:56.901Z Reads: 117

```
Sorry for necroposting, but shouldn't EU Law also apply to Germany, if there is no applicable german one?
EU Law, specifically "Durchführungsverordnung (EU) 2015/386 der Kommission vom 5. März 2015", states that "electric skateboards are not Kraftfahrzeuge"
Link:
http://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX%3A32015R0386
```

---
## \#83 Posted by: Ackmaniac Posted at: 2017-08-03T19:32:50.273Z Reads: 119

```
But what does this mean for us then?
```

---
## \#84 Posted by: Witya Posted at: 2017-08-03T19:50:40.865Z Reads: 124

```
I assume it means police cannot give us criminal charges for "driving without insurance" or any other nonsence.
I am still waiting for a reply from insurance and lawyer.

I believe this EU law triggered this Bundesrat topic:
http://www.bundesrat.de/SharedDocs/drucksachen/2016/0301-0400/332-16(B).pdf?__blob=publicationFile&v=1

but it might take 10 years for these robots to actually do somehting...
```

---
## \#85 Posted by: Achmed20 Posted at: 2017-08-03T20:24:01.639Z Reads: 129

```
[quote="Ackmaniac, post:80, topic:8759, full:true"]
When you limit it to 6 km/h i also would set the motor max and battery max really low. Just tell them you use the motors for braking and that they are too weak to move a human faster. I guess the average police man doesn't know that much about brushless motors.
And if they test it they can't proof you wrong.
[/quote]
i doubt thats going to work. they probably just confiscate your board since there is no E number or similar certificate on it. 

[quote="Witya, post:84, topic:8759"]
I assume it means police cannot give us criminal charges for "driving without insurance" or any other nonsence.
[/quote]looks more like a import/buying regulation[quote]
but it might take 10 years for these robots to actually do somehting...
[/quote]
it took segways about 3-4 years to be legalized here. but they had segway behind it. so yeah ... 10 years might be right
```

---
## \#86 Posted by: BelviGER Posted at: 2017-08-31T13:43:24.942Z Reads: 119

```
Just fyi, due to the limited track width of less than 460mm, electric longboards count as two wheeled, two axle vehicles.
So Segway laws do not apply, E-Bike laws apply
```

---
## \#87 Posted by: Maxid Posted at: 2017-09-01T06:24:04.114Z Reads: 111

```
You mean motorcycle laws apply - that is why people get charged for not having the right driver's license.
```

---
## \#88 Posted by: BelviGER Posted at: 2017-09-05T09:43:10.427Z Reads: 109

```
That depends.
If the board is slower than 45kph and 50ccm, it's a scooter (Roller), below 25 it becomes a Moped (Mofa), so anybody who has a car license should be safe.
```

---
## \#89 Posted by: Maxid Posted at: 2017-09-05T10:25:50.505Z Reads: 112

```
Unfortunately no - if i remember the news articles correctly people get charged for not having a motor cycle license
```

---
## \#90 Posted by: Wubbalubbadubdub Posted at: 2017-10-14T18:53:03.626Z Reads: 103

```
About three weeks ago I found myself with not enough time to taxi from the place I'm staying to downtown Stuttgart in order to meet a buddy here for a limited time for drinks. I decided to grab the esk8 and threw all caution to the wind. I even didn't wear any safety gear, which is very unlike me. 

I didn't think anything of it until I found myself ripping past the front of the city polizei station at about 25mph in the bike lane. I let off the throttle and got real low on the deck to make a smaller profile. It was funny, it was dumb, and I guess I'm lucky there weren't any cops out front paying attention that night. Anyways it made me think of this thread.
```

---
## \#91 Posted by: TarzanHBK Posted at: 2017-11-07T10:44:32.084Z Reads: 95

```
I had two conversions about my street board with the Polizei Saarbrücken.
Both were interested in the board and told me everything is fine, i should use the bike lane, don´t go faster than bikes and wear a helmet. They also appreciated the lights :slight_smile:
I guess it´s a bit easier in a rural area like mine and i will still riding regularly and spreading the word ;)
```

---
## \#92 Posted by: HifuSk8 Posted at: 2017-11-07T13:44:02.278Z Reads: 98

```
Here in Bern Switzerland I got stopped twice by the Police. 

One Time they just told me that they appreciate me wearing Helmet and Lights but that I cant ride in the Street/Bikelane because Skateboards are not allowed to. I then told them its motorized and that I know that I shouldnt drive it on public Roads. Then they replied to me that Yes in Fact it's illegal to so as I do but that they can't take it away from me. I then smiled and thanked for the Chat and drove off.

The other Time the Guys were just curious about that Thing that just flew uphill and were more impressed by the Fact I built it myself than concerned about the legal Status. 

So I guess most of the Time it depends on all circumstances like what you do, where, your safety-measures and the individual Cop wich stops you.
```

---
## \#93 Posted by: hornet90 Posted at: 2017-12-26T08:35:10.189Z Reads: 88

```
Hi every one that worked so hard on this.I live in Ireland and I'm going to put time into making a legal street board so I'm thinking it needs to work like a ebike if any one in Europe have made a legal street board I would like to fly and meet up.
```

---
