# Can power switch functionality be achieved using the VESC&rsquo;s hardware or software?

### Replies: 4 Views: 886

## \#1 Posted by: Hillso Posted at: 2016-12-05T02:33:31.408Z Reads: 113

```
Theoretically, it seems to me redundant to use an external switch. I mean, the external switch only turns on the VESCs processor and not the power to the motor (the VESC already have it's own mosfets switches), and still, the switch has to have the mosfets.

http://www.st.com/content/ccc/resource/technical/document/application_note/ff/0a/dc/d2/5e/f5/4b/5a/CD00171691.pdf/files/CD00171691.pdf/jcr:content/translations/en.CD00171691.pdf
<img src="/uploads/db1493/original/3X/7/2/72e0c07f7b2d0189d270b5a08c302f31c298a7b0.PNG" width="420" height="500"><img src="/uploads/db1493/original/3X/6/9/691475ad1466b8ffda0fdf6f0b1b87f11a1c766d.PNG" width="549" height="340">
```

---
## \#2 Posted by: saul Posted at: 2016-12-05T02:59:37.654Z Reads: 100

```
well 6.0 includes hardware for a soft switch. but I suppose vesc4 could do some kind of firmware mod to put the processor in sleep mode.

**But I'd imagine there is some reason not to do this** or else vedder would have just included it in 4.12. 
Maybe post on his forum and see what he was to say..
http://vedder.se/forums/
```

---
## \#3 Posted by: Hillso Posted at: 2017-02-22T17:03:04.529Z Reads: 49

```
http://www.st.com/content/ccc/resource/technical/document/application_note/13/0a/06/b9/1e/2f/4d/9d/DM00096220.pdf/files/DM00096220.pdf/jcr:content/translations/en.DM00096220.pdf
```

---
## \#4 Posted by: Maxid Posted at: 2018-05-19T08:33:07.819Z Reads: 26

```
Have you ever achieved something in this regard? I'd like to implement a sleep mode too
```

---
