# Flipsky Dual 6.6 plus green led off 1 side problem

### Replies: 5 Views: 232

## \#1 Posted by: Airwolf Posted at: 2019-06-01T09:37:20.683Z Reads: 66

```
I've been trying to install Flipsky Dual 6.6 Plus ESC's with Raptor Enertion 2 Hub Motor Wheels. 

Unfortunately, during initial programming with Vesc Tool, 1 of the 2 Green LED's  on the Flipsky Dual 6.6 Plus turns off. This means the main computer chip for that side of the ESC is irreversibly broken. 

I am better than 90% sure I know what the problem is now. My ESC's are out getting the failed Computer Chips replaced, and I will verify my belief once I recieve them back.

But in my case, a problematic "Temperature Sensor" in my Raptor Enertion 2 Hub Motor Wheel is causing rhe Flipsky Dual 6.6 Plus ESC to have a fatal error during programming.(I.E. the Green LED turns off and nothing can be done to remedy the situation except to replace the 64 pin main Computer Chip for that side of the ESC.)

Basically, I am posting this so that anyone who has 1 green led go off on 1 side of Dual Flipsky 6.6 Plus ESC will at least stop to consider the fact that the problem may be an electrical issue coming in via the Sensor Wires. 

If you have a FOCBOX Unity ESC, uou can try connecting the Raptor Enertikn wheels to the FOCBOX Unity ESC with the USB cable. Then, take a look at the Temperature that appears near each of the rear wheels near the bottom  of the "HUD" System monitor screen. 

If one of the 2 wheels shows an incorrect temperature or no temperature at all is shown, and if the wheel with the problematic Temperature is the same side on which the Flipsky Dual 6.6 Plus just lost a Green LED, I bet you the Problematic Temperature Sensor just turned off tour Green LED. 

My advice, which I will try soon, but may not take the time to record kn the forum is to cut the "TEMP" wire (TEMP stands for temperature) in the Ribbon Cable that comes in from the wheel with the problematic temperature sensor before you attempt to do the initial programming of the Flipsky Dual 6.6 Plus. It is my belief that this is a simple way to avoid killing your Flipsky Dual 6.6 Plus ESC. Presumably, your Thermal Throttljng for both wheels can still be used, if desired, based solely upon the input from the Temperature Sensor in the other wheel which is not problematic. 

If there is a problem of some sort related to the Thermal Throttling which there should not be, then you will simply need to deactivate the Thermal Throttling.

Remember, if your Green LED turned off when you tried to program your Flipsky Dual 6.6 Plus ESC, you will probably need to send it back to have a the 64 pjn Computer Chip replaced, and your real Root Cause is probably something reaching the ESC via the Sensor Rjbbon Cable on the side of the ESC on which the Green LED turned off. ; )
```

---
## \#2 Posted by: Pimousse Posted at: 2019-06-01T09:55:01.127Z Reads: 58

```
Try to flash it with a ST-Link.
```

---
## \#3 Posted by: Airwolf Posted at: 2019-06-04T09:00:30.702Z Reads: 40

```
Thanks for the Suggestion. I did try the ST-Link. However, whatever causes this to happen in my case causes a Fault on the main Computer Chip which makes it impossible to read out from the chip, to Erase the chip, or reprogram it. I put 10 hours in to trying to make it happen and also no one a t Flipsky can make it happen with the ST-Link. Basically I am sending my units back to Flipsky so the 64 pin ARM ST Computer Chips can be replaced. 

In the mean time, I got a new FOCBOX Unity ESC which is currently working well. I will post more info eventually about the resolution of the Flipsky problem if one is ever reached. I think i'm going to try programming one of the repaired Flipsky Dual 6.6 Plus ESC's  with both TEMP Sensor wires cut from the Hall Sensor Ribbon Cable. I'll post my results when I finally come back around on this. 

I was hoping to be able to provide an accurate comparison of the performance of the FOCBOX Unity ESC versus the Flipsky Dual 6.6 Plus ESC. However, thus far, the Flipsky Dual 6.6 has incurred a fatal  hardware error during  programming in 3 out of 3 attempts. ..
```

---
## \#4 Posted by: Soflo Posted at: 2019-06-09T19:47:10.339Z Reads: 29

```
I have problems with my fsesc6.6.... i can power on the board and both fsesc will come on and work.  But if i take a short break (less than 2 min) my slave fsesc will stop working.  The only way to get it to work again is with a power cycle.  I've checked wires,  updated firmware, and still the problem persists.  I have contacted customer support and they are zero help.  (Told me to downgrade firmware, after they told me to update to fix the problem) good luck  i don't know if I'll keep supporting flipsky
```

---
## \#5 Posted by: Airwolf Posted at: 2019-06-10T08:32:27.365Z Reads: 24

