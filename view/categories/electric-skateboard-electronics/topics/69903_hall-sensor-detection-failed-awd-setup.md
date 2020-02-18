# Hall sensor detection failed (AWD setup)

### Replies: 8 Views: 615

## \#1 Posted by: frameto Posted at: 2018-10-02T20:44:53.240Z Reads: 150

```
Hi guys,

I have an AWD (All-Wheel-Drive) e-board (10S5P / FocBox / Maytech 5065 sensored 220kv : see setup below).
After some 40km of ride without any issues and visible damages on any electrical component (motor, wires...),
I started it the next morning as usual and it began suttering : slow motion / normal / slow motion  / normal.
I checked the four motors and one had a temperature quiet higher than the three others (the front right one).
I decided to check this motor with the bldc tool and the "Start Detection" made the motor spin normally, 
but returned a "Hall sensor detection failed" (see detail below).
I made also a "Start Detection" of the front left motor to compare with, and it made the motor spin the same,
yet it returned a correct result with a "Detected hall sensor table" (see detail below).
Then I saved as xml the firmware configurations (of focboxes) of both motors, to compare them and maybe find something...
As you can see below, the xml hall sensor table of the faulty motor has "good values", that is : not the ones
returned now by the "Start detection" which are bad -1 values; and the xml hall sensor table of the good motor
is the same as the one returned now by the "Start detection".
So I conclued that this xml hall sensor table of the faulty motor, is the one that was written in the firmware
after a correct "Start detection" when the board was built.

From this I made the following hypotheses :
  A : the sensor wire adaptor is broken somewhere;
  B : the motor sensor wire is broken somewhere;
  C : a motor sensor is broken somewhere;
  D : something changed over the time between the focbox and motor, making the current firmware configuration obsolete...

For hypothesis A : I interchanged the adaptors of both motors and "Start detection" still returns the same : so this hypothesis is canceled.
For hypothesis B : See motor photos below : all are not that good, yet no visible damage, 
and according to an electronics guy : a continuity check of each cable is quiet impossible due to the way they are connected in the motor.
I doubt hypothesis C can be checked...
I have no clear ideas how/if hypothesis D can be checked.

So if you guys have ideas to further check some of these three last hypotheses it's cool,
otherwise just a vote on which part(s) to replace is welcome : without further checks (and/or votes),
I will replace the motor by a new one of the same model.

A last point : the 7th value of the failing sensor table detection is 1, whereas I read everywhere that
this value should always be -1 (or 255 which is the same in the firmware internals).
May be this 1 value instead of -1 can give further informations about the problem...
... and by the way : if someone can give the mapping between these values and their role its cool, I mean :
<hall_table_1> is the detected ground cable ? dtected voltage cable ? detected temperature cable ? 
<hall_table_2> same question
etc...

Thank's to have read my post anyway !

Franck

All-Wheel-Drive setup :
https://drive.google.com/open?id=1dUzzwHplBlBZniYbRBQGiHbisCsLHuUs


Motor photos :
https://drive.google.com/open?id=1EH46MGEru5Br2-u1LEF-71_wv-OfyOaY

Bldc tool start detection of faulty motor (Sensor mode : hybrid):

  - Detect parameters :
	Current : 6,00 A
	Min ERPM : 600,0
	Low duty : 0,05
  - Results :
	Detection results:
	Integrator limit: 106.65
	BEMF Coupling: 858.81

	Hall sensor detection failed:
	-1, -1, -1, 4, -1, -1, -1, 1

Bldc tool start detection of good motor (Sensor mode : hybrid):

  - Detect parameters :
	Current : 6,00 A
	Min ERPM : 600,0
	Low duty : 0,05
  - Results :
	Detection results:
	Integrator limit: 96.55
	BEMF Coupling: 839.77

	Detected hall sensor table:
	-1, 6, 2, 1, 4, 5, 3, -1

Saved xml configuration of FocBox of faulty	motor (= hall sensor table detection when the motor was ok) :

    <sl_bemf_coupling_k>800</sl_bemf_coupling_k>
    <hall_table_0>-1</hall_table_0>
    <hall_table_1>5</hall_table_1>
    <hall_table_2>3</hall_table_2>
    <hall_table_3>4</hall_table_3>
    <hall_table_4>1</hall_table_4>
    <hall_table_5>6</hall_table_5>
    <hall_table_6>2</hall_table_6>
    <hall_table_7>-1</hall_table_7>


Saved xml configuration of FocBox of good motor (matches the detection above) :

    <sl_bemf_coupling_k>850</sl_bemf_coupling_k>
    <hall_table_0>-1</hall_table_0>
    <hall_table_1>6</hall_table_1>
    <hall_table_2>2</hall_table_2>
    <hall_table_3>1</hall_table_3>
    <hall_table_4>4</hall_table_4>
    <hall_table_5>5</hall_table_5>
    <hall_table_6>3</hall_table_6>
    <hall_table_7>-1</hall_table_7>


Parts references :

Maytech motor model :
https://psychotiller.com/product/custom-maytech-5065-sensored-220kv-motor

FocBox motor controller :
https://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/

Bldc tool : 
https://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/

Posts found with similar issues/topics :

https://www.electric-skateboard.builders/t/unknown-hall-error-255/37058

https://vesc-project.com/node/85

https://www.electric-skateboard.builders/t/hall-sensor-detection-failed/19878

https://www.electric-skateboard.builders/t/hall-sensor-detection-has-failed/38515
```

