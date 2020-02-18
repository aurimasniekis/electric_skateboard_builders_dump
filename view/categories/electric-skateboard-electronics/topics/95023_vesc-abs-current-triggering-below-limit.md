# VESC ABS Current triggering below limit?

### Replies: 6 Views: 129

## \#1 Posted by: skaterscooter Posted at: 2019-05-26T14:22:34.050Z Reads: 43

```
Today I decided to setup the hall sensors on my ebike motor which mostly went fine, needed a bit of tweaking, but as far as I'm aware the sensors are working as they should. When I went to test however, the VESC kept cutting out and throwing up ABS_Over_Current errors. When I looked at the terminal, the wierd part was that the detected current is lower than the filtered current! Correct me if I'm wrong but the Current Filtered is the limit set in the Current tab? (which in my case is 90A). Does anyone know where this is coming from, have I accidentally lowered a setting somewhere else? If not, I'll restore to defaults and build up from there
```

---
## \#2 Posted by: skaterscooter Posted at: 2019-05-26T14:23:07.224Z Reads: 41

```
Here is the error:![06|443x499](upload://8o8VFdNVZpxz9xE2eZfmxr5ZOyY.png)
```

---
## \#3 Posted by: skaterscooter Posted at: 2019-05-27T07:35:01.628Z Reads: 24

```
Solved it - I just restored the defaults and then changed the settings I needed. Still not sure what causes this though?
```

---
## \#4 Posted by: pjotr47 Posted at: 2019-05-27T07:41:07.713Z Reads: 22

```
You must set abs over current on 120-130A
```

---
## \#5 Posted by: skaterscooter Posted at: 2019-05-27T07:52:13.652Z Reads: 19

```
As high as that? My batteries can only handle 110A max.
```

---
## \#6 Posted by: pjotr47 Posted at: 2019-05-27T07:55:13.952Z Reads: 18

```
I think it is that by default. Due that I can take some amps spikes. No worry’s about your battery.
```

---
