# Remote-ly Possible?

### Replies: 27 Views: 1416

## \#1 Posted by: SoulSnatcher Posted at: 2018-05-29T06:20:55.233Z Reads: 274

```
I have included pics of my components. I am trying to figure out how to combine these two but I think I'm missing a middleman. I need some kind of electronics to make these communicate with each other but my limited knowledge of electronics is hindering me and I need help. Can anyone tell me how I can get this 36v 1000w brushed motor controller ![brushed motor controller|572x392](upload://cGMeyo96JLzwRyRJk4VS3aKKPg6.png) to function in conjunction with this 2.4GHz radio remote? ![remote controller|561x500](upload://xE16L9SHOnzkhZddKDEe3N9cQLW.png) Ideally, I would like to add regenerative braking function as well (maybe a pipe-dream), but if I could just get the speed control to work with the hall sensor throttle I'd be happy. First I thought I could combine them with arduino but I've been told it can't handle that much juice and a 10s ESC is even more than a VESC and I can't afford it. This setup is used to control a 36v 600w 3600rpm brushed DC motor. I was using an 800w controller but I burnt it up, so now I'm running a 1000w controller. Currently I use a corded twist throttle (which works off of a hall sensor in the throttle handle) and I'm sick of it. Any help or directions to where I can find help would be greatly appreciated. If anyone needs pics of the interior electronics or anything else from me please ask and I will post whatever you need as soon as possible. The connections on the motor controller are for Battery, Motor, Key Lock (on/off), Brake Lights, one labeled 'Brakes' (it just kills the throttle so both can't be on at the same time), Digital Battery Level Indicator, and one for Charging the battery ![same basic layout|690x489](upload://kFtOAKiEkSe0AJLV19MiAX6VXp4.png) Thank you.
```

---
## \#2 Posted by: Acido Posted at: 2018-05-29T06:45:55.582Z Reads: 238

```
Did you consider vescs?
```

---
## \#3 Posted by: SoulSnatcher Posted at: 2018-05-29T07:04:45.516Z Reads: 230

```
Yes @Acido I believe I stated that in my post, I cannot afford one plus I already have these components so I'd like to try and get them to work. Kinda seems like a little overkill also to use a VESC for an old school brushed motor. I know you can run them with a VESC but they were building these with brushed motors and using RC remotes for them long before Mr Vedder blessed everyone with his advanced knowledge, I just don't understand the circuitry and am hoping for some help. Thank you for your reply.
```

---
## \#4 Posted by: Slak Posted at: 2018-05-29T10:19:55.673Z Reads: 205

```
I don't really understand why an Arduino can't be used to convert signals from a 2.4 GHz receiver to the "Throttle/Handle Brake" system ? Are you sure there is too much current going from "Throttle/Handle Brake" to the motor controller ? Did you measure voltage and current in those wires ?

Do you have any ideas how the motor controller works for the throttle/brake part (what can you signal to you need to send to it) ? Any specs maybe ?
```

---
## \#5 Posted by: Okami Posted at: 2018-05-29T10:58:42.982Z Reads: 183

```
Well i know it is possible to do it other way around. Hook up hall sensor throttle to esc that needs PPM ,(remote signal)

This is possible with servo tester.

So.. I assume u need 5v signal instead of PPM.. though im not sure what converter might do this

Maybe this helps:

https://electronics.stackexchange.com/questions/260367/how-to-convert-pulse-position-modulation-ppm-to-duty-cycle
```

---
## \#6 Posted by: xilw3r Posted at: 2018-05-29T16:51:10.853Z Reads: 155

```
definitely possible, dont those controllers use ADC input for throttle ? You may need to get a DAC thingy to hook up your arduino onto. PPI signals are definitely possible to decode on the duinos. Or perhaps you can find a PPM to ADC converter on hobbyking just for this...

But all in all, brushed motors ? Man you will be missing most if not all the fun with that set up. Its like making a steam powered car when you have IC's all around (hope IC jokes are not tabu here ?)
```

