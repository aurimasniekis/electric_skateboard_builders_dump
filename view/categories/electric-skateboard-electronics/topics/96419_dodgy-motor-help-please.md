# Dodgy motor? HELP PLEASE

### Replies: 1 Views: 107

## \#1 Posted by: Nedtrampz Posted at: 2019-06-12T07:38:13.274Z Reads: 39

```
So i have a sensored 6374 maytech motor being run by vesc 6. What ive landed on is running sensorless.. BUT, when i spin it up it goes both ways. Depending on where it lands. When i plug vesc in it flashes red for about 3 -5 seconds is this normal? No fault codes shown in terminal.

It was being run sensored before using a vesc4 which burnt out motor locked up and threw me off. Was never sure if it was in the motor or because i wrapped the vesc4 up in bubble wrap & was drawing high currents from it. Anyways all motor wire survived. 

I have just gone to do the setup today with vesc 6 / 12s & have had a series of problems..

First off i ran the motor detection with everything plugged in to be sensored. It did the detection fine & spun up fine. BUT, when i tried to test motor direction it locked up instantly & screamed at me VERY LOUD!! HIGH PITCH NASTY SOUND.. 

Then someone suggested swapping 2 phase wires. Tried that & when i ran the detection again it came up sensorless. It didnt seem to spin as nicely that time either.

I then had it do the detection WITHOUT SENSORS, which went fine but after that i goto spin it up & it can spin both ways.. depending on where it lands i think it decides which way it wants to spin. Yes i am using current no reverse / w brake. 

I tried the motor detection 1 more time & it didnt spin the motor up this time. It didnt know which way to spin. But it did finish successfully. 

The new vesc tool is strange it does all 3 tests on motor in sequence. & doesnt allow you to set the current limits til after.. it automatically set me at 48A motor / 99A for my battery which way too high.... i have 70c lipo batteries but i only want it on 50 which i had to do after..

I am scared to run the motor detection again because i dont want to fuck my trampa vesc6. 

No fault codes show on the vesc but the motor just simply wont work the way it should. 

ANY HELP APPRECIATED
```

---
