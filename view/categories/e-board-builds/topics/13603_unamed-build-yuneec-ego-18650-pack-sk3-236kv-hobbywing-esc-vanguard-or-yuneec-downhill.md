# Unamed Build &#124; Yuneec Ego 18650 Pack &#124; sk3 236kv &#124; Hobbywing ESC &#124; Vanguard or Yuneec Downhill

### Replies: 23 Views: 2087

## \#1 Posted by: rpn314 Posted at: 2016-11-24T16:32:37.508Z Reads: 221

```
To not get the [Choosing 18650 cells](http://www.electric-skateboard.builders/t/choosing-18650-cells/6240/131) off topic, let's continue here @DIY4Life. You can use this as your build thread. 

[quote="DIY4Life, post:131, topic:6240"]
I am building a e-longboard, did a lot of reading past weeks and i have a basic knowledge of electronics. But still i am having some questions.my basic electrical setup/important parts is:100A on/off switch with keyvolt and amp meter LCD display 100A DC.turnigy sk3 236Kv (60A max).Hobbywing ESC HV(12S max) 100A + cooling fanYuneec ego 7S3P battery 18650 pack (with build in standard BMS).13T small pulley, 35T big pulley, 5m timing belt.GT2E reciever and controller.UBEC xxV-&gt;6V 7A (for reciever)on a Loaded Vanguard or Yuneec Downhill Board 

Now will this setup work? I calculated max speed, diameter of wheels, pulleys,.. and stuff..thats all OKbut will it electrically work... wont i burn something up? Did i select the right hardware?

My ESC can handle my Motor current... but can my ego battery 7S3P 18650's with build in BMS handle that current? (no specs on the standerd BMS used by ego)Can i change the BMS with some diysoldering and keep my 7S3P battery pack, or do i need another battery?What kind of BMS should i use? or just a battery pack without BMS and so without limitations..Lipo istead of Li-ion18650's? new lipo= Expensive :sweat:

I'll take pics during the building process, so you all can see the progress and the finished result.Someone can help me? So i dont burn up some parts?All advice welcome. Thanks co-diy'ers
[/quote]

I don't see anything glaringly wrong with what you've got. Not familiar enough with most of your parts to talk too much specifics without links to them.

Is [this ESC](http://www.hobbywingdirect.com/products/platinum-100a-hv-v3) the one you're looking at?

I have no idea what output current the ego battery can handle, but I wouldn't worry about the current that the motors will take. If the BMS and ESC can handle 40-60 amps, you should be just fine. If you do need to change the BMS, you've got a few options but those from bestech and batterysupports seem to work very well. I would strongly caution you against going without at BMS entirely. It's a little bit less risky with Li-Ion cells that Lipo cells, but still not recommended.
```

---
## \#2 Posted by: Eboostin Posted at: 2016-11-24T20:43:42.041Z Reads: 176

```
The batteries in the ego are 10A continous. It's 3p so 30A continous. I'd probably only pull 20A continous to leave some headroom on the pack.
```

---
## \#3 Posted by: rpn314 Posted at: 2016-11-24T20:55:45.746Z Reads: 169

```
Yeah, I didn't even know what cells were in it. I assume the BMS's current limit is around 30 as well?
```

---
## \#4 Posted by: DIY4Life Posted at: 2016-11-25T08:15:08.849Z Reads: 146

```
yeah i checked 'NCR18650PF'=10A continious 7S3P so 30A
But wil my setup use over 30A? 
The motors max current is 60A, and the ESC 100A... but does that mean they will use the 60A (max current of the motor?) , i dont think so?

Is there a way to limit the current so my BMS doesnt fry up? underclock/underpower the ESC? something possible with my 'hobbywing program card'? diffrent settings? (aint a VESC sadly enough) 
Modify the hardware of my BMS so it can handle more current?
Or just a 24V-30A breaker switch? 

A 24V-60A BMS for a 7S3P pack is damn expensive... :frowning:
```

---
## \#5 Posted by: DIY4Life Posted at: 2016-11-25T08:27:57.688Z Reads: 136

