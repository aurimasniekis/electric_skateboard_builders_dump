# NEED HELP - vescs not working but i dont know whats wrong

### Replies: 15 Views: 429

## \#1 Posted by: alfiepauley Posted at: 2018-03-21T15:07:51.598Z Reads: 77

```
ive been building my board for a while now and riding it too. but earlier this week i had come accros a problem where everything on my board just shut down, including the battery indication that was connected straight to the on off series connector that i made. now only one of my vescs work but still, that cuts on and off with the motor and the other vesc is not working at all. i will be uploading pictures soon but in the mean time please help me figure out whats wrong. i had a 10s4p battery and dual vescs but it will have to now be a single motor build. please help and ask questions so i can get back riding

thank you
```

---
## \#2 Posted by: Martinsp Posted at: 2018-03-21T15:40:23.443Z Reads: 68

```
Try to remove everything between battery and VESC. Plug each VESC separately to the battery to test if they work. It may be a BMS issue or a switch issue or the VESC.
```

---
## \#3 Posted by: alfiepauley Posted at: 2018-03-21T16:42:49.437Z Reads: 62

```
I’ve tried that, the battery is charging and I’m reading 40V from the battery itself but one vesc that I thought was broken supply’s power to the receiver but none of the leds turn on, on the vesc
```

---
## \#4 Posted by: Martinsp Posted at: 2018-03-21T17:00:59.053Z Reads: 61

```
So without bms only one vesc works, correct?
And with the whole setup (battery,switch,indicator) the other vesc works correctly? 
If that is the case it seems like one of the vescs is broken. I am not sure if that is the main cause of the Robles since you mentioned that the indicator turned off too.
```

---
## \#5 Posted by: alfiepauley Posted at: 2018-03-21T21:52:28.905Z Reads: 46

```
On the other ‘working’ vesc the leds appear and it connects to a laptop just fine but when connected to a motor it doesn’t work
```

---
## \#6 Posted by: Martinsp Posted at: 2018-03-21T22:15:41.288Z Reads: 39

```
Does it show any faults? either from the start or when you press arrow keys
```

---
## \#7 Posted by: alfiepauley Posted at: 2018-03-23T07:10:25.191Z Reads: 32

```
When the vesc is connected to the computer?
```

---
## \#8 Posted by: Martinsp Posted at: 2018-03-23T08:05:25.655Z Reads: 29

```
Yeah, try pressing arrow keys and then type "faults" in the terminal
```

---
## \#9 Posted by: alfiepauley Posted at: 2018-03-23T12:33:40.961Z Reads: 22

```
If that doesn’t work then what’s the problem
```

---
## \#10 Posted by: Martinsp Posted at: 2018-03-23T12:53:42.799Z Reads: 22

```
What do you mean does not work? It should say either what fault there is or no faults registered since startup. One or the other.
```

---
## \#11 Posted by: alfiepauley Posted at: 2018-03-23T12:57:29.871Z Reads: 21

```
Hold on, I’ll connect it to my computer in a minute and I’ll tell u what it says
```

---
## \#12 Posted by: Deckoz Posted at: 2018-03-23T12:57:34.097Z Reads: 22

```
If he doesn't get faults and only the blue and green LEDs turn on then the MCU (stmf4) is fried or d4/5 are messed up. If the red led still works you should be able to connect to PC and use the terminal.
```

---
## \#13 Posted by: Martinsp Posted at: 2018-03-23T12:59:13.116Z Reads: 22

```
I think he said he is connected to PC, I might be wrong. I assumed he is so I did not consider the mcu to be at fault.
```

---
## \#14 Posted by: alfiepauley Posted at: 2018-03-23T13:07:23.272Z Reads: 20

```
I’m going to connect it to my pc soon to see what happens, should I run a motor detection?
```

---
## \#15 Posted by: Deckoz Posted at: 2018-03-23T13:40:06.806Z Reads: 16

```
If it can do it yes.
```

---
