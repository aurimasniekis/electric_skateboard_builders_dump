# Dual vesc sharing same ID

### Replies: 3 Views: 88

## \#1 Posted by: Songsta Posted at: 2019-09-18T07:25:25.876Z Reads: 32

```
I'm having a strange problem. My 2 vescs are sharing the same ID for some reason. Previously when I scanned the CAN bus I would get 32 and 81 as the 2 IDs, but now they're both showing up as 81.

![Screenshot_20190918-091249|243x500](upload://72s7790prkSI5Qtih40aY9dVhbs.jpeg) 

I probably wouldn't mind this, but what's happening is that this morning the one motor wasn't working, even though it worked perfectly last night without any changes being done. I scanned for devices on the can bus but couldn't find any. Then I opened up the enclosure and moved the Bluetooth module from one vesc to the other, suddenly both vescs are there after a scan, but now with the same ID.

How can I set then up to be different IDs?
```

---
## \#2 Posted by: olestra Posted at: 2019-09-18T15:04:15.261Z Reads: 19

```
connect to only one of them and change it. easily done with vesc tool, no idea with the mobile app
```

---
## \#3 Posted by: Songsta Posted at: 2019-09-18T15:44:47.353Z Reads: 17

```
Thanks. tried that and it didn't work, so I reflashed them both. They're working now. 

Weird.
```

---
