# HyperEV Resurrected &#124; Custom Deck &#124; &#124; Dual Diagonal APS Outrunner motors &#124; Aliendrivesystems Mount &#124; 10S &#124; APS 150a twin ESC

### Replies: 35 Views: 5654

## \#1 Posted by: Sebastiaan Posted at: 2016-01-30T19:53:47.904Z Reads: 297

```
Hey, to make a long story short, i bought a complete Eboard from Richard at Aliendrivesystems.com
Why? Because i don't know anything (at the time) about electronics. (still learning though, bear with me)
To give you an example, i did not know that red is positive and black negative (Just to give you an idea about my level of expertise :D )
Richard is a great guy, he helped me through the whole setup, modding my battery balance ports to fit in a 10s charger 
and other, maybe very obvious stuff that i was struggling with.
Check out his site (for people who don't know it yet @ aliendrivesystems.com
He is having a sale, you can do some bargains there !

Okay so what happened, i really had bad luck with a small water puddle, as you can imagine, the ESC went in total meltdown... took out the BECs and the receiver.... disaster !(walk of shame was painfull)

Soooo i'm gonna rebuild everything and mount them on a new deck, which i made during sulking and grieving over my small accident.

So this tread is worthless without pics...

This is the deck i made,
I don't have pictures however when i was creating it, forgot.
Taping....
<img src="/uploads/db1493/original/2X/4/408caf70fa7344bd9513910f45eac6b31e3dfc13.jpg" width="690" height="388">


Other side already done (This is a very strong multiplex layered board, no flex, i milled out three rows and put some strands of oak in there
  <img src="/uploads/db1493/original/2X/b/b86251ebf3bb087fd614da05284414b3b8ab0f1e.jpg" width="690" height="388">


After four layers of glossy clearcoat.
<img src="/uploads/db1493/original/2X/1/1384cca5f798ae97e4d29d1efde87e998dee9fed.jpg" width="281" height="500">


<img src="/uploads/db1493/original/2X/9/96c7785dd13f2653668ecdb27a3ea484a4c9a14c.jpg" width="281" height="500">


<img src="/uploads/db1493/original/2X/c/cf5b011a9849b92573d15115c97e7601dbf78566.jpg" width="375" height="500">

My tool of the trade :smile:
<img src="/uploads/db1493/original/2X/0/046b8a2230c229d7eeda0019a149ac36aad90c2a.jpg" width="690" height="388"> 



Okay so i still have the other board which i'm about to restore since it took quite a beating already,
Gonna sand it down, fill up the gaps and dents with some putty and then sticker it with a carbon sheet i've got from aliexpress. (It's possible i will use this board instead of the custom made one)


Okay so this is my electrical diagram which i mostly reverse engineered from Richard's build, the only thing that changes is the new Dual output BEC instead of (two seperate BECs) which delivers 5v to the receiver and 12v to the tail, head and ledlights.
I'm still looking into how to wire up the Turnigy RC switch in there.
This is my funky looking diagram, hope this is correct and a good example to people who are also want to DIY.
All credits go to Richard though, i've learned a lot when looking at how everything is wired up.
<img src="/uploads/db1493/original/2X/6/6816f2e19429ba04ad3a271246acf81a6355c478.png" width="625" height="500">

As you can see, the lightning is not yet connected as well as the switch, because i still don't know how to.
I don't want to bother Richard too much since i already asked a LOT of questions already :P
The external balance port is also left out.

I'm gonna need some help on how to connect the switch and arrange the lightning.
And the installing of the ESC and configuring it.

Also one small problem, the board came with a unique receiver that pairs with a unique transmitter, 
I still have to check if the receiver is fried, i'm waiting on my BEC to arrive so i can try it.
If it is broken i have no idea which receiver will work with this transmitter. 
Maybe i can get a spare one. I will post update.

That's about it. 
Just waiting for the ESC and the BEC to arrive so i can get cracking.

Also talking about customer service, the ESC went back to alienpowered and the owner is sending me a new one.
Thanks !!!:birthday:
```

---
## \#2 Posted by: lowGuido Posted at: 2016-01-30T23:33:32.524Z Reads: 269

```
Most of the GT2B style of transmitters have a 3rd channel that you could easily hook up to switch the lights on.
just plug your switch into the 3rd channel on the receiver.
you may have to change out the momentary switch for a toggle though, depending on how your circuit works.
```

