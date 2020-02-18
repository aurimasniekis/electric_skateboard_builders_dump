# Smart Reverse on the FOCBOX Unity (And other VESC-based controllers) - Seeking Input on desired Behaviour -

### Replies: 13 Views: 613

## \#1 Posted by: Deodand Posted at: 2018-11-08T17:17:36.699Z Reads: 174

```
Hey guys, started to implement a smart reverse feature in the ppm app the other day and ran into some questions on what is the most intuitive way it should behave. For the uninitiated the short and simple of smart reverse is:

-When riding your board normally, the reverse throttle acts as a brake (as in current no rev w brake mode)
-If you hold the brake until you come to a complete stop then center back to 0 throttle and pull the brake a second time in it enters a "reverse mode"

Is this something **if done correctly** that people are generally interested in (also has it been done before by someone else?) or does everyone just want their board to go one way. I could imagine a few cases in which I might like to pop my board in reverse due to laziness. 

If the answer to that is yes (as an optional setting) then there is a few more targeted questions regarding behavior of the mode  in special cases. I just responded to someones post that got me thinking on this a bit ago:

[quote="Deodand, post:9, topic:1218"]
The described behaviour isn’t implemented in vesc FW. I started implementing it on the FOCBOX Unity, but came across some behaviour questions during implementation that I still need to tackle.

1. Say I am going forward up a hill, I pull the brake and my board comes to a stop then begins to roll backward as I’m holding the brake in. In this instance I guess the board should stay in brakes mode?
2. Say no throttle is applied and I am moving in reverse when I pull the throttle backward does it then continue to push me in reverse? Does the forward throttle then become brake? Or is it a timeout window on the reverse functionality i.e. pull in the brake release it check if speed is 0 or reverse then switch the backward throttle to reverse mode.
3. if you fully brake then press in the throttle into reverse a second time to enter “reverse mode” release the reverse throttle does it switch back to brake again? Or is it now locked into reverse mode until velocity becomes greater than 0 again (or some threshold)

Need to investigate what feels intuitive. A non-intuitive control interface is bound to piss people off and throw them from the board potentially injuring them.
[/quote]

Then realized it would be good to seek some outside input from you all :smile:
```

---
## \#2 Posted by: mackann Posted at: 2018-11-08T17:40:17.146Z Reads: 146

```
Hi, yes I would like that. Many times atleast in the beginning when I got my raptor 2 I wish I did have that function. I tried current reverse but didn't like it. This would be great if you could implement it. I think it have actually been done: https://www.electric-skateboard.builders/t/extended-ackmaniac-esc-tool-based-on-vesc-tool/35116
```

---
## \#3 Posted by: Mich21050 Posted at: 2018-11-08T17:40:47.401Z Reads: 142

```
I would also love to have that feature :smile:
```

---
## \#4 Posted by: Deodand Posted at: 2018-11-08T17:41:22.533Z Reads: 141

```
Thanks for the link, I thought I had seen this somewhere before :smile:
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-11-08T17:46:13.478Z Reads: 133

```
He has his FW uploaded to GitHub somewhere if it's not linked in that thread. 

I like how his reverse (is it just standard current w/ reverse or something special?) works. Brake until a certain erpm, then 0 throttle, then pull back to reverse. I use this all the time, mostly at stoplights and cross walks to change direction. Accelerating after reverse doesn't brake the reverse, it just accelerates forward from there and I find that works great for me to get going forward again without worry.
```

---
## \#6 Posted by: luis99945 Posted at: 2018-11-08T19:16:47.575Z Reads: 111

```
Hello i think you need put this function I like this idea 
Sorry for my English
```

---
## \#7 Posted by: dougpage Posted at: 2018-11-08T19:21:20.588Z Reads: 107

```
It doesnt hurt to have this feature. Maybe make it optional in the app with the unity
```

---
## \#8 Posted by: Silverline Posted at: 2018-11-08T19:21:26.256Z Reads: 104

```
For me, no thanks. I want brake to be brake, and nothing else
```

---
## \#9 Posted by: Deodand Posted at: 2018-11-08T19:23:09.917Z Reads: 99

```
Yes, I would never make it compulsory or even default I think. The behavior just seems like it might feel unpredictable when you first start using it and that will probably turn a lot of people off of it.
```

---
## \#10 Posted by: Titoxd10001 Posted at: 2018-11-08T19:38:09.914Z Reads: 94

```
Yes I like reverse in ackmaniac firmware. Double tap to go reverse. 

I would like the option of also having brakes when going in reverse or having a long delay or a way slower acceleration than normal if I accidentally pull full throttle forward. It's a accident waiting to happen if you let someone borrow your board otherwise like has happened to a friend that ate it while switching from reverse to forward.

Also max reverse speed is a good option. I use erpm limit to about 10mph.
```

---
## \#11 Posted by: b264 Posted at: 2018-11-08T19:43:06.739Z Reads: 88

```
[quote="Deodand, post:1, topic:73934"]
Is this something **if done correctly** that people are generally interested in
[/quote]

Yes!

[quote="Deodand, post:1, topic:73934"]
-When riding your board normally, the reverse throttle acts as a brake (as in current no rev w brake mode)
-If you hold the brake until you come to a complete stop then center back to 0 throttle and pull the brake a second time in it enters a “reverse mode”
[/quote]

Remember the "complete stop" part here needs to be configurable.  Sometimes on a steep hill, you want to engage reverse before coming to a complete stop -- because it's a hill going down and you don't want to roll forward and can't completely stop without using a foot.


Double-triple-super bonus points awarded for making a second PPM channel control a "brake and hold" feature where, for example, turning the wheel on the mini remote stops you completely -- using power if needed -- but you stay at a dead stop, even on a hill
```

---
## \#12 Posted by: b264 Posted at: 2018-11-08T19:43:45.601Z Reads: 88

```
[quote="skatardude10, post:5, topic:73934"]
He has his FW uploaded to GitHub somewhere if it’s not linked in that thread.
[/quote]

Of course he does, it's the law ;-P

This is copylefted software.
```

---
## \#13 Posted by: huntercasillas Posted at: 2019-05-01T03:44:58.668Z Reads: 34

```
Any way to update this feature on the Mac application? I tried using the windows one with a virtual machine but it never defects that it’s plugged in via USB. I had it as forward/reverse but when I would shift the throttle too fast from either direction the motors jolt and it makes a loud clunk which can’t be good right? I also would love traction control on the Mac app.
```

---
