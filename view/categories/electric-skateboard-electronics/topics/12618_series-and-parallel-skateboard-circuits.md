# Series and Parallel Skateboard Circuits

### Replies: 123 Views: 7197

## \#1 Posted by: Esrapp21 Posted at: 2016-11-07T03:17:30.893Z Reads: 331

```
<img src="/uploads/db1493/original/3X/1/5/1524f49af25ed6cf25e9f954e24de45eeb501355.PNG" width="690" height="472">
This is my circuit design. I'm sorry that it isn't in the schematic format, this was just easier for me to read. If you can't tell what is happening: all of the wires from the batteries are being put into reverse Parallel connectors, splitting it into 4 positive wires and 4 grounds. 2 positives and 2 grounds are being hooked up to a series circuit that powers the VESC, while the others connect to a Parallel connector, which connects the 2 positives together and the 2 negatives. The balance ports for each Battery are connected via a parallel balance board, then are fed to right next to the charging port so I can keep all the batteries in an enclosure with port holes. 
I would love any critiques that could make this efficient or stop it from blowing up if I did something VERY wrong! I hope that once this is finalized it would be a great starting point for other first time electric skateboard builders.
```

---
## \#2 Posted by: DilatedPupils Posted at: 2016-11-07T03:58:35.335Z Reads: 295

```
[quote="Esrapp21, post:1, topic:12618"]
something VERY wrong!
[/quote]

It looks like you're trying to summon the magic dragon.<img src="/uploads/db1493/original/3X/8/d/8d6830d0cca635ef98a70b967e0d0b8ee6de956e.jpg" width="690" height="377">
```

---
## \#3 Posted by: Esrapp21 Posted at: 2016-11-07T04:12:27.506Z Reads: 282

```
The whole goal was to make a 12s system so I could get 44.4 volts out of it, and have Parallel charging because of its simplicity. I want to keep it in the enclosure so charging wouldn't require Battery removal. It's basically a mix of the two: the charging system is Parallel, while the motor system is series for those extra volts.
```

---
## \#4 Posted by: DilatedPupils Posted at: 2016-11-07T04:17:23.456Z Reads: 278

```
I understand what you're trying to accomplish. But you're gonna need a switch to disconnect the series connection when charging, then disconnect the parallel when discharging. You can't have them in series and in parallel at the same time.
```

---
## \#5 Posted by: Jinra Posted at: 2016-11-07T04:18:06.643Z Reads: 272

```
The moment you hook up the wires, your lipos will go boom. You're essentially shorting them out if you hook it up this way.
```

---
## \#6 Posted by: Esrapp21 Posted at: 2016-11-07T04:20:36.047Z Reads: 262

```
It's good I posted this before I did it...
```

---
## \#7 Posted by: Jinra Posted at: 2016-11-07T04:22:11.547Z Reads: 262

```
Ah nevermind, I followed the wrong wire on the diagram.
```

---
## \#8 Posted by: Blasto Posted at: 2016-11-07T04:24:58.285Z Reads: 266

```
@Jinra No you are right, big boom.

The parallel conections shorts out because of the series connection

<img src="/uploads/db1493/original/3X/5/a/5a2e97d0b91036e1fab05d6106b812c3bb86df13.jpg" width="375" height="500">
```

---
## \#9 Posted by: anorak234 Posted at: 2016-11-07T04:32:41.842Z Reads: 260

```
@Esrapp21 this is doable but as @DilatedPupils stated you need to disconnect the series connection when the batteries are charging or as @Jinra stated you will promptly need new batteries - and likely a new house. The easiest way I found to doing this was to place an XT90-S key in my series connection so that the circuit to run the motor is off while charging

Example (diagram is not mine):
<img src="/uploads/db1493/original/3X/2/0/201bbe3e2b14327c6e88592ad349367c179eeb9b.png" width="690" height="399">
```

---
## \#10 Posted by: Esrapp21 Posted at: 2016-11-07T12:52:30.000Z Reads: 238

```
Thanks for the advice. Boy am I glad now I posted this before I got the parts :slight_smile:
```

---
## \#11 Posted by: Namasaki Posted at: 2016-11-07T13:07:12.476Z Reads: 237

```
The best way to accomplish what you want is with an onboard 12s BMS and a simple charger.
```

---
## \#12 Posted by: mountainboardlover69 Posted at: 2016-11-07T13:28:36.694Z Reads: 238

```
okay to help esrapp 21 a bit i made a diagram wen u ride u plug in the xt90 as(antie spark)
and if u charge plug the xt90 out and the xt60 in and the balance  connecter if have any question plz contact me 
<img src="/uploads/db1493/original/3X/6/e/6e63f8365ef39731088b9087cd3f9656daec8456.png" width="681" height="500">
dual bl = dual balance lead (12s)
```

---
## \#13 Posted by: DeathCookies Posted at: 2016-11-07T13:42:33.211Z Reads: 217

```
I would suggest to move the XT90-S loop key to another position. Maybe between one battery and the esc instead of between both batteries.

When you will charge it like your diagramm everything will works. The only downside is that you power the esc becauce you get positive from the upper battery and negative of the "downer" battery. It will not destroy your esc but i do not know the longterm side effects.
```

---
## \#14 Posted by: mountainboardlover69 Posted at: 2016-11-07T13:44:36.788Z Reads: 209

```
dont they have a on and of switch at least my one and his first diagram  2
and if u move it u wil shortcircuit no body likes that
```

---
## \#15 Posted by: DeathCookies Posted at: 2016-11-07T13:51:19.481Z Reads: 207

