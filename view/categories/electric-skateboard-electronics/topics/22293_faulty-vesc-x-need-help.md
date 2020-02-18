# Faulty vesc x, need help

### Replies: 17 Views: 1411

## \#1 Posted by: KenTw Posted at: 2017-05-03T11:23:06.302Z Reads: 148

```
guys, i posted my problem on the other forum with my dual 6374 setup
https://www.electric-skateboard.builders/t/dual-6374-190kv-rear-motors-like-a-boss/18898/34
i guess it didnt really suit the post so no one bothered....
i contacted both @onloop and his support team several times, with only one reply of please wait and its been almost one month and lots of emails sent to them with no reply back...
this is what it looked like when i first had it on the board
when i do the detection on the BLDC one of the motor kept having stuck sound as if it is somewhat jammed
i swapped the vesc from other motor and it worked, swapped back and the motor stuck again
i confirmed the problem and contacted them and nothing was done....
it was frustrating, but it is even worse now, iit doesnt even detect the motor when i do motor detectiion on the BLDC
it shows that it is connected to the BLDC, but when i do the detect parameter test it shows detectiion failed....
the other vesc x worked with both motors
but the faulty vesc x.... ARGGGGG
here is a picture of the BLDC detect with the working motor
<img src="/uploads/db1493/original/3X/2/6/2643318f04979efaed7e7622c1cbc1cc96758c28.jpg" width="690" height="413">
and here is a picture of the fail detection
<img src="/uploads/db1493/original/3X/0/b/0b15a15e933cabea5d33e87db7a3f9cee563af31.jpg" width="690" height="415">

thanks for reading, ken
```

---
## \#2 Posted by: KenTw Posted at: 2017-05-03T11:24:54.499Z Reads: 138

```
[quote="KenTw, post:1, topic:22293"]
even
[/quote]

this is how iit looked like when i first triied to detect the remote, u can see how it jams
https://www.youtube.com/watch?v=XPoFlUEye_M

and now it doesnt even detect
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-05-03T11:34:09.032Z Reads: 128

```
I see that you changed the Min ERPM in the BLDC Tab. This is a very sensitive value.
Please set oit to the standard 150.
And you are also using Delay as Comm Mode. Please set it to Integrate.
And also change back the Phase advance at BR ERPM to 0.80.
```

---
## \#4 Posted by: Blasto Posted at: 2017-05-03T12:20:45.346Z Reads: 122

```
Your motor leads are exposed.... they touched and damaged the vesc...

Oh now i remember, you created the same exact thread.... i stll dont see an issue w that motor detection
```

---
## \#5 Posted by: KenTw Posted at: 2017-05-03T14:38:46.064Z Reads: 109

```
idk this setup was from another guy on youtube
but making it back to default doesnt make it work either...
are you saying the setup you linked me would make the motor detectable???
i will try it tmr
```

---
## \#6 Posted by: KenTw Posted at: 2017-05-03T14:45:19.643Z Reads: 101

```
it doesnt connect now...
look at the two pictures one is motor detect with the specs and the other one is detect failure
as for the march 16th 2017, 
at 0:14 u see the motor ran smoothly through the vesc x (which is what is suppose to happen)
at 0:59 u see the motor running smoothly on the higher spin, but the lower spin it would jam in a wrong way which it isnt suppose to happen
and thats the vesc x thats not working now
motor leads are wrapped when i do the runs outside, these bullets are only exposed because i need to exchange the motors with each other to find out if it is the motor problem or the vesc problem
```

---
## \#7 Posted by: KenTw Posted at: 2017-05-03T14:51:06.346Z Reads: 99

```
maybe i did somethiing wrong somewhere, but i did give it a shot to everythiiiing suggested to me
thats also how i found out that it wasnt the motor problem but rather the vesc x problem
because someone suggested swapping the connection between the vesc x and motor to make sure which one doesnt work, i only happened to be able to do this because i got two vesc and two motors
and yes, swappingi bbetween them does mean ii have to keep unpluggiing the bullet connectors if that is what you mean bby motor lead
```

---
## \#8 Posted by: Blasto Posted at: 2017-05-03T14:52:43.682Z Reads: 95

```
[quote="KenTw, post:6, topic:22293"]
it doesnt connect now...
[/quote]

well that has nothing to do with the motor detection.

