# SNAGGLEPUSS &#124; *REBUILD TO ARBOR HIGHGROUND* &#124; Dual 6354 &#124; Dual Ollin VESCs &#124; Mini Remote &#124; Dual DIYv4 Mounts &#124; DIY 13/36 &#124; 8s3p 9Ah Zippys &#124; 44d Caliber IIs &#124; 97mm ABEC11 78a Flywheels &#124; Kydex Box Enclosure

### Replies: 44 Views: 4770

## \#1 Posted by: SageTX Posted at: 2016-12-11T02:45:47.588Z Reads: 436

```
Bought and slightly changed @jwoodsentertainment 's deck and components he had for sale.

Changed to 8s because this is my first elec build. Used Balance Board from SuPower, bypassing current limit for charging. 

SOLVED Can't get Mini Remote i purchased from @JLabs to bind. (surely something stupid, but kicking myself here) SOLVED

SOLVED Added Battery Capacity meter (currently not working (I may have it wired in wrong)) {Nope, well technically yes, but the leads that came with the monitor were in backwards.}


I've gotten most of the hardware installed and enclosure made.  Electronics wired.  I'm wanting to do @Ackmaniac 's watt control mode version of the VESC firmware and this is where I'm hitting information overload.  I have watched the VESC firmware tutorials until I can't see straight. 

I have updated the firmware. no problem there.

Motors detected and seem to be fine, but when detecting hall sensors is says failed. I rewired the sensor wires in order (as far as I know they are correctly connected to VESC, but I would like a confirmation).  

Too many numbers to for setting limits.  I'm just confused here.  I follow ESK8 supports video, but get confused every time he mentions hub motors and dont change this or that,  I would really appreciate some simple settings for Dual 6354 (from @JLabs Group buy) and Dual Vesc Settings with 8s 20c lipos.

Uploading a few  pics of build now and could upload VESC setting screenshots, but they are DEEFAULT @Ackmaniac 2.52 settings right now EXCEPT for controller ID set to 0(the one with the ppm receiver attached) and 1(the other one).  

I do have a BTLE 4.0 nano board I would like to hook up, but can't remember where I saw the thread and the information to hook it up correctly.

Thanks for anyone that helps, I will greatly appreciate any insights I can get.
```

---
## \#2 Posted by: SageTX Posted at: 2016-12-11T02:50:45.565Z Reads: 423

```
<img src="/uploads/db1493/original/3X/a/8/a89b2887e3b9fd40aeea6fa4ce885a0564e70108.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/2/1/21b30f50e15dd5ea311c4487a2c0c935fd230a31.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/e/0/e0bf0ee519e36e27f934acd30dba45c18d532012.jpg" width="690" height="388">
```

---
## \#3 Posted by: JLabs Posted at: 2016-12-11T03:00:28.159Z Reads: 409

```
[quote="SageTX, post:1, topic:14482"]
Can't get Mini Remote i purchased from @JLabs to bind. (surely something stupid, but kicking myself here)
[/quote]
I bind and test the remotes before sending so you should have received it plug and play. Make sure you have the cable plugged into channel 2 in the correct orientation, and then power on the receiver.
1. Turn off the controller
2. Hold in the bind or pair button on the remote
3. Power on the remote
4. Release the bind button when the led inside the receiver blinks
5. Your all paired and ready to go (there are also paper instructions included in the package)
```

---
## \#4 Posted by: SageTX Posted at: 2016-12-11T03:34:32.253Z Reads: 387

```
THANK YOU!! I was trying to bind it using the bind plug. Definitely Connected now.  On to VESC Settings.
```

---
## \#5 Posted by: SageTX Posted at: 2016-12-11T05:03:33.914Z Reads: 394

```
OK Some Preliminary VESC Settings...
VESC 0 / Motor 0
<img src="/uploads/db1493/original/3X/2/f/2f51a59fe60ee964bf623c28440d23ba662bda82.png" width="690" height="387"><img src="/uploads/db1493/original/3X/4/4/444e51c584b27685fbd4d9fdbd00faf6c88e6f2e.png" width="690" height="387"><img src="/uploads/db1493/original/3X/3/3/3322592b27f11d4eadb192db4d43959d3c35c9d5.png" width="690" height="387"><img src="/uploads/db1493/original/3X/4/a/4a242164580e551afe6111b1e8741b9f515063f2.png" width="690" height="387"><img src="/uploads/db1493/original/3X/d/3/d3451160247395b71aef665f56815719f058a517.png" width="690" height="387">
```