```
I assume you will use a parallel board to charge both batteries at once.

When you are charging both batteries at once you will have a positive wire (upper battery) and a negative wire (downer battery) that goes to the ESC. when you charge both batteries at once you will have power on both cables even if the loop key is detached.
--> The energy comes from the charger not the batteries but this energy goes into the esc and power it on with your current wiring.
```

---
## \#16 Posted by: mountainboardlover69 Posted at: 2016-11-07T13:51:42.562Z Reads: 203

```
here is is fix for no switch users<img src="/uploads/db1493/original/3X/2/5/25b29168889c880ca592aef64b2ae6efa3f9b434.png" width="667" height="500">
u can make the xt60 a xt 90 antie spark but this way u need a different  key to nulock more thief protection
```

---
## \#17 Posted by: DeathCookies Posted at: 2016-11-07T13:55:00.409Z Reads: 196

```
i would recommend the following part of the wiring for the loop key:
<img src="/uploads/db1493/original/3X/0/c/0cb4a61f9a175d3fa9c3bced6fedeae6027c3e17.png" width="690" height="397">
laod = esc
```

---
## \#18 Posted by: mountainboardlover69 Posted at: 2016-11-07T14:02:03.117Z Reads: 183

```
ur charger wont like that if u charge paralel  like @Esrapp21
```

---
## \#19 Posted by: DilatedPupils Posted at: 2016-11-07T14:04:07.075Z Reads: 176

```
This would work if he wasn't trying to charge in parallel.
@mountainboardlover69 has the right diagram. Maybe switch the xt90s and the added xt60
```

---
## \#20 Posted by: DeathCookies Posted at: 2016-11-07T14:09:21.485Z Reads: 177

```
Lol... His new diagramm is correct too but the additional XT60 is not neccessary when you reposition the xt90s.

In my diagramm there are two black xt60. these can be wired in parallel (like he did in his wiring). I was just too lazy to draw it...
```

---
## \#21 Posted by: mountainboardlover69 Posted at: 2016-11-07T14:11:09.254Z Reads: 171

```
sorry i f up the balance lead here is the final digram haha<img src="/uploads/db1493/original/3X/b/e/bec733c22d1d26d9cab49b0554a98fe8b272052d.png" width="667" height="499">
```

---
## \#22 Posted by: mountainboardlover69 Posted at: 2016-11-07T14:12:36.152Z Reads: 157

```
yes i know but ur charger wil short circuit
```

---
## \#23 Posted by: DilatedPupils Posted at: 2016-11-07T14:13:21.919Z Reads: 158

```
You have to disconnect the series before you charge in parallel
```

---
## \#24 Posted by: mountainboardlover69 Posted at: 2016-11-07T14:19:33.163Z Reads: 167

```
here u go u can se wat u did rong<img src="/uploads/db1493/original/3X/5/6/56a7ccb9be0c9d52e916ff40766854e365231c68.png" width="690" height="456">
chagers dont  like a 700 amp draw thay may exsplode but hey if u like fireworks
```

---
## \#25 Posted by: DeathCookies Posted at: 2016-11-07T14:55:51.249Z Reads: 151

```
Oh damn me... You are correct.

Charging will be a hassle. Disconnect series connector and disconnect xt90s for charging.
Maybe someone has a better idea to charge parallel and discharge in series by de-/connecting only one plug?
```

---
## \#26 Posted by: DilatedPupils Posted at: 2016-11-07T15:34:40.218Z Reads: 141

```
yep, the pain of using lipos. maybe use a bms or need to get better charger, but then again , might as well go with liion
```

---
## \#27 Posted by: mountainboardlover69 Posted at: 2016-11-07T16:09:25.098Z Reads: 143

```
liion is the same pain
```

---
## \#28 Posted by: Esrapp21 Posted at: 2016-11-07T16:18:59.110Z Reads: 146

```
I don't know if this makes a difference, but that little gray box in my diagram is a high voltage power switch. Would the circuit work if whenever I charged the batteries, that was off?
```

---
## \#29 Posted by: SteveS Posted at: 2016-11-07T16:21:52.532Z Reads: 148

```
I had the same goal of 12S power with 6S parallel charging. My simple solution is here: http://www.electric-skateboard.builders/t/trampa-street-carver-sk3-6374-12s-vesc-and-trampa-mount-kit/10259
```

---
## \#30 Posted by: Esrapp21 Posted at: 2016-11-07T16:56:44.633Z Reads: 140

```
This is the switch: diy-electric-skateboard-kits-parts/electric-skateboard-on-off-power-switch/
It's way overpriced but it looks professional and has built in spark protection. I think, as long as this switch is off, charging would be fine and the circuit would work. Look at the original picture of my circuit to see where it is, and tell me if I am incorrect.
```

---
## \#31 Posted by: DilatedPupils Posted at: 2016-11-07T17:13:12.166Z Reads: 132

```
@Esrapp21 The only thing that that switch is doing is replacing the xt90s on @mountainboardlover69 diagram. But your diagram is still wrong.
Maybe @SteveS can make you a diagram of what he did.
```

---
## \#32 Posted by: mountainboardlover69 Posted at: 2016-11-07T17:22:22.968Z Reads: 138

```
this is the diagram you have to use then <img src="/uploads/db1493/original/3X/9/4/9452afba5f84692ed61c7c7507dfb8163180b5b0.png" width="668" height="500">
```

---
## \#33 Posted by: Esrapp21 Posted at: 2016-11-07T17:45:24.756Z Reads: 127

```
I see. Ok, thanks for the response. I'll post my final circuit and when it is done. Thank you all!
```

---
## \#34 Posted by: Esrapp21 Posted at: 2016-11-07T18:50:44.352Z Reads: 131