---
## \#3 Posted by: laurnts Posted at: 2016-01-31T00:01:42.888Z Reads: 270

```
You will need some sort of small relay that has the ability to toggle.
I used to have this within my build purchased from HK
http://www.hobbyking.com/hobbyking/store/__40044__Turnigy_TX_Controlled_Relay_Switch.html

But it broke somehow and now I am going to test this
http://www.hobbyking.com/hobbyking/store/__43894__Dr_Mad_Thrust_Electronic_On_Off_Switch.html

they only need to be mounted now to my eboard :D
```

---
## \#4 Posted by: lowGuido Posted at: 2016-01-31T00:15:49.586Z Reads: 250

```
he already has a switch in his diagram.
```

---
## \#5 Posted by: laurnts Posted at: 2016-01-31T01:41:26.803Z Reads: 241

```
Ohh yea didn't notice seems the shape was not quite familiar :) my bad
```

---
## \#6 Posted by: Sebastiaan Posted at: 2016-02-04T17:56:39.249Z Reads: 236

```
Okay i'm working on updating the diagram including connected lightning and the turnigy switch...

Soooo LOL, i've received the SBEC today, and as always i did not take my time to check things first :smile:
Guess i was too excited???
I wanted to try it right away so i hooked it up directly to the 10s lipo pack, without the antispark :smile:

It's dead... 1v on the 5v output, 3.3v on the 12v output. Gonna try for RMA.

Another lesson learned, Stay calm and take your time. Which is were i mostly fail.
```

---
## \#7 Posted by: laurnts Posted at: 2016-02-04T19:44:22.067Z Reads: 224

```
Antispark doesn't do anything besides limiting the current draw. Hence with / without it any module should be fine, only damage the connectors over time. So you might wanna take a look again in your SBEC if it can handle 10S input.

10S is around 42 Volt. Thats quite big and I barely seen any SBEC can handle over 40V voltage, at least I found one from Hobbyking. http://www.hobbyking.com/hobbyking/store/__42754__Turnigy_HV_SBEC_5A_Switch_Regulator_8_42V_input_EU_Warehouse_.html
```

---
## \#8 Posted by: Sebastiaan Posted at: 2016-02-04T20:06:00.700Z Reads: 241

```
Are you sure? From what i've read, if you connect the lipo's directly to something else, it draws high current for a short moment of time.
I hope i'm not wrong, i have no clue otherwise what caused this...  

It's this one.
http://www.hobbyking.com/hobbyking/store/__72700__Turnigy_Multistar_Twin_Output_5_10_Amp_6_50V_SBEC_for_Lipoly.html

Here is some information for the electronic magicians here, maybe someone can help me with this?

So what happened, as said i connected the SBEC directly to the lipo 10s pack (lead wires)
First the pos than the neg, the polarities were correct. I had a spark on the negative lead. 

I was spooked by this so then i've connected the SBEC to the OUTPUT of the wattmeter. (Which also has leads to the ESC) 

So it's Lipo - > Antispark - > Wattmeter -> SBEC (JST) and ESC
                                                          

(ESC is still RMA)

This output reads (seperate JST connector from the wattmeter) 33 volt (maybe due the watt meter powered on?) , when i measure the lipo pack directly at the leads it's 39 volts

I'm almost positive (in a bad way) that i fried the SBEC with connecting them directly to the lipo leads.

EDIT : 

I checked the wattage meter and i found something weird, there is a little piece of copper disconnected from the board, i will try to show you.
(Not my picture)
<img src="/uploads/db1493/original/2X/6/6a00504fb76af956ea8dd454be09851a950fbd9f.JPG" width="486" height="457"> 

the copper connector betweet the negative leads.I have voltage though on the wattmeter outputs...
```

---
## \#9 Posted by: trbt555 Posted at: 2016-02-05T08:47:44.043Z Reads: 229

```
It's a 50V SBEC, I'd be surprised if you fried it by just connecting it to the lipo's. It's meant to be connected that way.
So maybe it's a bad unit, or maybe you shorted something without realizing.
The spark is just a momentary inrush of current to the capacitors and shouldn't damage it.

If you're feeling adventurous and really want to check your watt meter you can connect a 24V 35W halogen bulb (hardware store) to it like this:
<img src="/uploads/db1493/original/2X/b/ba4e74594432069235a7ac26e2d3944d3db83894.PNG" width="690" height="196">

If you use a freshly charged lipo, the wattmeter should read 20-21V.
The halogen bulb will light up and you should get a current of approx. 1.6A.
```

