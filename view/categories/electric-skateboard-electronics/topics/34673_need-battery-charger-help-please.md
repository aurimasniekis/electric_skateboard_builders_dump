# Need battery charger help please

### Replies: 12 Views: 564

## \#1 Posted by: Weirdboards Posted at: 2017-10-03T13:23:25.336Z Reads: 120

```
Trying to decide between two configurations for batteries and charging in my first board build. But I have read so much on amps watts votes and others I just need some simple guidance. I’m sure I’m making it more difficult in my head, but I need help. 

Here are the two configurations I am looking at:
- the 8s 15c config using two 4s 15c 10000mah turnigy graphene batteries, 14.4v each. 
at:
- the 10s 15c config using one 4s 15c 10000mah turnigy graphene batteries, 14.4v, and one 6s 15c 10000mah 22.2v turnigy graphene battery. 

Which bms and charger setup should I use for each? I would like to avoid removing the batteries to charge.
```

---
## \#2 Posted by: krloz Posted at: 2017-10-03T14:11:53.150Z Reads: 117

```
Firstly. What is your motor kv and are you using vesc?
```

---
## \#3 Posted by: Weirdboards Posted at: 2017-10-03T14:45:37.762Z Reads: 110

```
Dual sk3 168kv 6374s, dual VESC.
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-10-03T16:17:00.622Z Reads: 96

```
I'd go with 10s because it's a better fit with a 168kv motor, but I'd go with two 5s batteries instead of one 4s and one 6s. Less chance of getting mismatched cells that way. Either way, I'd recommend going with higher than 15c batteries just to improve the voltage sag under load.

As for BMS and charging, you need a BMS with the same cell count as the battery it's managing. Ditto for the charger, so for a 10s battery you need a 10s BMS and a 10s charger.

You don't need a balance charger, just a two-wire power supply that gives the right maximum voltage (42 volts for 10s).
```

---
## \#5 Posted by: krloz Posted at: 2017-10-03T22:34:34.118Z Reads: 83

```
+1 in the 10s and the higher than 15c discharge.  I don't quite agree that 5+5 will mismatch less than 4+6 @MysticalDork what do you mean with that.  The packs are made of the same cells and it will total to an array of 10 anyway.   
Apart from all that was said about the bms.. you will need one that can output more than your max amps. This depends on what you want to set on your vesc. but your motor maximum amps x2(motors) should be a good estimate.  And your charger shouldn't go higher than 1c Which in your case is 10A. Most simply give 2A
```

---
## \#6 Posted by: JdogAwesome Posted at: 2017-10-04T04:55:13.702Z Reads: 67

```
While using a 6S and a 4S battery and putting them in series would work I don't really recommend it even though the capacity and cells are most likely the same, there's really no way to know for sure. You could end up having some balancing problems when riding your board and it could end up either over discharging or over charging a particular cell because of the mismatched battery cells. What I would recommend however is using two of the exact same 5S battery's, preferably even bought together, and putting those in series for a 10S pack. Anyways BMS and Charger wise you just need either a 8S or 10S BMS and if you want to go the simple route just get a charger for that specific voltage or cell count.
```

---
## \#7 Posted by: krloz Posted at: 2017-10-05T22:37:51.287Z Reads: 50

```
I still don't get why you think 5+5 is better than 6+4. If at all you will be getting a mismatch of 5 equal against 5 equal instead of 6 equals against 4 equals. 
The only alternative is if you could get a single peek of 10 matches cells.
```

---
## \#8 Posted by: jmasta Posted at: 2017-10-05T22:42:15.221Z Reads: 48

```
4x3 > 6+4

12char
```

---
## \#9 Posted by: krloz Posted at: 2017-10-05T22:53:40.914Z Reads: 47

```
Wut?
We are comparing 6+4 against 5+5 .
Where did you get the 4x3?
```

---
## \#10 Posted by: jmasta Posted at: 2017-10-05T23:16:37.271Z Reads: 44

```
That's my opinion and what I use personally..  Using 4x 3S is better for several reasons.  First of all, the 3S batteries are thinner. 12S requires less current for the same power output as 10S or 8S, resulting in less voltage sag.  And 168kv is perfect for 12S.  They can be easily charged with a 6S balancer as 2x3S if needed.  Easy to fit in your enclosure in a 2x2 configuration.  And it's less batteries than 5x2S

But if you are stuck on 10S with only 2 batteries,  2x5S is a better combo
```

---
## \#11 Posted by: krloz Posted at: 2017-10-06T07:51:18.148Z Reads: 39

```
Ok. I understood wrong.  Yeah 12s is better if your vesc can handle it and the erpm. In my case I'm mounting 5x 2s under the board because of clearence and 2x 5S on top for extra.
But previously I was using a setup ood 2x (6s+2s+2s) and worked and balanced just as well. 
Note I can't go higher than 10s.
```

---
## \#12 Posted by: Weirdboards Posted at: 2017-10-07T12:07:44.779Z Reads: 35

```
Thanks everyone for the feedback. Decided to go with a balanced 5sx2 set up, but I went with 30c batteries instead of the 15c batteries. Sounds like it is better for my set up and best cost option based on what I priced out.
```

---