---
## \#7 Posted by: SoulSnatcher Posted at: 2018-05-29T20:01:08.434Z Reads: 141

```
LoL @xilw3r No way dude. I built a king size Mack Truck/Navigator/enduro hybrid. I have a Sector 9, 57 1/2" longboard with Paris V2 all-terrain longboard truck on the front and an old school truck on the back that the motor bracket, motor end cap, and belt/pulley protector are basically all cast as one unit. Those are sitting on 4, 6"x2" pneumatic wheels. To push it, I built a 10s8p Li-ion battery and made my own electronics cover and battery cover out of Kydex. I'm 230lbs and it goes about 25mph with about 25 mile range and I can even start out rolling backward on about a 20deg incline and I climb 30 to 45deg hills fairly easily as well. I don't push... Ever! :sunglasses: It's against my religion.  I live in Oregon so I ride in the rain and puddle jump a lot also with no probs. It's pretty sweet to just be cruisin' down the street and veer off down a dirt trail then down a gravel alley.  Believe me, I have plenty of fun!
But I digress. Now about your response: IDK what ADC or DAC even mean? My controller (as it said in my post) functions off of a hall sensor (I believe I was told that's a PWM signa)l. But I was told the arduino can't handle that much juice to use it like an ESC and something like that the duino's translation from PPM to PWM was choppy and that I'd lose a fair amount of range at the top and bottom end of the throttle using it as an accelerator/translator alone. Then there was something about adding resistors or capacitors or some such but I really kinda stopped paying attention after I heard "loss of range on the throttle" to be honest. I don't want less... I want MORE. Everything now is all geared for brushless and touted as "zero maintenance" motors but I see that as a detriment as well. To me, that just means I can't work on it, not that I don't have to. If (and it has happened) I burn up my motor I can fairly cheaply rebuild it, not just chuck it in the trash heap. I'm not rich so I like engines I can tear down and rebuild. I'm also not overly concerned with weight... I've got 25 mile range. I don't push and I don't carry. I also designed a carry handle for it in the bottom middle between the battery and motor controller which also serves as a means to Krypto lock it to any bike rack as well. I just take the key out of the throttle. If someone wants to steal it, good freaking luck! Ain't nobody running anywhere with a 5' board that has a 10s8p battery and a 36v 600w brushed motor strapped to it Rofl.
```

---
## \#8 Posted by: SoulSnatcher Posted at: 2018-05-29T20:17:31.437Z Reads: 109

```
Yes @Okami in a nutshell, that is my problem. I will definitely take a look at your link and let you know what I find out. Thank you for your reply.
```

---
## \#9 Posted by: Deckoz Posted at: 2018-05-29T20:19:40.392Z Reads: 108

```
You need an Arduino to convert ppm to an ADC signal, and then wire the ADC to the throttle cable
```

---
## \#10 Posted by: SoulSnatcher Posted at: 2018-05-29T20:27:28.000Z Reads: 115

```
@Slak I pulled the following info from Robotics.lib:

Arduino Power, Current, and Voltage Limitations:

Input Voltage Limits:
Recommended: 7~12V
Absolute: 6~20V
Input/Output (I/O) pins: -0.5V to +5.5V (the actual max is “Vcc + 0.5V,” which for a 5V Arduino, is +5.5V) (Note 1)

Output Current Limits:
When powered by USB: total of 500mA
With external battery or power supply: total of 500mA~1A (see below for specifics)
5V pin: same as above: 500mA or 500mA~1A
Each input/output pin: 40mA
Sum of all input/output pins combined (but NOT including the “5V” pin): 200mA

My setup runs at 36v and I regularly pull 20-30a. Way too much to just run it through an arduino. I could just try to have the duino translate the PPM signal to a PWM signal but I was told this is fairly inefficient and the duino's translation was choppy and that I'd lose some range at the top and bottom end of the throttle doing that and I don't want that. Thank you for your reply.
```

