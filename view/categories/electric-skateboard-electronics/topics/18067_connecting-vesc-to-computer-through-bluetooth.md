# Connecting vesc to computer through bluetooth

### Replies: 6 Views: 628

## \#1 Posted by: Michael319 Posted at: 2017-02-22T02:31:30.697Z Reads: 153

```
So I connected bluetooth to the vesc. Everything is working 100%. but I would like to program the vesc through the bluetooth module on my computer. I tried using the apps and they didn't work 100%, so how would I connect the  bluetooth module to the computer

I connected via bluetooth and it is paired, but nothing is showing up in bldc tool.
```

---
## \#2 Posted by: rpn314 Posted at: 2017-02-22T19:18:04.140Z Reads: 127

```
Did any of the apps work? If none worked, than you probably need to change the UART baud rate on the VESC.
```

---
## \#3 Posted by: Michael319 Posted at: 2017-02-22T20:16:50.612Z Reads: 117

```
@rpn314 I did change the rate, it works and I can use it to see voltage speed etc, but I can't write to the vesc
```

---
## \#4 Posted by: Marksmoura Posted at: 2018-08-28T04:39:02.915Z Reads: 63

```
Did you found out how to do it?
```

---
## \#5 Posted by: Michael319 Posted at: 2018-08-28T14:49:43.338Z Reads: 45

```
Well the metr.at app with their own Bluetooth module allows you to edit some setting not all. Never figured it out fully tho.
```

---
## \#6 Posted by: SuperBen Posted at: 2018-08-28T17:17:26.897Z Reads: 40

```
I was able to connect to mine to the ESC Tool with an HM-10 module via Ackmaniacs firmware and Tool. Was able to read settings but wasn't able to get written configs to stick. Probably could fix with a little troubleshooting but haven't picked it back up to try since
```

---
