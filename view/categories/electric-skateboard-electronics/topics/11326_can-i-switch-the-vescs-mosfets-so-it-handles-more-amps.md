# Can I switch the VESCs mosfets so it handles more amps?

### Replies: 9 Views: 1145

## \#1 Posted by: Hillso Posted at: 2016-10-18T03:04:29.219Z Reads: 121

```
or there are other limits?
I guess it needs to be in the same form factor, so heat dissipation will be the same.
or, can I connect the VESC to an external board with fets?
Thanks.
```

---
## \#2 Posted by: Blasto Posted at: 2016-10-18T03:12:01.619Z Reads: 119

```
What is the application?
```

---
## \#3 Posted by: saul Posted at: 2016-10-18T03:13:21.955Z Reads: 119

```
this would be more work than its worth...
i think you can connect 2 vesc in parallel and get double current. still probably not worth the trouble...
```

---
## \#4 Posted by: Hillso Posted at: 2016-10-18T03:13:42.933Z Reads: 117

```
electric skateboards :smile:
```

---
## \#5 Posted by: Hillso Posted at: 2016-10-18T03:17:04.366Z Reads: 116

```
I don't think its possible, phase cycle need to be timed unless I modify the motor so it has 6 phase like this:
https://www.youtube.com/watch?v=LgRK4_4ElhU
```

---
## \#6 Posted by: saul Posted at: 2016-10-18T03:20:46.766Z Reads: 110

```
pretty sure someone was doing it on es for an ebike. :sunglasses:

same signal in, same resistance out..w.hat would shift it out of phase?
```

---
## \#7 Posted by: saul Posted at: 2016-10-18T03:22:29.248Z Reads: 108

```
50A already flings me up hills at 20mph...how much more current do you need? 
planning a trip to the moon?
```

---
## \#8 Posted by: Blasto Posted at: 2016-10-18T03:23:31.978Z Reads: 106

```
Would the vesc-x suit your needs?

http://www.enertionboards.com/?afmc=1o

It's sporting these fets

http://www.infineon.com/dgdl/irf7749l1pbf.pdf?fileId=5546d462533600a4015356043d6b1ca0
```

---
## \#9 Posted by: Hillso Posted at: 2016-10-18T04:25:35.933Z Reads: 92

```
Need more amps with low voltage battery
```

---
