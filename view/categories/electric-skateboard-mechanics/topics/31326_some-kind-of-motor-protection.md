# Some kind of motor protection?

### Replies: 22 Views: 1562

## \#1 Posted by: Bloop Posted at: 2017-08-23T19:17:49.129Z Reads: 226

```
Hello today during my ride i has some unexpected little breaks while keeping my remote at constant speed. It was kinda strange but i trust my remote so i didnt think the remote would make me problems..

I flipped my board inspected it a bit nothing strange.. so i went forward without problem till i get home. I connected my vesc to BLDC tool no faults. Well thats good.

At further inspection i saw a little rock inside my motor just stuck between the faze wires... 

Im using the enertion motor and used it for like 5 weeks with no problems till now. How could i protect the motor? any ideas or suggestions .. the roads around here are full of small rocks and im trying to avoid it as much as i can but not always possible ..
```

---
## \#2 Posted by: jrpwit Posted at: 2017-08-23T19:25:39.851Z Reads: 221

```
Did removing the rock fix the random breaking issue?
```

---
## \#3 Posted by: karma Posted at: 2017-08-23T19:29:27.057Z Reads: 217

```
You could buy sealed motors or motors with very small gaps. I am sure you could 3d print a little enclosure but that would make the motor run hot because of less aircooling
```

---
## \#4 Posted by: Bloop Posted at: 2017-08-23T19:38:35.273Z Reads: 213

```
not sure. I will have to test it tomorrow. I will keep you updated.. but so far is the only problem i could think of ...
```

---
## \#5 Posted by: Bloop Posted at: 2017-08-23T19:40:15.365Z Reads: 206

```
ye im actually looking for some sealed motors .. but i need some $$ first. 

And my motor is already getting hot while im riding. now i think is only normal.. is not too hot.. i mean i can keep my hand on it so yeah .. if ill add protection it will go even hotter ..
```

---
## \#6 Posted by: darkkevind Posted at: 2017-08-23T20:00:05.649Z Reads: 193

```
Just use very fine metal mesh over the holes...
```

---
## \#7 Posted by: Namasaki Posted at: 2017-08-23T20:10:38.492Z Reads: 195

```
You mean like this:
<img src="/uploads/db1493/original/3X/7/6/76d6caa7a775e9f8c03fe77d1b0a240ec611f249.JPG" width="375" height="500">
It happens. Not sure you can stop it without sealing up the motor and then what about heat.
```

---
## \#8 Posted by: Bloop Posted at: 2017-08-23T20:13:00.919Z Reads: 189

```
Yes something like that .. just mine was near the hole so i could just poke it and remove it without opening the motor..

Im afaraid of damaging the motor if a rock gets stuck inside.
```

---
## \#9 Posted by: Bloop Posted at: 2017-08-23T20:14:15.248Z Reads: 188

```
wouldnt that mesh break if a rock jumps into it ? 

And do you have some example of mesh not really sure what i could use :-?? .
```

---
## \#10 Posted by: banjaxxed Posted at: 2017-08-23T20:26:07.574Z Reads: 186

```
@trampa has a pictorial guide for doing this I'm going to try it, HEV motors are another option I think but I haven't found sensored HEVs
```

---
## \#11 Posted by: darkkevind Posted at: 2017-08-23T20:29:56.903Z Reads: 187

```
Something like this, and no, it wouldn't break if it's fixed correctly...

<img src="/uploads/db1493/original/3X/f/6/f694a1fbad18e46ea5115e74fde0d7a2705c46a9.jpg" width="562" height="500">

Search Google for "metal gauze mesh".
```

---
## \#12 Posted by: Bloop Posted at: 2017-08-24T14:26:16.649Z Reads: 167

```
Well sadly it did not fix the issue.. My board is losing signal sometimes and accelerating for 2 secs before it stops.. 

Any idea what that could be? I tried to reproduce it at home but nothing is just random during my rides .
```

---
## \#13 Posted by: jrpwit Posted at: 2017-08-25T02:19:27.301Z Reads: 148

```
That sounds really weird my board had been acting funny ever since I put it into foc. It would sometime brake randomly whenever I am coasting. 

I think it just the remote though. I have the nunchuck and have dropped it a couple times.

Your problem sounds really strange though. I have no idea :confused:
```

---
## \#14 Posted by: Bloop Posted at: 2017-08-25T14:02:32.738Z Reads: 137

```
Yesterday when i was out i was waiting at a stoplight and the board was accelerating for a bit without pushing the throttle .. I flipped it over and then i saw the red led on the vesc turning on and motor acelerating but my remote was on the ground .. 

Now that i think might be from the remote cables to vesc .. somewhere probably form the vibrations it got disconected a bit or idk .. i will resolder it and see how it goes
```

---
## \#15 Posted by: Deckoz Posted at: 2017-08-25T14:09:43.996Z Reads: 137

```
Vesc led turns white when accelerating... If its turning red, like you said it could be the receiver/ppm connection. But if its accelerating while doing that your failsafe isn't setup properly on vesc as well as your ppm endpoints and center point is probably wrong.

Oh and the original question motor scrape guards...if you have duals just make their height high enough so they don''t touch. And put mesh if you want over the mounting plate holes...should keep rocks out
```

---
## \#16 Posted by: ninja Posted at: 2017-08-25T14:17:38.944Z Reads: 139

```
Maybe woman's tights over the motor holes will be o.k. 

I"m planning to try that out with my sk3 motor😁

Imagine your motor look like this 😍:

<img src="/uploads/db1493/original/3X/3/0/30f856714957db49dc92d62878fe8b50a4eddf61.jpg" width="400" height="500">
```

