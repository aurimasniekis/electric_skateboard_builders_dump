# Cutting out under load - Fault finding

### Replies: 1 Views: 287

## \#1 Posted by: bloke900 Posted at: 2018-05-21T06:31:03.593Z Reads: 60

```
TL;DR   
Check to make sure you don't have any high current wires anywhere near your receiver. I have an enertion nano-x and was having problems until this was resolved. Problems included rough throttle and power to motor cutting out entirely. 

I had a 125kv 2000w motor that I had been running on my board with a max speed of 25kph. I felt the need to upgrade, and rather than change gearing I bought one of the new Hobbyking SK8 6374 192kv motors. It arrived, I swapped the motors over, updated settings in the VESC and headed out to try it. 

New motor felt like a suitable upgrade until I gave it more than a 1/4 throttle, and then the board would die. I ended up going through a tonne of different threads on here to look for a solution:
Adjusted motor amp and battery amp settings - no change.
Made sure my receiver was nowhere near motor phase wires - no change. 
Changed my low voltage cutoffs and kept and eye on my voltage meter while riding - no change. 
Checked for fault codes - none. 
Swapped out for a friend's SK8 6374 - no change.
Swapped out a friends Focbox - very slight change...

After checking settings on both Focboxes, and confirming they were identical, I was starting to get disheartened when I noticed when I put my friends Focbox in, I had rerouted the power to sit neater and coincidentally further away from the receiver. After completely rerouting all power wires the maximum distance away from the receiver that I could - everything worked perfectly. I have since moved back to all my own equipment, even trying my old motor again. MUCH smoother over the entire throttle band.
```

---
