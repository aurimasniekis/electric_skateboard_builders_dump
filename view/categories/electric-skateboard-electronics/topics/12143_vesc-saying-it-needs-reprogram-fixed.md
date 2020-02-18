# Vesc saying it needs reprogram - (fixed)

### Replies: 5 Views: 660

## \#1 Posted by: maxz Posted at: 2016-10-30T07:59:45.301Z Reads: 65

```
i have a dual drive set up, two diy 6355, 10s3p and dual diy vescs, main one works great and set up right secound says need reprogramming, cannot connect to the vesc. Its connected via canbus to the other. Any help would be great. Thanks.
<img src="/uploads/db1493/original/3X/4/4/445b3b60260094f8b826db08e9c34f7b9c3af129.PNG" width="690" height="334">
```

---
## \#2 Posted by: maxz Posted at: 2016-10-30T08:03:15.800Z Reads: 61

```
secondary vesc works with normal settings
```

---
## \#3 Posted by: Luke Posted at: 2016-10-30T08:08:51.724Z Reads: 57

```
https://youtu.be/eXQdMIlKb-o
Also worth mentioning that both vescs work, it's just that the slave vesc doesn't connect to bldc tool, so it's settings are in default and will be drawing more current than it should if left like this
```

---
## \#4 Posted by: Skitzor Posted at: 2016-10-30T08:57:42.381Z Reads: 52

```
Yo man, either update the firmware on the same level as your first vesc or download an earlier version of the BLDC tool for your second
```

---
## \#5 Posted by: Luke Posted at: 2016-10-30T09:27:35.574Z Reads: 46

```
Fixed by reconnecting the vesc a load of times and re-downloading bldc tool and restarting computer till the vesc finally connected
```

---
