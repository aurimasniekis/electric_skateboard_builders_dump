# Kid in a Candy store, Torque, MSB, Vesc

### Replies: 17 Views: 985

## \#1 Posted by: Bluecro Posted at: 2017-06-24T05:35:15.555Z Reads: 178

```
<img src="/uploads/db1493/original/3X/4/b/4bb6dfd18aa6e66520b493432707b6dbd5e5d82a.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/1/5/15433e5259fbef22d425b1b5259fc549b2504ca9.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/4/f/4f7b6268a984651a2245be02b8a4bf6b5d3d966b.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/e/7/e7fad77a81e01cd85ea02bbf5303005f0b366c12.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/2/c/2c5f174aa494376623d94aa0f6f162d66e497266.jpg" width="690" height="388">
```

---
## \#2 Posted by: wmj259 Posted at: 2017-06-24T07:34:17.933Z Reads: 151

```
I took you to the candy shop.
```

---
## \#3 Posted by: anorak234 Posted at: 2017-06-24T08:17:51.482Z Reads: 142

```
What battery config? Top speed? Looks absolutely amazing, but give us the details!
```

---
## \#4 Posted by: Bluecro Posted at: 2017-06-25T21:10:17.825Z Reads: 103

```
Battery: Two 5000 mah, 6S, 20C in series. I carry two sets while riding.

Theoretical top speed is 32 Km, my first run I had it up to 26 Km, but i wasnt pushing it.

Two Motors 6374 190KV 3150 W

Two TORQUE ESC VESC Electronic Speed Controller enclosed in a vented Pelican box.

Trampa  trucks.

TorqueBoards 2.4ghz Nano Remote Controller. 

Board rides good but I have a couple of issues. The breaking is too strong so i decreased the amount of motor min amps. 
The other issue im having is the throttle, its too sensitive, like really sensitive, like knock you on your ass sensitive. Do you guys of any suggestions on programming for smooth acceleration?  Any thoughts would be much appreciated.
```

---
## \#5 Posted by: jazzcool Posted at: 2017-06-26T00:04:53.439Z Reads: 71

```
I like your design of pulling the wires underneath the board!
Btw, do you feel 6S configuration is powerful enough? What's your drive train ratio setup?
```

---
## \#6 Posted by: JLabs Posted at: 2017-06-26T00:28:21.858Z Reads: 59

```
That is the nano remote. Very unreliable and all around a terrible remote. For your safety get a mini, benchweel, or GT2B.
```

---
## \#7 Posted by: Bluecro Posted at: 2017-06-26T00:44:32.613Z Reads: 51

```
72 / 13, Ive only had one ride so far, lots of power, I went with  lower kv so i have higher torque.
I use two 6s in series.
```

---
## \#8 Posted by: Bluecro Posted at: 2017-06-26T00:46:05.010Z Reads: 48

```
I went with the nano because i like the size, Is the benchwheel better?
```

---
## \#9 Posted by: pennyboard Posted at: 2017-06-26T00:50:38.824Z Reads: 43

```
I've used the nano for 9 months and built 3 boards for other people using the nano, and haven't had any problems with it.
```

---
## \#10 Posted by: jazzcool Posted at: 2017-06-26T00:51:46.630Z Reads: 40

```
I am using same ratio and same kv (68/12, 192kv) on a 10S. Still building it and yet to test. I fear it's going to be  over powered ..
```

---
## \#11 Posted by: Bluecro Posted at: 2017-06-26T00:52:54.413Z Reads: 38

```
What have been the comments from the riders you built for regarding the nano?
```

---
## \#12 Posted by: Bluecro Posted at: 2017-06-26T00:55:56.209Z Reads: 39

```
I know you can adjust the throttle curve in Foc mode and with a firm ware upgrade but thats too technical for me. I would love to be able to just the throttle curve in BLDC mode.
```

---
## \#13 Posted by: pennyboard Posted at: 2017-06-26T00:56:56.795Z Reads: 37

```
I've specifically asked them about the controller because I was aware it had issues and was ready to replace it if they had any problems, but they've all told me that they've never experienced a signal cut-out or any other issues while using it.
```

---
## \#14 Posted by: pennyboard Posted at: 2017-06-26T00:58:58.839Z Reads: 38

```
That being said, I do suspect that the remotes can have issues depending on which batch the remote comes from, because some members have had complaints about the remote, but as far as I know, the last batch that had issues was shipped in July/August of 2016, so the new batches should work fine
```

---
## \#15 Posted by: Bluecro Posted at: 2017-06-26T00:59:56.631Z Reads: 42

```
Thats good to hear but can the throttle issue be addressed.
```

---
## \#16 Posted by: pennyboard Posted at: 2017-06-26T01:06:07.535Z Reads: 42

```
I'd suggest first reducing your start-up boost in BLDC Tool under the advanced tab. That's the simplest and probably easiest way to keep it from knocking you off the board.

What are your motor amps set at? Reducing those slightly will also make the acceleration less aggressive but it will come at the expense of power.
```

---
## \#17 Posted by: Bluecro Posted at: 2017-06-26T05:02:08.550Z Reads: 27

```
I adjusted the startup boost from .16 to .15. That along with the lower motor max and adjusting the display settings gave it a smoother speed acceleration. I think ill adjust both a little more. 

On a side note, as i was locking my feet in I accidentally gave it full throttle. Wow, we both went vertical, me on my ass and the board straight up in the air. Thankful for my G form padding and helmet.  Top speed today was 33 km/hr. thats 20.5 Miles/Hr. and that wasn't even pushing it. It was a great ride on an doff road. 15 km. trip.
```

---
