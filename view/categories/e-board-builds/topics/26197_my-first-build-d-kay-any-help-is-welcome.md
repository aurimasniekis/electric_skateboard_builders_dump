# My first build ( d-kay) (any help is welcome)

### Replies: 35 Views: 2983

## \#1 Posted by: d-kay Posted at: 2017-06-26T11:43:15.172Z Reads: 244

```
hey all
I am looking to build an electric skataboard that would beat evolve.
After doing some research I desided on using these  motors in dual drive. Please leave any comments on them.
KEDA 63-64 190KV Brushless Outrunner 10S 2000W
I am buying them at hobby king. Does anyone know where I could get them cheaper or other motors with about the same specs that are cheaper? I live in Belgium.
https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html 
Furthermore I have some questions on bateries.
1: does the discharge in Ah go up if you connect bateries in series or in parallel?
2: if you connect  two the same batteries in parallel does it double the outcoming voltage?
at the moment I am thinking about putting two packs of two of these bateries in parallel.
is that a goed idea or does anyone have a better posibility?
could you tell me how to charge al these bateries at once?

Could someone please tell me what I should use an ESC or VESC and how to connect them?
Could you also tell me witch ESC or VESC I schould use.

at last does anyone know a goed controller with buttons ( as the evolve gt controller )for the board so I can program different speed modes?

Thanks in advance for your help.
```

---
## \#2 Posted by: d-kay Posted at: 2017-06-26T11:44:22.075Z Reads: 233

```
i forgot to mention witch batteries.
it are those
https://hobbyking.com/en_us/zippy-flightmax-5000mah-6s1p-30c.html
```

---
## \#3 Posted by: pat.speed Posted at: 2017-06-26T12:00:38.582Z Reads: 241

```
Hey dude, 

I have that same motor on my board that I've been using for the last few weeks. It's great pulls me up any hill I come to although I do have a 3:1 gear ratio. The only complaint about this motor is that I don't think it is actually 190kv. I am running it on 6s now 5s because one of the cells died and I get 22kmh. The Speed calc I used said I should only get about 18kmh so I think it is around 230kv
```

---
## \#4 Posted by: Challlsss Posted at: 2017-06-26T13:58:12.601Z Reads: 223

```
Yo what? [quote="pat.speed, post:3, topic:26197"]
one of the cells died
[/quote]

How TF do you just "run it on 5S" pretty sure it doesn't work that way homie. (unless it's a Liion?)

@d-kay In response to your questions. 
1) Parallel
2) No
3) I'd recommend going a little deeper into the forum hint* use the search button and find some older threads asking about how batteries work. With an hour of time you should have a very good grasp on exactly what system you should get.
just from looking at what you have postied I'd recommend looking up stuff about 10S Lipo systems
```

---
## \#5 Posted by: pat.speed Posted at: 2017-06-26T21:46:31.709Z Reads: 188

```
What I meant is that one of my LiPo cells got over discharged so I opened the pack up and disconnected the bad cell and resolved the other 2 back together so now I have a 2s and a 3s in series to give 5s. Sorry for hijackjng your thread a bit. @Challlsss is right about the other stuff though
```

---
## \#6 Posted by: Alanhunt123 Posted at: 2017-06-26T21:49:58.615Z Reads: 179

```
Looks like that motor you found is out of stock. Unfortunately, a fair price for 63mm motors starts around $65. Hobbyking seems to be out of all their 63mm motors at the moment, but you can find some decent ones from  or from Ollinboards. I'm sure someone else can chime in for some more options!
```

---
## \#7 Posted by: pat.speed Posted at: 2017-06-26T22:02:14.752Z Reads: 167

```
It is in stock but is only available in Aus lucky me😉
```

---
## \#8 Posted by: Challlsss Posted at: 2017-06-26T22:06:03.659Z Reads: 166

```
@pat.speed Wow man props. When my cell died I got scared to use it so I took a hammer and nail poked a hole and filmed it haha.
```

---
## \#9 Posted by: pat.speed Posted at: 2017-06-26T22:09:30.453Z Reads: 169

```
Hah nice I'm gonna do that with 2 bad cells I have just need to find somewhere safe to do it
```

---
## \#10 Posted by: d-kay Posted at: 2017-06-27T06:36:58.044Z Reads: 155

