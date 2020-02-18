# Flipsky dual vesc 4.20 dual motor connection problem

### Replies: 5 Views: 190

## \#1 Posted by: Jesse7 Posted at: 2019-04-14T09:57:41.454Z Reads: 63

```
Im Having trouble   with  vesc tool   and cant  get both  motors  to spin ,its eithet one or the other. is there  something im missing in wizard .

( sorry im sure this topic has come up before but i can't seem to find much info on it)
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-04-14T10:44:17.156Z Reads: 59

```
are you running split ppm or CAN?

if CAN , have you got each vesc set as controller id 0 and 1? Have you also got the can bus cables right? 

If split ppm, have you removed a 5v rail from one side of the esc?

if you search for these things you'll find them.
```

---
## \#3 Posted by: Jesse7 Posted at: 2019-04-14T11:06:21.172Z Reads: 56

```
Running can i think . I didn't  think i would need a cable to link both vesc together as it s all on the  same pcb ?
```

---
## \#4 Posted by: mynamesmatt Posted at: 2019-04-15T00:33:48.070Z Reads: 39

```
i believe you still need to set master and slave on the vesc tool
```

---
## \#5 Posted by: Jesse7 Posted at: 2019-04-15T02:34:18.396Z Reads: 31

```
Ok i will give that a go  thanks
```

---
