# VESC with wired Hall effect throttle with reverse

### Replies: 2 Views: 414

## \#1 Posted by: Rednx Posted at: 2018-03-30T14:57:56.287Z Reads: 59

```
First build newbie here. I'm in the designing phase of a build. My build needs to have a wired Hall effect throttle control. I understand using a servo tester for the conversion. What I have not been able to figure out is how to program/ switch for reverse/ braking. I have done a vast amount of research and have been unable to find anything that covers this. Any thoughts or input would be greatly appreciated.
```

---
## \#2 Posted by: Martinsp Posted at: 2018-03-30T15:19:38.046Z Reads: 53

```
I looked into this once but abandoned the idea. What you would need is something (arduino for example) to transform the information about the distance of the magnet from the hall sensor (both hall sensor and magnet are inside the throttle of ebikes/emotos usually) which would be transformed to PPM signal for the VESC to read. Or maybe you could utilize uart but I am not familiar with that enough to give any guidance, maybe someone else with more experience can elaborate on this option.
```

---