[quote="KenTw, post:6, topic:22293"]
but the lower spin it would jam in a wrong way
[/quote]

set the low duty to 0.1 on the motor detection.
```

---
## \#9 Posted by: KenTw Posted at: 2017-05-03T15:00:20.211Z Reads: 93

```
and personally i dont thiink it would be my installation problem, because these two motors and vescs are set up NEARLY IDENTICAL, but BOTH motors only work normally through ONE of the vesc x...
someone suggested re soldering the bullet connectors and i tried that too, result is still two working motors through one vesc x but the other one always have problem (tested two weeks ago)
now the vesc x still can connect to the BLDC but it shows detection failure only on this vesc x
i will try to reset them bback to factory, but the last time i tried, it didnt work
```

---
## \#10 Posted by: KenTw Posted at: 2017-05-03T15:01:52.301Z Reads: 91

```
ok ill tell u the result tmmr
```

---
## \#11 Posted by: NilsS Posted at: 2017-05-03T17:28:18.420Z Reads: 81

```
did you insulate the VESC outputs if they touch while the motor is running it will fry. im talking about the golden contact points
```

---
## \#12 Posted by: KenTw Posted at: 2017-05-04T05:02:06.268Z Reads: 68

```
not when i do tests and leave them around my computer
when i do test rides i use electric tapes to wrap them
but u know, when i try to unplug them to test how the motor react to each vesc x, they will need to e unplugged therefore they are exposed
```

---
## \#13 Posted by: KenTw Posted at: 2017-05-04T05:03:49.155Z Reads: 67

```
hey, would u kindly send me a picture of how u setup ur vesc x on the BLDC?
ill try to configure it to that and see if it works
```

---
## \#14 Posted by: treenutter Posted at: 2017-05-04T15:03:07.022Z Reads: 57

```
@KenTw pls see the forum guideline below and edit your post accordingly. Consider removing screenshots of vendor communications and revising your title to reflect the problem with the product. 

Have you tried to reinstall firmware on the VESCx that you believe is faulty? It seems that you've edited a lot of parameters without success, it would be worthwhile to start from a fresh firmware update.

https://www.electric-skateboard.builders/t/new-forum-guideline-vendor-transactions-and-complaints/20290
```

---
## \#15 Posted by: KenTw Posted at: 2017-05-05T02:05:32.256Z Reads: 41

```
@treenutter here, i deleted all the negative stuff as told, even though i think they should stay on at least till i get a feedack from enertion...

and as for reinstall firmware... i only know how to make it back to factory setting through BLDC... i tried to set it back to factory setting quite a few times, still doesnt work
what bothers me is that both vesc x are setup in the exact same way, but ever since i got them, one works perfectly fine and the other one just doesnt, through a lot of ways
so far the things ive tried
-make sure bullets are sealed (it was always sealed when i fully mount the battery up for a test run)
-swap the motors to see if the vesc x works with other motor (nope, same problem) (both motors work perfectly on the other vesc x, through this setting AND factory setting)
-make vesc x back to factory setting (problem still not solved)
-reconnect the bullet connectors, maybe one is connected poorly (done, still no improvements)
-contact enertion and ask for help (did that, said "wait for reply" and no replies were found within a month with me reminding them with several emails)
-the motors might be fried due to your extreme setup (swapped motor with other vesc x and it works, so both motors are still fine, just that they wont work through the vesc x which is flashing red
```

---
## \#16 Posted by: KenTw Posted at: 2017-05-05T02:37:36.395Z Reads: 41

```
someone asked me if i had error after i did some personal setting
the answer is no, i had one motor jaming in a weird way when i first had them on the board without setup
in fact i was actually struggling with how to get the vesc x to connect to the BLDC
i still have the chat record saved on march 17th
to the time when i needed help to connect the vesc to the PC
so back in factory setting it was already acting weird...
<img src="/uploads/db1493/original/3X/1/c/1c1deafede0d193a8dbf76dfd8e409bc2cf849b8.jpg" width="690" height="270">

thats why i really think this is a problem ever sinice i had it....
```

---
## \#17 Posted by: KenTw Posted at: 2017-05-15T02:57:45.157Z Reads: 32

```
guys new update
after around 6 weeks of no reply, i got an email 
they will add a replacement for me when there are stock!
im pretty happy to hear this

ill update this when i do get a vesc and see if this problem is solved or not
```

---
