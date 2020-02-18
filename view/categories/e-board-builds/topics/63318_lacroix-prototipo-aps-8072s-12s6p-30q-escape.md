# LaCroix Prototipo &#124; APS 8072S &#124; 12s6p 30Q &#124; ESCape

### Replies: 16 Views: 1262

## \#1 Posted by: chocol4te Posted at: 2018-07-30T16:42:47.350Z Reads: 287

```
[Video and pictures](https://www.instagram.com/p/Bl1JQ1EjQ1O/?utm_source=ig_web_copy_link)

**Parts:**

* LaCroix deck - Very highly recommended. I was having real trouble actually buying a nice-looking 12s4p enclosure for an Urban Carver but LaCroix provides an all-in-one solution. Feels very nice, very comfortable, doesn't feel too wide.

* APS 8072S - I didn't have the budget for a dual drive, and I wanted a higher efficiency build, so I went with a single motor. Considering an 8072S is about the same price as a 6374 I thought I could use the extra power, especially since I am not looking at adding a second motor. So far I have had fairly good experiences with it. I was having some resonance issues at 65% but it is much quieter when the belt is on and I am standing on it. I certainly don't feel like it doesn't have enough power, although max braking current doesn't seem very strong - this is probably due to ESC configuration and not the motor. Although warned about, I have not felt any turning to either side when accelerating or braking due to being a single motor.

* 72 Samsung 30Qs - The board can fit 72, so I bought 72. Arranged in a 12s6p configuration. Definitely makes the board a bit on the heavier side.

* ESCape - Works as expected, but JST-PH connectors are more difficult to find contacts, terminal blocks and crimping tools for. I would've preferred to seen the more common JST-XH, although I accept size constraints may have factored in.

* Urban Carver trucks - Purchased with an Urban Carver deck and not replaced when switching to the LaCroix deck, maybe thinking about swapping for the wider MTB hangers (16 inches).

* 6.5" Trampa pneumatics - Smaller than recommended for the board but I haven't encountered any clearance issues. Feels very firm at 40PSI but can be lowered on rougher terrain and reportedly safe up to 75PSI for smoother.

Guitar stands are great for eboards:
![IMG_1067|500x500](upload://oKhoAWaDa7vn7AVnpg3g68f11UM.jpg)


XLR for charging and braided motor cable:
![IMG_1042|666x500](upload://tgbS8LRZNpQwxJFbifxgEEHRJqt.jpg)


Battery spot welded with 12x0.15mm (I think) nickel strips:
![IMG_0958|375x500](upload://cUQ7GsdGR8TIYaObn6cGJx0dPWV.jpg)

Still waiting on my BMS so having to charge 6 cells at a time:
![IMG_1057|375x500](upload://mtMwfwyl5ez5BS8D61JnBVBnfJI.jpg)
```

---
## \#2 Posted by: legend27 Posted at: 2018-07-30T18:04:39.553Z Reads: 243

```
Nice build! What did you use to weld the batteries?
```

---
## \#3 Posted by: chocol4te Posted at: 2018-07-30T18:17:10.808Z Reads: 243

```
Thanks!

Car battery with a solenoid attached to a relay attached to an Arduino giving 50ms pulses.

![IMG_0959|375x500](upload://fPkNZeZ10dnRBTbXy5LZHZLodgm.jpg)
```

---
## \#4 Posted by: moon Posted at: 2018-07-30T18:19:38.075Z Reads: 237

```
@chocol4te 

Building a spot welder similar to that but without an Arduino, I am going to be so triggered if it doesn't work out
```

---
## \#5 Posted by: Becker33 Posted at: 2018-07-30T19:17:47.998Z Reads: 223

```
Could you share the code you used with the arduino? I have built the same setup with a momentary switch but have a spare arduino nano lying around that could be put to use.
```

---
## \#6 Posted by: legend27 Posted at: 2018-07-30T20:57:40.572Z Reads: 207

```
Cool! I have also build a car battery spot welder but without the audrino. Glad to see it works.
```

---
## \#7 Posted by: sleekjazz Posted at: 2019-02-05T03:58:36.794Z Reads: 114

```
How did you get 12s6p batteries to fit in the Lacroix enclosure?
```

---
## \#8 Posted by: chocol4te Posted at: 2019-02-05T06:31:13.080Z Reads: 102

```
I put another 2 6p packs in the space mean for ESCs, only leaving enough room for my BMS and forcing me to mount my ESC externally.

I’m actually not super sure I’d recommend it :confused:
```

---
## \#9 Posted by: sleekjazz Posted at: 2019-02-05T07:03:05.394Z Reads: 97

```
How did you externally mount the esc? Do you have pictures?
```

---
## \#10 Posted by: chocol4te Posted at: 2019-02-05T07:09:31.086Z Reads: 85

```
I'm sorry, I can't seem to find any pictures and its currently disassembled, but I just stuck it using double sided tape to the top side of the rear mounting hardware. My current plan is to make it an 11s6p and keep everything internal
```

---
## \#11 Posted by: Andy87 Posted at: 2019-02-05T07:10:04.473Z Reads: 86

```
I made an 3D printed case for the ESCapes.
In case you have a dual heat sink that would work also on any other deck, not only on trampa.
https://www.electric-skateboard.builders/t/ice-crusher-16ply-holypro-4w-chain-drive-mtb-4x-6374-170kv-aps-quad-escape-steering-damper/65823/31?u=andy87
```

---
## \#12 Posted by: chocol4te Posted at: 2019-02-05T07:12:42.672Z Reads: 80

```
I can't find the original sketch, it was something like this:

```
void setup() {
     pinMode(13, OUTPUT);
     digitalWrite(13, HIGH);
     delay(30);
     digitalWrite(13, LOW);
}

void loop() {

}
```

Pressing the reset button can then be used to control the welder.
```

---
## \#13 Posted by: chocol4te Posted at: 2019-02-05T07:13:57.099Z Reads: 74

```
That looks awesome! I don't suppose you could send me the STL?
```

---
## \#14 Posted by: Andy87 Posted at: 2019-02-05T07:18:27.813Z Reads: 73

```
I can do later.
The thing is that the battery cables made to come out for a top mount battery.
It could be changed to the side but for this I need a pc and I have only access to a pc next week.
The case is mounted via the inner spring holes of the trampa truck.
If you don’t have this holes, some wood threads in your deck would do s great Job too.
If you still interested just sent me your mail via pm 😉
```

---
## \#15 Posted by: chocol4te Posted at: 2019-02-05T07:32:56.220Z Reads: 70

```
Ahh okay, I wouldn't want you to go to any trouble, thanks anyway though :)
```

---
## \#16 Posted by: Andy87 Posted at: 2019-02-05T08:14:51.708Z Reads: 62

```
It’s not a big thing.
I can change the design next week or sent you the step files and you can modify it to your needs
```

---
