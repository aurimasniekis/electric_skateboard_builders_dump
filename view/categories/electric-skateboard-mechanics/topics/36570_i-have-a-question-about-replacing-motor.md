# I have a question about replacing motor

### Replies: 4 Views: 395

## \#1 Posted by: Alderins Posted at: 2017-10-26T13:47:09.190Z Reads: 77

```
Soo I bought a single conversion kit from MIB miami electric boards and it 
came with a 12S2P battery a vesc and an uncensored 250 KV motor. I've read that with a 12S battery Its better with a motor with a bit lower KV, like maby 170 - 200. Can I just buy a new censored 170 KV motor and replace it without changing the VESC settings? Or is it more to it?

Sorry for any bad spelling, English is not my first language..
```

---
## \#2 Posted by: ShutterShock Posted at: 2017-10-26T14:07:46.749Z Reads: 73

```
250kv is wayy high to run at 12S.  I run a 190kv at 12S and that is slightly dangerous.  Buying a new 170kv sensored is a much better option.  And as with any motor, you will need to at least do a motor detection and tuning of the settings for that specific motor.  There are some videos and many threads on the forum describing what settings people have used.  I am sure you would be able to find one for 170kv by using the search function. :slight_smile:
```

---
## \#3 Posted by: mmaner Posted at: 2017-10-26T15:00:18.144Z Reads: 53

```
As @ShutterShock said 250kv is too high for a 12s pack, but you can still use it by unticking the negative torque option and limiting the ERPM to 60k in the BLDC tool.  I would use a 190kv 6374 motor, both @torqueboards and @JLabs have them/will have them soon.
```

---
## \#4 Posted by: ShutterShock Posted at: 2017-10-26T18:27:44.140Z Reads: 35

```
Yeah you could do that, I think would probably just get a different motor cuz I've already blown a drv lol
```

---