---
## \#10 Posted by: Sebastiaan Posted at: 2016-02-05T11:27:04.910Z Reads: 220

```
Okay thanks for that guide, Gonna try it this weekend, it's really weird, i have the correct voltage going out of the wattmeter, 33v to the ESC and the BEC.... There are no shorts on the wattmeter, it's working correctly.
Let's see what happens with the lightbulb on a lipo. 

I don't however have that little copper plate on the wattmeter, the one going between the negative IN and OUTputs..
But it's working none the less... Any idea what's it for? its like a bridged connection?
```

---
## \#11 Posted by: trbt555 Posted at: 2016-02-05T12:24:21.287Z Reads: 204

```
Don't worry about the little copper part, unless it actually came loose and you still have it, you may be drawing conclusions based on wrong info. If you have voltage coming out of the wattmeter, it should be ok.
```

---
## \#12 Posted by: Sebastiaan Posted at: 2016-02-05T16:29:45.959Z Reads: 201

```
Sooooo i hooked it up to a single lipo, it's working. 

Steady as she goes on 12v and 5v.
Even my receiver is working, hell, even my BECS that i supposedly fried together with the receiver.... are working....

So i was thinking of bad solder joint or bad jst connector. None of them

What happens if hook up the BEC: The voltage drops from the wattmeter toward the BEC to around 3.3 volt.
Unconnected it's 19 volt.
I have no clue.
```

---
## \#13 Posted by: trbt555 Posted at: 2016-02-05T18:01:10.619Z Reads: 180

```
You have only a bec connected to the lipo via the wattmeter, right ?
Does the wattmeter register current when the bec is connected ?
```

---
## \#14 Posted by: Sebastiaan Posted at: 2016-02-05T18:11:40.066Z Reads: 183

```
There is also a antispark in between. battery -> antispark -> wattmeter -> BEC

Did not think of that -_- Wattmeter was upside down, its still attached to my casing.

When the BEC is connected :  
Wattmeter display wrong readings, 220+ amps (lol) 4000+ watt (lol) 19.4 volt (correct) and 3.3 volts output

Nothing connected shows standard readings. And 19 volts output.
```

---
## \#15 Posted by: trbt555 Posted at: 2016-02-05T18:22:24.473Z Reads: 165

```
Is ths wattmeter connected the right way ?
Source = lipo, load = bec
Do you have a multimeter ?
```

---
## \#16 Posted by: Sebastiaan Posted at: 2016-02-05T18:26:14.683Z Reads: 177

```
Yes everything is connected the right way, Gonna disconnect the wattmeter and try with the output on the antispark.
It's probably the antispark, due the short i had with the water situation maybe something blew up in there.

Yes i have a multimeter. Thanks for helping fellow Belgian :smile:
```

---
## \#17 Posted by: Sebastiaan Posted at: 2016-02-06T15:12:04.682Z Reads: 187

```
I've found out what the issue was, it is indeed that little copper bridge that went missing, found it under my working table, re-attached it and now the BEC is working and no drops in voltage out coming from the wattmeter when something is hooked up.

Weird !
```

---
## \#18 Posted by: Sebastiaan Posted at: 2016-02-08T17:19:57.873Z Reads: 210

```
Picture update !

Refurbished the beat up board from Richard to something more .. awesome.
Removed the griptape also, gonna sticker it with custom grip.
<img src="/uploads/db1493/original/2X/f/fda577e120a47886bdf61ca6d13b66ab7e42a400.jpg" width="690" height="388">
<img src="/uploads/db1493/original/2X/a/a4c89c6fce01de1e99e53a952379348c1d802e9d.jpg" width="690" height="388">

Here you can see the BEC and receiver finally working : 
<img src="/uploads/db1493/original/2X/5/58a2ddd9b4e042c9487bee7675c3a42d8cc37211.jpg" width="690" height="388">  

And here i was fixing the small copper plate : 
<img src="/uploads/db1493/original/2X/7/7b9bffedd7e6a53c4ed6ba045b2afe02b09c85c8.jpg" width="690" height="388"> 

I've ordered these new shiny riserpads : 
<img src="/uploads/db1493/original/2X/0/053a3aa461ccae77f2ed438dab902355d24d6730.jpg" width="500" 
height="500">


And gonna coat the trucks in matte black instead of hippy purple :)

Updated electrical diagram. (Richard 'www.aliendrivesystems.com' wired this bad boy up)
<img src="/uploads/db1493/original/2X/b/bd97bcaf82805d2d2ba47bf3810b571de51be4b0.png" width="625" height="500">
```

