# Meepo 12s2p upgrade issues

### Replies: 53 Views: 1145

## \#1 Posted by: Skyart15 Posted at: 2019-03-17T03:10:42.589Z Reads: 163

```
Hello! I am wondering if someone can help me. I have a Meepo V2p board and i bought a 12s2p battery from torque boards. But after installation the board turns on but thats it. The transmitter turns on and it seems to pair, but does not do anything when i oush or pull of the scroll wheel. I am wondering if i am missing something or if the ESC is programmed a certain way that does not allow it to send 12s voltage to the motors. Any helo would be much appriciated![20190316_195037|375x500](upload://x5o7DxkqN0LVGZKzYWKZpqBLDWO.jpeg)
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-03-17T03:11:42.728Z Reads: 153

```
I don't think the meepo controller can do 12s. I think you killed it lol
```

---
## \#3 Posted by: Skyart15 Posted at: 2019-03-17T03:12:35.730Z Reads: 154

```
No after i plugged the old battery back in, it works fine.
```

---
## \#4 Posted by: BillGordon Posted at: 2019-03-17T03:23:04.913Z Reads: 151

```
Meepo ESC not suited for 12s. Suggest you get a 6.6 dual, Unity, or a pair of Focbox.
```

---
## \#5 Posted by: Skyart15 Posted at: 2019-03-17T03:27:24.912Z Reads: 148

```
Thanks. Reason im confused is because others have done this mod and it workes fine.
```

---
## \#6 Posted by: dtaoo Posted at: 2019-03-17T03:41:11.690Z Reads: 146

```
ESC could only run 10s, 7s, and 6s. Gotta get a VESC
```

---
## \#7 Posted by: Wilsonliang777 Posted at: 2019-03-17T03:44:13.489Z Reads: 143

```
I think ppl that did the 12s upgrade did it with the old meepo esc.    I might be wrong.   The eac you have is the v2 eac that came with an enclosure.
```

---
## \#8 Posted by: Skyart15 Posted at: 2019-03-17T03:53:45.631Z Reads: 140

```
Yes, its the ESC that came with the enclosure. And yeah i just realized the people that did this swap did it with the old ESC. Just ordered a flipsky dual 4.20 VESC
```

---
## \#9 Posted by: M.Hboards Posted at: 2019-03-17T03:57:21.384Z Reads: 135

```
Sorry to be the breaker of bad news but the flipsky 4.20 dual are known not to be reliable at 12s also your going to need a remote with a reciver to use with a vesc.
```

---
## \#10 Posted by: Skyart15 Posted at: 2019-03-17T03:59:33.245Z Reads: 129

```
Oh?! Lol i cancel the order. What would you guys recomend?
```

---
## \#11 Posted by: M.Hboards Posted at: 2019-03-17T04:02:05.468Z Reads: 129

```
Focbox Unity or flipsky 6.6. i would recommend a unity in your case  as it has an antispark built in. Or u can wait for the flipsky dual 4.20 plus to come back in stock as it is much more reliable at 12s and has a built in antispark.
```

---
## \#12 Posted by: Wilsonliang777 Posted at: 2019-03-17T04:30:50.447Z Reads: 120

```
It's no longer a simple battery upgrade anymore.  Battery, vesc and remote why not change hub motors to regular out runner belt gear system while you at it.
```

---
## \#13 Posted by: Skyart15 Posted at: 2019-03-17T04:32:51.182Z Reads: 117

```
Yeah i might as well at this point lol!
```

---
## \#14 Posted by: Wilsonliang777 Posted at: 2019-03-17T04:38:12.574Z Reads: 119

```
If you are looking for a remote.  I just designed to and built a very dependable rc remote with built in LED light.   I am taking orders now.   ![IMG_20190315_215055|375x500](upload://q1d9GmTfQkJdUfjioG1C4je5GGT.jpeg)
```

---
## \#15 Posted by: sayekim Posted at: 2019-03-17T11:37:10.577Z Reads: 108

```
Is the battery fully charged? You might have some luck draining the battery to less than 50v. 

Otherwise get the unity or two focboxes and antispark and build a loop key in there too.
```

---
## \#16 Posted by: Skyart15 Posted at: 2019-03-17T15:01:31.374Z Reads: 100

```
What do you think if i get the flipsky 6.6 dual?
```

---
## \#17 Posted by: sayekim Posted at: 2019-03-17T15:06:44.925Z Reads: 99

```
I haven’t tried it myself but others have had success with it. Same goes for the 4.12 single. 

I tried the 4.20 dual and that’s a no go if you want to pull anything more than 29amps on foc.
```

---
## \#18 Posted by: Skyart15 Posted at: 2019-03-17T15:07:37.014Z Reads: 100

```
Awesome! Thanks man! Ill make a post about how it turns out.
```

---
## \#19 Posted by: KaramQ Posted at: 2019-03-17T15:31:44.159Z Reads: 98

```
Hey, just buy a dual fsesc
```

---
## \#20 Posted by: Skyart15 Posted at: 2019-03-17T20:08:26.294Z Reads: 89

```
This is what i got and i got their transmitter and reciever ![Screenshot_20190317-084721_Samsung%20Internet|243x500](upload://nvP1A7z2jnoohRMzUFiLa03QVN.jpeg)
```

---
## \#21 Posted by: KaramQ Posted at: 2019-03-17T20:12:55.392Z Reads: 82

```
Great, all you need to do is just some soldering and you’ll have a full working board, remember to configure it with the vesc tool
```

---
## \#22 Posted by: Skyart15 Posted at: 2019-03-17T20:16:56.954Z Reads: 82

```
Soldering? I dont own a soldering kit, is there some sort of crimp on connections i can buy?
```

---
## \#23 Posted by: Skunk Posted at: 2019-03-17T20:20:44.477Z Reads: 85

```
You should just buy one and learn. It's kinda 101 of board upkeep  .
You'll eventually need to.  Or you'll have to find help every time somthing comes up that could take you minutes to fix yourself.

Also i wouldn't trust crimp on Connectors with the vibrations our boards go through.
```

---
## \#24 Posted by: KaramQ Posted at: 2019-03-17T20:30:49.667Z Reads: 80

```
Soldering is key in esk8, it’s pretty easy but you can get hurt real easily if your not cautious. I would recommend getting one off amazon, it’s like 20$. Also simply go on YouTube and you’ll find thousands of videos on how to solder. Good luck
```

---
## \#25 Posted by: Skyart15 Posted at: 2019-03-17T21:03:57.799Z Reads: 77

```
Thanks guys, is there a good place to purchase the various connectors and soldering things i need? For example what will i need to get in order to connect my motors to the Vesc i ordered. I beliave the motor leads are #14 wires maaaybe #16 and the vesc likely comes with #12 motor wires. Also there are sensor wires coming off my motors, i didnt check this ahead of time but does the flipsky dual fsesc have a spot for those to land on? If so will i need diffrent connectros? Or will the meepo stock ones that are one there work ok. Thanks for all your help.
```

---
## \#26 Posted by: M.Hboards Posted at: 2019-03-17T21:32:57.438Z Reads: 70

```
Your also going to need a anti spark switch i would recommend one from here
http://sprusi.com/index.php
```

---
## \#27 Posted by: Skyart15 Posted at: 2019-03-17T21:38:44.540Z Reads: 68

```
What exactly is an anti spark and what does it do?
```

---
## \#28 Posted by: M.Hboards Posted at: 2019-03-17T21:41:04.920Z Reads: 66

```
The meepo esc has one built in but in short it is a high voltage switch that turns on and off your board.
```

---
## \#29 Posted by: Skyart15 Posted at: 2019-03-17T21:44:43.583Z Reads: 66

```
Gotcha and if i dont have this i will have to disassemble my board everytime i want to turn it on and off.. i see.
```

---
## \#30 Posted by: Sn4pz Posted at: 2019-03-17T21:45:30.032Z Reads: 63

```
There are alternatives to an antisparks: loop keys, but I won't tell you what that is. You'll have to search for it :)
```

---
## \#31 Posted by: Skyart15 Posted at: 2019-03-17T21:46:50.569Z Reads: 58

```
Ive seen these, just look like xt style connectors. I think this is what i will try to get. Easy available on amazon prime
```

---
## \#32 Posted by: Mich21050 Posted at: 2019-03-17T21:48:04.912Z Reads: 58

```
@Andy87 can explain that for sure.. :slight_smile:
```

---
## \#33 Posted by: Sn4pz Posted at: 2019-03-17T21:50:53.830Z Reads: 60

```
The wiring is the cruicial part, and I'll give you a hint, as I don't want you to burn your house or board down... Don't bother with the regular xt90 for the plug in bit of the loopkey. You'll need the xt90s, Amass is a favorite manufacturer for legitimate ones.
```

---
## \#34 Posted by: Skyart15 Posted at: 2019-03-17T21:55:54.958Z Reads: 64

```
What about this? ![Screenshot_20190317-145505_Amazon%20Shopping|243x500](upload://ltdIs5OZFnzXuasdhXwOAHF1V6W.jpeg)
```

---
## \#35 Posted by: Mich21050 Posted at: 2019-03-17T21:56:21.659Z Reads: 59

```
https://www.electric-skateboard.builders/search?expanded=true
```

---
## \#36 Posted by: Sn4pz Posted at: 2019-03-17T21:59:23.289Z Reads: 57

```
This is indeed an antispark. 

Please use the search function like Mich provided. I've got unlimited time, but my poor young thumbs just can't type all day.... 


Or can they ;)
```

---
## \#38 Posted by: Skyart15 Posted at: 2019-03-17T22:01:46.044Z Reads: 54

```
You guys are great! Thanks! I will use the search as much as i can.
```

---
## \#39 Posted by: Sn4pz Posted at: 2019-03-17T22:02:16.210Z Reads: 59

```
Also, if it's not associated with @torqueboards / Dexter, and it has a DIYE / @diyeboard in the seller name, stay the fuck away 😂😂

Once upon a Time ago, a name named Jason Volan (if that's his real name :roll_eyes:) was a giant piece of shit and leaked critical customer information into the public, as well as selling parts that fail as frequently as a trucker curses. 

Stay away. stay smart.
```

---
## \#40 Posted by: Sn4pz Posted at: 2019-03-17T22:02:54.208Z Reads: 59

```
Sorry man 😭😭♥️♥️♥️
```

---
## \#41 Posted by: Mich21050 Posted at: 2019-03-17T22:03:39.035Z Reads: 59

```
All good... :smile: :smile:
```

---
## \#42 Posted by: M.Hboards Posted at: 2019-03-17T22:13:03.179Z Reads: 55

```
I wouldn't recommend that one and flipsky ones i have linked a good source for one above.
```

---
## \#43 Posted by: Meeep Posted at: 2019-03-17T23:53:44.876Z Reads: 52

```
I know you are already getting a VESC of sorts but the V2 meepo ESC has a high voltage cutoff of 48volts.

The original V1 ESC could do 12s but is locked at 22mph but you would have very little sag compared to 10s. I use 11s on the V2 ESC.
```

---
## \#44 Posted by: Sn4pz Posted at: 2019-03-18T00:38:30.984Z Reads: 51

```
Is it worth the upgrade? Or is it just a little extra pep in it's step

Karam I wasnt trying to shade you I promise 😂😭😭I just saw the post you liked
```

---
## \#45 Posted by: KaramQ Posted at: 2019-03-18T00:44:24.703Z Reads: 50

```
II would have just sticked to the Sanyo battery meepo has to offer. It doesn’t seem like your ready to build and mod this board. I’m not saying you can’t but it is a huge upgrade that will take some time to do. Here’s a list of what you really need to do this upgrade:

Loop key, preferably xt90, as @Sn4pz said, or a antispark switch as @Mich21050 mentioned, definitively not a diye board one 

Knowledge on soldering, and buy a soldering kit off amazon

Fsesc 6.6, which you already have in possession 

Bullet connectors, preferably 5.5mm male and female 6x

Don’t forget a remote, buy the mini remote that you can find on amazon, @torqueboards sells it 

That’s about it, but you really have to do some thorough research on here to be able to do this.
```

---
## \#46 Posted by: KaramQ Posted at: 2019-03-18T00:47:22.308Z Reads: 49

```
Hahah, don’t worry about it, I take full responsibility of it
```

---
## \#47 Posted by: tkc Posted at: 2019-03-18T03:06:44.460Z Reads: 46

```
Problem solved:
https://youtu.be/I7PD2yKegH8
```

---
## \#48 Posted by: Skyart15 Posted at: 2019-03-18T04:36:40.350Z Reads: 41

```
So i came up with this temporary fix for my meepo range problems. I had a soare meepo battery laying around and a battery from a one wheel. Hooked em up in parralel. Works great! Untill i get the rest of the parts i ordered this will have to do. Also regarding the video posted here. I checked the voltage on my battery it was like 47.8 i dont know...il try again and see what happens. But in case anyone is still reading this i have a question about charging. So![15528837580916450849466084764665|375x500](upload://9QefrseulEhfnNloCJHH5hVIn1h.jpeg)  my two meepo batteries have charge leads that hook up to my meepo charger...however the one wheel battety does not. Since i have them hooked up in parralel...will all 3 of my batteties charge sumultaniusly? And just take longer? Or am i playing with fire here?
```

---
## \#49 Posted by: Skyart15 Posted at: 2019-03-18T04:37:51.692Z Reads: 39

```
Also many thanks yo everyone who has posted here...i cant express my appriciation enough for all your help!
```

---
## \#50 Posted by: Meeep Posted at: 2019-03-18T04:50:33.574Z Reads: 37

```
Probably feels closer to a extra pep in it's step :smile: I like to cruise in the 24-26 mph range so it's worth it for my needs. I wonder what my top speed will be when I switch to the Unity and 100mm hubs :thinking:
```

---
## \#51 Posted by: Skyart15 Posted at: 2019-03-18T04:52:55.638Z Reads: 38

```
Are you running yours on 12s?
```

---
## \#52 Posted by: KaramQ Posted at: 2019-03-18T04:59:10.360Z Reads: 38

```
What’s holding everything together, a sheet of plexiglass?
```

---
## \#53 Posted by: Meeep Posted at: 2019-03-18T05:17:00.746Z Reads: 40

```
Not until my current 11s3p pack dies.
```

---
## \#54 Posted by: Skyart15 Posted at: 2019-03-18T06:32:49.048Z Reads: 37

```
Basicly, not sure exactly what kind of plastic but someyhing like that. Pretty cheap at home depot.
```

---
