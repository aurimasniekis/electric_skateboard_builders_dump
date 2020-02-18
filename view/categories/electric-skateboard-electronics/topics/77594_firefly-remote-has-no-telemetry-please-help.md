# Firefly remote has no telemetry please help

### Replies: 14 Views: 335

## \#1 Posted by: Pete75 Posted at: 2018-12-10T09:56:38.367Z Reads: 111

```
Hi guys sorry but I have used the search functions and gone through many topics.
I have built the Firefly remote by SOLIDGEEK and it is connected to the FOCBOX.  I have configured the focbox to the best of my ability with Ackmaniac esc_tool. I get the motor to spin up and brake but get no telemetry for voltage or speed etc. The only telemetry that works is when I turn off the receiver the wifi icon on remote starts flashing(don't know if that is telemetry).  I have not touched the coding as I am not shore if anything needs to be changed.
I have included some screanshots, not shore if those settings are right as they are standard.![1|690x388](upload://lhapGGQfdna6Nqlmu0LSeyljf8B.jpeg) ![2|690x388](upload://cLSKYtVDqsawbIK99RR9Ybqini7.jpeg) ![3|690x388](upload://fQpUqyHcFtMILTfxGlHq6foHdeb.jpeg) 

On the remote I have it set to ppm and uart and I have the tx and rx pins populated on the focbox, and yes I have even tried reversing the wires but still no go.
I am using the nRF24-Esk8-Remote-development code.

I don't expect to be spoon fed but if someone could kindly point me in the right direction I would be grateful.
Regards Pete
```

---
## \#2 Posted by: Zyb Posted at: 2018-12-10T11:38:31.774Z Reads: 95

```
I would try standard vesc tool first to see if it is working at all. Development branch has solidgeeks modified library and he noted that in order to get telemetry you need to upgrade your fw to 3.40. I can confirm it doesn’t work with 3.38. Don’t forget to match your baudrate and it should be good.
```

---
## \#3 Posted by: Pete75 Posted at: 2018-12-10T20:09:05.942Z Reads: 79

```
Thanks Zyb I will check my firmware, I downloaded ackmaniac's tool yesterday and flashed it with the default few as I was not shore what the other ones were. With baudrate you mean setting it in Ackmaniac vesc tool? 
Thank you for the information I appreciate it.
```

---
## \#4 Posted by: Pete75 Posted at: 2018-12-10T22:36:20.767Z Reads: 74

```
Just upgraded to 3.4, must be the settings that are wrong as I still have no telemetry.  Oh well back to the drawing board lol
```

---
## \#5 Posted by: sofu Posted at: 2018-12-10T23:00:07.184Z Reads: 68

```
Try setting the baud rate to 115200, I don't remember if that's correct but worth a try. Also make sure you're using the correct vesc utiities version for your vesc. I'm unsure if the vesc6 utilities is backwards compatible with 4.*. Last resort is to check your soldering I suppose...
```

---
## \#6 Posted by: ervinelin Posted at: 2018-12-10T23:15:15.353Z Reads: 61

```
Did you use solidgeeks Uartcontrol library instead of rolling geckos? This is necessary for the latest vesc standard firmware.
```

---
## \#7 Posted by: Pete75 Posted at: 2018-12-11T02:21:24.321Z Reads: 57

```
Oh I didn't know that, so I should use the one from here?
https://solidgeek.dk/docs/firefly-remote/software/
Vescuartcontroll NEW.
```

---
## \#8 Posted by: Pete75 Posted at: 2018-12-11T02:22:55.780Z Reads: 50

```
The baudrate gets set in Vesc tool? right or do I need to change something in Arduino?
```

---
## \#9 Posted by: sofu Posted at: 2018-12-11T03:20:34.372Z Reads: 46

```
Vesc tool 10c
```

---
## \#10 Posted by: Pete75 Posted at: 2018-12-11T05:31:22.495Z Reads: 42

```
Sorry not shore what 10c means. I proboubly should by the sounds of it sorry.
```

---
## \#11 Posted by: sofu Posted at: 2018-12-11T06:08:12.270Z Reads: 36

```
"10c" is just filler letters because this forum doesn't allow you to give replies less than 10 characters long 🤣You can safely ignore it.
```

---
## \#12 Posted by: Zyb Posted at: 2018-12-11T09:16:28.732Z Reads: 32

```
Baudrate is in one of your pictures I can see it’s set to 9600 change it to a value whatever is set in your receivers code and it’s most likely 115200
```

---
## \#13 Posted by: Pete75 Posted at: 2018-12-11T09:22:54.091Z Reads: 34

```
Lol feel like a idiot....
```

---
## \#14 Posted by: Pete75 Posted at: 2018-12-11T09:23:22.666Z Reads: 34

```
Cheers Zyb will do
```

---
