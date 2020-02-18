# Encoders and VESC

### Replies: 5 Views: 1498

## \#1 Posted by: Deskonhecido Posted at: 2018-03-13T16:31:32.428Z Reads: 143

```
Hello, I am using the FOCBOX 4.12 motor controller and I have hooked up a DC motor to it. I've managed to figure out how to configure it despite the lack of information on it. I feel like the DC side of the VESC needs more information and love for new people. At this moment I'm trying to hook up a diferent DC motor, this time it has an encoder so I can read it speed, a quadrature encoder.

My question is, how do I connect the encoder when I can only find HALL input?
```

---
## \#2 Posted by: mccloed Posted at: 2018-03-13T21:29:15.697Z Reads: 125

```
http://www.electric-skateboard.builders/t/my-vesc-with-as5047-sensor-setup/6568
```

---
## \#3 Posted by: Deskonhecido Posted at: 2018-03-19T18:09:30.011Z Reads: 97

```
Thank you for the help and sorry for the delay, I will look into this and test it, I will give feedback when possible.
```

---
## \#4 Posted by: Deskonhecido Posted at: 2018-03-21T13:40:05.416Z Reads: 83

```
Ok, after analyzing what you shared I can say it doesn't help my problem.

Perhaps I didn't explain well. I have a DC motor hooked up to my VESC and after a few tests I can control in  open loop with the software but now I want to run it in a closed loop, the motor itself has an integrated encoder which outputs 2 signals, normally you only need one signal to determine the speed but with 2 signals 90º apart from each other you can determine if it's rotating left or right.

The main objective is connecting the VESC to a CAN bus where it will receive a speed value and with the aid of the encoder the motor will achieve that speed.

My problem is that I don't understand where should I hook up this encoder signal, all the posts and videos I've seen only use encoders with the BLDC or FOC configuration on the software but I'm using the DC configuration.
```

---
## \#5 Posted by: abrac Posted at: 2019-03-30T18:26:18.939Z Reads: 35

```
Hi do you still need help? If you've solved the issue can you post the answer? Perhaps the reason for your problems was this: I found that sensored speed control for DC motors was only added to the firmware at the beginning of this year (Feb 2019). Also what encoder are you using? ABI?
```

---
