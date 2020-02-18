# Dual Motor Reciever

### Replies: 11 Views: 785

## \#1 Posted by: Andy12 Posted at: 2017-03-25T20:25:14.983Z Reads: 89

```
When doing a Dual Motor setup with two VESC would I have to plug in the ports to CH1 and CH2 or what would it be. BTW using HK- GT2B
```

---
## \#2 Posted by: barajabali Posted at: 2017-03-25T20:31:06.496Z Reads: 87

```
You need a Y splitter for servo leads. You can make it or buy it

Both motors come off one channel which would be channel 2
```

---
## \#3 Posted by: Andy12 Posted at: 2017-03-25T20:34:33.060Z Reads: 83

```
like this for example
 https://hobbyking.com/en_us/servo-splitter-lead-1-female-to-5-male.html
```

---
## \#4 Posted by: rpn314 Posted at: 2017-03-25T20:36:44.975Z Reads: 80

```
You can control 2 VESCs in 2 ways. You can either split the connections so the one trigger signal goes to both VESCs (just a splitter wire) or you can just connect to one VESC and then connect the two VESCs via the can-bus
```

---
## \#5 Posted by: Andy12 Posted at: 2017-03-25T20:38:15.250Z Reads: 77

```
so you're saying that with the can-bus I will only have to put it in CH2 and then the other VESC will be blank
```

---
## \#6 Posted by: mmaner Posted at: 2017-03-25T20:40:21.039Z Reads: 74

```
That is correct, plus with can bus you can use traction control.
```

---
## \#7 Posted by: Andy12 Posted at: 2017-03-25T20:40:55.074Z Reads: 73

```
Sweet so whats more efficient, Y Spliiter or Can-Bus
```

---
## \#8 Posted by: rpn314 Posted at: 2017-03-25T20:42:23.888Z Reads: 72

```
Not sure either is more efficient for ppm. Personal preference and if you want any bonus that can-bus can give (traction control, adding a Bluetooth module to the slave VESC and programming them both through that, and a few other things like that)
```

---
## \#9 Posted by: Andy12 Posted at: 2017-03-25T20:43:44.566Z Reads: 67

```
Thanks guys Now I know
```

---
## \#10 Posted by: rpn314 Posted at: 2017-03-25T20:45:50.602Z Reads: 62

```
You have to configure the can bus on the VESC a little to get it to work, and if it dies (cable breaks or something) while traction control is on, the master VESC will only go as fast as the traction control difference (which is supposed to be quite small). So the extra features add a little more work and a slight more possibility for issues, but I thought it worth it :slight_smile:
```

---
## \#11 Posted by: Andy12 Posted at: 2017-03-26T16:59:18.262Z Reads: 35

```
what would your configurations be on the dual motor
```

---
