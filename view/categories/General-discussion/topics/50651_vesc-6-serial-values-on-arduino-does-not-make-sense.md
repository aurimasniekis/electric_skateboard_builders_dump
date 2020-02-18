# VESC 6 serial values on Arduino does not make sense

### Replies: 1 Views: 324

## \#1 Posted by: arsh Posted at: 2018-03-30T14:24:53.098Z Reads: 40

```
Hello, 

I received my VESC 6.0 today. I totally love it. It detect the motor instantly and I am running it on FOC (without sensor). However I need to control and monitor the parameters and I tried the serial communication like this 

VESC 6.0 --> Arduino Hardware Serial --> LabVIEW (through software serial). 

However the values I am receiving on LabVIEW does not match the Real-time values on VESC-tools which by the way looks more reasonable. 

I do not have a bluetooth module or a TTL-USB connector otherwise my setup would have been less complicated. 

I used RollingGecko implementation for communicating VESC and Arduino over serial. I am sure I am getting the data from VESC (I used LED to check if the data was receiving and then I used myRio , labview hardware, and I am getting the values) 

Please see attach images. 
![Untitled|690x194](upload://lHQbs4ptXlSxWq6Jj9Vp6xniqvR.png)
```

---
