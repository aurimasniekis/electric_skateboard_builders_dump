# Please help! I am not sure how to program my ESC, and I don&rsquo;t want to make a mistake

### Replies: 25 Views: 1268

## \#1 Posted by: jbalint1122 Posted at: 2017-05-05T12:36:09.132Z Reads: 126

```
So, I have one of these:
https://szfvt.en.alibaba.com/product/60449510282-802501949/Newarrival_brushless_DC_motor_electronic_skateboard_12S_HV_120A_ESC.html
and a compatible programming card.

These are my problems:
 - My ESC only has a signal wire, while some tutorials show ESCs with dedicated signal AND programming wires.
 - On the product page of the ESC it says that there is a 5-12V BEC included. Does this mean that I don't need external power to the programming card, and it is enough to only plug the signal wire in?

These ones are kind of stupid, but better safe than sorry, right?
 - What does "BEC: 5-12V/5-8A SBEC" mean? Is it 5V or is it 12V? Just asking because I think I would fry my receiver with 12 volts...
 - Do I have to have my motor connected while programming the ESC?

Sorry if this has been asked, but I couldn't find a similar thread at the first glance.
Thanks for your help in advance.
```

---
## \#2 Posted by: sl33py Posted at: 2017-05-05T13:08:34.996Z Reads: 112

```
I've never seen this particular ESC... but i did stay in a holiday day inn express last night!

I see your confusion on the BEC voltage output.  I would guess there is a toggle to select 5v or 12v.  Agreed - 12v to your Rx would be *bad*.  Their site info for the ESC is pretty poor w/ no additional info.  Did it come w/ any documentation that might be more specific?

Worst case - multimeter!  I'd measure actual voltage to ensure it's safe to connect to Rx.

You don't need to have motor connected to program.  It's good to test and *tweak* so you can minimize some of the cogging as you program or try settings for best performance.  But you'll really need to test and tweak usually - especially for brakes!

GL!
```

---
## \#3 Posted by: jbalint1122 Posted at: 2017-05-05T13:11:40.773Z Reads: 97

```
Thanks for the reply!
So do you think it would be enough to only plug that single cable in to the programming card?
```

---
## \#4 Posted by: sl33py Posted at: 2017-05-05T13:17:14.040Z Reads: 96

```
It's been a minute since i've programmed an XERUN which is similar.

Looking at FVT programming LCD card:
[quote]
For quick and easy programming of our FVT Car ESC's in the field, this LCD Program Box is the ticket.  Simply plug in your ESC lead, switch the power on and all your ESC settings are at your fingertips and can be adjusted with the push of a button.  Very easy to navigate menu can also restore all your default settings with the push of a single button, and the bright blue-backlit screen is easy to see in bright sunlight or the dark of night.

 

QUICKLY AND EASILY ACCESS THE FOLLOWING SETTINGS:

    Motor Timing: Very Low, Low, Normal, High, Very High
    Acceleration: Low, Medium, High, Very High
    Running Mode: Forward/Brake, Forward/Reverse/Brake, Forward/Reverse
    Brake Force: 10%, 20%, 30%, 40%, 50%, 60%, 70%, 80%, 90%, 100%
    Drag Brake: 0%, 5%, 10%, 15%, 20%, 25%, 30%, 35%
    Cut-Off Voltage: 2.6V/cell, 2.8v/cell, 3.0v/cell, 3.2v/cell, 3.4v/cell
    Max Forward Force: 20%, 40%, 60%, 80%, 100%
    Max Reverse Force: 20%, 40%, 60%, 80%, 100%
    Motor Rotation: Normal, Reverse
    Neutral Range: 3%, 5%, 7%, 9%
    Battery Type: NiMh, LiPo
[/quote]

So i'd guess we need power supplied and the ESC lead.  I think i struggled with this last time i tweaked my XERUN, and found a youtube on programming which helped.  

Do you have the ESC already?
```

---
## \#5 Posted by: jbalint1122 Posted at: 2017-05-05T13:20:07.926Z Reads: 80

```
Yes, I have it.
It is also known under "Sleeping lion". It is mainly used in mountainboards.
```

---
## \#6 Posted by: bartroosen12 Posted at: 2017-05-05T14:08:00.156Z Reads: 71

```
HI man!
Yes, you need to connect your motor to it.
It is 5V BEC don't you worry
- connect motor to esc
- connect programcard to your esc (only with the signal wire)
- connect battery to esc an power the esc on
That should be all and the programcard must turn on
If you're done just power off and remove battery
<img src="/uploads/db1493/original/3X/9/a/9ab34856aaa3378b2a6351da85eea5122c1a2e16.jpeg" width="690" height="388">
This is my esc, I know its another one but works the same to program.
Do you have some pictures of you esc,motor,programcard and battery which you wanna post?
```

