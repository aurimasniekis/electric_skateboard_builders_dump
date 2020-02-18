# Vesc fault_code_drv help

### Replies: 10 Views: 185

## \#1 Posted by: MadPatch Posted at: 2019-11-30T20:14:19.576Z Reads: 44

```
Hey so I have been running my setup for about 2 weeks now with probablly about 10 miles on it. And recently my vesc has been reporting "fault_code_drv" I built a custom remote from a wii nunchuck similar to a lot of examples out there with nrf and arduino. I have been having issues with the remote dying on me because of a short I believe and am working to fix it. So i was about 1/2 mile away from my house when the remote died on me, no surprise here. And so I walked it back but there was a hill so I decided to just jump on the board with the battery unplugged and cruise down the hill so I wouldn't have to walk. I have ridden it before with no power and had no issues. 

Could the motor create enough current as a generator to blow my vesc? I know with the old vesc tool you could limit the amount of current from an input, but with the new tool there isn't an option so I guess I just didn't think of it. Is it practical to try and replace the drv chip or is there probally other componets blown too? 

I am kinda less concerned on fixing it and more on undestanding why this happened so I can avoid it in the future!

Let me know if you have any thoughts. 
Patrick.
```

---
## \#2 Posted by: Skunk Posted at: 2019-11-30T20:46:45.766Z Reads: 41

```
Like actual trampa vesc?
Or other?
```

---
## \#3 Posted by: Santino Posted at: 2019-12-01T04:57:32.507Z Reads: 33

```
I think it could be a short from the motor wires (touching each other) o a loose bullet connector, a short could easily damage the Vesc, but if you have all the connectors checked, the fault my go away...Unless DRV it is broken for good...
```

---
## \#4 Posted by: mjaffee Posted at: 2019-12-01T07:11:08.570Z Reads: 29

```
From what I know about DRV faults:

-its possible that there were some bad settings that led to the component failing. 
-vibrations can loosen the smd soldered component and cause issues, or cause things to short
-lots of brake can weaken the longevity of the component??(not sure but maybe)

The DRV can be ordered from texas instruments and replaced with using a reflow air solder machine. Its very difficult to do correctly without the proper experience. I fried my pcb attempting to fix it. About $100 in parts and electrical consumables without paying for the equipment. Probably just best to order a new vesc
```

---
## \#5 Posted by: MadPatch Posted at: 2019-12-01T15:47:55.123Z Reads: 24

```
I have the equipment and decent experience with soldering smd components. But not too much experience with vescs themselves that's why I was asking if there is any other components that would need repair as well. I did notice one of the 6 mosfets seem to have gotten real hot because the heat shrink around it was shrinking to it's shape.

Anyway, I ordered a new vesc, I just don't want it to happen again.
```

---
## \#6 Posted by: RedEagle Posted at: 2019-12-01T23:02:38.225Z Reads: 17

```
Looks like your DRV got blown due to a brown out. It's not a good idea to disconnect the battery and then jump on the board because, as you know, the motors are generators themselves. Then there's also the issue of back-emf. Please do keep the erpm limit in mind.
```

---
## \#7 Posted by: MadPatch Posted at: 2019-12-02T02:11:40.666Z Reads: 14

```
So what settings should I limit next time that will help prevent this. Thanks.
```

---
## \#8 Posted by: RedEagle Posted at: 2019-12-03T19:13:24.504Z Reads: 11

```
Don't go over the erpm limit and always keep the battery connected.
```

---
## \#9 Posted by: MadPatch Posted at: 2019-12-04T00:20:46.495Z Reads: 10

```
Is the erpm limit fixed?
```

---
## \#10 Posted by: alexnz Posted at: 2019-12-04T00:31:27.318Z Reads: 10

```
Anyone in the game of replacing the DRV chip on a Maytech 4.12 ? 
I can supply the part, but I don't have the skills or the tools. 
Preferably in South Pacific with shipping costs that need to match the alternative of a FSESC at $46 on AliX.
```

---