---
## \#6 Posted by: SageTX Posted at: 2016-12-11T05:04:15.885Z Reads: 336

```
Vesc 1 / Motor 1
<img src="/uploads/db1493/original/3X/e/4/e477026c76d79bb5f478dae005ece7e6d189bb48.png" width="690" height="387"><img src="/uploads/db1493/original/3X/2/4/24f8c7241f8346029e474ac69e389ac9d2ff4738.png" width="690" height="387"><img src="/uploads/db1493/original/3X/b/2/b26f37c71e4db401b5dc5c9ea4351358f28049b7.png" width="690" height="387">
```

---
## \#7 Posted by: Blasto Posted at: 2016-12-11T05:05:24.093Z Reads: 279

```
Sorry i did not read the whole thread, but set your max input voltage to 57V, on both vescs
```

---
## \#8 Posted by: SageTX Posted at: 2016-12-11T05:06:31.988Z Reads: 288

```
Even with 8s? Thought it's 8 * 4.2 = 33.6
```

---
## \#9 Posted by: lox897 Posted at: 2016-12-11T05:08:24.160Z Reads: 285

```
It's safer because if you have a voltage spike it could shutdown your board. Also, the vesc's maximum input voltage is 57v so why not?
```

---
## \#10 Posted by: Blasto Posted at: 2016-12-11T05:08:50.726Z Reads: 286

```
[quote="SageTX, post:8, topic:14482, full:true"]
Even with 8s? Thought it's 8 * 4.2 = 33.6
[/quote]

Always, it is a safety feature that seems to cause more problems than prevents them
```

---
## \#11 Posted by: SageTX Posted at: 2016-12-11T05:11:10.436Z Reads: 268

```
OK i get it.. 57 is the max the VESC will take, even though My batts will only give 33.6.  Gotcha.
```

---
## \#12 Posted by: SageTX Posted at: 2016-12-11T05:13:07.376Z Reads: 262

```
Maximuim Input Voltage set to 57.00v on  BOTH VESCs.  :+1:
```

---
## \#13 Posted by: SageTX Posted at: 2016-12-11T05:28:05.646Z Reads: 264

```
Solved Battery Capacity Monitor.  Bad Wiring Leads
```

---
## \#14 Posted by: SageTX Posted at: 2016-12-11T05:29:48.342Z Reads: 281

```
Now.  Hall Sensor Wires.  Any Pointers???  :nerd:
```

---
## \#15 Posted by: SageTX Posted at: 2016-12-11T05:58:51.885Z Reads: 316

```
<img src="/uploads/db1493/original/3X/7/9/7996735696cb9f66ea3dc355c3e910181cdf243b.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/e/b/eb73cc31f35b3032ae9f371831f86c595023f2ef.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/b/5/b57e5854ee4b98dbf4961b3e3067e73bdd5017aa.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/d/a/da462e6011228f815a5b33af50207fb0970ad9eb.jpg" width="281" height="500">
```

---
## \#16 Posted by: SageTX Posted at: 2016-12-11T06:08:33.649Z Reads: 298

```
[It's Alive!! Alive!!!!!](https://youtu.be/EKJEoUhUyhU)

OK.   Most is working,  just want to be sure my settings are correct before I try to ride it.  
Left off Sensor wires and kept it in sensor-less.  Would like to run Sensor-ed FOC but I need to understand those settings first.

Thanks for the all the inspiration and help from the community,  If it looks like I took an idea from someone, I did.  None of  the ideas I had for the board were mine originally, I just picked and chose what I thought would work. Again -- this couldn't have been possible without this forum.  Sincerely,  Thanks. :joy:
```

---
## \#17 Posted by: jwoodsentertainment Posted at: 2016-12-11T06:45:47.422Z Reads: 278

```
Nice job looking really good!!!!
```

---
## \#18 Posted by: SageTX Posted at: 2016-12-11T07:03:09.566Z Reads: 281

```
Thanks!  
Not to proud of the enclosure, except - -  I made it!  Really sloppy compared to others, but maybe that'll get a redo. Again, thanks for bringing the parts together.
```

---
## \#19 Posted by: Ackmaniac Posted at: 2016-12-11T10:41:52.525Z Reads: 291