```
<img src="/uploads/db1493/original/3X/8/6/863ea01f209338ad1bf9fdd91161ba46518386b3.PNG" width="591" height="500">
I've added a way to disconnect the Parallel charging circuit while in use by putting the xt60 connectors at the ends of the Parallel connectors, as you guys suggested. This should be the final circuit, assuming nothing goes wrong. I will post the physical circuit when I get the parts. Thank you guys again!
```

---
## \#35 Posted by: jmasta Posted at: 2016-11-07T18:58:46.486Z Reads: 116

```
The positive lead of the lower battery is still permanently wired to the negative lead of the upper battery.  By this diagram, you would then be creating a short when you connect the parallel connector.
```

---
## \#36 Posted by: mountainboardlover69 Posted at: 2016-11-07T19:12:22.551Z Reads: 129

```
no ur chager wont like this set up i made a scets take a good look
<img src="/uploads/db1493/original/3X/a/4/a48398f2b533a4498af91bab7670546bb5309a31.png" width="576" height="500">
i markt wat u did rong but if u change every ting u need change it wil look just like this<img src="/uploads/db1493/original/3X/4/6/466f8d21d6502628f72dcb01b97fc33c164ff6b9.png" width="668" height="500">
```

---
## \#37 Posted by: Maxid Posted at: 2016-11-07T19:17:24.337Z Reads: 121

```
just do it like this:
http://www.electric-skateboard.builders/uploads/db1493/original/2X/2/2f29006da60749bdad79fcd60305918de7ca4792.PNG

Also you should probably have a look at this thread:
http://www.electric-skateboard.builders/t/how-to-discharge-in-series-and-charge-in-parallel-solved/1589
```

---
## \#38 Posted by: mountainboardlover69 Posted at: 2016-11-07T19:39:29.554Z Reads: 126

```
um that is the same but u wil power the vesc btw and no anti spark plug (u need that)@SteveS this is your digarm or did i made a mistake<img src="/uploads/db1493/original/3X/7/f/7fecfd70e73734ce6960d1d1ee3e32e81f243256.png" width="664" height="500"> @Esrapp21 if you use @SteveS setup u need to take the lid of every singel time
```

---
## \#39 Posted by: Maxid Posted at: 2016-11-07T19:53:46.476Z Reads: 113

```
it is not the same - in my diagram there is a loop key that acts as an anti spark.
```

---
## \#40 Posted by: mountainboardlover69 Posted at: 2016-11-07T20:03:44.009Z Reads: 117

```
<img src="/uploads/db1493/original/3X/c/a/ca099d2bc3e67ca948075e7c7545b472ed6099dd.png" width="551" height="277"> 
it is but i need 2 put a volt meter in my xt60 so i need to get 2 free ports not one and  the xt60 is that key and if i look at my other diagram u can se the xt90 antie spark 
and how do u stop puting the esc on power
```

---
## \#41 Posted by: mountainboardlover69 Posted at: 2016-11-07T20:22:22.438Z Reads: 126

```
okay for every one here are 2 great options 1 is not mine it is @Maxid
fist option i wil take a bit more connectors  but i dont need to open ur case or have any cables sticking out just connectors great if u want to seal ur case whit silicone  u need to take out those (keys)xt90 and 60 before u charge <img src="/uploads/db1493/original/3X/7/6/762e002d1484cd91687f9c28dd0e2ff38f581987.png" width="667" height="499">
second one simpel bit i wil need to be abele to open ur case / housing easy this is not mine its @Maxid ones i dont take credit <img src="/uploads/db1493/original/3X/4/b/4bc6946a9ed229ebaeef54fdfd52d89e55c0436d.png" width="690" height="454">
it is up to u witch u like the most if u have any question plz ask me
```

---
## \#42 Posted by: SteveS Posted at: 2016-11-07T20:33:36.791Z Reads: 102

```
Yup, the second diagram @mountainboardlover69 posted is my setup (except I use XT90s throughout). On my Trampa, opening the case is easy, but I used the same setup with a conventional @psychotiller enclosure. I cut a hole in the enclosure, then used a [Ford truck body plug](http://www.macsautoparts.com/ford_truck_late/ford-pickup-truck-firewall-plug-rubber-oval-1-375-x-2-875-f100-thru-f350.html?utm_source=google&utm_medium=paid_search&utm_campaign=paid_search_google_pla&scid=scplp16023020&sc_intid=48-14488-2&gclid=CjwKEAiA6YDBBRDwtpTQnYzx5lASJAC57ObMCRdR3yHD6LfttFPnuZewqrveV0vQvlvMZja1fVhLzxoCQbTw_wcB) to access the connectors.
```

---
## \#43 Posted by: SteveS Posted at: 2016-11-07T20:46:26.010Z Reads: 107

```
Incidentally, I don't see the advantage of the first diagram @mountainboardlover69 posted above. Wouldn't one have to disconnect the xt90s connector and the xt60 connector that puts the batteries in series before parallel charging?
```

---
## \#44 Posted by: Esrapp21 Posted at: 2016-11-07T22:11:25.965Z Reads: 113

```
After all this, I realized that there was a simpler solution. I scraped the original circuit design and shifted to a Great Scott (Youtube) inspired design from this video: https://youtu.be/zaTskMjpXtA . Here is the new design that features a three way switch system. One question: Will the battery display and VESC Parallel circuit part be an issue? <img src="/uploads/db1493/original/3X/2/0/20e20dbf28e82a0a2bbebcac075d4d3ba06aeb83.PNG" width="387" height="499">
```

---
## \#45 Posted by: jmasta Posted at: 2016-11-07T22:21:54.066Z Reads: 104

```
Now you have both batteries wired in parallel permanently, regardless of switch configuration
```

