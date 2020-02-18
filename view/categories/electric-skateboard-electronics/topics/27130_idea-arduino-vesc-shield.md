# \[IDEA\] Arduino VESC Shield

### Replies: 4 Views: 371

## \#1 Posted by: lox897 Posted at: 2017-07-09T07:19:43.366Z Reads: 107

```
I just had an idea and want to hear you guys' thoughts. What if we had some 2mm JST-PH headers on top of the vesc and then had a shield that included an NRF or BT so you just snap it in and can connect to an Arduino remote or phone? Could probably just use the existing VESC design and edit it to basically have the same shape PCB on top with male headers.
```

---
## \#2 Posted by: Sander Posted at: 2017-07-09T11:27:39.577Z Reads: 89

```
Wont fit in my board tho, it wil be too thick.
```

---
## \#3 Posted by: Maxid Posted at: 2017-07-09T11:35:17.424Z Reads: 88

```
what will be the benefit compared to just using cables?
This would only make sense if you want to have multiple UART devices connected at the same time - which I don't see a reason for.
```

---
## \#4 Posted by: lox897 Posted at: 2017-07-09T12:07:54.108Z Reads: 71

```
The main thing I'd see as a benefit is less surface space taken up, and a cleaner setup. Imagine if we could have the vesc 4.12, with lots of addon modules, like BT, NRF, dual ESC.

You could eliminate some of the things needed on the shield VESC, such as a power connector, because it would run parallel with first vesc. There's probably quite a few more things a shield could enable, temperature sensors for the board, maybe even an LED shield or a camera connection for a gopro.

You could also have an NRF and BT module on same shield and switch it with a PCB jumper
```

---
