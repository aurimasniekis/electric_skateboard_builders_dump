# 4.12 nolimit wont stay at 60v

### Replies: 13 Views: 172

## \#1 Posted by: g1tana Posted at: 2019-02-13T14:56:13.912Z Reads: 78

```
Hi guys, i got a 4.12 that i run in my scooter. The scooter runs on 14s 58.8v and i run the no limit fw and set it 60v with no regen or braking.
Was running fine for a long time with everyday use, it wouldnt go 1 day and when i hooked it up to the pc, i noticed it had gone back to 57v but every time i set it back to 60v and hit motor update it goes back to 57v.

I tested the vesc on my kids scooter which only runs 6s and it went thtough the detection with no problems.

Thanks
```

---
## \#2 Posted by: linsus Posted at: 2019-02-13T15:23:57.765Z Reads: 65

```
14s on 4.x hardware?...
```

---
## \#3 Posted by: g1tana Posted at: 2019-02-13T15:35:58.747Z Reads: 64

```
Is that a question?
```

---
## \#4 Posted by: sayekim Posted at: 2019-02-13T15:36:38.971Z Reads: 64

```
Ya right. Amazing. 

@b264 you really wouldn’t like this.

To op, it is recommended to only go 10s on 4.xx hardware. 

Can’t help with the setting jumping back. It usually indicates that 57 is the max possible.

Were you perhaps never running the scooter with a max charged battery as in less than 57 volts?
```

---
## \#5 Posted by: Battosaii Posted at: 2019-02-13T15:37:19.648Z Reads: 59

```
I heard it's okay if you don't set brake Regen.
```

---
## \#6 Posted by: Battosaii Posted at: 2019-02-13T15:37:29.014Z Reads: 58

```
Check for a drv fault
```

---
## \#7 Posted by: g1tana Posted at: 2019-02-13T15:37:46.524Z Reads: 57

```
Yes that is right, been running it for 6months solid
```

---
## \#8 Posted by: g1tana Posted at: 2019-02-13T15:59:58.007Z Reads: 50

```
Been running it for 6months. There is a no limit fw that allows you to set it to 60v
```

---
## \#9 Posted by: g1tana Posted at: 2019-02-13T16:54:17.487Z Reads: 45

```
How do i do that, i suspect it is the drv. Waiting for some to arrive
```

---
## \#10 Posted by: Battosaii Posted at: 2019-02-13T17:15:33.842Z Reads: 42

```
Go into the terminal and type Fault
```

---
## \#11 Posted by: Battosaii Posted at: 2019-02-13T17:16:08.210Z Reads: 41

```
Also.does a red light turn on the Vesc when you try to.throttle? Also does it have a heat sink?
```

---
## \#12 Posted by: Mich21050 Posted at: 2019-02-13T17:18:32.585Z Reads: 40

```
On the new vesc tool you just click print faults.. :slight_smile:![Screenshot_1|461x233](upload://zsDe5j3JQrXaHrlcLMuM7LklF0V.png)  
@Battosaii... :joy: :slight_smile:
```

---
## \#13 Posted by: g1tana Posted at: 2019-02-13T17:48:59.916Z Reads: 35

```
Yh i checked for faults there is none, i thought there was a way to pyhiscally test the chip.
```

---