---
## \#11 Posted by: SoulSnatcher Posted at: 2018-05-29T20:41:59.330Z Reads: 106

```
@Deckoz ADC (Attack Damage Carry) is an archaic term used to refer to a champion that deals strong, continuous damage with their basic attacks and scales with attack-related stats - i.e. attack damage, critical strike chance and attack speed. Lmfao. Ok, analog to digital converter... Yes and there lies my problem, the inefficiency of that translation with arduino. What can I use as a go-between that won't create choppy lossness. Ya lossness, I'm sticking with it lol. Also, do you mean wire it to the motor controller? The only throttle cable currently runs from the thumb twist throttle to the motor controller and that's what I'm trying to eliminate...
```

---
## \#12 Posted by: Deckoz Posted at: 2018-05-29T20:51:25.622Z Reads: 102

```
The thumb twist throttle signal is ADC.

Wire a mini receiver to an Arduino like a pro mini. Put code on pro mini to convert ppm to an analog signal output by a digital pin. Wire the digital pin to the motor controllers ADC pin of the thumb throttle. And a ground wire from Arduino to the thumb throttle ground. The actual thumb throttle is no longer connected. A little dongle with above parts are dangling off the motor controllers thumb throttle connector

Boom wireless throttle

If your smart you'll make use of one of the analog pins on the Arduino to temporarily plug in the thumb throttle to calibrate the range of the ADC signal that the Arduino needs to translate from ppm.
```

---
## \#13 Posted by: Slak Posted at: 2018-05-29T23:19:39.273Z Reads: 86

```
[quote="SoulSnatcher, post:10, topic:57107"]
My setup runs at 36v and I regularly pull 20-30a. Way too much to just run it through an arduino
[/quote]

A remote receiver is usually powered by 5V  coming from a VESC/Focbox and I think it's the same for others ESC. Why would you have 10S going through the receiver? Oo

Think of the Arduino we're talking about as an extension/plugin of your 2.4 GHz receiver. A PWM signal goes by radio from transmitter to the receiver, then it goes to the Arduino wired on the CH2 receiver's channel. The Arduino convert this PWM signal to an ADC signal and output the result to a pin wired the Motor Controller.

I don't know about the quality of the conversion performed by the Arduino but did most of your research results concluded that (bad conversion job) or just some/few of them ?
```

---
## \#14 Posted by: SoulSnatcher Posted at: 2018-05-30T01:20:41.467Z Reads: 72

```
@Deckoz Ok I'm not familiar with arduino at all. So which Pro mini receiver do I need? Which arduino board do I need? What code? How do I wire the Pro mini to the arduino? Where do I connect and how do I bind the radio remote? When and how do I calibrate the throttle to the arduino? And after all that I have to try and fit the whole thumb throttle with both boards connected to it into my electronics cover?
I know, what a tard right lmao. Sorry I'm arduino illiterate, that was all greek to me:roll_eyes:
Thank you for your reply and in advance for all the help you're going to have to give me so I can get this to work lol... No seriously.
```

---
## \#15 Posted by: biggdaddyhawk Posted at: 2018-05-30T05:04:14.485Z Reads: 69

```
Stick with the twist throttle or get a used vesc from the used items for sale section .
```

---
## \#16 Posted by: SoulSnatcher Posted at: 2018-05-30T08:59:36.848Z Reads: 67

```
Ya thanks @bigdaddywank that's really helpful. Maybe next time you don't have any advice you should just keep it that way. Thanks so much for stopping by though, you brightened the whole room..
```

---
## \#17 Posted by: pat.speed Posted at: 2018-05-30T09:56:18.728Z Reads: 64

```
You will need any arduino although pro mini or Nano are preferred for size reasons. Then find some code online that translates ppm/pwm pulses into analog signals (varying between 0-5v) then plug the output pin that you set into the signal wire on the arduino and connect the hand throttle ground wire to the arduino
```

