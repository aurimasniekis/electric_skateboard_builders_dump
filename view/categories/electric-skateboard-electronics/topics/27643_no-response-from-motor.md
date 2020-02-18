# No response from motor

### Replies: 13 Views: 695

## \#1 Posted by: tomerwei Posted at: 2017-07-14T19:31:43.789Z Reads: 76

```
Hi guys!
I build my first eSkate using Enertion's VescX, 2 5000mah turnigy 5c lipo connected in series and a turnigy sk3 6374 192kv motor.
I used it for about two weeks and now it suddenly stoped working. 
I connected the vesc to the bloc tool but it responds normally. no faults but the motor is still not responding. 
Checked all the motor wires for shorts but found nothing

Do you have any ideas?
Thanks!
```

---
## \#2 Posted by: Martinsp Posted at: 2017-07-14T19:34:58.739Z Reads: 74

```
Have you done the motor detection successfully?
Also try spinning the motor using the arrow keys if you have been trying remote you have to configure it first in the app config tab.
```

---
## \#3 Posted by: tomerwei Posted at: 2017-07-14T19:35:58.335Z Reads: 66

```
Tried motor detection and it failed.
Also tried the arrow keys and that didn't work also
```

---
## \#4 Posted by: Martinsp Posted at: 2017-07-14T19:38:19.235Z Reads: 62

```
Do you have any other  motor to test it with? 
Because it seems that either that is faulty or mosfets, if there is no fault in bloc tool.
```

---
## \#5 Posted by: tomerwei Posted at: 2017-07-14T19:40:43.211Z Reads: 59

```
sadly I don't have any other motor... do you have any ideas?
```

---
## \#6 Posted by: Martinsp Posted at: 2017-07-14T19:44:14.547Z Reads: 62

```
Well if the motor was faulty it would take the mosfets too. You can test them easily. Measure the resistance between positive and the three phase vires and the same with negative battery wire. Of course nothing can be plugged in during this.
```

---
## \#7 Posted by: Martinsp Posted at: 2017-07-14T20:14:45.875Z Reads: 53

```
Oh. forgot to add.. it should not be shorted if it is then you have a blown FET.
```

---
## \#8 Posted by: tomerwei Posted at: 2017-07-15T18:42:25.688Z Reads: 42

```
didn't checked the mosfets yet but can you see anything wrong?
<img src="/uploads/db1493/original/3X/3/3/33414f55add3fd941fe786ce497ce3b3ddee327f.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/d/7/d708ac3c574be9a6d49a9532efc03ec2b2edbcb9.JPG" width="375" height="500">
```

---
## \#9 Posted by: tomerwei Posted at: 2017-07-15T18:52:22.066Z Reads: 41

```
and can someone tell me why its happened? even if its only an assumption...
```

---
## \#10 Posted by: Martinsp Posted at: 2017-07-15T23:43:09.158Z Reads: 35

```
I dont know if it is just the picture, maybe some reflection or something but there seems to be exposed copper on the PCB next to the capacitor to the left of the DRV chip... That might be just a manufacturing fault but I think that that would not get through visual quality inspection. Usually what this is a sign of is short that caused a lot of heat and this defect in PCB. 
I am not sure if this is your problem or cause of another problem like destroyed component or something.
Definitely do the measurements and send the results, we will see from there.
```

---
## \#11 Posted by: Martinsp Posted at: 2017-07-15T23:55:08.454Z Reads: 34

```
Well now that I look at it closely with a schematic, It looks like something went wrong (cant really tell what, not enough info) and the VESC/FOCBOX shorted your battery due to faulty component or possibly something else like loose piece of metal/conductive material that shorted pins of DRV and that resulted in a direct short of your battery  (on that capacitor c44 and c43) and that is why that trace has exposed copper. 

You might have fried DRV or it is not working because it is missing the input from the battery because that trace is missing that is coming from your battery on pin 54 and 53.
```

---
## \#12 Posted by: tomerwei Posted at: 2017-07-16T12:24:08.460Z Reads: 29

```
Can you mark where i should touch the mosfets in order to check them... I tried to learn from this youtube video:
https://www.youtube.com/watch?v=RkWy1EirEu8
but its different components from what I have...

Thanks!
```

---
## \#13 Posted by: Martinsp Posted at: 2017-07-16T22:59:56.261Z Reads: 24

```
Your mosfets are the direct fets and you dont really have any way of testing the mosfets directly with a multimeter without desoldering them because the pads that connect to the PCB are underneath the metal shiny case you see...

What you can do is test if there is continuity between phase wires and input/battery wires. They should not be shorted. Also test if there is continuity between the phase wires. Again, they should not be shorted.
```

---
