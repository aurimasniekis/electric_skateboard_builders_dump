# Yin-Yang &#124; 3D printed dual mtb motor mounts \[Development\]

### Replies: 47 Views: 2546

## \#1 Posted by: notepad Posted at: 2018-01-11T03:25:45.342Z Reads: 333

```
As someone who wants cheap and cheerful, but then ends up spending wayy too much on parts just to fully bodge it up. It hurts when I see that mtb motor mounts are so expensive. so I thought I would try my hand at designing my own, which hopefully work and are much cheaper than the alternatives.

Luckily I got some Trampa Infinity trucks on the cheap so I can test the designs as they iterate.


----


The aim of the project is to make a dirt cheap, solid, motor mount that eventually can get versions to work for the most common types out there.  easy to make, easy to repair, easy to mod, and mostly cheap. (because my wallet definitely cannot afford quality stuff :P )
And luckily I own a pretty bawller 3d printer to test stuff on.

Currently this is what I have come up with. (real tests yet to come)

![mmountain_board_dual_trucks_2018-Jan-11_02-41-20AM-000_CustomizedView5356642790|666x500](upload://utY9a3nFgmwftpnVVjCHrD4T0ab.jpg)![mmountain_board_dual_trucks_2018-Jan-11_02-40-43AM-000_CustomizedView30653624108|666x500](upload://pSHs4wyfqlLCbzsYOyzvelNnwmS.jpg)![mmountain_board_dual_trucks_2018-Jan-11_02-39-35AM-000_CustomizedView29845955971|666x500](upload://cNZe0y2WkUfEplReHCZcobB4gkB.jpg)![mmountain_board_dual_trucks_2018-Jan-11_02-41-07AM-000_CustomizedView20546900198|666x500](upload://A23d0NDtgeBDtPS4TlgtQQYm0Bu.jpg)![mmountain_board_dual_trucks_2018-Jan-11_02-40-55AM-000_CustomizedView17239775023|666x500](upload://920aPKafoRHRri4fBCzt3PqnQoT.jpg)![Screenshot_31|690x421](upload://sRwDWjuJATTHALiblnciziQtLgK.jpg)

---

This current design is supposed to be used for dual motors.    The backing plate locks the mount into place as the trucks get larger the closer to the center they get, and can probably be modified later on to have a plate for lights and other LED goodness.
As for the material thats being printed, it would be PETG.  mostly because I have loads of rolls laying around, and im too lazy to worry about the hydroscopic tendencies of nylon yet is incredibly strong as an engineering material - especially printed completely solid.

---
![DSCF8633|666x500](upload://1tBRReNg7l96TWrhIvaGrgsOCOo.JPG)![DSCF8642|666x500](upload://rk1t0SUorqK8nVlKw7Oeiqss4Z0.JPG)![DSCF8637|666x500](upload://rW51YMQ5ST8VFmEGeSDYVxs5odk.JPG)

Other than the tempory bolts holding together the parts. the mounts feel super solid.
It was easy to assemble, and by the looks of it no strain on the mount themselves.

---

next is mounting them to a standard longboard so I am going to have to make some angled mounts that wont break instantly. But I am looking forward to it - if anyone wants to throw in some ideas they would like to see added just ask away, Ill see what I can throw up.  as for the current iteration, other than designing some indentations for the bolts and nuts, I think its ready for an alpha test.

.
.

**EDIT:** Completely forgot to mention the name.  I own two motors, one a high KV, one a low KV, im going to be testing them together to see if there are any benefits to multiKV setups.   That and my printer can print two things at once, and one can print in black, the other is in white, hence the name (and it cuts down on printing time)
```

---
## \#2 Posted by: kylepls Posted at: 2018-01-11T05:36:50.256Z Reads: 278

```
I've 3d printed a lot of stuff but I would expect a printed part to hold under the load that a typical motor mount is. The edges will probably wear in after a fair amount of accelerating and breaking and then the mount would be prone to fail during a hard acceleration/deceleration. I wouldn't want that to fail when I am going 20mph.

I also doubt 2 m4 screws are going to do the job.
```

---
## \#3 Posted by: High-roller Posted at: 2018-01-11T05:40:06.265Z Reads: 271

```
This is excellent work so far! Will you be sharing the Stl files or the full design files? 
I can't tell from the photo, are both mounts identical and you just flipped one over? Having them be symmetrical would be so much easier to work on.
I agree with kylepls that the material matters and you should perform some long term stress testing to see how it holds up over time.
 I'm working on fenders for trampa wheels at the moment, it'd be great to be able to design bolt holes or even the fender itself right into the mount!
```