```
Man, 
I'm sorry to hear that You are having issues with your Flipsky Dual 6.6. I

My first thought is that if you plug in the USB Cable in to the Slave side and connect to the VESC Tool Program successfully, then there is probably a "Setting" somewhere that says something like: "How many minutes of inactivity should the ESC wait until it shuts down". Basically, the ESC will automatically turn off the Flipsky ESC after a certain length of time. 

I am guessing that maybe you need to set the "How many minutes of inactivity should the ESC wait until it shuts down" for both the Master Side and then again on the Slave Side. 

For example, this setting might currently be 10 minutes on the Master side and only 2 minutes on the Slave side.   

Now with regard to supporting Flipsky, I basically asked Paypal to get a refund for me. They have a great looking product with great specifications for Power capabilities, but I could not get the ESC through programming without irreversible hardware damage

So check this out: I originally started pursuing the Flipsky Dual 6.6 Plus ESC because the FOCBOX Unity ESC was on Back Order at the time when I ordered it, whereas the Flipsky unit was available to ship right away. 

 I observed that the Power and Motor Wires on the Flipsky 6.6 were bigger than the FOCBOX Unity ESC. I figured that this meant the Flipsky 6.6 Dual ESC unit was designed to handle greater Electrical Power throughput as the specifications seem to suggest.

So in the middle of my trials and tribulations with the Flipsky ESC, the FOCBOX Unity Dual ESC finally shows up. I put it in and it worked perfectly. I have put about 75 miles on it and I can say that it has plenty of capacity to handle my system which includes 12S6P Sony VTC5A Batteries and Raptor Enertion 2.1 Hub Motor Wheels. 

It is so important to be able to rely on your ESC when you are in potentially dangerous riding conditions. I am now definitely a fan of the FOCBOX Unity ESC and would highly recommend that You try the FOCBOX Unity ESC next time instead.

The FOCBOX Unity ESC has a simplified Cell Phone App for programming which tells me that someone became intimately familiar with the firmware and hardware of the FOCBOX Unity ESC to be able to write such a simple first try home run App form it. With the Flipsky, You need to use the General Vesc Tool which I am sure is a great tool, but I couldn't get through the programming because certain windows that are supposed to pop open at certain times when going through the wizard didn't pop up. Then, you take your best guess at what to do next and its 1 click and your done with irreversible hardware damage. This is Flipsky's new product so maybe they are just working out the bugs. 

Anyway, the real renaissance of riding FOCBOX for me came after doing a little adjustment of the "Input's Advanced Configurations". Basically, you can tell the ESC how much time to use when making the adjustment to the power output to the motor wheels based on changes in the joystick position. So if the power is jerking you to hard when you push the joystick forward, just make it take longer to manifast the change on the output side until it is sufficiently smooooth... riding..... Baby...... WHOOOO YEEAAAHH!!!  

You can also implement functions on the Input so that when the joystick is closer to the zero position, say from zero to 30 percent of the joysticks forward range, then the output changes at a lesser rate than 1 to 1 with the input. 

SO like at 10% Joystick your at like 3% Output, then at 20% input you are at like 9% output, and at 50% input your like 35% output, and at 60% input your at 50% output, then by like 80% input your at 75% output, and at 90% input your at 90% output. 

This is kind of hard to follow and these numbers aren't exact, but you can see a graph that shows the entire range of input percentages and corresponding output percentages and you can drag the curve up or down to vary it. You can also apply Polynomial, Exponential, etc function characteristics. 

For me, this was the key because at first, I would just be touching the joystick the littlest amount and the board would fly out from under me. But by adjusting the acceleration time to take longer, and by making it require more joystick movement when the throttle is close to zero, my board is like a 600 cubic inch Cadillac with some 4.56 gears Man.  You hop on and push the throttle forward a reasonable amount and the acceleration comes up nice and easy, but after you get past about 50% throttle, it starts tomove back towards a 1 to 1 correspondance between the input % and output % which is sweet because the second half of the throttle range has some scary speed. I'm not sure i'll ever go past 75% throttle unless i'm wearing a wingsuit!  

And also, until you get it adjusted just right, beware of over throttle. This is when you push the joystick like all the way forward when your just starting to roll at like 1 mile per hour. This can cause something like a stall to occur. I'm not sure exactly why this happens, but it doesn't happen anymore now that I made my adjustments to the input to output correspondence. But just remember to apply the throttle gradually. 

Anyway, the moral of the story is that I would strongly recommend trying one of the latest and greatest FOCBOX Unity ESC's and then programming it via  Bluetooth using the Cell Phone App. then, do a little adjustment in the "Advanced Throttle configuration " menu and life will be GOOD!
```

---
