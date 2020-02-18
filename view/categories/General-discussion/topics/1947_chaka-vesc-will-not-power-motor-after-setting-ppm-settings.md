# Chaka VESC will not power motor after setting PPM settings

### Replies: 11 Views: 1703

## \#1 Posted by: gamma2 Posted at: 2016-03-24T04:10:09.396Z Reads: 91

```
I received my VESC and began to set it up. I powered it with a lab power supply that does a maximum of one amp. I got my receiver and transmitter set up and the VESC was driving my motor just fine, however it was not calibrated with the same 50% throttle as the center of the transmitters trigger. So, I adjusted the min/max PPM settings until I had 50% throttle displayed. I used slow acceleration to test the motor and it seemed to work. I let go and began to pull the trigger again and....nothing. The VESC now will not drive a motor. I still get a green light. I have no fault codes. For a while after that the lab supply would not give it more than 7 or 8 volts, so I let it sit for an  hour. Its now taking full voltage but still no response from the motor. I have tried resetting everything to default and that hasn't made a difference. I'm not sure what else I can do other than send it in for repairs/replacement. Thanks for the help guys.
```

---
## \#2 Posted by: trbt555 Posted at: 2016-03-24T06:11:04.405Z Reads: 88

```
Green light and no fault codes mean there probably isn't a problem with the vesc.
Your power supply sounds wonky, rule it out by using an alternate one.
Rule out the tx/rx by hooking up to BLDC tool and using the arrows keys to drive the motor.
```

---
## \#3 Posted by: gamma2 Posted at: 2016-03-24T07:27:44.913Z Reads: 85

```
Power supply works fine on other devices. Fluke meter confirms its fine. Also just tried driving the motor directly through BLDC with no response.
```

---
## \#4 Posted by: onloop Posted at: 2016-03-24T07:32:50.566Z Reads: 85

```
Power cycle vesc
Power cycle PC
Use another power source, maybe 1 AMP is not enough
Do another motor detection 
Check motor wire connections
```

---
## \#5 Posted by: gamma2 Posted at: 2016-03-24T07:34:05.328Z Reads: 83

```
Done, Done. I tried a 3s and a 6s with no different results. Motor detection does nothing. Wire connections look fine. At this point I'm thinking I popped an IC and can't see it.
```

---
## \#6 Posted by: onloop Posted at: 2016-03-24T07:35:03.383Z Reads: 84

```
Screen shots for all your common BLDC pages
```

---
## \#7 Posted by: gamma2 Posted at: 2016-03-24T08:14:10.204Z Reads: 81

```
I'm on my way to bed now but I'll send them when I get home from work tomorrow. Everything was default except enabling PPM and changing the min/max. I also changed the two numbers from motor detection. I believe they were 107 and 875 ish.
```

---
## \#8 Posted by: Tarzan Posted at: 2016-03-24T10:10:44.406Z Reads: 75

```
Did you read your config before you made the changes?
```

---
## \#9 Posted by: chaka Posted at: 2016-03-24T13:34:23.859Z Reads: 71

```
What version of the BLDC-tool are you using? What motor are you running? Have you re-soldered any connections?

Take some pictures of your connections and post them, maybe we can see something that might be causing issues.
```

---
## \#10 Posted by: gamma2 Posted at: 2016-03-24T18:26:46.936Z Reads: 67

```
Hey guys. I asked my roommate to take a look at it while I was out. It appears that I somehow popped my DRV8302. I figure I must have hit the 1 amp limit on the powersupply and it tried to reset and that resulted in a spike in voltage/amperage. This also occurred a couple times while trying to do motor detection. I have heard that you should not use a LiPo to do motor detection but I can't get the motor to spin with less than 5 amps or so. Should I use a higher amperage power supply next time? How can I avoid popping the DRV8302? Also does anyone know of the best source to purchase a new IC from and what exact model I need?
```

---
## \#11 Posted by: NIK Posted at: 2016-04-08T09:50:23.994Z Reads: 53

```
Texas Instrument DRV8302, [TI DRV8302][1] I purchased from this site when mine was broken


  [1]: http://www.ti.com/product/DRV8302
```

---