---
## \#4 Posted by: notepad Posted at: 2018-01-11T15:49:43.382Z Reads: 240

```
[quote="kylepls, post:2, topic:43438"]
fail during a hard acceleration/deceleration
[/quote]

That is something I am semi worried about, no matter how I look at it the material is always going to be quite soft in comparison to aluminium.  when its mounted Ill see how far it can go before starting to fail.  it might just be simple enough to add washers to spread out the force.

[quote="High-roller, post:3, topic:43438"]
great to be able to design bolt holes
[/quote]

If you have the spacings for the mounting holes, I can see if I can impliment them, maybe even make an adaptor.  would be nice to make them compatible with other products.

after initial testing, Im probably going to remake them but printed in either Polycarbonate, or again in PETG but at 600Microns instead of 200,  it should streangthen the part substantially.
```

---
## \#5 Posted by: Der6FingerJo Posted at: 2018-01-11T16:39:47.757Z Reads: 214

```
Hey man, i see you followed through (we talked on reddit). I agree with @kylepls, you should try to add more/bigger screws and also consider grub screws. I'm using threaded inserts molten into the plastic for my 4 grub screws and they seem very solid. Otherwise i really like the look of the mount, very interested in seeing it in action! :D
```

---
## \#6 Posted by: notepad Posted at: 2018-01-11T22:46:27.257Z Reads: 195

```
Glad you like the look of it.  tried to keep it similar to what we know without doing something insane.  definitely going to try to add some form of grub screw based assistive locking - should increase stability a decent ammount)

one thing I am going to change is how far apart they are.  at the moment they only fit 11mm belts due to thicker pullys clipping the wheels tread, which I personally do not use, im a 15mm person, so I am going to try to change that up a little bit.

plus as to increase strength of the parts and reduce possible plastic damage, im going to try to thicken the parts and have indentations for the motor and other screw parts.

unfortunatly doing so would mean the motor doesnt have any adjustment, but it does mean I can thread all the holes, and probably add a belt tentioner if people would want to use one.
```

---
## \#7 Posted by: bimmer Posted at: 2018-01-11T22:50:46.944Z Reads: 166

```
Are you worried about printing the nylon or the properties during use? I'd say those made of taulman nylon or maybe carbonx would be pretty hard to break.
```

---
## \#8 Posted by: notepad Posted at: 2018-01-11T22:53:48.475Z Reads: 176

```
mostly the properties after printing,  when fresh they are super strong, but it absorbes water over time weakening it.   Cant really risk my life on a material that degrades when in moisture.  otherwhise it would be perfect.  the next material im tempted to test is Polycarbonate,  but thats only if this doesnt work.
```

---
## \#9 Posted by: FredrikHems Posted at: 2018-01-11T22:56:49.591Z Reads: 172

```
And If polycarbonate doesnt do the job (which I think it will) Try POM
```

---
## \#10 Posted by: bimmer Posted at: 2018-01-11T22:56:55.790Z Reads: 177

```
Hm I dont think it really weakens it  just  makes it crap to print with also you can anneal it after printing.
Also since strength is an Issue I'd make every 90 angle  that does not need to be one a radius.
```

---
## \#11 Posted by: notepad Posted at: 2018-01-11T23:02:32.260Z Reads: 182

```
[quote="FredrikHems, post:9, topic:43438"]
And If polycarbonate doesnt do the job
[/quote]

Im hoping it doesnt come to that because it would increase the price and remove the ease of modding.  but if it doesnt work, next would be injection moulded parts,  that way they can be much more dense and probably stronger.

edit: do you know where I could get that material, I havent heard much of it before.

@bimmer
You might be right on that.  I just dont want to risk it incase it does.  annealing is probably a good idea tough. going to do some research into correctly doing it!
```

---
## \#12 Posted by: Achmed20 Posted at: 2018-01-11T23:43:35.158Z Reads: 168

```
do yourself a favor and put metal rods as support inside the mount.
printed mounts on their  own will not hold with 6374 motors.  they usualy break on the plate where the motor is mounted on.

take a look onn my build diary for info on how "not" to do it :slight_smile:
https://www.electric-skateboard.builders/t/the-printa-6374-192kv-9s-5000mah-3d-printed-mount/22749/8
```

---
## \#13 Posted by: notepad Posted at: 2018-01-11T23:53:25.180Z Reads: 159

```
Very interesting read.  nice to see your development process. lots of stuff to keep in mind aswell.   First I am going to test what I have printed already to see how long before it inevitbly breaks, then change the design based around that!

The idea to inset rods into it is actualyl a good idea.   its cheap to get threaded rods so I might have a look at trying to get some of them!
```