```
http://www.hobbywingdirect.com/products/platinum-100a-hv-v3
that is indeed my esc
http://www.dancovershop.com/product-images/GA36010.pdf
ego yuneec specs
http://store.ezdrone.com/Yuneec-E-GO-Battery-Pack-p/egocr014.htm
ego battery
https://hobbyking.com/de_de/turnigy-aerodrive-sk3-5065-236kv-brushless-outrunner-motor.html
my motor
h ttp://www.ebay.com/itm/172198235119
my lcd display

h ttp://www.ebay.com/itm/12V-24V-DC-HOME-SOLAR-SYSTEM-WATERPROOF-CIRCUIT-BREAKER-RESET-FUSE-INVERTER-CK-/311696264294?var=&hash=item48928b8c66:m:mSeWPr7_l_N4bF82H4CblwA
the breaker switch i was talking about... but then ill never be able to drive at full speed/max motor current??

SOLUTIONSSSSSS?? I got enough tech skills and equipment to build/edit everything myself
```

---
## \#6 Posted by: DIY4Life Posted at: 2016-11-25T09:46:58.923Z Reads: 116

```
IM AT THE OFFICE, SUPPOSED TO BE DOING WORK BUT I CANT KEEP MY MIND OF THIS BUILD..
I think i found a solution for my issue but would love if you thnik it is possible...

if i now deassemble my 7s3p and make it into a 7s4p (40A) i can still keep te same bms for charging.. and when decharging i bypass the bms.. just straight to my esc.. so that bms and esc are in parralell.... then when charging i use the balance charger/bms

i then i have a little spare current :slight_smile:
Possible?
```

---
## \#7 Posted by: TarzanHBK Posted at: 2016-11-25T09:55:59.616Z Reads: 112

```
Fist let me check some things:

How much do you weight?

Your Motor is a 5065 - not the best one for going single, 63er motors are the way to go, but ok with your small battery you are not able to run with more power.

motor pulley 13t is the lowest you should go, better go with a 14/36, which leads you to close to your 13/35.

I´m not sure why you pick this ESC, better get a VESC for that price.

The ego battery is 7s3p which allows max 30A, so get yourself a 7s 30A BMS and use it for discharging and charging - otherwise you´ll probably damage this small battery because of no protection while discharging.

This will work but it´s not a super fun setup!
```

---
## \#8 Posted by: DIY4Life Posted at: 2016-11-25T10:06:45.470Z Reads: 108

```
Damn, that aint fun to hear... already orderd the motor... this was the only one that fitted my motor mount and motor cover.

Why isnt it a fun setup? 

I can't change my motor or ESC.. but if really needed i can change my battery setup... but there is a BMS on my pack but i dont know how much it can take..
will it be a solid/thought build? that was my goal....

i have a 12T-36T setup? will this one tooth make the difference?
```

---
## \#9 Posted by: DIY4Life Posted at: 2016-11-25T10:09:04.105Z Reads: 98

```
75kg weight
and yeah i would have better bought myself an VESC and limited the current in its settings... but this ESC is already on its way.. and i hear that the waiting time for a VESC is lonngggggg
```

---
## \#10 Posted by: TarzanHBK Posted at: 2016-11-25T10:23:00.687Z Reads: 89

```
[quote="DIY4Life, post:8, topic:13603"]
Why isnt it a fun setup?
[/quote]

Because with your battery you´re only able to get about 756W on the street, ok for cruising along but it will struggle on every hill you´ll encounter with 75kg.

If thats the original BMS on the battery, it will do the job for you. But like i said, your build is basically a yuneec ego, which is ok, but nothing more.

i would ship that esc and motor back, get a vesc (where are you located, everyone has them in stock!) and a nice 63er motor and a new battery.
```

---
## \#11 Posted by: TarzanHBK Posted at: 2016-11-25T10:25:59.922Z Reads: 81

```
another option, (perhaps a bit cheaper):
Get a second E-Go battery and parallel them to get more power. And a 7s 60A BMS
```

---
## \#12 Posted by: DIY4Life Posted at: 2016-11-25T10:43:10.913Z Reads: 84

```
What if i disassamble my laptop batterys and make the 7s3p into a 7s5p for excample, i can still charge it with my BMS i have now? correct? just parrallelling cells... some voltage

I have an amp meter on my board, so if i bypass the BMS on discharge and just watch out that i dont cross the 50Amp limit (LCD display), my batteries will discharge balanced, and not overcurrented... and i can still charge them with my BMS

i would like to stay with my 18650'S
```

---
## \#13 Posted by: DIY4Life Posted at: 2016-11-25T10:47:53.565Z Reads: 85

```
So a different battery... with more wattage available would make it more fun/easier going uphill??
```

---
## \#14 Posted by: TarzanHBK Posted at: 2016-11-25T11:25:27.137Z Reads: 88