```
Do the motor detection correctly.
You have to run the motor detection and afterwards you have to press the apply button.
Then you have to press the "Write Configuration" Button.
But you have to **disbale** the PPM control mode for that. Otherwise your remote would disturb the motor detection. maybe that was also the reason for the wrong hall sensor detection.
Correct values in your case would be Integrator limit = 130 and BEMF Coupling = 900
<img src="/uploads/db1493/original/3X/3/5/357e695afc33f93ca1ea44db18ba8a1f4b799365.png" width="690" height="387">
```

---
## \#20 Posted by: Ackmaniac Posted at: 2016-12-11T10:53:24.123Z Reads: 273

```
And your battery cutoff start and end is a bit too low for lipos.
I recommend to strat the ctoff at 3,6V (8S * 3,6V = 28,8V) and set the end to 3,4V (8S * 3,4V = 27,2V) per cell. Li-ion batterys could go lower.
And you should adjust your PPM Pulsewith settings. Because i don't think that the standard ones are correct.
First set the Control mode to disabled.
Then active the Display checkbox. So you will see the PPM signal from your controller.
Then set the center Pulsewidth to the value that stands there when you don't touch the throttle on the remote.
Then the minimum to the value when you brake fully and the maximum to the value when you give full throttle.
Don't forget to write these settings and activate the Watt control mode again.

<img src="/uploads/db1493/original/3X/e/e/eeac24ae616632ea69a24cee5a15a0e2fd2b0506.png" width="690" height="390">
```

---
## \#21 Posted by: SageTX Posted at: 2016-12-11T16:13:38.202Z Reads: 226

```
Redid Motor Config :  Integrator limit came to 127.17 and rounded down to 125. That OK?
Also hall sensor detection failed. and wont spin in hybrid mode.  changed back to sensor-less and unplugged h s wires.

PPM settings :+1:

Is the Max Watt setting accurate for Dual Motors? (1200)
```

---
## \#22 Posted by: Ackmaniac Posted at: 2016-12-11T16:39:47.620Z Reads: 234

```
you have to calculate battery amps * battery S * 3,7V (3,6 for li-ion)

So in your case 25A * 8S * 3,7V = 740W

If you want it powerful then set your battery max for both vescs to 40A and set  max watt to 1184W.
```

---
## \#23 Posted by: SageTX Posted at: 2016-12-11T21:58:39.752Z Reads: 238

```
Oh man! That was awesome! Took my first ride to the truck to go to work. The skys cleared , beaming sunshine down on Texas for a maiden run in the 70°s (f).  

I went with the low wattage setting, and soft limit the erpm to 35000 for now. (about 15mph / 25kph). Seriously, I don't know how you guys are looking at 25mph+ boards.  That's seriously fast!  

It was so sweet cruising  up to the truck, right to the door, packing it up, and off to work. My dream come true! 

Still  looking for hall sensor help, but I'm on the road now and can't adjust things fast/ take quick pictures, but I I'll do what i can.
```

---
## \#24 Posted by: SageTX Posted at: 2016-12-28T02:24:40.794Z Reads: 222

```
@Ackmaniac - moved to my build thread for clarity and not to muck up your thread --

 [quote="Ackmaniac, post:448, topic:12286, full:true"]
Seems that you don't give full power. And your gearing is quite short. Because at 21 miles you reach max speed already.So you also see that you only need like 450 watts for 21 mi/h (34 km/h). Most people think they draw full amps.
[/quote]

No. I do not  give full power.  I only weigh 135 and that would put me on my butt.  I am slowly getting more confidence to squeeze harder, but the added power is appreciated on hills. I definitely over-engineered my board.  But with your firmware, I have tamed it until I can take full advantage.

The gearing is 13/36. I have 97mm wheels. With my weight, I figured there was enough torque but ability for speed.  But it seems to stop at 21MPH no matter the settings.  Maybe that's the max for 8s?

----------------------------------
Well according to the ESK8 calc, TOP speed is 23.07 18.46 weighted.  So I guess I'm pretty close.
```

---
## \#25 Posted by: Ackmaniac Posted at: 2016-12-28T08:26:12.188Z Reads: 219

```
The reason for your topspeed is the 8S Battery. But you can modify your battery's easily to a 12S with 6Ah. So you would get 50% more speed. But you should set the max ERPM in the motor settings to 60000 if you have 190kv motors or higher. You will not reach those ERPM's on the street but on the bench. And you should switch off the "Limit ERPM with negative torque" to be safe. Because if you reach those speeds on the street you do not want to start braking. The VESC should simply don't give any power anymore.

<img src="/uploads/db1493/original/3X/c/0/c057d6bb5e35c329a1903b90f1406c52c554153f.png" width="690" height="421">
```