---
## \#18 Posted by: biggdaddyhawk Posted at: 2018-05-30T12:22:36.620Z Reads: 62

```
I was gonna say I have several vesc just lying around but I'm gonna just leave it that way. Have fun with your electric motorcycle esc
```

---
## \#19 Posted by: SoulSnatcher Posted at: 2018-05-30T20:56:53.733Z Reads: 60

```
@Deckoz, "The thumb twist throttle signal is ADC".No it isn't, it's PWM. ADC is not a type of signal. Ok the lightbulb has finally just clicked on now and I think I see what you are talking about. Gawd now I feel like Wee Todd the Sofa King for my last reply but it wasn't my fault. Your verbiage is wrong. You keep saying "ADC" in strange places and weird ways. "ADC" means Analog to Digital Converter which is what the Pro mini or the Arduino would be right? ADC is NOT a type of signal itself, it's a device that converts signals. "ADC Definition - A device in the form of a chipset that receives analog signals, measures the input at a regular sampling interval (or on command), and reports a digital output of the results.".(Dictionary.com) The motor controller doesn't actually convert an analog signal to digital. So when you say, " Wire the digital pin to the motor controllers ADC pin of the thumb throttle. And a ground wire from Arduino to  thumb throttle ground." You mean, "Wire the digital pin to the motor controller's throttle (Hall) sensor pin. And a ground wire from Arduino to the motor controller's throttle ground pin. Then when you say "A little dongle with above parts are dangling off the motor controllers thumb throttle connector." Do you just mean that the Arduino and Pro mini will be wired to the motor controller where the old twist throttle used to be connected"? And lastly, you suggest to, "...plug in the thumb throttle to calibrate the range of the ADC signal that the Arduino needs to translate from ppm." You really mean, "...plug in the thumb throttle to calibrate the range of the PWM (Analog) Signal (as again, ADC is not a type of signal) that the Arduino needs to send to the motor controller after it translates it from the radio remote's PPM (Digital) signal.

So I have a few questions: What is the name of the Arduino board that I need? What is the name of the Pro mini board that I need? Are there any other Capacitors? Resistors? Reducers? Transistors or anything else I need add to this circuit to protect it or to make it work correctly? And, would I use the motor controller's remaining +5v throttle connection pin to power the radio remote receiver and/or the Arduino? If not, what do I use to power those?
```

---
## \#20 Posted by: Deckoz Posted at: 2018-05-30T21:05:02.399Z Reads: 55

```
Lol. 

Arguing because you don't understand will get you nowhere.

It's an analog signal on DC voltage hence ADC. The voltage being the signal. PWM is pulse width modulation. While it caries a voltage similar to a simple analog signal with varying voltage(ADC) there is actually a timing between the modulated voltage(hence the pulse width)

So yea ADC is a type of signal. So is PWM, and so is PPM.

 Good luck lol
```

---
## \#21 Posted by: SoulSnatcher Posted at: 2018-05-30T21:17:59.137Z Reads: 52

```
Well @bigdaddyhawk then I apologize but I'm supposed to know that how? Because that isn't what you said whether you were going to or not and it just sounded to me like you were telling me to give up. Anyway, no hard feelings and thank you I will. I try to always have fun.
```

---
## \#22 Posted by: Slak Posted at: 2018-05-30T22:12:04.480Z Reads: 50

```
Really ?

You come here asking everything with your only 2h reading on this forum. When people try to help you, giving you hints and pointing directions to find answers (instead of a full solution freely delivered to your house, i'm sorry, i only get it now !), instead of using those informations you got to continue your own researchs, you just tell people with shit loads of days of reading they are wrong and don't use the right wording. Hahaha, so funny sorry :)

Example : you just had to type "pro mini' in google and would have learn (first result) that it is a kind of arduino board but you didn't and instead asked "How do I wire the Pro mini to the arduino?". Sorry it's enough for me. Hope you won't hurt yourself with your system if you manage to finish it.

My advices : be humble, use google more and read the forum a lot more than you did (you will say less bs and  people will help you if you make some efforts on your side too).
```

