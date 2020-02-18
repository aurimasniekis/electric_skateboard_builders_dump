# FOCBOX Revision Question

### Replies: 4 Views: 184

## \#1 Posted by: MatrixWriter Posted at: 2019-01-16T19:28:24.564Z Reads: 82

```
This question is geared towards the regular Focbox and not the Unity.

I was wondering what is the difference between the revision numbers, ie v1.6 and v1.7?
The design files that used to be released are for v1.3. So wondering what exactly has changed?

It was mentioned somewhere, on a side note that do not disconnect CAN Bus if both ESCs are powered on? I use CANH and CANL connections by the way.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-16T19:44:56.907Z Reads: 79

```
That issue is fixed with 1.7.
Don’t ask me how exactly but that’s what @onloop told us.
```

---
## \#3 Posted by: Deodand Posted at: 2019-01-16T19:57:24.037Z Reads: 75

```

we switched the CAN bus transceiver IC to an isolated one. Basically prevents the CAN transceiver from blowing things up unintentionally.
```

---
## \#4 Posted by: MatrixWriter Posted at: 2019-01-16T22:16:38.023Z Reads: 51

```
Ah very good to know, thanks! Unfortunately I have v1.6 revision.

I don't get how CAN Bus breaks things on the ESC from a simple disconnect? Wondering if other VESC brands have this issue as I didn't know about this.

To bad Enertion and others do not provide a detailed changelog and such with new revisions...isn't that required for open source projects?
```

---