---
## \#7 Posted by: jbalint1122 Posted at: 2017-05-05T14:19:55.705Z Reads: 70

```
Thanks for the reply!

I have:
 - The ESC I linked
 - An SK3 6374 192KV motor
 - 2*5000mah 4S lipo (making an 8S)
 - The same programming card as you

My only question left is that connecting motors is a must, or it is only good for seeing the response in changes?
```

---
## \#8 Posted by: bartroosen12 Posted at: 2017-05-05T21:50:12.072Z Reads: 58

```
You mean the 3 motorwires?
Just connect them random, you can't connect them wrong.
And yeah the motor will beep when you save a setting which you programmed.
```

---
## \#9 Posted by: jbalint1122 Posted at: 2017-05-06T06:41:36.276Z Reads: 49

```
Thanks for the reply, but I was asking if you have to connect the motorwires WHILE programming the esc. 
I've had experience with brushless motors before, so I know the basics of how to use them.
Sorry if I wasn't clear, I would just rather keep the motor dsconnected because the bullet connectors have not arrived yet, so I would have to solder them together.
```

---
## \#10 Posted by: Big_belly_sean Posted at: 2018-12-12T12:26:22.751Z Reads: 29

```
hi there i need help HELP
```

---
## \#11 Posted by: Andy87 Posted at: 2018-12-12T12:28:22.704Z Reads: 26

```
than say with what....
```

---
## \#12 Posted by: Big_belly_sean Posted at: 2018-12-12T12:28:48.832Z Reads: 24

```
to program my motor
```

---
## \#13 Posted by: Big_belly_sean Posted at: 2018-12-12T12:29:09.097Z Reads: 23

```
idk which and what to use
```

---
## \#14 Posted by: Andy87 Posted at: 2018-12-12T12:30:17.865Z Reads: 22

```
nobody is programming a motor.
```

---
## \#15 Posted by: Big_belly_sean Posted at: 2018-12-12T12:30:40.075Z Reads: 22

```
no me i need help
```

---
## \#16 Posted by: Andy87 Posted at: 2018-12-12T12:31:48.513Z Reads: 21

```
don´t bring up a 2 years old thread if you just trolling.
```

---
## \#17 Posted by: Big_belly_sean Posted at: 2018-12-12T12:34:12.176Z Reads: 22

```
no i am not i am just worried i dont want to fry my motor its a sk3 192 kv running of a 10s3p and it says that the motor max is 80 a and i put it at 60 but i want the thing to go faster but not lose much battery pls help
```

---
## \#18 Posted by: Andy87 Posted at: 2018-12-12T12:37:02.032Z Reads: 23

```
https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559/2039?u=andy87
its now a sk3?
```

---
## \#19 Posted by: Big_belly_sean Posted at: 2018-12-12T12:49:03.070Z Reads: 21

```
ye i upgraded thats y i am asking
```

---
## \#20 Posted by: Andy87 Posted at: 2018-12-12T12:53:19.759Z Reads: 20

```
than can you please write a bit more in detail, what exactly is your problem and where and with what you need held.
to only say in need help will not help anyone...
```

---
## \#21 Posted by: Big_belly_sean Posted at: 2018-12-12T13:13:28.337Z Reads: 17

```
hahah sorry so my motor max is 80 a but i put in 60 a on vesc tool my board goes slow i want a faster board but it with taken so much battery how can i do that and should i put 80 a on vesc tool???
```

---
## \#22 Posted by: Andy87 Posted at: 2018-12-12T13:15:37.759Z Reads: 18

```
i don´t remember your set up.
we need to know if you still have a singel drive or already dual.
which vesc you have and what is your bat max settings actual.
what is your battery and which cells you used for it.
what is your gearing ratio and wheel size.
```

---
## \#23 Posted by: Big_belly_sean Posted at: 2018-12-12T13:40:37.705Z Reads: 19

```
wow ok so i got a 10s3p lg cell i am using the oesc from miami boards i am usinf 60 to 15 gear thing and single drive
```

---
## \#24 Posted by: Andy87 Posted at: 2018-12-12T13:48:58.649Z Reads: 17

```
Which lg cell? Hg2?
Which wheel size and your current battery max setting in your esc please
```

---
## \#25 Posted by: Big_belly_sean Posted at: 2018-12-12T14:18:29.491Z Reads: 15

```
oesc from mimai boards and lg cell idk but i have a 6inch wheel
```

---
