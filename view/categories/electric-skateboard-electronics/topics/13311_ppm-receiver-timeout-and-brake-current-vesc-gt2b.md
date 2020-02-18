# PPM Receiver Timeout and Brake Current (VESC - GT2B)

### Replies: 2 Views: 717

## \#1 Posted by: Gmcfarla Posted at: 2016-11-19T04:27:06.956Z Reads: 90

```
Hello all,

Having trouble finding an answer and hoping someone can chime in here. I have a VESC and GT2B receiver and prior to going out for a maiden voyage I wanted to test the fail safe functionality. I have the failsafe of the receiver set so that when I disconnect/turn off the remote the board will slow down. The issue i'm having is with the receiver timeout and associated brake current which from what I'm reading should allow me to either coast (set at 0.0) or reduce the current to the motor (any value greater than 0.0) if I were to pull the 3 pin cable out of the receiver (simulating a receiver becoming disconnected from the VESC.) unfortunately what I'm seeing is the motor spooling up with the only way to stop it by plugging the receiver back in or pulling power. Looking for any insight into what this could be...

Thanks in advance for any coments.
```

---
## \#2 Posted by: Gmcfarla Posted at: 2016-11-19T05:29:45.645Z Reads: 87

```
Looks like I found the issue. I was trying it with BLDC tool being connected which I guess sends keep alive packets which will cause it to not timeout... solved.
```

---