```
thank you for the information I will caclculate that in.
```

---
## \#11 Posted by: d-kay Posted at: 2017-06-27T13:08:09.105Z Reads: 149

```
how do you connect two ESC's or VESC's
```

---
## \#12 Posted by: d-kay Posted at: 2017-06-27T16:53:31.440Z Reads: 143

```
how do I double the volts @Challlsss
```

---
## \#13 Posted by: d-kay Posted at: 2017-06-27T16:57:01.788Z Reads: 139

```
or enlargen it @Challlsss
```

---
## \#14 Posted by: wafflejock Posted at: 2017-06-27T17:42:24.343Z Reads: 151

```
@d-kay you should research some more on batteries and connecting them in series vs parallel there is a ton of information on the forum and on the internet in general about this.  You shouldn't mess with these batteries if you don't know what you're dealing with just buy a prebuilt pack that is made for what you want (you'll still need to have a basic understanding to make an informed purchase).

The answer to your specific question is you add more batteries in series or more cells in series to increase the voltage (stack a couple of AA batteries together an use a voltmeter to see, can also do them in parallel, use some foil and tape can make simple connections to test things with lower voltage safe(r) stuff).  A battery is really just a collection of cells in series (S) or parallel (P), with LiPo chemistry the cells have a fully charged voltage of 4.2V and are typically mostly drained at 3.7V.  Min voltage per cell is actually around 3V but there can easily be a half volt sag while the battery is under load (supplying power to the motor).  Typically RC enthusiasts who want their batteries to last will only usually drain 80% of the total capacity of the battery to avoid dropping any individual cell in the pack below the minimum safe voltage.

When you put batteries in parallel you don't increase the voltage (they are just both applying their voltage to the lines their attached to), but you are drawing current through both the batteries so you increase the amount of current you can safely draw if you have more cells or batteries in parallel (you also add the Ah in parallel, in series you are only adding voltage not Ah, can think of Ah as amount of fuel in the tank, measured in terms of how much current you can draw for how long before empty).  The RC style LiPos are typically rated with a C rating, the C rating relates max safe amperage drawn from the battery to the capacity of the battery.  A 5Ah battery with a 20C rating can have 5*20 = 100A current load on it.

For the most part the safety concerns are if you short things out the battery will deliver that 100A+ through whatever is shorting and quickly turn whatever is in the path into vapor (releasing a lot of light and heat in the process, or worse the battery itself goes up).  So if you do start working on the batteries or taking off leads be sure you know what you're doing, you can also buy premade series connectors or parallel connectors to join the batteries together if you aren't confident in your knowledge of working on the batteries (it's somewhat high voltage stuff and you're probably going to need to solder it which means you're dealing with melting lead/tin on live leads).

---
Edited a few times to add some details, just added link as well for more explanation on batteries and various chemistries available.
https://learn.sparkfun.com/tutorials/battery-technologies?_ga=2.120028872.1972349059.1498586180-994420620.1490732809
```

---
## \#15 Posted by: d-kay Posted at: 2017-06-27T18:08:54.108Z Reads: 118

```
I am thinking about using 10s2p richt now
```

---
## \#16 Posted by: Challlsss Posted at: 2017-06-27T18:26:30.684Z Reads: 117

```
Do your research. You will thank yourself later when you realize how many mistakes you avoided.
```

---
## \#17 Posted by: d-kay Posted at: 2017-06-27T20:33:44.537Z Reads: 117

```
I have a question 
how do you improve the amount of amp hours without enlargening the amount of current flow or the amount of volts @Challlsss
```

---
## \#18 Posted by: Challlsss Posted at: 2017-06-27T20:52:44.749Z Reads: 115

```
amp hours is the size of the battery. You can't change that
```

---
## \#19 Posted by: wafflejock Posted at: 2017-06-27T21:11:57.524Z Reads: 127