---
## \#26 Posted by: SageTX Posted at: 2016-12-28T16:01:47.424Z Reads: 190

```
Thanks, and great info.  I will probably rewire my batteries in the future, but for now 22mph is fast enough!!  :checkered_flag:
```

---
## \#27 Posted by: mason Posted at: 2017-01-01T21:11:33.712Z Reads: 182

```
you're in TX? where at? we should ride
```

---
## \#28 Posted by: SageTX Posted at: 2017-01-01T21:43:00.112Z Reads: 177

```
Fort Worth, but I'm out of town A LOT.   Where are you?
```

---
## \#29 Posted by: mason Posted at: 2017-01-01T21:54:39.732Z Reads: 170

```
McKinney :/
```

---
## \#30 Posted by: SageTX Posted at: 2017-01-01T22:01:44.426Z Reads: 171

```
That's not too bad, if I'm out that way I'll hit you up. 😎
```

---
## \#31 Posted by: mason Posted at: 2017-01-01T22:21:55.276Z Reads: 169

```
Even if not, we can meet in-between. I know a few other guys in the Dallas area that I could contact for a group ride.
```

---
## \#32 Posted by: SageTX Posted at: 2017-01-22T23:50:23.276Z Reads: 165

```
I have finally figured out the sensor wires from the motors, and thanks to @Ackmaniac's new update to the BLDC tool, I have set up FOC mode with sensors with the no-miss tool tips.  Things are coming together for this hobby!!  

Gotta go for a test drive!!
```

---
## \#33 Posted by: SageTX Posted at: 2017-01-23T00:36:41.931Z Reads: 175

```
Aaaaaand.. SUCCESS!  Man that's smooth.  And super quiet!
```

---
## \#34 Posted by: SageTX Posted at: 2017-04-29T15:38:38.242Z Reads: 150

```
Well... she snapped in two!

<img src="/uploads/db1493/original/3X/a/b/abc7701a752cbccbebcc6732fb16ba1b3d540309.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/b/0/b0c40e5df5a03da2210a15979a0aff82e6d105ec.jpg" width="690" height="388">  

Gonna have to transfer the guts to a new deck.
```

---
## \#35 Posted by: SageTX Posted at: 2017-04-29T15:58:59.803Z Reads: 148

```
Bought this to replace the deck.

<img src="/uploads/db1493/original/3X/a/f/af6f6ae01db6447c07fd08fe01c64e7c6583b9db.jpg" width="304" height="500">
```

---
## \#36 Posted by: Tuomalar Posted at: 2017-04-29T16:26:59.279Z Reads: 140

```
How did that happen?
```

---
## \#37 Posted by: SageTX Posted at: 2017-04-29T16:35:47.354Z Reads: 145

```
Welly its a really cheap deck to begin with.  I expected it at some point.  The weak point was at the holes for the truck mounts.  There are small cracks along the length of the deck around both the front and back mounting points.  

It happened at very slow speed though,  just a walk off when I heard the motor mounts start to scrape. I thought i had tun something over and it was dragging.  There are a few potholes / pavement cracks that I have to hit on my way to work. I'm sure this was the cause of the stress that cracked it.
```

---
## \#38 Posted by: SageTX Posted at: 2017-04-29T16:37:08.284Z Reads: 151

```
It didn't help any that the deck was a drop through mount.  That hole is definitely a stress riser.
```

---
## \#39 Posted by: ATLesk8 Posted at: 2017-04-29T22:00:37.290Z Reads: 164

```
Well your replacement (arbor highground) is an awesome choice. I have one with dual hubs and I love it.
```

---
## \#40 Posted by: SageTX Posted at: 2017-05-09T00:08:14.174Z Reads: 160