```
you should not combine different batteries! If they are the same cells with the same age and usage, it´s possible - otherwise don´t do that.

you can´t drive and look all the time at your amps.

Don´t make it so complicated :smiley:

There are several group buys at the moment for really good 10s4p with samsung 25r cells and a bms.
Combine that with a nice 6374 190 kv motor and all your problems are gone!
```

---
## \#15 Posted by: DIY4Life Posted at: 2016-11-25T11:58:20.400Z Reads: 82

```
[quote="rpn314, post:1, topic:13603"]
batterysupports
[/quote]
I live in Europe , Belgium, were do you order your batteries+BMS?
I can not change my motor or esc.. ordered them and cant send them back... and it fits my motor mount and motor cover...
so my setup will be with the 236kv motor....

You thnink a 10s4p would be good for my board?
```

---
## \#16 Posted by: TarzanHBK Posted at: 2016-11-25T12:10:25.131Z Reads: 76

```
@ajaynagra is your man for all the parts you need ;)

still don´t know why you can´t send them back :D but ok like i said, you´ll be able to run with this small motor on flats.

a 10s4p is the way to go.

and if you run a bit with this setup and feel like you´re ready for and upgrade you can still use that battery.

an other thing you could do is a second esc and motor for a diagonal drive with enough power!
```

---
## \#17 Posted by: DIY4Life Posted at: 2016-11-25T12:25:56.028Z Reads: 75

```
I bought all my stuff on ebay... so i dont think i can send it bac to the seller... that is why..

It will have enough power in single drive.. but it will need a better battery... ill be looking out for a 10S4P...
Or isnt it then better to just buy me some zippy's on hobbyking? and build a 10s4P pack with liploys istead of 18650's
```

---
## \#18 Posted by: TarzanHBK Posted at: 2016-11-25T13:18:39.894Z Reads: 73

```
read a bit more on the forum and then decide for the best way ;)
```

---
## \#19 Posted by: rpn314 Posted at: 2016-11-25T16:46:40.376Z Reads: 86

```
@DIY4Life to be frank with you, you probably should have read a whole lot more and started a build thread (like this) before you started buying parts.

@TarzanHBK is right. 

- For a single drive, the small 5065 motor will not be able to climb hills very well (if at all). And when it does, it will try to pull a lot of current, which the batteries can't safely supply, and the motor (and possibly the battery) would get hot even if you did.
- While the battery is a little under-powered, but it will probably work on level ground. You'll just have to figure out some way to limit the current draw to 30A (or less, because batteries really don't like pushing out their max current. For example, my 10s4p pack can push 80 amps, but I limit it to 40 amps max from my VESC).
- Any wait time on the VESC is worth it IMHO. Though to be honest, I'm not sure where you're seeing wait time. From the last I saw, almost everyone who ships in/to europe has the VESC in stock.

So my recommendations are:

- Return the ESC and Motor and get a VESC and a motor that's at least 63xx (6374 for a single drive would be my recommendation)
- Get a different battery pack. If i'm reading that link correctly, the e-go battery is $300 (USD I think). For that price you can almost get a Space Cell or get someone around here to build you a custom pack. Unless you've already purchased the e-go, in which case it may be cheaper to just buy a second one and put them in parallel.
```

---
## \#20 Posted by: Eboostin Posted at: 2016-11-25T17:26:27.734Z Reads: 83

```
From what I've seen with the 5065 builds, the motors are pretty stout and reliable. @chaka motors seem to put up a decent fight against the 63s.
```

---
## \#21 Posted by: DIY4Life Posted at: 2016-11-26T11:13:15.249Z Reads: 73

```
Thats what i heared to.. i aint climbing hills.. maybe a bridge here and there thats it...but i really think/have the feeling you guys underestimate the 50mm's... 'if' it burns up in a few months ill buy myself a 63mm guys
```

---
## \#22 Posted by: DIY4Life Posted at: 2016-11-26T11:41:28.463Z Reads: 68

```
I ordered some perfectly the same 18650 cells, my battery pack is going to be upgraded to a 7S6P + new/editted BMS. charge them with a balance charger.. Gonna rebuild it.. cheapest and best way.. that solves my current problem.. i can then use 40-50A continious safely... (60A max)... and im planning on limiting my board at 50amps with an inline breaker switch.
i aint going for sick speeds or insane torque... i never go uphill, we dont have hills around here.. i wanne get to work.. so my max range is way more important..
```

---
## \#23 Posted by: rpn314 Posted at: 2016-11-26T21:44:00.662Z Reads: 61

```
That sounds like a good solution. I'm curious how you plan to "edit" the BMS though....

Yeah, I probably do underestimate the 50s.
```

---