---
## \#14 Posted by: Achmed20 Posted at: 2018-01-12T00:00:02.149Z Reads: 166

```
doesnt even need to be a threaded rod probably (shouldnt? because those are usualy made from iron). get those steel rods for RC cars, they will do the trick.

something like this.
https://www.amazon.de/gp/product/B00QC2DMKA/ref=oh_aui_search_detailpage?ie=UTF8&psc=1
```

---
## \#15 Posted by: bblacklock Posted at: 2018-02-10T03:51:54.842Z Reads: 147

```
Did you consider using the plus shaped default mounts that come with the 6374 and I think all of the SK3s? I'm working on printing a mount that attaches to the default mount so I can use PLA without it warping due to heat.
```

---
## \#16 Posted by: notepad Posted at: 2018-02-10T12:56:54.320Z Reads: 147

```
Personally I didnt consider it incase other people would want to use non sk3 motors which might not come with the backplate.  If heat isnt a problem, PLA with the right design should be fine.

at the moment devolopment has come to a standstill while the new machine is being renovated ( picture incoming - coke bottle for scale )
```

---
## \#17 Posted by: notepad Posted at: 2018-02-10T12:57:35.148Z Reads: 155

```
![IMG_2539|666x500](upload://tHzd0DurgbGOrhXsJzO0T1e7yYX.JPG)
```

---
## \#18 Posted by: FredrikHems Posted at: 2018-02-10T14:14:29.128Z Reads: 150

```
seems like some pretty big stepper motors for the X/Y axis.. What are those, nema 23?
```

---
## \#19 Posted by: moon Posted at: 2018-02-10T17:19:02.964Z Reads: 144

```
Will you be sharing the files? :sunny:
```

---
## \#20 Posted by: Acido Posted at: 2018-02-10T17:40:59.739Z Reads: 143

```
Maybe to make them stronger wrap them in fiberglass
```

---
## \#21 Posted by: notepad Posted at: 2018-02-10T18:17:09.684Z Reads: 134

```
@FredrikHems yup, Nema 23's and I can honnestly say they are massive,   £40ea with a holding torque of 1.26Nm  - Have a look [Here](https://uk.rs-online.com/web/p/stepper-motors/5350502/) for the motors.
They are going to be driven by a duetWifi when completed   

@moon   Im still considering it, it will be open source eventually but untill I can make sure its safe and working I dont want to risk other people beta testing for them to break on them and could cause seious harm.

@Acido  Thats a good Idea,  I have toyed with inserting carbonfibre wrap half way during the print to impregnate the parts with it.
```

---
## \#22 Posted by: moon Posted at: 2018-02-10T18:36:31.761Z Reads: 132

```
[quote="notepad, post:21, topic:43438"]
@moon   Im still concidering it, it will be open source eventually but untill I can make sure its safe and working I dont want to risk other people beta testing for them to break on them and could cause seious harm.
[/quote]

Probably the most responsible thing to do, I do have access to CNC machines to I was looking forward to see what can happen
```

---
## \#23 Posted by: notepad Posted at: 2018-02-10T21:25:13.770Z Reads: 131

```
After im fairly sure that the alpha version wont up and murder someone, ill start posting links to them for testers.  See what people like and dislike along with what people would like changed and added
```

---
## \#24 Posted by: moon Posted at: 2018-02-10T21:31:30.974Z Reads: 139

```
Cool, here is some inspiration.

The guy is doing similar stuff as you

https://www.facebook.com/ideatb/photos/a.965670716892345.1073741843.723191694473583/1095175123941903/?type=3&theater

Look at his other pictures aswell
```

---
## \#25 Posted by: moon Posted at: 2018-02-10T21:34:05.846Z Reads: 142

```
![image|690x434](upload://22619JK8X0eQpEGVhAoTNW45xT8.jpg)
![image|645x500](upload://cfQcWSOJrSqoA2s5HjwyEzPQm9y.jpg)
![image|666x500](upload://ks02KPLUScTHIZO0Ed1DpbHKQCX.jpg)
```

---
## \#26 Posted by: FredrikHems Posted at: 2018-02-10T21:35:05.036Z Reads: 141

