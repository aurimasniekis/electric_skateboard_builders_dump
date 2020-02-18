# Need help programming a dual vesc

### Replies: 20 Views: 295

## \#1 Posted by: starstuck8 Posted at: 2019-02-03T03:16:16.691Z Reads: 57

```
I know it's probably easy to find the numbers to use for builds with all pro3 conversion kit parts but I am doing a slightly different setup with diagonal configuration drive motors toward the middle and 6380 instead of 6374 motors, and a 12s5p 30Q pack. I don't have the parts yet.
```

---
## \#2 Posted by: Andy87 Posted at: 2019-02-03T03:18:52.075Z Reads: 54

```
And what is your question now?
```

---
## \#3 Posted by: starstuck8 Posted at: 2019-02-03T03:20:35.168Z Reads: 53

```
The dual motor settings for the vesc.
```

---
## \#4 Posted by: Noob-at-building Posted at: 2019-02-03T03:22:36.601Z Reads: 52

```
are you ppm splitting or using canbus?
```

---
## \#5 Posted by: starstuck8 Posted at: 2019-02-03T03:23:21.252Z Reads: 52

```
I think the front slave motor is going to have reversed positive and negative numbers because it is reversed direction
```

---
## \#6 Posted by: starstuck8 Posted at: 2019-02-03T03:25:24.553Z Reads: 51

```
can bus is on my shopping list but i dont know what ppm splitting is.
```

---
## \#7 Posted by: Andy87 Posted at: 2019-02-03T03:28:27.621Z Reads: 52

```
It’s super easy and the same like you mount both on the back.
Just swap two of the phase wires and the motor will turn the other direction.
Or tick the box „invert motor settings“ while programming your front vesc
```

---
## \#8 Posted by: Noob-at-building Posted at: 2019-02-03T03:28:44.338Z Reads: 51

```
split ppm is where the vesc have there own data and and don't connect at all, this means the motors will spin at different rates. This is apparently more relivable than canbus
```

---
## \#9 Posted by: starstuck8 Posted at: 2019-02-03T03:48:26.452Z Reads: 48

```
Which components does that go between?
```

---
## \#10 Posted by: starstuck8 Posted at: 2019-02-03T03:52:22.383Z Reads: 48

```
Doesn't the vesc have sensors for both motors? I was thinking the can bus was between master and slave vesc. But I'm planning on using a dual vesc now.
```

---
## \#11 Posted by: Andy87 Posted at: 2019-02-03T04:06:53.545Z Reads: 45

```
No need for split ppm if you use a dual vesc.
And yes there is a port for each motor sensor wires on the dual vesc.
```

---
## \#12 Posted by: Noob-at-building Posted at: 2019-02-03T04:08:34.232Z Reads: 46

```
split ppm is where you take both vesc and put them into the receiver so they use the same remote,
there is 3 wires 
+5v
Signal
ground

you connect both the signal to each other and the ground, but you only use one 5v wire to power the receiver![62|690x388](upload://goUDK8RBOkjaS2CkzS49VIfJIDH.png) 
ignore receiver inputs, there not correct. don't judge my art work :frowning:
```

---
## \#13 Posted by: Noob-at-building Posted at: 2019-02-03T04:10:50.086Z Reads: 42

```
or just read this
# [Question on CAN vs split ppm](https://www.electric-skateboard.builders/t/question-on-can-vs-split-ppm/52443)
 [quote="RedEagle, post:13, topic:52443, full:true"]
You have three wires of the receiver.
+5v
Signal
Ground

Solder signal together.
Solder ground together.
You have two +5v wires. One on each vesc.
Cut one +5v wire. You only need to connect one +5v wire to the receiver.
So in the end you’ll have one +5v wire, 2 signal wires and two ground wires connected to the receiver.

Hope this helps.
[/quote]
```

---
## \#14 Posted by: ZachTetra Posted at: 2019-02-03T04:10:58.270Z Reads: 38

```
How does split ppm make a difference?  Isn't all canbus do is send the same signals?
```

---
## \#15 Posted by: Andy87 Posted at: 2019-02-03T04:17:40.643Z Reads: 37

```
No.
CAN = master slave traction control 
Split ppm = master master
```

---
## \#16 Posted by: Noob-at-building Posted at: 2019-02-03T04:18:35.050Z Reads: 36

```
canbus shares information between vesc to make sure they are spinning at the same rate, you can also make them have traction control where as split ppm don't send information between them as they are not connect to each other, this means they have there own information. It generally means if one vesc goes down then the other one will still be powered, unlike over canbus they both go down. This makes it more reliable unless the vesc with the 5v output goes down then they both go down.
split ppm is used {in my case when i fried my canbus connector cause i dropped solder in it}  because you can configure the vesc separately, its more reliable, and also is the safest method.
```

---
## \#17 Posted by: starstuck8 Posted at: 2019-02-03T04:30:39.467Z Reads: 37

```
Does that apply to dual vesc?
```

---
## \#18 Posted by: Noob-at-building Posted at: 2019-02-03T04:38:32.383Z Reads: 36

```
yes
10char
```

---
## \#19 Posted by: Santino Posted at: 2019-02-03T05:08:36.709Z Reads: 32

```
I use can, no problems at all... You can check at https://www.vesc-project.com, then go to manuals. Tons of info...
```

---
## \#20 Posted by: starstuck8 Posted at: 2019-02-03T05:15:21.834Z Reads: 33

```
Are there two remote channels, one for each side of the vesc?
```

---
