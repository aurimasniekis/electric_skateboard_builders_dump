# Brushless Ragebridge

### Replies: 6 Views: 929

## \#1 Posted by: laurnts Posted at: 2017-07-26T10:15:29.170Z Reads: 105

```
So there is a new custom ESC released. The guy who build it studied at MIT (Charles) that have been joining battle bots and dissecting numerous chinese ESC for the last few years. He developed Ragebridge earlier to control brushed motor and now he released a new version for the bruhsless Ragebridge brushless.

The link is below
http://e0designs.com/products/brushless-rage/

http://e0designs.com/wp-content/uploads/2017/07/blrage-clean.jpg

Some details (taken from the site)
Quick Specifications

Voltage Input Range
20V to 90V (SimonK Signal Board)
Up to 60V (6FET and 12FET Power Boards)
Control Scheme	Sensorless Block Commutation (SimonK Signal Board)
Switching Frequency
21KHz (SimonK Signal Board)
Braking
Synchronous rectification with regenerative braking default
Inputs	1ch R/C Servo, 1100-1900us reversible default (SimonK Signal Board)
Size	1.6″ x 1.6″ x 0.2″ (SimonK Signal Board)
2.75″ x 2″ x 1.1″ (6FET Power Board)
4.3″ x 2″ x 1.1″ (12FET Power Board)
Weight	1oz (SimonK Signal Board)
3oz (6FET Power Board)
7oz (12FET Power Board)
Heat Management
Aluminum heat spreader plate
More Information

Brushless RageBridge is designed as an expandable platform for the brushless experimenter. With a Signal Board and Power Board, a complete ESC can be made, but each half can actually be used on its own in your custom application!

The SimonK Signal Board is a carefully tuned variant of the open-source SimonK multirotor & drone ESC firmware. Originally developed for quicker response for aerobatics, it features many tunable parameters and is considered to be a more robust firmware for applications needing to overcome inertia, such as robot and EV drivetrains as well as large propellers. We tuned SimonK using our own robots and vehicles to start and reverse most sensorless BLDC motors reliably, with a mere 2.1% minimum duty cycle. Many settings are changeable using a AfroESC USB adapter (or similar USB flashing tools) on a dedicated 3-pin connector, communicating with the KKMulticopter Flash Tool. Programming instructions can be found in the User Manual and Tuning Guide.

Powerful 4.5 amp peak gate drivers and heavily optimized noise isolation, plus an opto-isolated input, enable you to pair it with very large output transistors to drive outsize loads. Up to 90v input voltages mean you can run higher than usual system voltages for maximum efficiency.

We recommend the SimonK Signal Board be used only in dynamic applications, i.e. loads which carry and change velocity frequently, and do not recommend its use in loads which require sensitive position or torque control.

The 6-FET and 12-FET power boards use the latest generation Infineon surface-mount flat-package MOSFETs on an isolated aluminum heat sink for maximum current throughput and switching efficiency at up to 60V maximum. We put enough bus capacitance on these boards to handle their continuous rated current forever at partial duty cycles, and 4oz double-sided traces complete the robust and reliable power handling package.

Both power boards feature onboard phase voltage sensing and two current sense resistors on the phase outputs. Mate these power stages to your own logic board through the common interface connector to create your own motor controller. Want something smarter than R/C? Don’t wait for us, build it yourself!

Documentation

User Manual and Tuning Guide – SimonK Signal Board (Coming Soon!)
Installation Drawing (Coming Soon!)
SimonK Signal Board CAD Model
6FET Power Board CAD Model
12FET Power Board CAD Model
Brushless RageBridge Connector Interface Pinout (Coming Soon!)
Brushless RageBridge Custom Power Stage Example Schematic (Coming Soon!)
SimonK Signal Board Default Firmware (Coming Soon!)
SimonK Signal Board Schematic and PCB Files (Coming Soon!)
6-FET Power Board Schematic and PCB Files (Coming Soon!)

---
Would be interesting if someone tested this or create some analysis over the performance. Maybe someone with some extensive electronics skills might now some plus minus points.
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-07-26T10:26:07.549Z Reads: 98

```
6 fets - 60A
12 fets - 120A
sounds interesting :slight_smile:
Price point is in the Vesc region.
I´d love to see someone putting that on an eMTB and give it a go!
```

---
## \#3 Posted by: Cobber Posted at: 2017-07-26T11:27:30.136Z Reads: 92

```
could be a good eMTB style control system, 

[quote="laurnts, post:1, topic:28673"]
We recommend the SimonK Signal Board be used only in dynamic applications, i.e. loads which carry and change velocity frequently, and do not recommend its use in loads which require sensitive position or torque control.
[/quote]

In eSk8 talk, I think this means: only use this if you ride like @Nowind
```

---
## \#4 Posted by: evoheyax Posted at: 2017-07-26T17:36:05.500Z Reads: 67

```
@Cobber  Video of nowinds riding? :stuck_out_tongue:

Can't wait to see someone try it.
Seems interesting.
```

---
## \#5 Posted by: laurnts Posted at: 2017-07-27T08:29:01.657Z Reads: 38

```
I'm waiting for @jtag to analyze :smiley:
```

---
## \#6 Posted by: laurnts Posted at: 2017-07-27T08:30:48.843Z Reads: 36

```
What I find interesting is that it doesn't look like it use DRV chip that often get burned down.
```

---
