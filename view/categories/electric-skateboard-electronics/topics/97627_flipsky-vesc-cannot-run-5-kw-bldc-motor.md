# Flipsky Vesc cannot run 5 kw BLDC motor

### Replies: 7 Views: 411

## \#1 Posted by: bilkenter Posted at: 2019-07-01T06:29:51.406Z Reads: 123

```
Hello everyone,

I have started to build my own electric motorcycle. My setup consists of 5 kw golden BLDC motor and flipsky 6.6 vesc. 

I have tried to find my necessary values(R, L etc.) to run my BLDC motor by using Vesc tool. Vesc cannot rotate in FOC mode or BLDC mode so it cannot detect necessary values. I have recorded video which shows my setup and parameters that I have assigned. 

I bring the youtube links which shows my setup and parameters:
https://www.youtube.com/watch?v=hRUGamM8dpY&t=54s
https://www.youtube.com/watch?v=zhvGCOrkup8

I am waiting your suggestions to solve this issue.

Thanks
```

---
## \#2 Posted by: Giga Posted at: 2019-07-01T07:58:53.970Z Reads: 112

```
The blinking red led tells you that something is wrong. I would check the fault codes and disconnect the motor and see if that fixes the red led issue. As long as the controller blinks red something is defect (low voltage, connection, wrong settings or could be hardware defect as well) and it wont be able to spin up the motor.
Maybe try the other side of your controller (looks like dual flipsky 6.6).

Also if you really want help make some high resolution video in landscape mode; I think I got eye cancer only by watching the first quater of the first video :nauseated_face:
```

---
## \#3 Posted by: bilkenter Posted at: 2019-07-16T13:31:08.305Z Reads: 78

```
Thank you Giga. It works well it detects everything except temperature sensor. I have problem with temperature sensor now. RED LED is blinking when I connect temperature sensor and VESC cannot detect temperature sensor. I bring the datasheet temperature sensor. I am not sure but maybe VESC cannot understand this kind of temperature sensor. I am open to suggestions.

https://www.goldenmotor.com/certs/KTY84_SER.pdf
```

---
## \#4 Posted by: Acido Posted at: 2019-07-16T15:23:31.736Z Reads: 64

```
Just disconnect the temp wire and try it that way

If its really important you can get a temperature beeper or something like that as an alternative
```

---
## \#5 Posted by: Gamer43 Posted at: 2019-07-17T06:31:22.335Z Reads: 47

```
The connector is trash, the wire for the temperature sensor doesn't make good electrical contact.
```

---
## \#6 Posted by: bilkenter Posted at: 2019-07-17T10:44:24.878Z Reads: 40

```
I resolder connection points but still it doesn’t work. I think problem is something else.
```

---
## \#7 Posted by: Giga Posted at: 2019-07-18T22:27:20.065Z Reads: 26

```
For the vesc you need a 10k NTC (just google it).

You linked a 500ohm PTC...no wonder it doesnt work. Wrong base divider, wrong beta, wrong type...

The schematics of the vesc are open source, just have a look where it says motor temp, everything you need you can just read there...
```

---