---
## \#17 Posted by: Bloop Posted at: 2017-08-25T14:25:19.008Z Reads: 133

```
[quote="Deckoz, post:15, topic:31326"]
your failsafe isn't setup properly on vesc
[/quote]

What failsafe ??

The ppm endpoints and center are all good use this setup for like 2-3 weeks without problems and since then i never changed my vesc settings. 

Thats what i think too the receiver connection :\ ..
```

---
## \#18 Posted by: wafflejock Posted at: 2017-08-25T16:13:17.531Z Reads: 128

```
There is a failsafe in the BLDC configuration for if your receiver gives no input how long it should wait before going to idle (also can brake if you want that for example if you're in a hilly area and there's a chance it goes into failsafe while you're going downhill and you lose electric braking).  Under the app configuration tab see Timeout (when no control signal is received).

If the timeout is already active you might also have a failsafe on the controller side that needs to be set so the receiver sends an idle signal or stops sending a signal if it loses connection to the transmitter too though so would look at specifics for your controller.  Personally made my own transmitter/receiver so I used a jbtek cheap DIY oscilloscope to check the receiver output when my transmitter gets out of range or it is powered off randomly or I pull any of the pins between the actual radio and MCU on my custom setup.  There are phone apps for oscilloscopes but they're typically meant for just dealing with audio signals really so you'd likely need to use a voltage divider or otherwise step down the pwm voltage to use one of those, the jbtek one was around $30 for a kit you put together or $40 for a prebuilt one.  With an oscilloscope you can see the PWM signal clearly it's a 1.5-2ms pulse, you could also rely on the ADC on the VESC to show this to you in the PPM tab with the display checkbox selected.

---

Only issue with bench testing like this is if the problem only happens under load or when things are vibrating.  If it only happens under load you can partially simulate that using a belt or something similar wrapped around the wheel to provide friction but need to be careful to not break your wrist if you're holding onto things attached to the motor while running it (had a buddy mess his back up real bad from a drill that caught into concrete he was drilling into while up on a ladder).  If the problem manifests only while a load is applied would monitor the active sampling section and look for faults in the terminal (perhaps something overheating for some reason).

If it doesn't happen on the bench at all even when you apply friction then I'd start to lean more towards vibrations shaking a connection loose, if your receiver connections are all soldered would just wiggle all the wires to make sure nothing is a cold solder point or a weak connection and resolder any questionable parts, if you're using plugs (for the receiver/ESC connection) just make sure everything is glued into place after it's connected if it's meant to be a "permanent" connection, hot glue does a good job sticking plastic to plastic in a semi temporary way (can still be peeled away with some effort but should hold things in place when vibration is the problem).
```

---
## \#19 Posted by: Deckoz Posted at: 2017-08-25T17:46:37.828Z Reads: 113

```
The other part of proper failsafe is setting your PPM endpoints and center points properly. But I like your response

@Bloop 
Setting them to some value some guy on this forum told you to set is not accurate.

On PPM tab the green bar has a ppm readout.

Push your throttle on the remote to full. - in the box by the green bar, read the number and put that in ppm max pulse width, ie mine is 2.06

push your throttle to full brake and read the number - plase in ppm min pulse width ie mine is 1.03

release the throttle and allow it to center. read the number, mine for example is 1.55, set this as your ppm centerpoint.

If your centerpoint is not set to the actual ppm pulse width of what your remote is putting out. when you failsafe ie by loss of connection it wont start braking as long as you've set the time outs like waffle explained above. 

The other part of failsafe is done via binding, so if the remote failsafes on the receiver...ie you lost connection between transmitter and remote, when you set failsafe on the receiver it holds the neutral position of the normally received signal.

for example if you failsafe at the receiver, and you never set your failsafe, the default is whatever it was at the factory. this could be a ppm pulsewidth that doesn't match your actual transmitter output. ie

receivers failsafe is set to 1.45, but your transmitter puts out 1.55 when the throttle is in center. well as soon as connection is lost, 1.45 is lower then center, that means its braking.

you need to program all of the above for a good failsafe setup

-VESC timeouts
-Proper ppm end and center points
-setting failsafe on receiver during binding
```

---
## \#20 Posted by: Bloop Posted at: 2017-08-25T21:50:26.024Z Reads: 96

```
Thank you but as i said my ppm is set well for my remote i did these stepes. i asked what other failsafe o could add. 

The problem is not that is loaing signal cause when is loosing signal it will keep the currnet position for 1 sec then drop to 0. 

In may case i think the wire from receiver was moving so it sometimes though it is getting positive signal and went lil further.. not sure tho.. i did not resolder it only pused with my hand and today i had no problem... is so odd to me..
```

---
## \#21 Posted by: banjaxxed Posted at: 2017-08-26T08:58:58.741Z Reads: 78

```
Lady arse is always welcome but pretty sure motor heat would melt lady nylon, you can buy sheets of aluminium fine mesh from a motor factors, amazon, eBay it's not hard to find
```

---
## \#22 Posted by: adilism Posted at: 2018-03-16T12:23:31.822Z Reads: 47

```
Check [this](https://ru.aliexpress.com/item/Metal-Cover-For-Electric-Brushless-Motor-N63-Screen-Protected-Metal-Motor-Grille-External-Rotor-Motor-Guard/32826978673.html?spm=a2g0s.13010208.99999999.270.j9nv7X) thing out. It's a screen protector used for mountain boards. I'm currently doing a first build for myself and will be getting it to shield the motor. Small air holes should prevent overheating, at least that's what I'm hoping for.
```

---