```
Did you read the previous link (if so read the definitions again)? Amp hours (Ah) is the capacity of the battery nothing to do with how fast that current flows out of the battery (the current) or how big the electrical potential is on the battery (voltage).  If you have a simple circuit with just a battery and resistor in series the current through the circuit is the Voltage over the resistance (Ohm's law), that's to say you increase the voltage then you increase the current given constant resistance.  When you connect batteries or cells in parallel you increase the total capacity without increasing the voltage.  Since you are drawing the current out of more cells if you have them in parallel you are pulling less amps from the individual cells so you can pull more from the battery as a whole than if there were no cells in parallel.

https://en.wikipedia.org/wiki/Kirchhoff%27s_circuit_laws

The current through (in and out) some segment of a circuit sums to 0 (generally) so if you have 2 batteries in series and you have 10A flow through both batteries in order for that 10A to go into the rest of the circuit.  If you had those 2 batteries in parallel then each battery could supply 5A of the current to make 10A flowing into whatever is hooked up to the battery pack.  But if you have a constant resistance and you increase or decrease the voltage then you will increase or decrease the amps that flow through the circuit.

Long story short:

Parallel = increase the amp hours (capacity), also typically increases max current you could pull without the batteries heating up.  If you have two 5Ah 10V batteries in parallel you have the equivalent of a 10Ah 10V battery.

Series = increase the voltage, the amps are drawn from all cells at the same time though so you don't add any capacity this way.  If you have two 5Ah 10V batteries in series you have the equivalent of 1 20V 5Ah

---

I should add with regard to the increasing voltage with a eskateboard or something where you're powering a motor is typically going to mean it needs to draw less current to do the work it needs to do.  You get your wattage as a product of the current and voltage so if you have higher voltage you need less current to get the same power (Watts).  The motor load isn't a simple resistor but just wanted to explain the relationship between amps volts and resistance I = V/R.
```

---
## \#20 Posted by: d-kay Posted at: 2017-06-28T07:35:17.706Z Reads: 102

```
thank you verry much @wafflejock 
thats excactly what I needed to know.
I had a misunderstanding of the current flow.
I read somewhere that the current output of a battery is the amount of Ah times C so I thougt my battery would overpower the motors or would have little to no output.
11.1 volt 2000mAh -10C
2000 milliamps = 2 amps 
2 Amps x 10 = 20 amps continuous discharge
```

---
## \#21 Posted by: d-kay Posted at: 2017-06-28T07:36:59.564Z Reads: 91

```
do this with al larger battery and a larger C rating and it would overpower the motor.
```

---
## \#22 Posted by: d-kay Posted at: 2017-06-28T07:46:11.114Z Reads: 89

```
so I thougt.
but if it's only the pottential thats ok
```

---
## \#23 Posted by: Challlsss Posted at: 2017-06-28T13:21:28.733Z Reads: 90

```
@d-kay
You need at least 20C for your build to work well. Especially if you only have 2200 mAh batteries
```

---
## \#24 Posted by: wafflejock Posted at: 2017-06-28T13:49:15.940Z Reads: 96

```
Hah yeah no worries yeah the relationship between the C rating and Ah does tell you overalll current, but it's really kind of a matter of the choice by manufacturers to make the C rating based on Ah.

I suppose it makes sense because if they use the same chemistry and techniques, but just increase the capacity for the battery it also probably typically  can deliver proportionally more power as well but it's not strictly true that increasing mAh also increases the total current you can pull/push through it.  The reality is the batteries all have their own internal resistance and they get warmer when more current flows like with any resistor, so too much current and the battery gets too hot and basically starts cooking the components that make it up.

---

Also to add the max Amperage rating (C rating) on a battery is telling you what is the max you can pull from it without it overheating it doesn't tell you how many amps will flow at any given time.  The amperage is going to be based on the rest of the circuit the voltage is being applied to, if the rest of the circuit has a low resistance then the amperage at a given voltage will be higher, if the resistance in the circuit is higher then the amperage will be lower (if the circuit opens the amperage will stop flowing).  So really your issues when looking at a battery are based on the 3 specs in this way:

Voltage - if too high, the motor or other components in the circuit can get damaged from too high a voltage.  This is because the components have a particular resistance based on the materials they're made out of.  Apply a higher voltage and due to their resistance the current that flows through some components will be too high.  Power (W) dissipated by a component is calculated as I^2*R = P where I is amperage, so amperage squared times the resistance tells you power, so more amperages means much more power loss.  For an example say you have a 1 Ohm resistor you apply 1V to it then you get 1V/ 1Ohm = 1A of flow if you want to know the power you do 1A squared times resistance, so again 1W, say we change to 2V but still 1 Ohm resistor, now it's 2V/1Ohm = 2A and the power is 2A squared times resistance, so 4W.  So we doubled the voltage it doubled the amperage and it quadrupled the power dissipation needs (that 4W is usually just heat coming off the device, and 4W is actually a lot for a passive component like a regular resistor).

Amperage (typically described with a 10C-20C etc. rating) - There is the momentary flow of electricity rate of electrons through the circuit at any point.  With regard to the battery though the C rating helps you determine what is the max Amps rating for the battery that is how much current it can supply before it starts to damage itself (due to power dissipation as described above).

Amp Hours different from amps, this is the amount of time current can flow at 1A at the batteries voltage.  So if the battery says 5Ah it means you can draw 1A continuously for 5Hr (or 5A for 1 hr, either way).  A more "accurate" way of describing the power in a battery is to also take into account the voltage of the battery.  If you want an "apples to apples" comparison between batteries that have different voltages to see which has "more power" you want to compare Watt Hours, simply take the Ah and multiply by the volts, this tells you both "how much push" and "how fast for that much push" can the battery do work.
```

