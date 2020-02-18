# Problems with bluetooth module

### Replies: 13 Views: 266

## \#1 Posted by: Superflim Posted at: 2018-12-25T13:54:46.403Z Reads: 81

```
Hi guys,

I'm having some problems with my Bluetooth module. First, it didn't work at all but I guess that was because I was configuring my vesc with the VESC-tool, instead of ackmaniacs version.

So I got his version and out of the blue it worked, I was really surprised. But then I ran motor detection and configured my remote using the new ackmaniac vesc tool and the Bluetooth module stopped working. It doesn't send out any data but is connected.

It says 'ESC is not connected'

Anyone know how I can fix this? Thanks in advance

- Flim
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-25T13:56:37.747Z Reads: 74

```
Go back to your ppm settings and select ppm+uart, than double check the baudrate is 9600 and all should be good again
```

---
## \#3 Posted by: Superflim Posted at: 2018-12-25T13:59:23.623Z Reads: 69

```
It is already set like this.

But now I get the error Status: Invalid serial port: \\.\COM4, too
```

---
## \#4 Posted by: Sascha_stevenson Posted at: 2018-12-25T14:02:10.796Z Reads: 62

```
so you can't connect to the VESC?
```

---
## \#5 Posted by: Andy87 Posted at: 2018-12-25T14:02:26.766Z Reads: 60

```
You get this fault in the vesc tool?
Than your Computer tried to connect to the vesc via bt.
Switch off bt on your computer and connect again
```

---
## \#6 Posted by: Superflim Posted at: 2018-12-25T14:04:15.845Z Reads: 59

```
Yes in vesc tool.

BT wasn't even on... :/ double checked it ticked the boxes on and off.

It's defintaley off now but still not working
```

---
## \#7 Posted by: Andy87 Posted at: 2018-12-25T14:05:15.598Z Reads: 56

```
Switch off vesc
Close vesc tool
Restart everything again
```

---
## \#8 Posted by: Superflim Posted at: 2018-12-25T14:12:44.233Z Reads: 55

```
working now. Thanks Andy! <3
```

---
## \#9 Posted by: Andy87 Posted at: 2018-12-25T14:17:06.549Z Reads: 52

```
Welcome! One solution for me please 😜
```

---
## \#10 Posted by: Sascha_stevenson Posted at: 2018-12-25T21:09:17.442Z Reads: 44

```
good you got it working guys :grin: , this is the time to say that ironic phrase everyone hates "have you tried turning it on and off again?"
```

---
## \#11 Posted by: AlanZhou Posted at: 2018-12-25T21:28:18.503Z Reads: 39

```
I feel that sellers should really list setting the baudrate to 9600, because currently nobody does.
```

---
## \#12 Posted by: Superflim Posted at: 2018-12-26T00:35:38.136Z Reads: 34

```
Oh that wasn’t actually the problem. I kept ticking the box to ppm and uart but it didn’t save. Had to click some button that would save it
```

---
## \#13 Posted by: AlanZhou Posted at: 2018-12-26T02:40:33.125Z Reads: 32

```
Damn, XD

10 char
```

---