```
**_THE REBUILD_**  
She gave all she could.  Time to get a new deck.
<img src="/uploads/db1493/original/3X/e/0/e02e9e4cdda3be279e7907349f384b613291bd2a.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/0/3/032844d313725137ce01c67924298ea486e2345c.jpg" width="281" height="500">

Strip her clothes off!!

<img src="/uploads/db1493/original/3X/2/b/2b4a8688c098d6d2644c1525aa7e63d09a3804ae.jpg" width="281" height="500">

NSFW Guts Exposed!

<img src="/uploads/db1493/original/3X/5/b/5bbc842e87b7c4201d27edeb93efa808b84457fa.jpg" width="281" height="500">

Lined up the old box for some new recessed screw holes with brass inserts.

<img src="/uploads/db1493/original/3X/7/6/7657530ab9f83b5ad96fb1bd7c75edef0f11f29c.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/5/e/5e6be18825877d8a8207e2b4057f63785222f802.jpg" width="281" height="500">

<img src="/uploads/db1493/original/3X/c/4/c4594c420964eb357a6479c8fa244b111f5f36da.jpg" width="281" height="500">

That'll do just fine!!

<img src="/uploads/db1493/original/3X/b/f/bf6ebd0f8bdabe4450ad1f6153d00cc6839153f0.jpg" width="281" height="500">

I got really into the weatherseal. That was a PITA. Forgot I was taking pictures of this re-do.
I put a coat of paste wax on the exposed bottom and the wheel wells. Hoping this will repel whatever water might get splashed.

<img src="/uploads/db1493/original/3X/3/8/38d2e9b0ec361df93d2ced66a1193ff3e6868a3f.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/0/8/083d7bdf9a256b61abaebf61930e96eda834d531.jpg" width="281" height="500">

All Done!

<img src="/uploads/db1493/original/3X/b/a/bad23093d90889740127345783eb3c6745d15d08.jpg" width="281" height="500">

Check out that W concave!
<img src="/uploads/db1493/original/3X/4/0/402350ab5e79cc2ea933615138cfaab6fdf4687c.jpg" width="281" height="500">

Charger Attached for the next ride!

<img src="/uploads/db1493/original/3X/9/1/91dc0cfbed6c657d365709a2f9265b8a76d8b12d.jpg" width="281" height="500">

I was sooo worried the 97 ABECs would bite.  Didn't have a problem. I left the risers on because of the motor mount clearance.  NO BITES on the test run!  Back in business!!

<img src="/uploads/db1493/original/3X/d/0/d0221c709bce9bee0457f5522ff0cbf2a1b285ea.jpg" width="281" height="500">
```

---
## \#41 Posted by: tueboard Posted at: 2017-05-09T08:05:09.399Z Reads: 140

```
awesome board! i really like this kind of bolts makes de board clean and simple.

can i ask you which kind of bolts-screws and the size of these?
https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/5/e/5e6be18825877d8a8207e2b4057f63785222f802_1_281x500.jpg

i saw a lot of types and sizes on ebay but i don't know which one to choose
http://www.ebay.es/itm/M4-M5-M6-M8-M10-TYPE-D-METRIC-THREADED-WOOD-SCREW-INSERT-NUT-WITH-FLANGE-/191750463922?var=&hash=item2ca537e1b2:m:m669gMzKOcRxQr5WR-k6Elg

thanks
```

---
## \#42 Posted by: SageTX Posted at: 2017-05-09T14:09:50.009Z Reads: 125

```
Well I purchased them when I only knew the depth of my deck in inches and was really guessing, even thought they turned out perfect.  
They are 1/2" 8-32 socket head cap screws - 
and 1/4" deep inserts.  
Measured, the screws are about M4s approx 12mm and the matching inserts are approx 9mm deep.

Just get inserts that are less than the depth of your deck.  I would think M5s would be better, I had to use a small rubber/metal washer on the top to keep them from pulling through.

Also a TIP --  Cut a screw as close to the exact length of the insert.  After drilling holes to depth (just _barely deeper_ than the inserts)  put the screw in the insert and screw them into the board with that.  DONT use the slot on the top, It'll snap in half.    Then just back out the screw and use it for the next one.
```

---
## \#43 Posted by: Wolfcola Posted at: 2017-05-12T22:06:03.043Z Reads: 111

```
Whoa. Was about to get this deck because I also have 97mm wheels was scared of wheel bite. But if you say its all good I might just pick it up then.
```

---
## \#44 Posted by: SageTX Posted at: 2017-05-12T22:22:38.431Z Reads: 111

```
Just some info, in case it matters..  
I just cruise, no hard carving. There is a spacer for the motor clearance.  However i have 44 deg calibers.  But i couldn't get them to touch standing still and trying hard. Those wheel wells are the key I think.
```

---
