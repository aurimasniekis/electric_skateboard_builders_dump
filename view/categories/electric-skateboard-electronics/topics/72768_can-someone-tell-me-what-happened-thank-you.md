# Can someone tell me what happened, thank you

### Replies: 12 Views: 397

## \#1 Posted by: Devilmycry Posted at: 2018-10-30T02:50:25.649Z Reads: 188

```
Hi 
I’m starting testing different motor 
And my last test for some motor .
I have some difficulty to do motor detection like the vesc tool told my : we can’t detect motor flux linkage 
And tried 2 or 3 time for each motor for make it work 
Any idea what happened ?
Thank you
```

---
## \#2 Posted by: yelnats8j Posted at: 2018-10-30T02:58:15.848Z Reads: 176

```
send pictures of the settings and motor?
```

---
## \#3 Posted by: Eboosted Posted at: 2018-10-30T03:57:27.341Z Reads: 145

```
Your sensor wires might be wired incorrectly
```

---
## \#4 Posted by: linsus Posted at: 2018-10-30T09:59:44.978Z Reads: 97

```
Please provide more information. To me it sounds like you have a bad motor or a bad vesc. 
What faults do you get?
```

---
## \#5 Posted by: Devilmycry Posted at: 2018-10-30T12:21:44.456Z Reads: 71

```
Hi know I check them and is good
```

---
## \#6 Posted by: Devilmycry Posted at: 2018-10-30T12:25:59.423Z Reads: 69

```
When I do motor detection the 1 step work but when I do the 2 set when the wheel turne
I have to do it 2 or 3 time for the tool detect the motor flux linkage 
Same for the second motor 
I did it and know everything work but I don’t know why I have to do 2 to 3 time for make it work is bizarre for me
```

---
## \#7 Posted by: Devilmycry Posted at: 2018-10-30T12:26:50.489Z Reads: 62

```
No I check and is going
```

---
## \#8 Posted by: Devilmycry Posted at: 2018-10-30T12:27:20.811Z Reads: 56

```
Do the same with the sensor or not
```

---
## \#9 Posted by: linsus Posted at: 2018-10-30T13:07:35.697Z Reads: 49

```
try both bldc motor detection and FOC motor detection. 
What are your resistances in the motor? WHat does the vesctool say?
When you do motor detection, set the current abit higher then default, sometimes its too weak. What power source are you using when setting up?
```

---
## \#10 Posted by: r3vilo Posted at: 2018-11-03T11:13:27.750Z Reads: 35

```
I have the same issues <a href=https://www.electric-skateboard.builders/t/unable-to-accelerate-get-power-into-motors-via-remote-control/72786>here</a> PLUS that after motor and input setup my motors almost doing nothing when pushing the throttle on remote.

My solution for now - just a couple of minutes ago - was using BLDC mode without sensors. Because that worked. I never had this behaviour before. And in my case also trying 2-3 times detection fails. It fails everytime.

I was able to get flux linkage detection working by setting the D value from 0,5 to 0,3 but that didn't help with my problem.
```

---
## \#11 Posted by: Devilmycry Posted at: 2018-11-03T15:20:10.462Z Reads: 23

```
For me I do it 2 to 3 time and it work after 
I run 13 miles and everything work ok
```

---
## \#12 Posted by: Devilmycry Posted at: 2018-11-03T15:21:28.501Z Reads: 23

```
I use the battery 12s7p 
But after doing 2 or 3 time it detect the motor flux 
And know I run 13 miles everything look good
```

---
