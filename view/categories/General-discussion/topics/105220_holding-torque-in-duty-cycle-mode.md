# Holding torque in &ldquo;Duty Cycle&rdquo; mode

### Replies: 2 Views: 72

## \#1 Posted by: Petja Posted at: 2020-01-13T00:37:39.460Z Reads: 29

```
Hello everybody!  I faced a problem: when I use control type "Duty Cycle" in FOC mode and throttle (control type ADC) has full stop position, driver draw current nearly 0.1A (sometimes generate 0.1A). This current creates holding torque.
![Holding-torque|690x370](upload://d4PutJV7wTR6sli4IGZxLJJpqMs.jpeg) 
But I want to ride free-wheel on my bike.
Is it really impossible to fix this in "Duty Cycle" mode?
The same problem is about remote, which I want to use in "Duty Cycle" mode like on this picture:
![PPM%20control%20through%20remote|211x500](upload://9alVPpRMasoj18Kxw3ZQfXhCFlT.jpeg) 
I have holding torque in middle position of throttle now.
```

---
## \#2 Posted by: professor_shartsis Posted at: 2020-01-13T01:23:27.597Z Reads: 22

```
I think since in duty cycle mode, very small changes in duty cycle result in very large changes in motor current, and the max motor current is regulated by the motor current limit setting, your throttle will effectively become an on-off switch between 0 current or max current according to the current limit setting. just a guess.
```

---