---
## \#19 Posted by: Sebastiaan Posted at: 2016-02-10T11:46:31.484Z Reads: 207

```
These are the coated caliber trucks, also the motor mounts from aliendrivesystem.

Still working on these mounts, aiming for a cleaner look , also, the risers are gonna be milled down a bit to reduce them in thickness.

<img src="/uploads/db1493/original/2X/5/556c5b681d522ba98217f891672d0790a8a017fd.jpg" width="666" height="500">
```

---
## \#20 Posted by: Sebastiaan Posted at: 2016-02-10T16:38:29.070Z Reads: 207

```
Refreshed the griptape, one problem i've encountered, the griptape was not wide enough to cover the board.
I had some more carbon tape lying around and improvised a bit, 
currently its warming up on our central heating to make the tape stick better to the board.
And i have to cut off the sides ofcoure ;)


<img src="/uploads/db1493/original/2X/c/cfdcfde561e956b17e293fb2df52cd76bd0b0940.jpg" width="666" height="500">
```

---
## \#21 Posted by: Leonard Posted at: 2016-02-11T08:24:21.158Z Reads: 199

```
Love the carbon look of all your parts, what have you used to wrap the motor mounts?
```

---
## \#22 Posted by: Sebastiaan Posted at: 2016-02-11T21:24:30.892Z Reads: 196

```
I've used a simple carbon sticker foil, you can find them ultracheap on aliexpress, prepare to wait 2 - 3 weeks till they arrive though. 
I've received my batch in about 1.5 week which was fast, I'm located in Belgium.
Its a very good foil, a little thin, sticks very good to the surface.

http://www.aliexpress.com/item/Free-Shipping-127X30cm-3D-Black-Carbon-Fiber-Vinyl-Film-Carbon-Fibre-Car-Wrap-Sheet-Roll-Film/32314330964.html




I am looking for a solution on how to mount a case on my board, any suggestions?
Multiple solutions more than welcome.
```

---
## \#23 Posted by: Sebastiaan Posted at: 2016-02-15T17:08:15.368Z Reads: 196

```
Okay seems like a tight fit with the alien esc, i'm looking for a L type female to male bullet plug?
Does that exist?

something like this : 
<img src="/uploads/db1493/original/2X/1/10f9a5bb30173bf5c6f7b1ab21ca673ef42c77c6.jpg" width="625" height="500">

I mean the cornered connection, the dean plug has nothing of use.

I could use this as well, but i'm not sure i can bend the male plug into a 90 degree direction : 
<img src="/uploads/db1493/original/2X/6/6d7a0ce5fb904c8ac8de50863e4237453fcde167.jpg" 
width="565" height="414">
```

---
## \#24 Posted by: psychotiller Posted at: 2016-02-15T17:22:58.687Z Reads: 188

```
If you have a soldering iron and some heat shrink tubing you can make exactly what you want in about 20 minutes.
```

---
## \#25 Posted by: Sebastiaan Posted at: 2016-02-15T17:35:28.422Z Reads: 193

```
I was looking for the easy way out :smiley:

I will probably try it myself, the alienpowered ESC has 5.5 connectors
So i will need 

http://www.hobbyking.co.uk/hobbyking/store/__79661__Turnigy_High_Quality_10AWG_Silicone_Wire_1m_Black_EU_Warehouse_.html

http://www.hobbyking.co.uk/hobbyking/store/__44946__Polymax_5_5mm_Gold_Connectors_10_pairs_set_EU_Warehouse_.html
```

---
## \#26 Posted by: Sebastiaan Posted at: 2016-02-15T17:36:16.829Z Reads: 192

```
Current progress.

<img src="/uploads/db1493/original/2X/e/ea7b73568ec39a5de67f3656a14f2da124520903.jpg" width="666" height="499">
```

---
## \#27 Posted by: trbt555 Posted at: 2016-02-15T17:46:56.903Z Reads: 191

