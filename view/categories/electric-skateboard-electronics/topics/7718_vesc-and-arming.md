# VESC and arming?

### Replies: 2 Views: 545

## \#1 Posted by: Workaround Posted at: 2016-08-16T01:22:25.784Z Reads: 61

```
I can't find any information on if I need to arm a VESC.

I'm making arduino PPM connection for a build. I would like to know if the VESC needs arming like a regular ESC.

If the VESC need to be armed then how do you do it?
```

---
## \#2 Posted by: Blasto Posted at: 2016-08-16T01:26:42.549Z Reads: 60

```
Yes you will need to calibrate the vesc to your ppm settings, all done in the bldc tool. There's a safe start feature you can disable.

Put the vesc in the ppm disabled mode when checking the swing of your ppm (you will see the ppm in the display but the motors won't run), don't want to go full throttle in case you need to do some changes to your code.
```

---
