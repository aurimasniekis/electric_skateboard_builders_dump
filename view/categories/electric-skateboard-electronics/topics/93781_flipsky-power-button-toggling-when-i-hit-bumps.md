# Flipsky Power button toggling when I hit bumps

### Replies: 34 Views: 763

## \#1 Posted by: 3LD Posted at: 2019-05-14T05:38:40.539Z Reads: 154

```
Recently put together my first esk8 using Flipsky's Dual FSESC4.20 Plus. 
Last night I lost power at speed and had to perform a pretty bloody desperate foot break to avoid flying into a busy intersection. Found the antispark 'pro switch' in the off position.  Brushed it off as a fluke, maybe I hadn't pushed the button down hard enough, but tonight it happened twice more. Not sure if spring tension in the switch is getting rapidly worse, or due to me riding harder as I get more confident on the board. 

Switch is hard mounted(no vibration dampening) to a junction box which is hardmounted to the board, and I'm on traditional urethane wheels(90mm Abec11s) so it's definitely getting a good amount of vibration on bumpy roads. ![IMG_20190513_221505|675x499](upload://6n9JM7CLnUISAALLfs49rBUmMbK.jpeg) 

Anyone had any luck with opening up the Flipsky switches and replacing or stretching out the spring? Or installing some kind of Oring to reduce vibrations? Or can I just replace it with some kind of toggle switch? Any advice appreciated
```

---
## \#2 Posted by: deltazeta Posted at: 2019-05-14T06:12:40.684Z Reads: 144

```
Solder the connector backwards so it's off when pressed in and on when released
```

---
## \#3 Posted by: Anubis Posted at: 2019-05-14T06:28:13.548Z Reads: 142

```
I broke my leg due to something similar, fix before riding asap
```

---
## \#4 Posted by: bazis Posted at: 2019-05-14T08:28:57.642Z Reads: 132

```
Got the same issue with flipsky button. Tried to fix it. It's impossible. If spring bit stronger then stock, button can't hold in pressed position.

I replaced flipsky button with bigger one.
```

---
## \#5 Posted by: sk8l8r Posted at: 2019-05-14T08:28:58.787Z Reads: 126

```
I just got a flipsky 4.20 plus , it really sounds like the best thing to do with this switch is to simply unplug it and throw it away and use a loop key?
```

---
## \#6 Posted by: Pmac Posted at: 2019-05-14T12:39:10.110Z Reads: 117

```
What button can you use to replace it?

There is a warning inside the packaging that the switch needs to be connected when the ESC is powered on.

![IMG_20190514_223209|690x84](upload://xZxHL1JgIzsf4WU3GhUpQLua0Er.jpeg)
```

---
## \#7 Posted by: 3LD Posted at: 2019-05-14T16:13:57.082Z Reads: 113

```
What switch did you replace it with?
```

---
## \#8 Posted by: sk8l8r Posted at: 2019-05-14T17:01:39.313Z Reads: 104

```
Does this actually mean you can't run the vesc without the worthless toggles itself switch connected? Wow what a POS

Edit: or you can't use the switch without the LED part?
```

---
## \#9 Posted by: TowerCrisis Posted at: 2019-05-14T17:15:34.001Z Reads: 97

```
Actually most antispark switches are like that. It's because if it's disconnected you're leaving the mosfets "floating" somewhere between on and off. It's how most people blow them. You can replace the switch, but you always need one.
```

---
## \#10 Posted by: sk8l8r Posted at: 2019-05-14T17:28:47.457Z Reads: 92

```
no way to use the plus with just a loop key?

Wishing I did not buy this plus version now :smile:
```

---
## \#11 Posted by: Dirt_Bag Posted at: 2019-05-14T18:43:23.552Z Reads: 83

```
Its a really simple fix. A loop key will not work as direct switch replacement


This type of switch has 3 pins that matter. The others are for the led and can be ignored if you choose.

All common antispark switches have a nc/no layout. It means normally closed/normally open. It also includes a common pin. When the button is pressed in, the current is allowed to flow between the normally open and common pins and the normally closed and common is blocked. When it is turned off it is the opposite, current is now allowed through the NC and Com. side

No matter the position, one side is always turned on when the other is off. 

A loopkey can still be used, but the button needs to be permanately on and the loopkey is hooked up to the battery leads as normal.


To find a replacement, just search for a "spdt latching switch" anything matching those keywords will work.

To find a similiar style one, try adding " e switch" or "led push button"

They cost about 3-8usd for a good one. They are even on amazon


Edit: if you look at the bottom of the flipsky switch it will tell you what is nc/no/c in small print. Take note and label the wires so you can replace it correctly. The no/nc can be swapped but the common has to be correct. It can be tested with a multimeter to find them as well
```

---
## \#12 Posted by: Arzamenable Posted at: 2019-05-14T18:48:38.155Z Reads: 73

```
![image|374x500](upload://45dPrKXpIzPMQHvmJuuOZ97EjyY.jpeg) 

All my stitches were soldered to be permanent on, and using loopkeys.
```

---
## \#13 Posted by: brenternet Posted at: 2019-05-14T19:10:25.184Z Reads: 71

```
Show these gents how to do it friend.
```

---
## \#14 Posted by: sk8l8r Posted at: 2019-05-14T19:23:20.161Z Reads: 70

```
I think it's safe to say the safest Flipsky switch is the one....

[quote="Arzamenable, post:12, topic:93781"]
soldered to be permanent on
[/quote] 

:smile:
```

---
## \#15 Posted by: Arzamenable Posted at: 2019-05-14T19:34:28.132Z Reads: 70

```
![image|353x500](upload://cuvEl8AZDJz21O6781DHLsvYpHS.jpeg)
```