---
## \#2 Posted by: frameto Posted at: 2018-10-03T06:14:54.831Z Reads: 93

```
I also se that : 
  - the detected "BEMF coupling" of the faulty motor is now 858.81 whereas 800 was written in the firmware
  - the detected "BEMF coupling" of the good motor is now 839.77 whereas 850 was written in the firmware

So maybe changing the "BEMF Coupling" of the faulty motor to 850 (so same as the good motor) is a good idea...or not...
According to [this document](http://vedder.se/2015/01/vesc-open-source-esc/) putting 50 more or less on this parameter is not that much significant...
I fear to rewrite the original configuration to avoid loosing some critical parameter... yet now that I've saved it in an xml file, I can still reload it afterwords with the 'Read Configuration' button, but having no experience of reading/writing configuration on such a focbox...when I didi such repeated read/write with my previous setup with basic VESC 4.12 I experienced the "multiplied by 10" bug (for those who know this bug), so I fear fallin back on the same scenario with this version of the focbox...

I checked also the configured BEMF coupling of the two other good motors (the rear ones) and it's 900...
```

---
## \#3 Posted by: Andy87 Posted at: 2018-10-03T07:06:55.356Z Reads: 79

```
Did you do the motor detection with of without belt?
Why you still use bldc tool? 
You can flash the new firmware and use the vesc tool.
Did you try motor detection in FOC?
I read about issues with focbox and sensor detection in bldc.
```

---
## \#4 Posted by: frameto Posted at: 2018-10-03T11:10:04.960Z Reads: 72

```
Both with and without belt : same result.
The bldc tool is the tool provided by the provider of this release of the focbox (see parts reference in my post). I already used the vesc tool with my previous build, but I won't decide to be in a state where 3 motors are configured with the bldc tool and one with the vesc tool...and I won't take the risk to reconfigure all motors with the vesc tool as 3 on 4 work well with the bldc tool...
yeah : try the motor detection in FOC mode : I've read that...but same : the four motors have to be configured in the same mode, but yeah just to try a detection in foc mode and hope the sensor comes back to life, even if I switch back to hybrid mode afterwords...
Thank's for your feedback !
```

---
## \#5 Posted by: Andy87 Posted at: 2018-10-03T11:16:29.779Z Reads: 67

```
it´s really not a thing to flash the firmware.
takes 1min per focbox, just make sure you chose the right file (410, 411, 412) and don´t disconnect wires or powersupply while loading ;)
and I understood that you need always to change all of the focboxes.
But in case sensors work in FOC it will take you 2-3 min for each focbox to set them up in FOC. so in total less than 15 min.
```

---
## \#6 Posted by: Sebike Posted at: 2018-10-03T12:05:28.508Z Reads: 65

```
Sorry for not reading through all five (!) posts.. and maybe I'm just stating the obvious, but if you loose sensors, most likely scenario is that a connector has vibrated loose. The most simple causes often tend to be overlooked ☺️
```

---
## \#7 Posted by: Acido Posted at: 2018-10-03T12:28:01.001Z Reads: 64

```
Did you ride the board thru water?
I fried my sensors because i went thru a small rain "pool"
```

---
## \#8 Posted by: frameto Posted at: 2018-10-03T21:33:46.233Z Reads: 48

```
I don't remembrer having crossed a rain pool...

I finally did a "cross test" to check hypothesis D, that is  :
1. connect the front right focbox with the front left motor (the good one) and make a "start detection"
2. connect the front left focbox (the good one) with the front right motor and make a "start detection"

The start detection of #1 was ok, so the front right focbox and it's configured firmware is ok with a good motor.
The start detection of #2 gave the same "hall sensor detection failed" error : so the front right hall sensor motor detection fails with both focboxes => hypothesis D is canceled and the problem is one (or both) of B and C.
As I doubt these maytech motors are designed to be reliably repaired I will replace this motor ...

Thank's for your feedbacks guys !
```

---