---
## \#23 Posted by: SoulSnatcher Posted at: 2018-05-30T22:28:08.675Z Reads: 51

```
@Deckoz Yep and that'd be the reason for the sampling interval the ADC takes of the Analog signal it then converts to Digital. But in the application you're trying to describe, wouldn't it be DAC anyway? Isn't PPM the digital signal (digital modulation really, because while it carries a signal similar to a simple Digital signal it carries multiple values, not just two, and each value it carries can vary from 1000 to 2000 hence the Pulse Position in its Modulation) from the radio remote that the Arduino is converting into analog (a modified analog) for the motor controller? So what is that type of signal called? Digital signal on AC? No, because then it would be an Inverter (lol) because 'inverter' is a type of signal too right?  Not a device that converts DC electrical current into AC, so we'll just call that signal 'inverter' instead of modified or pure sine wave AC right? Ya, because that makes sense. Like I said, you are arguing with the dictionary, not with me. You could've just said you don't know the answers to my questions. That's ok, thank you anyway.
```

---
## \#24 Posted by: SoulSnatcher Posted at: 2018-05-30T22:45:53.712Z Reads: 49

```
@Slak I know the Pro mini is an Arduino board but there are several different types of them with different components and I don't know the differences so I was asking for help. I misunderstood what I was being told at first. When I heard, "Wire a mini receiver to an Arduino like a pro mini." I thought the Pro mini was a receiver I was being told to connect to an Arduino because again, I don't understand. I'm not afraid to admit when I don't understand or I'm wrong. But one thing I do understand is language, and if you can show me anywhere that says that ADC or DAC are actual types of signals, not devices that convert different types signals then I will admit that I'm wrong and apologize here too. If you know of anywhere that will say that please bring it to my attention. Thank you for your reply.
```

---
## \#25 Posted by: Deckoz Posted at: 2018-05-30T22:58:08.223Z Reads: 50

```
Dude you just don't get it. 

An ADC signal, is a voltage, there is no data. The voltage is measured, and compared to a table, with a range of voltages in a table in the code. You're implying that there must be "data" in the signal" when all it is is a voltage within a range. 0.9V to 4V~ on a 5V DC line.

It is "analog" because it is pure voltage, and read as pure voltage, there is no blocking of the signal. 

PPM is timed digital signal, that is on or off, the timing in between each packet is the same.

Pulse width modulation. Is a voltage that is turned on and then off, the length or time frame of these pulses of on and off have the same amplitude(voltage) so the signal is interpreted by time.

![image|666x500](upload://mK7UoZXtTCCthK4qMqBNT1fabWq.jpg)

Also just because analog looks like a sine wave doesnt mean that's its shape, analog is just a voltage that doesn't turn on and off, and is continually measured on a DIGITAL PIN of an MCU for accurately acquiring the voltage value.

But really, if you wanna be a smart ass know it all, go back to google and figure it out. Or better yet put a scope on your ADC throttle, because guess what? It's a 5v signal with a potentiometer that is varying the voltage from 0.9v-4V as you twist it. Potentiometers don't magically make the voltage into a square wave form of any type.

I can't believe your such a fuckin keyboard warrior.
```

---
## \#26 Posted by: Kug3lis Posted at: 2018-05-30T23:32:27.402Z Reads: 49

```
My suggestion for you is just drop this, you don't have programming or electronic skills to convert PWM(PPM) signal into analog voltage or even idea how to build circuit around arduino...

If you really want to do this here is example

https://github.com/fishpepper/ppm2analog

Good luck!
```

---
## \#28 Posted by: MoeStooge Posted at: 2018-06-08T12:13:22.263Z Reads: 25

```
1000w at 36v might power you to 15mph. Maby put this on you kids power wheel and make something fun for them. Best way to make this work is to Fab a servo to the control potentiometer the speed control is designed to use. Radio to mechanical to analog input.
```

---
