# Who is using Current with reverse with PPM

### Replies: 11 Views: 970

## \#1 Posted by: Ackmaniac Posted at: 2017-03-21T11:13:46.764Z Reads: 171

```
I guess most of you that have a PPM remote use the control mode **"Current without reverse"**.
Are there some which use the control mode **"Current"** (it's with reverse)?
Because when you do a hard brake the wheels start to spin backwards while your still driving forward. Then it detects that you are going in the opposite direction and starts to brake again. then spinning backwards and so on with a frequency of like once a second.

At the Nunchuk this is not the issue because you need to press a button to go reverse. But with PPM you don't have that. Or i could make that work with the steering wheel like with cruise control in my firmware mod. But i am trying to find a nicer way.

In my newest Version of the firmware mod 2.54 (**not yet relesed**) i implemented reverse for Watt control which has of course the same issues at hard braking as Current Control.
So i wanted to know if the community even needs it. I can imagine that EMTB with heel straps would like to have it.
```

---
## \#2 Posted by: onloop Posted at: 2017-03-21T11:26:31.713Z Reads: 170

```
Definitely useful for emtb. Not really important for anything you can pick up and turn around. Or pivot with kicktail etc.
```

---
## \#3 Posted by: PXSS Posted at: 2017-03-21T11:27:11.532Z Reads: 170

```
I don't currently use it but will give it a go on my next build. It's a "trick" deck that'll be used to do some free riding and the reverse function will be nice if it works well. 

How do brakes work?? Do you just command a zero throttle? You're getting oscillations from what I understand, correct? Is it a PID controller? If so, you can adjust your gains so that it doesn't overshoot
```

---
## \#4 Posted by: makevoid Posted at: 2017-03-21T11:28:30.379Z Reads: 160

```
Imho reverse is too dangerous, never tried on VESC thou. I've had an FVT esc configured w/ reverse (I didn't have the prog. card). I went over a small bump at moderate speed, wheel lost grip, reversed, locked down and sent me flying :) I don't recommend it ^^

edit: probably a timeout of let's say 0.5/1 sec. from a direction to the reverse would help against that?
```

---
## \#5 Posted by: Qwiksand Posted at: 2017-03-22T00:51:15.077Z Reads: 123

```
I 'd really like to use reverse more, but I can only get away with it at low speeds for the reasons you listed above- I've got a super slow mode that maxes out at 6mph and reverse is borderline usable there.

Maybe even having a pre-set delay before the the reverse kicks in might help, though this wouldn't work on a trick deck where you need quick switching. EDIT: just saw @makevoid made this suggestion above, I second his opinion :sunglasses: 

And thanks again for the awesome firmware/app!
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-03-22T01:14:54.567Z Reads: 111

```
I think i found a nice solution for that problem. But i need to make some test runs to find out if it suits in every situation. More or less if you go forward and brake then it will come to a stop as long as you hold the brake. Now if you want to go backwards you have to release the throttle and go on the brake again. And if you move already backwards then it keeps on doing that. But if you go forward again and brake then it will only do the brake. To go backwards you have to come close to a standstill and release the throttle again and then brake again to go backwards.
Sounds complicated but it becomes intuitive after a short while. But need to make more testruns.
If somebody has another good idea then feel free to leave your ideas here.
Of course the logic behind the described behavior above involves a bit more logic and details like hysterisys and a minimum erpm in the backwards direction. But i will let some guys do a testrun to see if they agree with me.
i also could build the logic to switch the direction via the steering wheel but i think the described behavior above is worth a try. And i need the wheel already for another function.
```

---
## \#7 Posted by: Titoxd10001 Posted at: 2017-03-22T02:25:53.223Z Reads: 101

```
That's how reverse works on Hobbywing ESCs. Its useful to move it out the if the board ends up in the middle of the street after having to bail. For riding it's difficult to ride opposite normal stance. I have accidentally reversed​ while going forward and shredded my belt. Maybe a option for pressing brakes two times and another for three times.
```

---
## \#8 Posted by: Pimousse Posted at: 2017-03-22T12:23:21.669Z Reads: 87

```
On dual, it could simply uses the CH3 button of GT2B to toogle from backward to reverse by a push on the button.
Like you already do for cruise control with PPM. ;)

BTW, it's really interesting. I'm building a MTB with heel straps so I'm defenitely in to test (but I'll use VESC 6... )
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2017-04-10T23:44:07.225Z Reads: 72

```
Did you release these updates? Switching between my other board that has a max6 it feels so weird to not have reverse
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-04-10T23:51:20.741Z Reads: 70

```
No i haven't released that yet. Only waiting for the last confirmation of some beta testers that everything is working well for Nunchuk. So hopefully tomorrow or the day after.
```

---
## \#11 Posted by: Titoxd10001 Posted at: 2017-04-11T00:12:35.176Z Reads: 64

```
Looking forward to going going backwards 👍
```

---