---
## \#46 Posted by: Maxid Posted at: 2016-11-07T22:24:27.896Z Reads: 103

```
these switches are usually not rated at the typical currents we use.
Also @jmasta is right - now your batteries are wired in parallel the entire time.

Please think a little bit more about what you actually want.
```

---
## \#47 Posted by: Esrapp21 Posted at: 2016-11-07T22:28:26.024Z Reads: 102

```
This is way more complex than I expected... I'm gonna use your guys design for the circuit. I'll send a picture of the final board.
```

---
## \#48 Posted by: Esrapp21 Posted at: 2016-11-07T22:47:00.032Z Reads: 108

```
Thank you so much for these designs. This is what I am going to use, assuming all is good and nothing blows up...
<img src="/uploads/db1493/original/3X/8/d/8d289f9296e839b2e2615ca2f26579cc8058bbbd.PNG" width="375" height="500">
Brown represents enclosure, note it is not the correct shape, but what is sticking out will be sticking out. For the exposed wires, I will have rubber covers on them while the port isn't in use.
```

---
## \#49 Posted by: Maxid Posted at: 2016-11-07T22:51:19.037Z Reads: 95

```
you can't make a parallel balancer cable when the batteries are getting used in a series configuration later.
Also there is no need for the switch since you have a loop key.
```

---
## \#50 Posted by: SteveS Posted at: 2016-11-07T22:54:03.118Z Reads: 91

```
If he removed the switch, wouldn't the batteries effectively be connected in series via the VESC?
```

---
## \#51 Posted by: Maxid Posted at: 2016-11-07T22:58:07.586Z Reads: 94

```
he should get rid of the switch and put the VESC behind the loop key. I was anyway urging him to change his layout since the balancer cables will not work like this. But it seems to me that the fundamental understanding of how electricity works is lacking in this thread. I will probably stop commenting since it seems to be an endless back and forth with the same mistakes over and over again.
```

---
## \#52 Posted by: SteveS Posted at: 2016-11-07T23:01:34.539Z Reads: 90

```
Agreed. Further, this most recent configuration is dangerous because if he forgot to turn off the switch before charging, the batteries would still be connected in series (as I said, via the VESC).

 I think @Kaly did what @Esrapp21 is trying to do. The magic is in the DPDT witch. He documented it nicely [here](http://www.electric-skateboard.builders/t/26650-a123-battery-pack-with-parallel-series-switch-selector/2893).
```

---
## \#53 Posted by: Maxid Posted at: 2016-11-07T23:07:07.706Z Reads: 96

```
thanks for the link - that looks really clean. I would just be worried about the currents going through the small DPDT switch. they are usually only rated at like 2-6A - not the 20-50A we typically use. But maybe @Kaly can comment on his experience and prove me wrong.
```

---
## \#54 Posted by: Kaly Posted at: 2016-11-07T23:31:45.390Z Reads: 109

```
Hello guys 
The switch works really well. It is rated for 20A @ 125V or 10A @ 250V this translate to 2500W and that is more than enough for our application. 

The switch need to be use with extreme care when choosing a setting because if the balance leads are connected in PARALLEL  while the switch is set to SERIES  you are going to BURN :fire: :fire: :fire: :fire: the balances leads. 

To avoid this 
You'll need to first choose the parallel position, then connect the charger and then connect the balance lead in parallel. 

As a precaution all the positions of the switch have to be label and a warning label need to be paste to the charging port and balance leads, to remind you to check the correct settings. 

If you are not sure you can follow the procedure do not do this, it's easy to make a mistake with the balance leads. 

Good luck.
```

---
## \#55 Posted by: SteveS Posted at: 2016-11-07T23:36:43.502Z Reads: 94

```
Yeah, while I admire the convenience in use and slickness of your setup, @Kaly, that my setup is idiot-proof good for my peace of mind.
```

---
## \#56 Posted by: Esrapp21 Posted at: 2016-11-08T00:17:01.949Z Reads: 89

```
It is exactly what I want to do. I'm going to use that for the project. Thank you for helping, as I am not the smartest with Circuits, as you can tell... @Kaly I get that is is good from a watt perspective, but are there any switches that can take like 50A?
```

---
## \#57 Posted by: Kaly Posted at: 2016-11-08T01:30:29.655Z Reads: 86

```
What really matters is the watts,  the switch can take 2500W this is really a lot of power for eSk8 application and besides the thing just cost $4.00 plus have a small foot print. :slight_smile:
```

---
## \#58 Posted by: Esrapp21 Posted at: 2016-11-08T01:34:05.955Z Reads: 84

```
Ok, thanks!
```

---
## \#59 Posted by: Esrapp21 Posted at: 2016-11-08T01:42:27.853Z Reads: 89

```
@Kaly one more thing. It's probably a stupid question, but I noticed on your project you had two balance ports for 2 batteries that were wired together. When charging the board, how does that work? What do you plug into the charger? Just one of the balance cables or is there an adapter to connect to both?
```

---
## \#60 Posted by: Kaly Posted at: 2016-11-08T01:46:57.706Z Reads: 89

```
You need to make a parallel adapter for the balance leads, you do this by soldering tougher balance lead extension. 
I'll post a pic in a couple of min.
```

---
## \#61 Posted by: Kaly Posted at: 2016-11-08T02:12:17.714Z Reads: 101

```
<img src="/uploads/db1493/original/3X/2/2/22b64d4d9b707077854739f039b4e26ddc4e4d5f.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/b/c/bc6ad2078edd7b6adc4dea04397274a89cd74a57.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/a/b/ab414c4a39e515da67f0004921e0419b782e3310.JPG" width="375" height="500">
```