```
Thats actully @Idea `s facebook. He have a thread about the mounts here one the forum :grinning:
```

---
## \#27 Posted by: High-roller Posted at: 2018-03-11T18:02:53.894Z Reads: 133

```
Hey, are there any updates to this project? I'm hoping you'll eventually post the stl files, I might try to make some add-ons to go with this design.
```

---
## \#28 Posted by: notepad Posted at: 2018-03-11T23:04:13.283Z Reads: 128

```
Hey @High-roller. I do appologise for the long delays in development.  Currently I have been building a Custom printer to make the prototype parts as my 'FlashForge Creator Pro' just isnt big enough for these large prints to keep it safe. 
![image|510x500](upload://ckn27bALj7V2RvpDHjzDKGTr4Wg.jpg)

It is fully built and operational. just getting it calibrated is taking its time. (TBH I though it would only take about 2-3 weeks to get it fully working, yet I started on this in december and its still not finished) If your interested I can post full details on the printer as I am planning on putting all the files on thingiverse.
```

---
## \#29 Posted by: FredrikHems Posted at: 2018-03-11T23:07:37.239Z Reads: 116

```
I would love to see more of the printer :drooling_face:
```

---
## \#30 Posted by: notepad Posted at: 2018-03-11T23:09:14.804Z Reads: 115

```
I guess an update post will be under way then :D  It is honnestly bigger than my coffee table. I am looking forward to a V2.0 as I have learned lots while building it.
```

---
## \#31 Posted by: FredrikHems Posted at: 2018-03-11T23:11:31.939Z Reads: 109

```
Did you convert your Flashforge, or did you start from scratch?
```

---
## \#32 Posted by: notepad Posted at: 2018-03-11T23:13:53.384Z Reads: 115

```
Start from scratch, The FF is a fantastic machine, but does have some limitations in the power and speed department. 
 I decided starting from scratch would be much nicer, and mean I can make it to function and keep the FF for smaller prints. plus this way I can have dual Titan Aero print heads, and the frame can be made out of 4545 extrutions. :D
```

---
## \#33 Posted by: FredrikHems Posted at: 2018-03-11T23:16:15.518Z Reads: 118

```
Will be looking forward for more information, and of course pictures! :wink:
```

---
## \#34 Posted by: notepad Posted at: 2018-03-11T23:17:18.927Z Reads: 118

```
Hopefully you might even get videos of its first prints.
```

---
## \#35 Posted by: High-roller Posted at: 2018-03-12T04:32:47.388Z Reads: 107

```
Nice, can't wait to see how it comes out! 
What are the build dimensions? I have a prusa i3 mk2, do you think that would be able to handle the print properly?
```

---
## \#36 Posted by: notepad Posted at: 2018-03-12T17:20:32.849Z Reads: 102

```
A mk2 should be able to print it loverly. it was originally supposed to be printed on a FFCP so build dimentions are only going to be slightly larger than that. if it can handle PETG it can print it.
```

---
## \#37 Posted by: notepad Posted at: 2018-03-14T13:03:04.190Z Reads: 96

```
Not going to lie. this build log for the printer is taking forever to word correctly. soo much information.
```

---
## \#38 Posted by: High-roller Posted at: 2018-11-04T06:44:42.542Z Reads: 59

```
Hey, what ever happened with this project?
Did you get your printer up and running?
```

---
## \#39 Posted by: notepad Posted at: 2018-11-04T11:45:48.571Z Reads: 70

```
so, Super Long story short. I did get the printer working, and it is amazing.  so good infact I decided to start a company to develop it further, because its the best damn printer I have ever used - and hopefully after 1 year of development, the printer will go live in a month or so.

As for the brackets, Ive currently just updated my ones to a V3 after having some problems with the clamp causing the brackets to skew,  so its been fully redesigned to be slimmer, and bolt into the grub screw holes on the axle for extra stability. (That and not realising I needed a 35deg deck made saving up for a new deck take forever)

Other than that,  In the coming weeks Ill be posting the .STL for the files as I find the mounts are bloody bullet proof with this new update, and with all the information of the new printer!
```

---
## \#40 Posted by: notepad Posted at: 2018-11-04T12:10:36.209Z Reads: 69

```
Since im talking about it, might as well do some shameful teasing of the printers functions (I cant show the test machines right now, But I will be able to soon)
![%C2%A3500_printer_design_2018-Jul-20_04-34-08PM-000_CustomizedView32703162683|666x500](upload://rmtjBciPiktRo24y1XqTIaxPl1r.jpeg) 

^^ This is the 14th Iteration from the first prototype. We havent decided on a name yet as all the good names are taken by bad kickstarter printers, so currently we just refer to her as "LE-350-P14".

My main aim is to release a printer that is going to shake up the printing eviroment showing you can get amazing performance without needing to sell your liver.  That being said, Ill list of the features then tell you the price point.

**FEATURES**

* 32Bit Wifi connected logicboard (DuetWifi Offical)
* 7" full colour touch screen display w/ sd card slot
* Custom E3D matte black Titan Aero w/ 0.6mm harderned steel Volcano upgrade & noctua cooling fan
* Custom Precision Piezo z sensor (Inbuilt into custom E3D hotend <- this is super cool)
* Full sensor less homing w/ 25 point auto bed & gantry levelling
* Custom plasma cut ar400Steel brackets (no acrylic or aluminium here)
* Spring steel insert-able plate (Just like prusa mk3's) with PEI pre-applied
* Full Aluminium frame & 5mm laser cut acrylic enclosure
* Rear storage compartment for hiding wiring and ample space for easy modding
* **True CoreXY kinematics**
* 11mm highquality gt2 belts
* print volume of 350^370^530

**Sale Price £599**

As you can probably tell, we have crammed in as many high end features we can into a price point sub £600, without compromising quality.   With the use of the DuetWifi mainboard, and custom E3D hotend, we can print roughly 230% faster than the competition, and have prints that are more accurate, and stronger to boot!
```

---
## \#41 Posted by: High-roller Posted at: 2018-11-04T12:17:19.795Z Reads: 58

```
Damn, that looks good and tempting! Is this going to be sold as ready to use out of the box, or will there also be a kit? Open source/ open materials?
```

---
## \#42 Posted by: notepad Posted at: 2018-11-04T12:22:48.629Z Reads: 56

```
Im currently thinking a bit of both, as some of the components are more likely to get damaged in shipping that others if pre assembled due to its size - and it might save some £££ on shipping a large box around.   

That being said, the current version only take roughly 1-2 hours to assemble from scratch. and I personally think if you assemble some parts like the hotend for example - people would be less scared to switch out nozzles to try something new.

As for open source, I forgot to mention this above,  but all the design files, all the suppliers, all the custom code **will be made available**, including my personal journals about what problems I ran into while developing this (whenever I get around to typing it up)
```

---
## \#43 Posted by: High-roller Posted at: 2018-11-04T12:30:07.313Z Reads: 48

```
I built my prusa from a kit, I have no problem with doing it again. And the savings are definitely a plus 😉
Could you show us some samples or videos so we can get an idea of what it'll be like?
```

---
## \#44 Posted by: moon Posted at: 2018-11-04T12:38:26.660Z Reads: 55

```
What goes into designing and making a 3D printer? Incoming stupid questions

Are you designing a sturdy frame and platform. And other stuff like levelling etc 

Then using good off the shelf parts? Or is there more to it
```

---
## \#45 Posted by: High-roller Posted at: 2018-11-04T12:43:28.668Z Reads: 55

```
@moon none of those are stupid questions, these are things that we need to know before we buy.
Here's another one for you @notepad:
If I'm reading the pictures right, the z-axis moves the whole bed, rather than the extruder, right? How many steppers+worm gears are you using? Or is it something else?
```

---
## \#46 Posted by: moon Posted at: 2018-11-04T12:44:52.351Z Reads: 56

```
Yeah I just like to know how stuff are designed, just to learn something..
```

---
## \#47 Posted by: notepad Posted at: 2018-11-04T12:51:38.092Z Reads: 59

```
@High-roller I cant show any more just yet as we only just started doing the promotional material about a week ago, and the final 2 prototypes have been shipped away for EU certification.

@moon tbh making a printer is super easy,  its ironing out the little quirks each design has is where it becomes time consuming and difficult.   At first I purchased a handful of the more "premium" printers to see how they overcame problems, which covered versions 1-10, before moving onto how the sub£300 printers are manufactured.   And surprisingly enough, those cheaper ones had much better frames than the more expensive ones.

The main problems actually come down to the flex materials have, hence why we are now using ballistic steel (its like 5p more expensive than mild steel,  why not use it :D ) for the brackets, and removing and 90deg brackets for the frame and instead threading the aluminium itself and bolting them together.

Theres lots of weird design choices that end up being surprisingly effective - don't hesitate to ask any questions, ill be more than happy to answer.

@High-roller  yes you are right, the bed is what moves in the z direction.  

 Currently we have decided to go with only one stepper with a 4mm pitch lead-screw. 
we did test having 2 screws with 4 linear rods for constraint, we even tested replacing two of the linear rods with the screws themselves (which worked out surprisingly good, so we might do that for a larger printer)   but after lots of testing, the machine didn't have any negatives with only using 1 z-axis motor with proper 4 linear rod constraints.    Mix in the 25 point bed levelling and even the slightest bit of misalignment is corrected in software.
```

---
