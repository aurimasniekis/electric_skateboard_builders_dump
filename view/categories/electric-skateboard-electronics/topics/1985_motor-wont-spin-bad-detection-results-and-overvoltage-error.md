# Motor won&rsquo;t spin, Bad detection results and overvoltage error

### Replies: 15 Views: 2498

## \#1 Posted by: shuey Posted at: 2016-03-25T15:42:43.902Z Reads: 175

```
Hello, I recently got my vesc up and running after to replacing the microprocessor, the green LED turns on when I give it input from my Nunchuck, but it doesn't spin the motor at all. When I have it in FOC it can read the R and L but the motor never jitters or anything after running tests, and when I give it input, it still doesn't respond. So after FOC failed I tried running the motor in  sensorless BLDC but it always spits "Bad Detection Result Received" back out at me. After that I ran faults in the terminal and I get FAULT_CODE_OVER_VOLTAGE, so I used my handy voltmeter to test the voltage at the motor leads and they are all just at a constant 42 volts (the power being put out by my power supply), even when I limit the voltage lower than that they still read the 42 volts. Does anyone know what this might be? I'm thinking it might be the DRV is dead too now.
```

---
## \#2 Posted by: trbt555 Posted at: 2016-03-25T15:48:32.262Z Reads: 172

```
What are your voltage cutoff settings ?
```

---
## \#3 Posted by: shuey Posted at: 2016-03-25T16:35:01.034Z Reads: 164

```
Currently they are:
Min input voltage: 8.00V
Max input voltage 30V
Battery cutoff start 10V
Battery cutoff end 8.00V
```

---
## \#4 Posted by: shuey Posted at: 2016-03-25T16:36:16.220Z Reads: 154

```
<img src="/uploads/db1493/original/2X/3/3c58b3163cc7634fb4790fbda9a9ec154321be56.png" width="690" height="388">
This is my current motor page

Also these are the faults I'm getting:
<img src="/uploads/db1493/original/2X/a/a91bdeb3810ee96b222f354a0791d6abb5768935.png" width="690" height="388">
```

---
## \#5 Posted by: trbt555 Posted at: 2016-03-25T18:25:16.480Z Reads: 143

```
Well there you have it.
If your power supply is giving 42v but your max input voltage is set to 30v, you're likely to get an overvoltage fault.
You need to raise the high limit to above your battery voltage.
```

---
## \#6 Posted by: treenutter Posted at: 2016-03-25T20:42:27.172Z Reads: 140

```
@trbt555 good looking out! I thought that the new VESC default setting was was higher than this. @shuey what firmware version are you using?
```

---
## \#7 Posted by: Haimindo Posted at: 2016-03-25T22:44:55.947Z Reads: 137

```
I had the exact same error today, glad I found this thread
```

---
## \#8 Posted by: shuey Posted at: 2016-03-27T18:14:46.162Z Reads: 123

```
@trbt555 @treenutter so I changed the voltages and stopped getting the overvoltage error, but it still wouldn't work. So i took the board to an oscillioscope and the signal from the nunchuck was making it into the DRV but there were no signals leaving it, soooo as far as i can tell it's a faulty DRV. I then replaced the DRV with another one, and tried running it with no luck again, and looking at it with the oscilloscope again, it was the same problem. I think it may be my motor which is causing these problems, so I'm going to have to go out and buy a new motor, hopefully once I have yet another new DRV in hand and a new motor I can get it working.
```

---
## \#9 Posted by: treenutter Posted at: 2016-03-28T00:49:57.923Z Reads: 114

```
[quote="trbt555, post:5, topic:1985"]
You need to raise the high limit to above your battery voltage.
[/quote]

Does anyone have a sense of how *much* higher this setting should be? It obviously needs to be high enough to allow a buffer for short voltage spikes, but then if it's too high it will fry the VESC. 

@trbt555 between you, me, and a few others on this forum I feel like we should write a "Welcome to your VESC, here's how to get started" sticky - there are so many parameters that get overlooked when first using it, and many can lead to a destroyed device or a streeted face (I've made every mistake I think!)
```

---
## \#10 Posted by: elkick Posted at: 2016-03-28T09:26:10.306Z Reads: 100

```
You can put it to 57V, no problem.
```

---
## \#11 Posted by: trbt555 Posted at: 2016-03-28T10:16:06.933Z Reads: 101

```
What pins are you measuring to conclude the DRV is at fault ?
You may be drawing wrong conclusions.
```

---
## \#12 Posted by: shuey Posted at: 2016-04-04T20:04:32.454Z Reads: 96

```
@trbt555 I tested pins 34 through 47 looking for anything, but they none of them changed at all while i was adjusting the input from the nunchuck (which was definitely connected).
```

---
## \#13 Posted by: trbt555 Posted at: 2016-04-05T04:57:37.974Z Reads: 90

```
So the DRV is not driving the mosfets, but is it being driven by the mcu ?
```

---
## \#14 Posted by: shuey Posted at: 2016-04-05T18:40:31.503Z Reads: 91

```
Correct, signal is coming out of the MCU, and being received by the DRV, but the DRV is not driving the mosfets.
```

---
## \#15 Posted by: jesser722 Posted at: 2016-09-23T00:09:51.635Z Reads: 62

```
I had the same problem and it was fixed when i set it to 57 amps, but now when i push start it and move the remote it does this short brake every time i press it. Any Ideas?
```

---
