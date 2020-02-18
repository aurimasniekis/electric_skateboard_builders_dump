# HOW TO: LED Lights on an Esk8

### Replies: 2 Views: 433

## \#1 Posted by: anorak234 Posted at: 2019-03-27T22:21:17.834Z Reads: 141

```
Heyo everybody, I know there are several threads about LED lights on skateboards, but I figured I'd make this one because I'm not using normal LEDs, I'm using Neopixels, which are individually programmable and easier to use than most people think. I'm also posting it here instead of the electronics category because the outcome has more to do with the look of the skateboard. I made the project through Hackster.io, so here's the original link:

https://www.hackster.io/anorak234/arduino-powered-e-skateboard-lighting-f1ca9b


*Let it be known that the board which I refer to as "my board" is not actually mine, I built it for someone else and have it right now for commuting to and from work*

And here's the project (copied and pasted for the most part)

**Parts Needed:** 

-Teensy 3.2

-Buck converter

-Microusb cable

-Jumper cables

-XT60 connectors & heat shrink

-soldering iron

-glue gun

## Story 

It started about two weeks ago in Hackster HQ with an inexperienced intern (me), and awesome mentor (Ben Larralde), and some great coworkers (namely Alex Glow). My passion is building Electric Skateboards, and Ben and Alex found a way to tie that together with coding by providing me with an Arduino and some Neopixels and letting me have my fun while learning how to code. This project is the result of that. I believe it turned out well, and so I am now sharing it with the community. 

**Part 1:**  Tools/Experience Needed

Obviously there's a parts list below, but I think a run through of what you really need and why you need it might help. Essentially, the important stuff to have here is really the Neopixels and some Arduino-type system. I started with the Arduino Uno and moved to the Teensy 3.2, but pretty much anything will work. The smaller it is, the less weight to worry about (since for me this was on the bottom of a skateboard). You'll need basic breadboard knowledge and some decent soldering skills since the pins tend to be pretty small. Additionally, I recommend owning an electric skateboard. Obviously this project applies to much more than just electric skateboards, but having one is fun and you'll be able to use this guide in a much more specific application if you do.

![IMG_1192|375x500](upload://rtb8j4kbprUTrNqomQeRCofaWmH.jpeg) 

**Part** **2:**  Initial Setup

So, assuming that you have all of the parts needed, or have at least ordered them, you can get started with setup. First, figure out how many Neopixels you want and where you want them on your deck. Some people like it on top, but I decided to use 21 pixels per strip, 2 strips, towards the back of the deck. That way when I accelerate it looks  *extra* *cool.*  Get everything laid out, connected first, and placed where you want it on your deck. Don't solder to the Arduino (or Arduino variant) yet, just solder one end of jumper cables to the tabs on the Neopixel strip (5V, Ground, and Data), and use a breadboard during the programming process (you'll thank me later). Once you've got that all set up, connect your Arduino to your computer. We'll program first, and then power the unit off of the skateboard battery later.

![img_1212_j8QGjyDGw4|374x500](upload://jXjrHCsk39aJA8bc6biERS4eKJb.jpeg) ![img_1286_ixFAgj8isx|666x500](upload://awSIBKXy3XLVKXz9kDLlLcl93FW.jpeg) 

**Part 3:** The Code

I am no expert in coding, and I started learning when I started this project. So, I mainly modified Alex Glow's wonderful tutorial and used that to control these Neopixels. The easiest way to get this running for you would be to copy and paste, modify it using the different strings (which control the individual Neopixels), and change the RGB values to whatever you want them to be. You can also modify the delay value to change how fast or slow you want the Neopixels to "move". When uploaded, test it out and make sure you like your pattern before moving on.

(for the code, click [here](https://www.hackster.io/anorak234/arduino-powered-e-skateboard-lighting-f1ca9b))

![img_1203_5SSJStEQvT|374x500](upload://6k3mS7q8oSxHUiF6auVCLfZt9SV.jpeg) 

**Part** **4:**  Battery Power

At this point in the project, after finishing the coding and layout with the Arduino Uno, I moved to the Teensy 3.2 because it is smaller and much easier to fit on the bottom of my board. It was easy to move everything over using the reference diagram that came with the Teensy, but the one thing to remember is that if using an external power source, it must be powered through separate Ground and 5V pins,  **not**  a hacked microusb cable. Getting the code to work is super easy, just download the Teensy attachment and run it alongside the Arduino software to connect. 

For the actual power side of things, I got ahold of a 24V to 5V buck converter, and wired that straight into the battery output of the board. From there, it's easy to connect the 5V output side to the 5V input and Ground of the Teensy. Again, be sure to connect this in the right place for it to power up. This is where we start soldering, and I recommend using XT90 connectors to make everything nice and modular. I also glued the buck converter to the bottom of my speed controller enclosure and the Neopixels to the bottom of the board at this point, since they weren't going to be moving anymore.

![img_1290_xWbu0x8i1A|374x500](upload://2uNB2mO7e3gOw5Ojvx0QSoyFpC8.jpeg) ![img_1273_RhL3LhXqiH|666x500](upload://6B55wZgDoLGENGoM6TsOQcd8vvd.jpeg) ![img_1289_4DdXfNqw83|374x500](upload://b7BmEiIuta5O1wyxthiUUb3T5my.jpeg) 

**Part** **5:**  Final connection

In order to power both Neopixel strips at the same time, I used different 3V and Ground pins available on the Teensy. The only pin that needs to be connected to both of the strips is pin 12, since that can't be replicated. Be mindful when soldering this, because although possible to wire the 3V and Ground pins in parallel for both strips, the pins are extremely small and I found it beneficial to keep them separate. 

Once those are all soldered up, I held it all together in one bundle with zip ties and went out riding! When the board is turned on, so are the Neopixels. It would also be pretty easy to put in a switch if I wanted, but showing off is more fun in my book.

![img_1292_PWknz6dLFf|666x500](upload://bBRoYeiypFuoTrkbPNwJgprnUuy.jpeg) ![png|690x382](upload://5043Eb82RrZIeFLUY8aGgnwHpJ5.jpeg) 

**Part 6:**  Waterproofing

Everything else on this skateboard is waterproof (believe it or not), so I want to make sure that riding through the rain won't hurt it too much. I [3D-printed an enclosure](https://www.thingiverse.com/thing:3522414) which can be easily sealed with hot glue, but which also has nice openings for the wires protruding in 3 areas. There is a hook that allows easy connection with zip ties as well.

![IMG_2982|375x500](upload://sxcKxvxtsBVnGTLiBm0uaQZnyQ4.jpeg) ![IMG_3370|375x500](upload://2c29nErmwZ4oAEdOlpLjnHBsDmf.jpeg) ![IMG_8840|375x500](upload://zKDEjDNx56FK4Zo8stHkJ8zbkSv.jpeg) ![org-created-That-feeling-When-fxe0id|390x390](upload://cbWYJqqqmI6yt6zbJHk37VonGK8.jpeg) 

More specific schematics and code for this project can be found at https://www.hackster.io/anorak234/arduino-powered-e-skateboard-lighting-f1ca9b

Thanks, and I hope you guys learned something from this. It took me quite a while to do, but I think my efforts will help make it easy for others.
```

---
## \#2 Posted by: anorak234 Posted at: 2019-03-27T22:22:32.615Z Reads: 98

```

```

---
