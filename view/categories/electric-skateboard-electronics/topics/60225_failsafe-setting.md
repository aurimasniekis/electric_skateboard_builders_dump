# Failsafe setting

### Replies: 5 Views: 271

## \#1 Posted by: Minim Posted at: 2018-06-27T16:31:16.307Z Reads: 93

```
I bought this remote from banggood and I’ve tried to set failsafe according to the book by removing the bind plug while the remote is centered. When I test the failsafe by powering off the remote on purpose it goes to 60% or so. center is spot on 1500/50%. What am I doing wrong?

![image|428x500](upload://6og3PEpO5oU1P3cogVwm10CS87r.jpeg)
```

---
## \#3 Posted by: Minim Posted at: 2018-06-27T18:01:36.017Z Reads: 64

```
When the receiver sends 1600 how are the vesc supposed to know if that’s me wanting to have 1600 or the failsafe kicking in then? I thought that I had to learn the receiver to go to 1500 when the connection failed.
```

---
## \#4 Posted by: wafflejock Posted at: 2018-06-27T18:05:18.779Z Reads: 58

```
The VESC internal timeout is set to kick in when it stops receiving a signal entirely from the receiver so you'll need to just debug the transmitter/receiver for its built in 'failsafe'.  Honestly sort of dumb though don't see why it wouldn't just default to sending a 1500 pulse when it loses connection.
```

---
## \#5 Posted by: Minim Posted at: 2018-06-27T18:08:19.159Z Reads: 55

```
That is how I'm used to from RC/drones/planes/copters also. The controller can detect a missing or a pulse width out of the 1000-2000 range but when something is within that it think that everything is normal. I'm looking for how to learn the receiver how to send 1500 when it drops the connection with the transmitter. English is not my first language so sorry for not being clear in OP.
```

---
## \#6 Posted by: wafflejock Posted at: 2018-06-27T18:10:20.771Z Reads: 48

```
Yup I follow you just wanted to clarify on when the VESC failsafe will kick in.  For the transmitter/controller have you tried pushing it into slight brake position while removing the bind key to see if it adjusts the value down?  Wonder if the procedure is working or if maybe 1600 is just a default they built in.

---

Also was just saying the receiver is sort of dumb for not defaulting to 1500, wasn't directed at you.
```

---