---
## \#62 Posted by: AbdeTy Posted at: 2016-11-08T02:41:22.832Z Reads: 98

```
i am also planning on using this system on my build, @Kaly Your DPDT switch is the missing part for me but now i guess its all clear , i learned alot from this discussion , i also made a diagram of how the set up will be with the DPDT switch maybe it will make things clear for others as well , because your instructable tutorial uses motors instead of batteries i got a bit confused so can you please confirm if this is correct ,   <img src="/uploads/db1493/original/3X/1/d/1de208aa032d3832741e1c98b1e3710c63d72b15.png" width="690" height="353">
```

---
## \#63 Posted by: Kaly Posted at: 2016-11-08T03:10:56.591Z Reads: 90

```
This diagram is correct :-) 
Just to clarify the balance leads only will be connected in parallel when charging. In any other state or configuration have to be disconnected.
```

---
## \#64 Posted by: Namasaki Posted at: 2016-11-08T03:14:37.234Z Reads: 96

```
Bottom line, The only way to run multiple Lipos in series and charge them conveniently is to use an onboard BMS and a laptop charger.
Then you will not have to disconnect and reconnect anything. You won't even have to open the enclosure.
You just plug in the charger and wait. The bms will monitor each cell individually and stop when each cell is fully charged.
and you won't have to charge in parallel, which btw is not really recommended for Lipos.
Check out my Lipo with bms build.
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#65 Posted by: Kaly Posted at: 2016-11-08T03:17:57.475Z Reads: 96

```
For sure this the most safe way to charge.
```

---
## \#66 Posted by: Esrapp21 Posted at: 2016-11-08T03:25:46.631Z Reads: 97

```
I have the same layout as you, @AbdeTy here it is:
<img src="/uploads/db1493/original/3X/f/a/fa938700065f2f18bc314654858e6060c7dea469.PNG" width="595" height="500">
I was wondering if this was a good setup and if the battery voltage checkers were setup correctly. (They are the black boxes with the red volt inside)
```

---
## \#67 Posted by: AbdeTy Posted at: 2016-11-08T03:31:05.591Z Reads: 88

```
good , about the balance wires yes i will be using a 15 pin VGA adapter that will have both the balance wires and the charging one and they wont be connected from the charging cable end :slight_smile: thank you
```

---
## \#68 Posted by: Kaly Posted at: 2016-11-08T03:32:07.843Z Reads: 86

```
For the voltage meter you can use a lipo saver alarm  connected to the balance lead with a small on/off switch on the negative wire of the balance lead.
```

---
## \#69 Posted by: AbdeTy Posted at: 2016-11-08T03:32:50.723Z Reads: 87

```
that's true , but with all what i read about BMs i find it hard to trust them , do you have any recommendation for a good place to get good quality BMSs ?
```

---
## \#70 Posted by: Esrapp21 Posted at: 2016-11-08T03:34:26.297Z Reads: 87

```
@Namasaki @AbdeTy The only reason why I don't do that (use BMS) is this: https://youtu.be/pljSZcEwc8Q
The video explains how using hobby chargers are safer and more reliable than BMSs. I would eventually look into it for a v.2 of the board, but for now I'll just stick with my hobby charger.
```

---
## \#71 Posted by: AbdeTy Posted at: 2016-11-08T03:39:24.045Z Reads: 79

```
lol yep i did see that one , that's when i decided not to use them as well , i would feel safer while riding my board if i am sure my battery is balanced after each charge and once there is a problem i  will know right away, the BMS can fuck up and you wouldn't know and if you dont monitor your batteries regularly that could cause a disaster
```

---
## \#72 Posted by: Esrapp21 Posted at: 2016-11-08T03:40:46.160Z Reads: 79

```
Until I can monitor the BMS easily, I will stick with the old-school system :wink:
```

---
## \#73 Posted by: AbdeTy Posted at: 2016-11-08T03:44:34.237Z Reads: 81

```
yep they really need to develop an advanced BMS, maybe a display and live data bluetooth and a smart app that can let you know if something is wrong, maybe we should develop it ourselves lol
```

---
## \#74 Posted by: Esrapp21 Posted at: 2016-11-08T03:45:00.632Z Reads: 83

```
I googled doing this, but this requires the balance cord. Is there a way to permanently install the meters while still being able to balance charge? Would I use a parallel adapter?
```

---
## \#75 Posted by: Esrapp21 Posted at: 2016-11-08T03:45:47.313Z Reads: 81

```
First there was the VESC as an open sourced ESC, now the needs to be a VBMS!
```

---
## \#76 Posted by: AbdeTy Posted at: 2016-11-08T03:47:57.248Z Reads: 77

```
yep i guess a  parallel adapter is what you need for each cell.
```

---
## \#77 Posted by: AbdeTy Posted at: 2016-11-08T03:48:46.513Z Reads: 77

```
yep hopefully we will see it soon
```

---
## \#78 Posted by: Namasaki Posted at: 2016-11-08T04:47:08.634Z Reads: 91

```
I don't know what bms the guy in that video is talking about. I did not recognize any of the boards he was holding and for all I know they are some of the $15 dollar cheapies that you get on eBay.
The Bms I'm using is by a reputable company and has overcharge protection, over discharge protection, over voltage protection, under voltage protection, short circuit protection(if there is a short anywhere in the entire system, it shuts off)  and overheat protection. It monitors every cell individually during charge and discharge. And if anything goes wrong, it shuts off.
It is important to use a quality BMS just like it's important to use a quality balance charger for manual charging.
And although you can charge lipos in parallel, you really shouldn't 
For one thing, the internal resistance in each cell of a lipo pack varies. thats why they never discharge or charge at exactly the same rate. If you want to stick with a balance charger and don't mind the hassle, the best and safest option would be a dual bank charger that can charge 2 6s Lipos separately and simultaneously.
Edit: As far as monitoring battery voltage, you can use multiple cell alarms like the guy in the video. You can use them with a BMS if you don't want to trust the protection circuits. The problem with them is that they constantly drain the battery unless you unplug them.
I'm pretty sure that all the people in this community who are building battery packs for retail, are building them with bms's
So are all of the commercial manufactures of electric skateboards.
```

---
## \#79 Posted by: lowGuido Posted at: 2016-11-08T05:35:03.977Z Reads: 87

```
[quote="DeathCookies, post:13, topic:12618"]
The only downside is that you power the esc becauce you get positive from the upper battery and negative of the "downer" battery. It will not destroy your esc but i do not know the longterm side effects.
[/quote]

