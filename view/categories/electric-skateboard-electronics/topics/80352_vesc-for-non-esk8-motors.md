# VESC for non esk8 motors

### Replies: 8 Views: 261

## \#1 Posted by: murdomeek Posted at: 2019-01-09T02:26:29.723Z Reads: 132

```
I was wondering if a flifsky 4.12 or a focbox will work for this motor? (565W version. 12/48v, brushless.  Sensored, although ideally we wouldn't have to hook up the sensor)
https://www.robotdigg.com/product/1239/48V-330W-or-565W-86BLS-BLDC-Motor

I am trying to use it for a school project, but the default driver that came with it is pretty garbage: https://www.robotdigg.com/product/1238/BLD500-48V-500W-BLDC-Motor-Driver

Is it safe to assume I can set up the VESC with the setup software and it'll be able to run it?

thanks a bunch :)
```

---
## \#2 Posted by: pat.speed Posted at: 2019-01-09T02:37:07.590Z Reads: 129

```
Well I’m sure there is no reason it shouldn’t work but for esk8 purposes it’s not the best choice. 

For robotics or other devices it seems like a good choice
```

---
## \#3 Posted by: linsus Posted at: 2019-01-09T08:31:03.533Z Reads: 108

```
The VESCs sole purpose wasn't esk8. Unless it has some nasty high kv or something else nasty about it (wierd inductance or so, 4.12 doesnt like that), it will work fine
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-01-09T09:20:43.074Z Reads: 94

```
Looks to be about 73kv, which should be a good value for a vesc to drive.
```

---
## \#5 Posted by: murdomeek Posted at: 2019-01-09T18:10:31.194Z Reads: 62

```
Thanks a lot for your replys guys!

Yeah, this motor seems less powerful than the typical 6355 or 6374's everyone uses for esk8, so i thought it'd give it a try.

Weird how a small 6455 motor is ~4-5 times more powerful (watts) than this large heavy thing.  Any ideas on why that is the case?  (Such as the rated power on esk8 motors are 'theoretical max power' for 0.1 seconds before it melts)
```

---
## \#6 Posted by: murdomeek Posted at: 2019-01-09T18:15:43.203Z Reads: 60

```
how did you get 73kv from the specs?

I thought it was ~62kv (3000 rated rpm/48v)

(or is this "close enough")
```

---
## \#7 Posted by: MysticalDork Posted at: 2019-01-09T18:56:39.122Z Reads: 50

```
In the spec sheet it shows "back EMF" in volts/1000 rpm. I just reversed that to get rpm/volt.

Regarding the power rating question, it's a matter of how it's rated. Those motors are designed for industrial-type workloads, which means continuous duty for hours. Our motors are rated for peak loads, probably 1 to 10 minutes at most, and that's with plenty of airflow for cooling.
```

---
## \#8 Posted by: murdomeek Posted at: 2019-01-10T07:31:10.928Z Reads: 33

```
update:
it works great! =D
thanks for all the help guys
```

---
