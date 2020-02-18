# VESC not working after changing to FOC - Please help!

### Replies: 6 Views: 336

## \#1 Posted by: maki Posted at: 2017-09-17T10:20:58.976Z Reads: 71

```
I have a VESC 4.12 with V 2.18 and I just tried  changing to FOC following Vedder's you tube video.
Did all the motor detection steps, tested it on the bench for 10 seconds then the motor stopped spinning.

So the ESC comes on with normal flashing lights but no response, motor still works as I tried it with another ESC.  When I accelerate or brake, the ESC red lights flashes, but nothing happens.

I tried reverting back to BLDC with the same settings as before, but not luck.

Can someone please help?
```

---
## \#2 Posted by: pat.speed Posted at: 2017-09-17T11:49:15.801Z Reads: 65

```
Sounds like drv error? Maybe someone can confirm this? try checking error codes in the Vesc tool
```

---
## \#3 Posted by: Tomer Posted at: 2017-09-17T12:22:52.024Z Reads: 59

```
Does your VESC is Maytech branded?

If so, well... I better stop here.
```

---
## \#4 Posted by: maki Posted at: 2017-09-17T12:40:45.781Z Reads: 51

```
I believe so, it says MT VESC on it.
Excuse my ignorance, why stop here?
```

---
## \#5 Posted by: scepterr Posted at: 2017-09-17T12:51:51.624Z Reads: 45

```
Just search maytech
```

---
## \#6 Posted by: darkkevind Posted at: 2017-09-17T13:16:08.271Z Reads: 43

```
Maytech VESCs don't support FOC.

You've blown the DRV I'd imagine. You'll need to get it repaired.

@JohnnyMeduse
```

---