```
Strip the insulation off the wire for 5mm.
Tin the copper core first.
Solder the tinned core to your bullet connector in a 90 deg angle.
You will need quite some heat so a big iron.
```

---
## \#28 Posted by: Sebastiaan Posted at: 2016-02-15T18:01:04.650Z Reads: 189

```
Thanks, it is good practice to enhance my soldering skills i guess.
Already did some resoldering with the lightning modules and the SBEC. :smiley:
I have a 65 watt soldering iron, also some thick soldering wire. 
Gonna take a pic when it's finished without shrinkwrap so you can see if there are any points i could work on.

I will order this and desolder the T connector and solder the male and female together since the 5.5mm bullet plugs are not in stock in the EU warehouse.

http://www.hobbyking.co.uk/hobbyking/store/__43082__5_5mm_Bullet_Connector_to_T_Connector_Battery_Adapter_2pcs_bag_EU_warehouse_.html
```

---
## \#29 Posted by: psychotiller Posted at: 2016-02-15T18:52:06.927Z Reads: 181

```
[quote="Sebastiaan, post:25, topic:1174"]
I was looking for the easy way out :smiley:
[/quote]

Shame Shame...Hahaha
It's pretty easy, and you'll have the satisfaction of doing it yourself for much less money. And you don't have to wait for the post man!
```

---
## \#30 Posted by: Sebastiaan Posted at: 2016-02-18T16:48:54.300Z Reads: 180

```
This was easy.

<img src="/uploads/db1493/original/2X/c/ca554956f04594fc3faac5d7a87f51666a9240f3.jpg" width="666" height="500">



Now i'll just have to wait for the programming cable so i can program the ESC.
It worries me however, one of the inputs of the ESC was a bit loose when it arrived, probably due the mail service not handling it with care and trowing it around, not on the soldering however , it's a little bit detached from the circuit board, a small film of the board is loose on the battery connector
Can i superglue this without problems?
```

---
## \#31 Posted by: trbt555 Posted at: 2016-02-18T17:33:49.590Z Reads: 172

```
Can you make a picture ?
```

---
## \#32 Posted by: Sebastiaan Posted at: 2016-02-28T12:48:18.344Z Reads: 173

```
I've fixed it, it should not cause any issues in the future, everything is now supertight and super isolated.

<img src="/uploads/db1493/original/2X/3/3631195b793a58c1351667db3da007a2e0f9fb3e.jpg" width="666" height="499">

I still have to fix the gaps between the enclosures, I'm looking at some double adhesive thick sealing tape.

I ran into another problem though, did a testride, and the belt was touching the wheel so i needed to adjust the mount a bit, and damaged the threads .... 

<img src="/uploads/db1493/original/2X/4/43b5b5bd576436f26b9ccc7593c7ff036e858997.jpg" width="666" height="500">



should have a new UST aliendrive mount this monday, ***is it possible to run the dual esc with only one motor or is this dangerous?***

Also here is a picture of the old board, i disconnected the led strip but i still have to remove it, i'm looking at a programmable WS2801 strip that i would use on this board to experiment on.

<img src="/uploads/db1493/original/2X/8/86df5d30429ffc08da386c65fd476fb8d99e8bbc.jpg" width="690" height="388">

As you can see there were big gaps between the enclosures because i did not have room because i was using two BECs, one with 5v for the receiver and another one with 12v for the front, back and led lights.
```

---
## \#33 Posted by: Sebastiaan Posted at: 2016-02-28T13:03:02.702Z Reads: 169

```

<img src="/uploads/db1493/original/2X/a/ada4a2a4a32a8b97c054ec40906fa2c45173fd3e.jpg" width="281" height="500">

Now i still have this board that needs converting to anti-push... 

I'm looking at a single motor setup, long range, not ridiculously fast. (It's for my girlfriend)
It has Paris trucks. It also needs some griptape.
```

---
## \#34 Posted by: willpark16 Posted at: 2016-06-04T20:39:52.800Z Reads: 139

```
is this board still going strong?
```

---
## \#35 Posted by: Sebastiaan Posted at: 2016-06-04T22:51:50.746Z Reads: 138

```
It still is :) Just had to add more bolts to the battery compartment case, can't handle shitty Belgian roads :) Also the pulleys are now attached with loctite because the tiny bolts were not enough to keep the pulleys in place. Second board is on the to-do list ...
```

---