Sorry but what?
Thats not right. You cant get negative and positive from 2 different batteries that arent connected. It needs to be a circuit.
```

---
## \#80 Posted by: mountainboardlover69 Posted at: 2016-11-08T06:01:27.964Z Reads: 80

```
Idk if that switch wil Handel it  my set up is 2x 2700w total max draw is 5400w
```

---
## \#81 Posted by: mountainboardlover69 Posted at: 2016-11-08T06:04:45.601Z Reads: 81

```
Wel then as I said u wil nod need 2 open the lid of ur longboard
```

---
## \#82 Posted by: mountainboardlover69 Posted at: 2016-11-08T06:53:05.087Z Reads: 90

```
SO THIS wat u are al doning ???? <img src="/uploads/db1493/original/3X/4/c/4c86250670ea0661b0f20103272c167d2dac5457.png" width="690" height="451">
```

---
## \#83 Posted by: DeathCookies Posted at: 2016-11-08T07:42:05.210Z Reads: 88

```
[quote="lowGuido, post:79, topic:12618"]
Sorry but what?Thats not right. You cant get negative and positive from 2 different batteries that arent connected. It needs to be a circuit.
[/quote]
Yeah i know. It must be a **closed** circuit.

But when you attach a parallel board or parallel wiring for charging you have a closed circuit ;)
<img src="/uploads/db1493/original/3X/c/f/cf6daff83e599e290477aa888ae6107856c6eeac.jpg" width="620" height="288">
If you connect the wiring in the right green circle you have on both wires energy. When the XT90s is detached you still have a circuit from the parallel wiring (other green circle)
```

---
## \#84 Posted by: Maxid Posted at: 2016-11-08T08:39:37.252Z Reads: 80

```
[quote="Kaly, post:57, topic:12618, full:true"]
What really matters is the watts
[/quote]

That is not true however. What causes heat is the current not the voltage (which is why powerlines usually operate in kV range). So if you use your switch at higher currents than its rating, you are introducing additional losses and resistance into your circuit. Basically up to a point where the metal in your switch acts like a fuse and blows/melts.
```

---
## \#85 Posted by: Kaly Posted at: 2016-11-08T11:50:15.660Z Reads: 80

```
Yes this can be done. That is how I have my packs wired. 
For this you need to use a parallel adapter on the balance lead one end will go to the charging port and the other to the voltage meter but on this one you will need to install a on/off switch on the negative wire so you can turn the meter off.
```

---
## \#86 Posted by: Esrapp21 Posted at: 2016-11-08T12:21:11.095Z Reads: 78

```
Have you had any problems with over heating of the switch like Maxie said?
```

---
## \#87 Posted by: Esrapp21 Posted at: 2016-11-08T12:22:34.121Z Reads: 75

```
When you charge, you remove the XT60 key to stop the ESC circuit. That is the one the positive lead goes through before hitting the ESC. You also remove the XT90 key.
```

---
## \#88 Posted by: DeathCookies Posted at: 2016-11-08T12:39:23.070Z Reads: 83

```
Indeed!
My initial question was what wiring can be used to charge in parallel and discharge in series by only plugging in/out one key. 
The current solution needs to keys.
```

---
## \#89 Posted by: mountainboardlover69 Posted at: 2016-11-08T12:52:05.657Z Reads: 84

```
@DeathCookies i made u a fix <img src="/uploads/db1493/original/3X/b/b/bb387f04ac5ce29adb57138c039956818a300106.png" width="625" height="500">
```

---
## \#90 Posted by: DeathCookies Posted at: 2016-11-08T12:58:42.651Z Reads: 81

```
Well that is an easy fix :D just make one plug ot ouf two but it is not very convenient to  de-/attach
```

---
## \#91 Posted by: mountainboardlover69 Posted at: 2016-11-08T12:59:44.681Z Reads: 76

```
wel if u glue the if ther in i weel be a okay fit hahahahahahahhahahahah:joy:
```

---
## \#92 Posted by: Esrapp21 Posted at: 2016-11-08T13:22:17.572Z Reads: 77

```
I liked this idea, but @Kaly s idea with the switch to switch between parallel and series circuits is in my mind more convenient. The only thing is with this talk of the switch not being able to handle the current. Any comments on that?
```

---
## \#93 Posted by: Kaly Posted at: 2016-11-08T13:56:45.246Z Reads: 77

```
@Maxid
 That is true about the current (Amps) being the source of heat. But you need real worl assessment on this. 

Don't miss interpret this :wink:
 but, I recommend you buy a switch open it up, take the contact elements make an evaluation of  the cross section and determine the heat that will be generated on the system  with the parameters we use on eSk8 applications and then we can resume this conversation :slight_smile:
```

---
## \#94 Posted by: Kaly Posted at: 2016-11-08T14:43:41.196Z Reads: 80

```
The switch works flawlessly for almost a year now. The contact elements inside the switch are capable of handling the current with not problem. 

