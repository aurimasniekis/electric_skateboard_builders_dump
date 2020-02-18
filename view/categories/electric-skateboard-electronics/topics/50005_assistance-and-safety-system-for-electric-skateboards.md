# Assistance and safety system for electric skateboards

### Replies: 8 Views: 817

## \#1 Posted by: niktwo17 Posted at: 2018-03-24T12:22:39.593Z Reads: 132

```
Hi guys,

I am 18 years old and about to graduate from german high school.
Over the past months I have been developing an assistance and safety system for electric skateboards.
This includes weight sensors as well as custom remote and receiver.

When I started building my own diy boards, there were some features I missed, so I decided to create my own system.
This project won the first place at the regionals of a competition you may compare to science fair, at the state competition I was rewarded with a one week entrepreneurship training.

The receiver is based on the Arduino Nano and the nRF24l01.

![bild board|349x500](upload://yo8JRFa96cMceAWiStCl1Y3mv50.jpg)

The remote is also using an Arduino Nano, a 0.96 OLED, two buttons and a potentiometer.
Housing is under developement, currently I am using a modified sparkle.
 ![Bild Fernsteuerung|469x500](upload://2uABVFlD3cGeiscxWDocuGLTOlx.jpg)

Weight sensor is based on "Velostat", a thin foil which is a force-sensitive-resistor.
You can see the schematic below. 
![sensor_velostat500|690x249](upload://oGYfd9EqJMsPyrJTZ9dvGXu10nE.png)

.

There are 6 pads distributed over the board, which allow to analyze the relative weight distribution of the rider.

![schematic6sensor|690x283](upload://hRSokpoyjW9VUZsUiLMNbYTpwAl.png)


.


Features of my system include:

Remote :

- OLED display with telemetry
- change speed modes
- activate parking brake 
- range estimation based on voltage and discharge curve of battery
- informs about errors such as faulty vesc conn, or weight issues

Board:
- dead man switch using weight data, so automatic braking when there is no one standing on the board
- acceleration/braking power is linked to your weight distribution, so you wont get thrown off when hitting full brakes as the system reduces braking power when your weight shifts to your front foot.
The linkage is PID based, however currently only proportional data is used.
- automatic brake light which is also linked to the deadman brake

...and as the newest feature a head up display.

![hud mounted|525x500](upload://bkjSLgeSkmwnoN7ecCOqcxO7e3j.jpg)

For this hud I used an existing design as reference. It works and displays data, however it is not ment for real world use.

So I looked for a better solution and found the USEE hud which was developed for bikes/ ebikes.
I contacted the inventors of the USEE and their company turned out to be not to far away from my home.
They invited me to their hq and will support the implementation of the USEE into my system.

Further documentation will follow.
```

---
## \#2 Posted by: RedEagle Posted at: 2018-03-24T12:29:48.293Z Reads: 119

```
Can't wait to see how this will pan out. Keep up the good work!
```

---
## \#3 Posted by: telnoi Posted at: 2018-03-24T12:48:16.629Z Reads: 112

```
Really cool and the sort of thing that might eventually make a difference in making ESK8 legal in Germany. Snowboarders have a cord attached to their leg. Mountain boards are too heavy for that imo.

Regarding weight detection. Is there a programmable timeout? Would suck if something like that happened during a jump.
```

---
## \#4 Posted by: niktwo17 Posted at: 2018-03-24T13:02:12.771Z Reads: 109

```
New government will think about "mobilität der zukunft" in 2019, 2020? according to their coalition agreement.

So there are two ways to prevent issues when jumping:
Programmable timeout, as you mentioned 

I implemented the protection by setting a very low switch value of 1kg , which shouldnt trigger while you have any kind of connection to your board and set the brakes to 2 Amps, which shouldnt throw you of but is still enough to stop an empty board.

I need to do further testing, maybe a combination of all 3 aspects will do it.
```

---
## \#5 Posted by: FabianOdermatt Posted at: 2018-03-24T15:49:46.389Z Reads: 88

```
Very nice work!
I assume you have some kind of piece of work or a documentation from your project. Is it possible that you can send it here?
```

---
## \#6 Posted by: Grolletje Posted at: 2018-03-24T16:24:57.019Z Reads: 85

```
Wow this sounds really cool!
```

---
## \#7 Posted by: niktwo17 Posted at: 2018-03-24T16:35:40.003Z Reads: 80

```
Thanks guys
I have got a written documentation, but as it is in german most folks wont be able to read it.
I will upload the german version for now, maybe I will later find some time to translate it.
https://drive.google.com/file/d/1g9cSTyKW5h9GrsArUczRL9qKGgSljpJ0/view?usp=sharing
```

---
## \#8 Posted by: FabianOdermatt Posted at: 2018-03-24T17:53:26.754Z Reads: 69

```
Thanks alot. I'm from switzerland, so perfect for me. :slight_smile:
```

---