---
## \#16 Posted by: Arzamenable Posted at: 2019-05-14T19:35:24.463Z Reads: 69

```
If not that, then it’s - and s
```

---
## \#17 Posted by: parkparkpark Posted at: 2019-05-14T19:41:24.585Z Reads: 69

```
thank you very much
```

---
## \#18 Posted by: Dirt_Bag Posted at: 2019-05-14T20:22:56.762Z Reads: 67

```
Sure thing. Glad i could help. The antispark is surprisingly reliable now, the only issue is the slightly cheap switch
```

---
## \#19 Posted by: bazis Posted at: 2019-05-14T20:24:45.079Z Reads: 67

```
Like this, with 16mm mount hole.
![image|360x360](upload://mObiIpXktkHydW4dzJxuIq8DueZ.jpeg)
```

---
## \#20 Posted by: parkparkpark Posted at: 2019-05-14T20:49:02.779Z Reads: 68

```
so, temporarily I am going to put a switch such as this 
![](https://i.stack.imgur.com/wWDTk.jpg)
will it be right? :)
```

---
## \#21 Posted by: Dirt_Bag Posted at: 2019-05-14T21:11:39.233Z Reads: 65

```
That will not work, it has 3 positions, it has to have just 2

When you cross the middle and it is not on either side, it will fry the antispark circuit. Its the same as not have a switch installed at all
```

---
## \#22 Posted by: Arzamenable Posted at: 2019-05-14T22:06:34.472Z Reads: 65

```
Wait! First, you must buy a latching switch if you are going to use a button Type switch. 

Second, you need a SPDT switch if you want a rocker type. 

![image|365x500](upload://gqgGkXd2UPCKnILPuVkoPCrF3NV.jpeg)
```

---
## \#23 Posted by: 3LD Posted at: 2019-05-14T23:35:10.803Z Reads: 59

```
I reversed the flipsky switch's connection to the vesc so it fails to closed and resoldered the connection so the LED lights up properly for the new configuration. 
Lasted 1 more ride and now doesn't latch at all. 

I got 8 rides out of it before it failed completely. Flipsky support's response was basically 'yep, you got a faulty switch. Not our problem'.

New switch ordered.
```

---
## \#24 Posted by: Dirt_Bag Posted at: 2019-05-14T23:48:19.095Z Reads: 59

```
What switch did you order?
```

---
## \#25 Posted by: Pmac Posted at: 2019-05-15T00:56:55.698Z Reads: 59

```
so from my 2 second testing on the switch when in the off position S is connected to - and in the on position S is connected to positive.

I assume this should work as a replacement?
https://www.aliexpress.com/item/10pcs-lot-3-Pin-6A-250V-Black-Button-Rocker-Switch-On-On-Import-Rocker-Power-Switches/32669016078.html?spm=a2g0s.9042311.0.0.27424c4d2n7K3z

Can anyone advise how i would implement an LED that could sit next to the switch?  I am yet to use the ESC so I am unsure what voltage it spits out for the LED.  So unsure what LED to buy and what resistor to use.
```

---
## \#26 Posted by: Arzamenable Posted at: 2019-05-15T03:35:29.989Z Reads: 57

```
![image|666x500](upload://bR0sYnldSIdkU3YBVj7f68a2vAU.jpeg) 

Whelp, you live you learn. 😒🙃
```

---
## \#27 Posted by: 3LD Posted at: 2019-05-15T03:35:58.438Z Reads: 57

```
Just a generic spdt vandal switch off amazon prime.  

https://www.amazon.ca/gp/product/B015GTWFUW/ref=ppx_yo_dt_b_asin_title_o00_s01?ie=UTF8&amp;psc=1
```

---
## \#28 Posted by: 3LD Posted at: 2019-05-15T03:36:31.834Z Reads: 54

```
what happened?
```

---
## \#29 Posted by: Arzamenable Posted at: 2019-05-15T03:39:50.940Z Reads: 53

```
Dunno, doesn’t matter anymore. Still runs. What are your 4th of July plans? Wanna see fireworks? 😬
```

---
## \#30 Posted by: Gamer43 Posted at: 2019-05-15T04:13:28.908Z Reads: 54

```
Adafruit sells a very nice toggle switch for $5 + shipping. $6-7 off Arrow if you don't want to pay shipping.

And the antispark CAN be bypassed rather easily, just a little bit of soldering and voiding the warranty.
```

---
## \#31 Posted by: parkparkpark Posted at: 2019-05-15T08:29:07.401Z Reads: 50

```
oh yes you are right! now I found another one.![20190515-112743|189x167](upload://itecuIjZEn0cBIqSiQURcZD27bh.png)

the middle leg is short with first leg  otherwise, connected with 3rd leg.
```

---
## \#32 Posted by: parkparkpark Posted at: 2019-05-15T08:29:45.069Z Reads: 50

```
what happened!!?!? what switch did you use? please share it so we can get the lesson from your experience
```

---
## \#33 Posted by: Arzamenable Posted at: 2019-05-15T17:52:22.934Z Reads: 49

```
Oh, I’m sorry, I don’t use switches ever. The pic of the burned board was to just give you all an idea of how serious to take their quality control
```

---
## \#34 Posted by: parkparkpark Posted at: 2019-05-16T07:17:40.775Z Reads: 40

```
![image|651x500](upload://runaCGzKn7eonvjxlQzziH1L1q1.jpeg) I made this switch for my dual FSESC 
https://flipsky.net/collections/new-accessories/products/dual-fsesc4-20-100a-plus-based-on-vesc-with-anodized-aluminum-heatsink
it worked very well!
```

---