I have wired 5 boards with this switch and no issues at all. 

The issue @Maxid bring up is correct but that is if you only judge by the rated current on the switch. In my case this is a $ 4.50 switch so I opened and got the cross-section dimension and did the calculations for the amount of heat that was going to be generate with the load of my application and the switch have almost a safety factor of 2.
```

---
## \#95 Posted by: mountainboardlover69 Posted at: 2016-11-08T14:45:56.686Z Reads: 77

```
do u have any 6000 wat switch u can recomend??????
```

---
## \#96 Posted by: jmasta Posted at: 2016-11-08T15:36:04.030Z Reads: 83

```
[quote="mountainboardlover69, post:95, topic:12618, full:true"]
do u have any 6000 wat switch u can recomend??????
[/quote]
A 6kW mechanical switch is not feasible for our purposes. It would be way too big.  That's why we build electrical switches from mosfets in parallel to achieve the necessary current rating

Here's a 4kW changeover switch. It's massive.  I bought one with the hopes of making it smaller. Not possible.  It's probably 3" in diameter and 4" long.

https://www.amazon.com/Positions-Changeover-Control-Rotary-Switch/dp/B0054U7IY2/ref=pd_sim_sbs_60_5
```

---
## \#97 Posted by: Kaly Posted at: 2016-11-08T15:45:09.076Z Reads: 79

```
That will. E a super big device. 
In thing we need to have clear is that if you use 10S or 12S battery you are not going to be pulling that many amps even in extreme situation even here I'm just pulling 50A on 12S, measure with a watt meter. 

 [eSk8Tube Video thread](http://www.electric-skateboard.builders/t/esk8tube-video-thread/47/17):
```

---
## \#98 Posted by: jmasta Posted at: 2016-11-08T15:55:31.235Z Reads: 81

```
[quote="Maxid, post:84, topic:12618, full:true"]
[quote="Kaly, post:57, topic:12618, full:true"]
What really matters is the watts
[/quote]

That is not true however. What causes heat is the current not the voltage (which is why powerlines usually operate in kV range). So if you use your switch at higher currents than its rating, you are introducing additional losses and resistance into your circuit. Basically up to a point where the metal in your switch acts like a fuse and blows/melts.
[/quote]

To add on to your statement...  The power dissipated is proportional to the current SQUARED.  Therefore the heat generated goes up exponentially with the current.  That's why it's not as a simple as saying the switch is good for 2.5kW.   

In real world testing the switch seems to work.  But for how long?  You are really pushing it to its limits.  But they are cheap, so maybe you are alright with that risk.  I was going to go this same path and then just went with a 12S BMS. So much simpler and safer for not much cost increase

P.S. @Kaly, I really do like your design!  So don't take this the wrong way.  I'm just being a conservative engineer.
```

---
## \#99 Posted by: Kaly Posted at: 2016-11-08T16:18:22.346Z Reads: 77

```
There is always a option for BMS 
Like this one http://www.batterysupports.com/lion-lipo-nbsp-36v-nbsp-10s-c-32_41.html
```

---
## \#100 Posted by: jmasta Posted at: 2016-11-08T17:10:44.517Z Reads: 86

```
If you really want to use the parallel/series switch, here's a way to double the capacity of your switch.

Use a 4PDT switch (4 pole, double throw) instead of DPDT.  Then split each of your leads in parallel across two poles.  This effectively cuts your current in half!

https://www.amazon.com/4PDT-Heavy-Duty-Toggle-Switch/dp/B001TJ6O9M
```

---
## \#101 Posted by: mountainboardlover69 Posted at: 2016-11-08T17:14:21.429Z Reads: 84

```
wel i will just go wit my 2 key disinge
```

---
## \#102 Posted by: Esrapp21 Posted at: 2016-11-08T22:48:45.939Z Reads: 89

```
<img src="/uploads/db1493/original/3X/b/d/bd6360dd447e50144497b4d98dc722f78e621999.PNG" width="545" height="500">
I'm going to use the same idea of the switch circuit with xt60/90 keys. Here it is: the Ps stand for parallel, while s stands for series.
```

---
## \#103 Posted by: mountainboardlover69 Posted at: 2016-11-09T08:46:12.846Z Reads: 84

```
i dont se any problems the circuit but this stil wil feed power to ur ecs /vesc
```

---
## \#104 Posted by: deucesdown Posted at: 2016-11-09T15:02:11.019Z Reads: 87

```
Series/parallel switch, I'm really inspired by @kaly's switching. And I know his experience has been good. I want to believe! But...

Those cheap small switches have 2 challenges. Current/heat, which has already been discussed, and [arcing](https://www.youtube.com/watch?v=Zez2r1RPpWY).

Appears DC arcs way more easily than AC. I think you can step around this using a loop key to open the circuit before switching. That adds one more step to the dance. And the switch may still arc because the contacts are so close.

I'm also struggling with a high current on/off switch. Don't want to pay $60, don't want to go solid state. Antispark loop key looks like an _okay_ solution, not great. Marine DC circuit breakers (with arc suppression), I maybe be wrong but I don't think circuit breakers are designed for many on/off cycles.

And BMS, if I could buy one from a non-china based company who can be held accountable for failure, I agree, this is a good way to go. But with the sources we have for diy, seems like a gamble. I know some vendors have established at least a decent reputation, still I feel the sample size is small. And you might not notice your BMS had partially failed and is killing one or more of your parallel groups. Some of these packs are like $500! I'm too paranoid...

But maybe @JTAG will [save the day](http://www.electric-skateboard.builders/t/diy-6s-to-12s-bms-with-can/2639)!
```

---
## \#105 Posted by: Kaly Posted at: 2016-11-09T15:42:39.631Z Reads: 78

```
This is a good perspective on the matter. 
Welcome to the nuance of DIY uncertainties. :slight_smile:
```

---
## \#106 Posted by: Mikeomania12 Posted at: 2016-11-09T16:11:37.202Z Reads: 77

```
Yeh I always thought it would be problem with BMS monitoring the parallel groups. Seems like its not very reliable...
You really still have to go in with a voltmeter and check every cell once a month to make sure.
```

---
## \#107 Posted by: Esrapp21 Posted at: 2016-11-10T02:57:58.428Z Reads: 79

```
<img src="/uploads/db1493/original/3X/b/2/b2175daeac5a3c7fe32e797fd5da02d50fbc83c8.PNG" width="656" height="500">
Here is the completed circuit with the series/parallel system built in. I also added lights for night riding :slight_smile:
```

---
## \#108 Posted by: DeathCookies Posted at: 2016-11-10T09:09:52.862Z Reads: 73

```
You cannot glue the two plugs together.
If you attach both plugs at once you will have one series and one parallel connection which will lead to a big meltdown...
```

---
## \#109 Posted by: mountainboardlover69 Posted at: 2016-11-10T09:11:24.354Z Reads: 74

```
nope
that is not true just dont connect the plugs
```

---
## \#111 Posted by: mountainboardlover69 Posted at: 2016-11-10T09:14:42.072Z Reads: 74

```
rip post  :joy:
```

---
## \#112 Posted by: DeathCookies Posted at: 2016-11-10T09:16:02.718Z Reads: 73

```
The wiring is correct ;) Only remaining problem:

If you attach the Voltmeter before any switch they will be turned on **all time**... if you connect them after the series connection you dont get individual measurements...
```

---
## \#113 Posted by: mountainboardlover69 Posted at: 2016-11-10T09:17:29.040Z Reads: 72

```
that can be fix wit a very cheap switch 20v 0.1a
like this one http://www.qspproducts.nl/schakelaar-flip-over.html#.WCQ7jDvObgI
```

---
## \#114 Posted by: jmasta Posted at: 2016-11-10T16:27:35.913Z Reads: 75

```
[quote="Esrapp21, post:107, topic:12618, full:true"]
<img src="/uploads/db1493/original/3X/b/2/b2175daeac5a3c7fe32e797fd5da02d50fbc83c8.PNG" width="656" height="500">
Here is the completed circuit with the series/parallel system built in. I also added lights for night riding :slight_smile:
[/quote]

What voltage are your batteries? Because with this configuration, your lights would be seeing the full pack voltage.  You can't just connect 12V LEDs to a 50V source without expecting a fireworks show in your mom's basement ;)
```

---
## \#115 Posted by: mountainboardlover69 Posted at: 2016-11-10T18:28:50.343Z Reads: 72

```
but i want fire works haha btw @Esrapp21 12s total
```

---
## \#116 Posted by: Esrapp21 Posted at: 2016-11-10T18:36:59.146Z Reads: 71

```
Your right, thanks for pointing that out? Any suggestions to reduce the voltage there? I don't think run of the mill resistors would work... If it is too big of a problem, I'll either just make a 2x AA separate circuit for them, or just remove them completely.
```

---
## \#117 Posted by: SageTX Posted at: 2016-11-10T18:43:02.202Z Reads: 75

```
Buck converter
```

---
## \#118 Posted by: mountainboardlover69 Posted at: 2016-11-11T07:54:42.545Z Reads: 74

```
18650 !!!!!
```

---
## \#119 Posted by: Esrapp21 Posted at: 2016-11-13T03:12:26.184Z Reads: 77

```
Yet another evolution of the circuit. This one incorporates the BMS and a permanent series connection. While at first I was a little skeptic about the BMS because of so much uncertainty over the internet, I found a reliable source, Battery supports.com, and felt more comfortable. This design, instead of having like 7 ports on the parallel/series circuit, has a power switch and is charged by laptop charging brick. I think the slim uncertainty is worth the sacrifice for the convenience. Also, there is a switch for the lights. As for them, I'm using a 6 led, 6.2x1.7 inch flood light bar, and a buck converter for the voltage reduction.
<img src="/uploads/db1493/original/3X/a/a/aa1ef6d77e60626fd5023a66224658201ecec1a3.PNG" width="593" height="500">
```

---
## \#120 Posted by: mountainboardlover69 Posted at: 2016-11-13T16:00:54.682Z Reads: 72

```
wat i tink of a bms it breaks
```

---
## \#121 Posted by: Esrapp21 Posted at: 2016-11-13T21:58:34.416Z Reads: 73

```
Does anyone have a solution to the anti spark switch for the motor? I like the DIYElectricSkateboard one, but that is $60. I think I want something a little more sophisticated than the XT90 anti spark key, but that can be a last resort.
```

---
## \#122 Posted by: Esrapp21 Posted at: 2016-11-13T22:11:38.438Z Reads: 69

```
Also, how far would this setup get me? Like 16 miles, according to the DIYElectricSkateboard calculator, but I don't know how accurate that is.
```

---
## \#123 Posted by: mountainboardlover69 Posted at: 2016-11-14T08:12:11.385Z Reads: 68

```
u can make them ur self ther are some kit's on the site
```

---
## \#124 Posted by: Joe2020 Posted at: 2017-01-31T11:42:06.946Z Reads: 55

```
you could use a sbec or ubec, im going to use this one [here](http://Hobbyking YEP 20A HV (2~12S) SBEC w/Selectable Voltage Output)
```

---
