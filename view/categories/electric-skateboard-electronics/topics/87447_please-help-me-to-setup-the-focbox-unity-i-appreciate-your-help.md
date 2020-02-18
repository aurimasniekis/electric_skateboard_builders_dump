# Please help me to setup the focbox unity I appreciate your help

### Replies: 11 Views: 522

## \#1 Posted by: Bas1 Posted at: 2019-03-17T20:49:28.279Z Reads: 146

```
Hello can you help me to setup up the focbox unity I have an dual 6s lipo 60c 8000mah 480a total I run them in series I have a dual 6374 149kv sensorless 70a motor max total and 12awg xt60 series cable and extension cable what is the ideal setting for my setup also i want to disable the reverse function
I'm new to esk8 so please help me!!
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-03-17T20:57:39.060Z Reads: 143

```
@Bas1 
[quote="briman05, post:5165, topic:9559, full:true"]
Well motor max put 70 and -60. As far as the reverse you will want to have current no reverse in your Ppm tab but do that after you set your max and min pulse for your remote
[/quote]
[quote="b264, post:5166, topic:9559, full:true"]
-60A motor minimum is going to be too much brakes on two motors. I’d raise that to -45A to start with. On one motor, sure…
[/quote]
 Your questions have already been answered in the first place you asked, 20 hours ago. No need to start a new thread copy-pasting the same question.
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-03-17T21:43:45.366Z Reads: 130

```
Lol I think he wants more info


In that case: 

https://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980

![giphy%20(6)|500x281](upload://iI0GCEVYJs43OUNaWnuiH8ESbAi.gif)
```

---
## \#4 Posted by: BigZwatt Posted at: 2019-03-17T21:58:13.654Z Reads: 117

```
**_remember to use that search function before creating a new  thread_**

[Here's the unity thread ](https://www.electric-skateboard.builders/t/focbox-unity-support-setup-troubleshooting/77861/610)
```

---
## \#5 Posted by: Bas1 Posted at: 2019-03-17T22:12:33.903Z Reads: 113

```
Thanks this is what I needed sorry for the new thread I want a little bit more info thanks.
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-03-17T22:15:12.545Z Reads: 111

```
All good, sorry if I sound disparaging. I just think everyone has to start somewhere, and taking the first step is always the most important
```

---
## \#7 Posted by: kevingraehl Posted at: 2019-03-18T03:05:05.042Z Reads: 93

```
https://www.youtube.com/watch?v=nBrxDHqVh1k   i need help to
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2019-03-18T03:10:13.327Z Reads: 85

```
@Bas1

https://www.youtube.com/watch?v=C7MtbMTKrOs

@kevingraehl 
You have to configure your focbox using the BLDC tool. Yes, on a computer. 

Here is a link that should help you

https://www.electric-skateboard.builders/t/vesc-faq-easy-vesc-configuration-in-windows-mac-for-noob/2963
```

---
## \#9 Posted by: kevingraehl Posted at: 2019-03-18T03:47:52.795Z Reads: 66

```
![20190316_221359|666x500](upload://x9T2F14zHChZnYQpuul3LeetkQA.jpeg) 

then i try to use the VESC tool.. but windows only..  ready to sell it all ..  I just want to ride.. went 20 mph on a single motor, and speed control hooked up.. but the want both..   do i use the servo y cable with the one cable cut, and canbus?  and like serial , need to make one send/receive ?   they are both hooked up to send,, usually in serial ways, the high goes to the low..  can't find a central youtube video on how to get a master/ slave.. and what wires to hook up with.. bought used with no instructions
```

---
## \#10 Posted by: TommyCnc Posted at: 2019-06-21T20:20:46.733Z Reads: 29

```
What was the solution I am now having this problem
```

---
## \#11 Posted by: CarlCollins Posted at: 2019-06-21T20:22:26.852Z Reads: 28

```
You have to use the VESC tool and have to flash the 2.18 firmware to use FOCBOX with BLDC tool
```

---
