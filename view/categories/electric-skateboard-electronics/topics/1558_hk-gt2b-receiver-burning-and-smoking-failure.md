# HK-GT2B Receiver burning and smoking failure

### Replies: 6 Views: 1193

## \#1 Posted by: b-rad Posted at: 2016-02-27T05:03:20.845Z Reads: 84

```
Okay, so I’ve put together this build last year and I never had any issues with the receiver or anything else really. I am using a skateboard deck, 190 kv enertion r-spec motor, hobbywing 150A ESC, HK-GT2B receiver, 6s lipo, enertion trucks, barefoot 83mm wheels. 

My problem is that 2 days ago I went to plug in the lipo to the ESC and everything was fine (it did spark as usual) then when I went to turn it on it made a crackle sound so I opened the case back up and the receiver was smoking. Every time I pressed the trigger on the remote the receiver would continue to emit smoke and the motor would not spin or anything. So I quickly turned everything off and disconnected everything. I checked all the wires to see if I caused a short circuit, but no wires seem to be cut or exposed to each other. 

Does anyone know what could be the cause/problem here? i was thinking maybe because i dident invest in a real switch instead of just using the ESC's switch.

<img src="/uploads/db1493/original/2X/a/a12f041fbe16d3e9d1b3c01f5e3144cc6110d54e.jpg" width="690" height="388">
```

---
## \#2 Posted by: Namasaki Posted at: 2016-02-27T05:50:35.746Z Reads: 83

```
Sounds like the bec circuit in the esc may have failed and is delivering 22+volts to the receiver.
Try disconnecting the 3 wire plug from the receiver and hook the battery up, turn on the esc and check the voltage output of the red(+) and black(-) wires. it should be 5 or 6 volts or something close to that. If it reads more, then you will need a new esc and a new receiver.
If the voltage output to the receiver is correct, 5-6 volts. Then you should be fine just replacing the receiver.
Note: The bec is a  type of voltage regulator.
Another note: The spark that happens when you connect the battery can damage the esc.
it is a very good idea to use some sort of spark eliminating device.
I am currently using an anti-spark connector that I got on amazon.com and it works like magic!
I am running 12s and I get no spark when connecting the battery. It is rated for up to 150 amps
http://www.amazon.com/gp/product/B00RVM93YO?psc=1&redirect=true&ref_=oh_aui_detailpage_o05_s00
```

---
## \#3 Posted by: b-rad Posted at: 2016-02-27T07:16:45.353Z Reads: 77

```
Okay thanks a lot! I will try that out and see how it goes. 

Is it safe to keep the batterys in the case plugged in when you have those anti spark connecters? I was thinking about buying a pre built connector switch but its like $60. I was wondering if those connectors you use will eliminate the need of the $60 switch

And i hate to sound like a noob, but how to i check the voltage of the red and black wires? With a regular 1-6s voltage meter?
```

---
## \#4 Posted by: Namasaki Posted at: 2016-02-27T14:50:01.231Z Reads: 67

```
The $60 switch is the best solution if convenience is a priority. 
The anti- spark connector is the best solution for a more pure connection.
(Assuming that any circuit is going to produce some resistance)
Less resistance = more amp flow. I=e/r  or current = voltage divided by resistance. 
Less resistance also = less heat. 
Now, since power = volts x amps. 
You will need lots of amps when using 6s battery. 
(If you end up getting a new esc, stay with 150a)

If you decide to go with the anti-spark connector, you will need to open the box and disconnect it when your done. Don't store you're board with the battery connected. And don't drain your Lipo battery below 3.2v on any given cell or you will degrade the battery. 

To check the voltage of the signal output wires, use a standard ac/dc volt meter. You can buy one at any hardware store or at Walmart. 
The black probe to the black wire and the red probe to the red wire.
http://www.amazon.com/gp/aw/d/B00TWTLWT8/ref=mp_s_a_1_2?qid=1456591662&sr=8-2&pi=SY200_QL40&keywords=volt+meter&dpPl=1&dpID=51LPPpUnIsL&ref=plSrch
```

---
## \#5 Posted by: Iceni Posted at: 2016-02-27T20:51:09.533Z Reads: 55

```
Just a small correction about the spark.
It will not cause damage to your ESC, at most it will cause some wear on your connector over time when plugged in/out enough.

Some people use the spark as a sign that the caps on the ESC is still healthy.
```

---
## \#6 Posted by: Namasaki Posted at: 2016-02-29T17:30:09.875Z Reads: 42

```
At 12s it doesn't just wear the connectors, it literally melts the tip with a loud pop where the arc occurs.
Whether the sparking and sudden rush of high current can damage any components or not. 
I say why take a chance. 
And why put up with the spark if you don't have to?
```

---
