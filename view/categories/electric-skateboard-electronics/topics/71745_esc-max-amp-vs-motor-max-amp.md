# ESC Max Amp Vs Motor Max amp

### Replies: 7 Views: 769

## \#1 Posted by: Savace Posted at: 2018-10-19T19:24:12.282Z Reads: 130

```
Quick question, I have an Trampa Eboard, just seen that the ESC are rated at 50AMP they are vesc v4.12 50a however each motor is a MTO6374 170KV Max. Current: 65A.

Should the ESC's not have a higher AMP rating than the motors? if so what is the danger of having a lower rated ESC than the motor can pull.

Thanks all
```

---
## \#2 Posted by: Andy87 Posted at: 2018-10-19T19:32:17.812Z Reads: 120

```
Motor amps not the same as battery amps.
For your vesc the rating is related to the battery amps.
A 4.12 vesc without heatsink shouldn’t be set over 35a.
If your motors rated to 65a it’s not an issue. You can set your motor max value to 65a than
```

---
## \#3 Posted by: Silverline Posted at: 2018-10-19T19:42:54.332Z Reads: 118

```
Are you sure, that VESC amp ratings are battery Amps ? Because it's the fets. that the amps is going through. And that is the motor amps.
```

---
## \#4 Posted by: professor_shartsis Posted at: 2018-10-19T19:45:03.266Z Reads: 118

```
[quote="Savace, post:1, topic:71745"]
Quick question, I have an Trampa Eboard, just seen that the ESC are rated at 50AMP they are vesc v4.12 50a however each motor is a MTO6374 170KV Max. Current: 65A.

Should the ESC’s not have a higher AMP rating than the motors? if so **what is the danger of having a lower rated ESC than the motor can pull.**
[/quote]

The 50a ESC rating means the esc can continuously cool 50a **motor current**. Sustaining 50a of motor current will require different amounts of battery current depending on the rpm, and the battery current is always lower than the motor current (higher battery current at higher rpms for the same quantity of motor current -- a result of higher back emf voltage at higher speeds which is produced in the motor windings by the spinning magnets). The ESC can also handle higher than 50a motor current (for a short time) according to your chosen motor current limit setting (some have gone as high as 100a+ motor current limit), but the ESC will get too hot after a while if you sustain more than 50a motor current continuously, for example on a long climb where you continuously need lots of torque.

to answer your question: the "danger" of having the lower current rated esc than the motor is the esc will overheat sooner than the motor during situations of sustained high torque demand.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-10-19T19:48:39.834Z Reads: 108

```
I read somewhere the explanation for it but I don’t remember so I don’t want to tell something wrong 😅 
But as other argument, the most people here have motors rated to 70-80a and run there vescs with min 60a Motor max without issues. That wouldn’t be the case if the rating would be related to the motor amps.
Which motor max you run with your escapes?
They rated for 60a constant. You run them not higher on the motor side?
```

---
## \#6 Posted by: Silverline Posted at: 2018-10-19T19:51:53.971Z Reads: 106

```
If they are like the original vesc6, they are rated 80a. At the moment i run motor max at 70a and battery max 60a. And with the dual heatsink 😀
```

---
## \#7 Posted by: Hummie Posted at: 2018-10-19T19:57:09.645Z Reads: 102

```
From what I’ve heard from experience the 6 won’t do that continuously.  Everyone exaggerates everything.  U can run huge amps, up to the programmed limit, and if it gets too hot, depending on what temp u set the max to, it’ll shut down. Doesn’t seem worth giving stated amp limits more than a though.  And then u add a heatsink or change the max temp shut down temp and poof the limit will change

On the 4.12 I set to 100 motor amps n never had a shutdown
```

---
