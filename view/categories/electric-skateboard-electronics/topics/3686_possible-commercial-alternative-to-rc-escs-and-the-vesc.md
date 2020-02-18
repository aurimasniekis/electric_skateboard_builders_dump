# Possible commercial alternative to RC ESCs and the VESC?

### Replies: 15 Views: 1435

## \#1 Posted by: Karmannghiagirl Posted at: 2016-05-23T15:28:53.628Z Reads: 151

```
Been reading a lot of posts on this blog http://www.etotheipiplusone.net/ (you should check it out, super fascinating stuff). And he talks about using this controller for his brushless motors (some of which he builds himself...). So I looked into it and although they are somewhat more expensive than the VESC, I would imagine they are 100x more reliable (false economy and all that). Have any of you looked into these or tried them out? 

They have a long list of features, here are some highlights from [the one I was looking at](http://kellycontroller.com/kbs48151e80a24-48v-mini-brushless-dc-controller-p-1305.html):
• Support three modes of regenerative braking: brake switch regen, release throttle regen, 0-5V analog signal variable regen.
• Configurable limit for motor current and battery current.
• Support torque mode, speed mode, and balanced mode operation.
• Battery protection: current cutback, warning and shutdown at configurable high and low battery voltage. 
• Rugged aluminum housing for maximum heat dissipation and harsh environment. 
• Rugged high current terminals, and rugged aviation connectors for small signal.
• Thermal protection: current cut back, warning and shutdown on high temperature. 
• Current multiplication: Take less current from battery, output more current to motor.
• Standard PC/Laptop computer to do programming. No special tools needed.
• User program provided. Easy to use. No cost to customers.
[
They have a whole range of these so you can get the exact one you need/want :grin:](http://kellycontroller.com/mini-brushless-controller-kbs12v-72v-c-60.html?sort=3d&page=1)
```

---
## \#2 Posted by: karma Posted at: 2016-05-23T17:38:22.039Z Reads: 126

```
Hmm this looks interesting, are you going to try it out?
```

---
## \#3 Posted by: willpark16 Posted at: 2016-05-23T17:42:26.794Z Reads: 122

```
I agree if this were possible to be applied to boards it could replace the vesc and other escs
```

---
## \#4 Posted by: Jinra Posted at: 2016-05-23T17:45:28.955Z Reads: 118

```
I don't think this will be replacing the VESC since the VESC was designed specifically for e-skates while these are more general purpose. Also, they're a lot bulkier than the VESC and more unsightly. As long as Vedder continues to support and develop for the VESC, it should be around for a long time.
```

---
## \#5 Posted by: willpark16 Posted at: 2016-05-23T17:48:28.106Z Reads: 116

```
Except so far i have not seen anyone had a vesc last without something failing at one point. And while the vesc is great its not necessarily where it needs to be so that it will last a few years. Also this is encased already so thats already taken care of
```

---
## \#6 Posted by: Karmannghiagirl Posted at: 2016-05-23T17:53:21.654Z Reads: 111

```
I might eventually save up the money to try one, but right now im still scraping together my first build
```

---
## \#7 Posted by: Jinra Posted at: 2016-05-23T17:58:42.407Z Reads: 107

```
I'm sure there are way more successes with the VESC than failures. You don't have many people creating threads about their VESC working fine. Most topics are here are people who have problems and need help. The beauty of open source technology is someone else can pick up and improve on it, or Vedder himself can. The VESC is still fairly new, and as development increases and improves, features will be added and quality can only go up.
```

---
## \#8 Posted by: willpark16 Posted at: 2016-05-23T18:00:51.092Z Reads: 103

```
i hear u hell i have a vesc two feet from my laptop rn but I would be willing to put my money on the fact that torqueboards esc has had less failures then the vesc
```

---
## \#9 Posted by: thisrealhuman Posted at: 2016-05-23T18:05:28.604Z Reads: 97

```
[The smallest one](http://kellycontroller.com/kbl48101x24v-48v100abldc-controllerwith-regen-p-54.html) is 4.2 lbs. It should work with 12s and any hobby motor, but it's a brick designed for under the dashboard of a golf cart. This might work for a bike or large scooter, but that's 4 lbs. You can get 300A in this size ESC, but a single drive skateboard with ~13kw in one wheel? 

This is a good find, but not for e-boarding I think.
```

---
## \#10 Posted by: Karmannghiagirl Posted at: 2016-05-23T18:06:54.965Z Reads: 95

```
Im pretty sure that is not the smallest... let me look for some more info
```

---
## \#11 Posted by: Karmannghiagirl Posted at: 2016-05-23T18:10:27.372Z Reads: 93

```
http://kellycontroller.com/mot/downloads/KellyKBS-EUserManual.pdf
Look at page 8, the smallest form factor is 125x94x41mm doesn't give a weight though.
```

---
## \#12 Posted by: willpark16 Posted at: 2016-05-23T18:22:10.583Z Reads: 88

```
http://kellycontroller.com/kbs48151e80a24-48v-mini-brushless-dc-controller-p-1305.html 
2.8IBS
```

---
## \#13 Posted by: Karmannghiagirl Posted at: 2016-05-23T18:24:35.086Z Reads: 86

```
derp, i didnt even see it listed there :stuck_out_tongue_closed_eyes:

Still thats not a horrible weight, most of it is probably the aluminum enclosure
```

---
## \#14 Posted by: thisrealhuman Posted at: 2016-05-24T02:59:54.768Z Reads: 73

```
that's only 80A, at 12s you can make a 3.5kw board. Mine is 2.9kw, so it would have plenty of power.
I'm wondering if the aluminum cases are filled with resin or poly fill like a scooter esc.
```

---
## \#15 Posted by: thisrealhuman Posted at: 2016-05-24T03:22:44.749Z Reads: 67

```
I picked the smallest amperage under "Sensorless BLDC Controller" assuming it would be the most useful for a skateboard. These would be great for controlling those balance scooter hub motors for just about anything.
Any of these ESCs connected to a hub motor with giant fan blades bolted to it on a tower will REGEN enough power to charge* your Lipos. 

Ta-Daa!


*trickle
```

---
