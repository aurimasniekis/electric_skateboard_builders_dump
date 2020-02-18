# ESC not calibrating

### Replies: 8 Views: 1048

## \#1 Posted by: Ryanliu Posted at: 2017-02-05T07:18:45.617Z Reads: 70

```
Im using this 
ESC: http://www.ebay.com/itm/Waterproof-120A-Brushless-ESC-Speed-Controller-Truck-Hobbywing-EZRUN-WP-SC8-/300854328202?hash=item460c50bb8a:g:9SkAAOSwKtlWsGyD
Battery: 18650 pack worked on my ebike. 42v ~10ah
motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html
controller: http://www.ebay.com/itm/2-4G-mini-size-remote-controller-w-receiver-W1-2-f-electric-skateboard-longboard-/172388976080?var=&hash=item28232f05d0:m:mU40HfeMoo4GXA63hHQ0iKA
(worked on my other esk8)
Followed these instructions:http://www.hobbywing.com/products/enpdf/XeRun120AV311S.pdf

Problem:
When i try to calibrate it i hold the set button down and turn it on and i let go of the set button when the red LED started blinking. I then pressed the set button again when my throttle was at neutral and no sound or green LED flash happened?
Am i getting anything wrong. Idk what is wrong
```

---
## \#2 Posted by: Lukas Posted at: 2017-02-05T07:22:35.695Z Reads: 63

```
Your battery is 10s.
Your ESC can only handle 4s.
Try it with a 4s battery :slight_smile:
```

---
## \#3 Posted by: Ryanliu Posted at: 2017-02-05T08:14:14.389Z Reads: 61

```
Just tried it with 4s and the same problem persists
```

---
## \#4 Posted by: Sander Posted at: 2017-02-05T11:04:41.119Z Reads: 51

```
is it lightning green?

if so:


First switch **OFF** the **ESC**, then **connect** it to the **battery** **pack**. **Turn** **ON** the transmitters(controller) and **pull** the **throttle** of the controller **backwards** end position(braking). 

Then you **hold** the **SET** button on the **ESC** and switch it **ON**, wait **2 second** for the **GREEN LED** to begin to flash and the motor make **beep beep**, then **release the SET button and pull the throttle of your controll to neutral also just let the throttle go to middle**. Then you will hear a **continous** **beep** **sound** and see a **red** **Led** **blink** **continous**. **then** click **SET** again and you will hear **another** **beep**!

Now **drag** your **throttle** **trigger** to the **end** of your **front** **position** of the **controller** and press the **SET** button one time and you will hear the **motor** **beep** **beep**.

Lastly **push** the **throttle** **trigger** to the **end** position of **backward** and **press** the **SET** button **one** time, and then you will **hear** **beep beep beep**. **red** and **green** will **blink**, then the **throttle range calibration is done**. the motor can be started after **2 seconds**.
```

---
## \#5 Posted by: Ryanliu Posted at: 2017-02-05T20:19:39.187Z Reads: 35

```
It beeps once and works for neutral but when i press full forward it doesnt beep at all. It just flashed the red LED really fast continuously and doesnt respond
```

---
## \#6 Posted by: Ryanliu Posted at: 2017-02-05T20:27:30.475Z Reads: 29

```
When i press the set button on full throttle
```

---
## \#7 Posted by: Sander Posted at: 2017-02-13T20:02:07.007Z Reads: 20

```
Didnt you get a information thing on how to use it?
```

---
## \#8 Posted by: Ryanliu Posted at: 2017-02-13T21:08:32.020Z Reads: 17

```
Just found out why. Im using a 10s battery on a 3s esc. Changed to 3s and it works now
```

---
