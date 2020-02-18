# Vesc 4.12 FOC - Unwanted torque

### Replies: 15 Views: 1198

## \#1 Posted by: haand22 Posted at: 2018-03-11T15:04:32.233Z Reads: 217

```
Helloo,
I've been using the vesc with ackmaniac 2.54 with BLDC for some time with no problems and really nice behavior in every way. I have a 9s battery with Nyko Kama Nunchuck controller. Now I have configured ackmaniac 3.1 with FOC and it works all good with nice startup behavior and so on. The only problem is that when applying full torque for a couple of seconds and than releasing it, the board keeps on accelerating for a brief moment, even if going from full throttle to full brake, the board keeps accelerating for a brief moment. No need to say that its really scary and unpredictable. 

My best guess is that there is something going on with an integral windup in some controller loop as full throttle is applied. If someone could pinpoint me to what settings to play with I would be grateful!
![foc2|690x339](upload://946yTlmX0GQS51yq9Nckmxn4Yi8.PNG)![general3|690x240](upload://7PYyMMmOYWK4frqdgnfXXSYiZdo.PNG)![foc|690x379](upload://zKC3qdInSmzyo3WzxaJILN1jC9h.PNG)![foc3|690x453](upload://yKuxdStbAJ8K7dQ3XNByThdzavW.PNG)![general|690x475](upload://dzhNfAF4A4HfHhxv19mDLfvvsmM.PNG)![general2|690x164](upload://hQpksmFnIqmlBwp5mTEadKSEdtp.PNG)
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2018-03-11T16:33:10.481Z Reads: 169

```
Can you see the delay in the PPM tab?
```

---
## \#4 Posted by: haand22 Posted at: 2018-03-11T17:33:09.595Z Reads: 158

```
![nunchuck|690x273](upload://nIw42m4sA8UaK4dZKvpaW1nbyQn.PNG)

This is for nunchuck, I don't use ppm
(edit. Changed around with the positive ramping time but no difference)
```

---
## \#5 Posted by: Der6FingerJo Posted at: 2018-03-11T19:17:34.481Z Reads: 134

```
I mean when you see the percentage of the Nunchuck throttle, if it's delayed as well when letting go of throttle.
```

---
## \#6 Posted by: haand22 Posted at: 2018-03-11T19:40:29.684Z Reads: 133

```
Okej, no, there's no delay when looking at the bar. When using bldc, the throttle behaves exactly as it should so I wouldn't think it's the controller
```

---
## \#7 Posted by: Der6FingerJo Posted at: 2018-03-11T19:47:40.688Z Reads: 132

```
Hmmm ok. Have you tried to do detection again? Honestly i don't know what to test after that. Maybe setup the firmware completely new.
```

---
## \#8 Posted by: haand22 Posted at: 2018-03-12T09:48:03.814Z Reads: 103

```
I will try the detection again but I don't think that's he problem. I have already tried with ackmaniac 2.54 with Foc, no luck there.

I suspect some integral windup going on in some control loop concerning the requested torque from the esc. However, I don't know what settings that are affecting this behavior. Maybe I should try changing the maximum duty cycle or maximum erpm or something. 

Thanks for trying to help mate!
```

---
## \#9 Posted by: Acido Posted at: 2018-03-12T10:32:01.424Z Reads: 94

```
This happens to me also with the winning remote
```

---
## \#10 Posted by: haand22 Posted at: 2018-03-19T10:49:41.772Z Reads: 71

```
Ive been looking through the code and found something suspicious to me. It seems like a maximum duty cycle of [-1, 1] is hardcoded into the duty cycle control in FOC. Shouldn't it be like the maximum duty cycle here? In my case thats about 0.4. @Ackmaniac 
![error|474x499](upload://fjRtBAQ0fD4NgysQbsiV9lytYv8.PNG)
```

---
## \#11 Posted by: pat.speed Posted at: 2018-03-19T10:53:43.557Z Reads: 66

```
I’m pretty sure this is to do with the remote. Both the nyko and winning remotes are very unreliable, they also tend to drop out a lot.
```

---
## \#12 Posted by: haand22 Posted at: 2018-03-19T12:29:25.275Z Reads: 57

```
But i'm having a hard time believing that the remote can cause this repeatable behavior. Especially as it only appears in FOC mode. There are no delay in control signals when connected to the tool.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2018-03-19T12:47:42.403Z Reads: 51

```
Have you try to put those Value at 0.01

![image|690x273](upload://8Uy9foohxkwuQLfpO1tvjvkuQSX.png)
```

---
## \#14 Posted by: haand22 Posted at: 2018-03-19T13:00:30.956Z Reads: 47

```
I've tried them at 0.1 but no difference. Can try even lower when I get the chance
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2018-03-19T13:50:19.925Z Reads: 41

```
Maybe this could help you : http://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116/97?u=johnnymeduse
```

---
## \#16 Posted by: haand22 Posted at: 2018-03-19T14:03:28.349Z Reads: 40

```
Yeah, okay ^^ Maybe that's it. I'll give it a go and see if that will effect the behavior :) Tanks for all input!
```

---
