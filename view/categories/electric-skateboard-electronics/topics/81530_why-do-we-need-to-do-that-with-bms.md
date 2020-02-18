# Why do we need to do that with BMS?

### Replies: 8 Views: 217

## \#1 Posted by: Arek Posted at: 2019-01-20T19:34:58.700Z Reads: 97

```
Almost all BMS pass all the current through few mosfets and in case they detect undervoltage, overtemp or over current they switch the load off.
And I think it's not a good idea, as it very often limits the maximum current we can pass through it and there's heat generated.

VESC can already measure current and switch it on or off(by just not spinning the motors), all we have to do is just have some kind of extension module that will measure voltage of each cell, voltage of entire pack, its temperature and we connect it via CAN to VESC so in case of for example undervoltage of one section of cells it simply sends the command to VESC to stop running the motors.

Example:
- Main uC STM32
- Multicell Battery Stack Monitor LTC6803G-2 up to 12S, used in DieBieMS, communicates through serial to uC
- Some CAN transceiver IC to communicate with VESC
- 5V to 5V isolated DC-DC converter with a 1S li-on charger IC for balancing, drains voltage of highest section and dumps it to the lowest, by switching between the cells with a lot of mosfets, can easily get 1A balancing current
- Automotive 50V 100-300A fuse to prevent fire in case of VESC failure
- Some kind of circuit to switch the logic of MBS completly off when not in use + VESC ultra low power mode.
- Just one big mosfet to switch off when charged

Disadvantages:
- less safe, voltage will be always present on the outputs
- ???

Is it a good idea?
I'm new to esk8 so I might be missign something :stuck_out_tongue:
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-01-20T20:59:24.687Z Reads: 67

```
Most people on this forum bypass their BMS for discharge already, for those exact reasons. The disadvantage is that the vesc always draws some power to run the microcontroller, and since it's a fairly high performance micro, it doesn't go as low-power as the ones in a BMS. 

Active balancing is much more difficult and complicated than a dc-dc converter and some fets. It's been done, but is a much more expensive and physically larger method, and you don't need 1 amp of balancing current unless you either have a huge battery capacity, or cells that are very badly matched, in which case you should not be using them in an esk8 in the first place. So basically you're reinventing the wheel and making it more complicated for no reason. It's easier to just get a cheap low current BMS and bypass it for discharge, if that's your intent.

I like having the extra layer of protection that a full-authority BMS provides, since the battery is the heart of any EV build, and often the single most expensive part.

Also, if you have ancillary equipment (lights, voltmeter, etc) on your board, the "vesc switch" idea won't allow you to turn them off. You'll still need a loop key or other main switch.
```

---
## \#3 Posted by: Arek Posted at: 2019-01-20T21:07:51.563Z Reads: 61

```
It wouldn't be more complicated that other uC based BMS.
Also just shorting the cheap BMS will remove most of the protection, no thermal protection, no P section undervoltage protection which might be needed even with a quality pack out of new cells.
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-01-20T21:27:56.014Z Reads: 56

```
There are basically two schools of thought regarding the role of a BMS. One is "A BMS is for balancing, nothing more." Minimum size, cost, and authority. 
The other is "A BMS is a complete management solution." Full authority, at the cost of greater size and pricetag. 
Both have solutions. I'm not saying your idea has no merit, just that I don't see a huge reason that it's better than the others.
```

---
## \#5 Posted by: mynamesmatt Posted at: 2019-01-20T22:52:22.508Z Reads: 42

```
correct me if I'm wrong but can't the DieBieMS do this...?
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-01-20T23:01:02.834Z Reads: 38

```
Shhhh

Hey op if you want to sell your diebiems I'll buy it off you, granted it's still in good shape 😭😂😂
```

---
## \#7 Posted by: Arek Posted at: 2019-01-20T23:09:08.207Z Reads: 34

```
It does communicate with VESC through CAN, but doesn't do most of the things I mentioned.
I thought DieBieMS is finally the BMS we needed but nah it has limited discharge current, doesn't support regen braking and has issues with balancing performance(overheating).

Though for now I'm going for DieBieMS, or at least trying to get it(hard to speak to that chinese guy that manufactures/sells these).
So sorry @Sn4pz I don't have one for sale...
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-01-20T23:09:48.231Z Reads: 32

```
All good :) 


I'll just have to be patient
```

---