---
## \#25 Posted by: wafflejock Posted at: 2017-06-28T16:17:55.975Z Reads: 81

```
Know that was already long but just wanted to add another little nugget of info that helps just grasp the whole thing.  As the temperature in a component (battery or resistor or whatever) goes up typically the resistance also goes up so it is a self feedback type situation where the resistance creates heat and the heat creates more resistance, this is why heat sinks are a thing, at some point the heat around the component builds up faster than air can naturally draw it away and you need a heat sink to give the component more surface area to dissipate the heat into the air (or possibly chuck a cooling fan on the heat sink like with desktops or server processors).
```

---
## \#26 Posted by: d-kay Posted at: 2017-06-29T09:42:40.642Z Reads: 70

```
I wil be shoure to use heat sinks on my build so it won't overheat.
```

---
## \#27 Posted by: d-kay Posted at: 2017-06-29T10:26:45.771Z Reads: 72

```
does anyone know where I could buy aluminum heatsink cassings for al my components to fit in.
```

---
## \#28 Posted by: wafflejock Posted at: 2017-06-29T14:45:57.009Z Reads: 72

```
Ah sorry again didn't mean you really need to use heatsinks (sometimes more information is too much) just saying in general why you see them used in various electronics.

In the case of the e-skateboard the only thing you might want to use heatsinks on in most cases is the MOSFETs on the ESC that deliver the power from the battery to the motor since they can get quite hot with all the amps flowing through them and constantly turning on and off very quickly, but in the VESC tool you can see the MOSFET temperatures (along with a few other temperatures) and see if it's really necessary or a good idea to throw some heatsinks on there.  At least one other forum member made an aluminum case for their VESC that doubles as a heatsink but in most cases it's not actually necessary.
```

---
## \#29 Posted by: d-kay Posted at: 2017-06-29T16:58:52.636Z Reads: 63

```
I was alraedy going to use heatsink so no problem. @wafflejock
and I am stil looking for a cassing and the aluminum seemed cool.
```

---
## \#30 Posted by: d-kay Posted at: 2017-06-29T17:06:10.050Z Reads: 63

```
how could it be a bad idea to put on heatsink
```

---
## \#31 Posted by: wafflejock Posted at: 2017-06-29T17:25:50.835Z Reads: 69

```
Yeah true you're not gonna really hurt anything so long as you keep it all safe from shorting just figured I'd be explicit about it not usually being an issue really (I tend to over-explain since I don't know people's backgrounds here yet at all).  Always funny when I'm giving advice or discussing with someone then see the board they made puts mine to shame :slight_smile:
```

---
## \#32 Posted by: d-kay Posted at: 2017-06-30T14:11:42.430Z Reads: 64

```
I'm completely new so that's not very likely and all help and advise is always welcome. @wafflejock
```

---
## \#33 Posted by: d-kay Posted at: 2017-07-01T15:57:52.160Z Reads: 61

```
does anyone know another place to buy good lipo's for hobbyking is apparently not that good.
```

---
## \#34 Posted by: Challlsss Posted at: 2017-07-05T14:29:10.272Z Reads: 56

```
hobbyking is good
```

---
## \#35 Posted by: hayachii Posted at: 2017-08-29T07:41:51.433Z Reads: 42

```
hi there. can i know what type of esc that u used ?
```

---
