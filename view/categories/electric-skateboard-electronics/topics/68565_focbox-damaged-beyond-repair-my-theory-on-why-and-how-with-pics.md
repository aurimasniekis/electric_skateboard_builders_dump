# Focbox Damaged Beyond Repair; My Theory on Why and How (With Pics)

### Replies: 6 Views: 333

## \#1 Posted by: pennyboard Posted at: 2018-09-19T21:25:07.349Z Reads: 131

```
I recently upgraded one of the VESCs on my board to a Focbox, and ran one FOCBox and one Ollin VESC without problem for a few months. Then this happened (See Pictures Below).

![32%20PM|445x500](upload://1I2mjpuCB1eUfYwT12dokWtpDE6.jpeg)  ![IMG_1530|375x500](upload://zno469QHPnJvTnvN58hofKYqHD0.jpg) 

It occurred when I ran over a thick crushed metal soup can in the road. The motor connected to this vesc locked up and threw me off. I tried turning the board off and just pushing it, but the motor was still locked up, making think the phase wires must have shorted. When I got home, I took apart the FocBox and saw this.

After disconnecting the motor from the focbox it spins fine, so I assume the phase wire was on the damaged focbox. Clearly, one of the fets is completely burned up, the PCB is damaged, and the DRV also looks very damaged.

Now I am trying to piece together what happened.

My theory is:
The metal can hit the motor, and cause one of the magnets to break off, and short two of the copper windings in the motor, causing a large amount of current to continuously flow through the fet till it burned it, and the heat generated from that is what damaged the PCB and DRV chip. 

Does that sound reasonable?
Any other theories as to what may have happened?
```

---
## \#2 Posted by: pat.speed Posted at: 2018-09-19T22:08:07.946Z Reads: 111

```
Is there any damage to phase leads?
```

---
## \#3 Posted by: electric Posted at: 2018-09-19T22:36:00.041Z Reads: 99

```
Do you have a picture of the motors insides as of now?
Maybe someone here who is experienced with electric motors could take a look and tell us  
What could have happened.


I would ask if the motor works but that would require testing it and if your theory was right well......
```

---
## \#4 Posted by: pennyboard Posted at: 2018-09-19T22:39:03.284Z Reads: 97

```
Not that I can see. Although I now noticed what appears to be debris from the broken fet collected on the focbox, and possibly another broken fet on a different phase wire. 
![image|375x500](upload://3QI8uDh7ujdnlHQbQO0JSZ6VTpr.jpeg)
```

---
## \#5 Posted by: pennyboard Posted at: 2018-09-19T22:41:20.745Z Reads: 90

```
Yeah I’m not too keen on plugging another focbox into it. It does spin freely and breaks when I touch the phase wire connectors, so it appears to be no longer shorted. One thing I should mention is that this motor had a magnet shatter before, I took it apart and removed the broken magnet and it seemed to work fine with 13 magnets. I wonder if that would have caused problems? 


I can try to get the motor apart and pictures ASAP, but I need to borrow the tools to do it again so can’t do it right away.

Edit: The more I think about it, the more I wonder if removing the magnet is what blew my VESC and it just happened to conincide with me running over the metal can.
```

---
## \#6 Posted by: AlexBE Posted at: 2018-09-20T01:55:10.832Z Reads: 66

```
You can always test by putting a ~10A fuse in series with each motor wire for the first spin up. That will help prevent a complete short from killing a second/repaired vesc.
```

---
