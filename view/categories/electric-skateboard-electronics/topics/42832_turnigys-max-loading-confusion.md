# Turnigy&rsquo;s Max Loading Confusion

### Replies: 8 Views: 503

## \#1 Posted by: shizzdogg Posted at: 2018-01-05T08:30:17.518Z Reads: 100

```
Hi all,

I am confused with the specifications of Hobby King's Turnigy motors. Specifically, the 'Max Loading' value e.g. Turnigy Aerodrive SK3 - 6364-245KV:

**Max Loading: 70A**
**Max Power: 2700W**

What is this value referring to? Is this the max current the motor will draw? I thought this max current would be: Imax = Pmax/V.

For example, if you are running this motor with a 6s LiPo, the max current that will be drawn is 2700/22.2 = 120A, which is significantly higher than the 70A? So I am not sure what the 'Max Loading' is.

Any help clearing this up would be appreciated.

Cheers
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-01-05T08:54:22.550Z Reads: 95

```
max load is for safe limit or continue draw. u can up the amp and voltage as long as u keep the motor cool
```

---
## \#3 Posted by: Luca1 Posted at: 2018-01-05T08:56:51.191Z Reads: 92

```
I think that If you put 22.2v in your motor you’ll  have a power of 22.2v x 70A = 1 551.4 watts max. If you put 120 A in your motor I think it’s gonna get broken. You’ll get 2 700 watts if you plug your esc with a 10s battery  because you have a 70 A max intensity you just have to do: 2 700/70 = 38v (approximately) wich corresponds to a 10s battery. You have to look the maximum amperage of your esc too because you don’t want to put 80 A in it if it only admit 70A. I hope I didn’t make any mistake and that I answered to your question.
```

---
## \#4 Posted by: onepunchboard Posted at: 2018-01-05T09:24:22.572Z Reads: 80

```
sk3 motor can take more than 120 amp. which is average 1/8 scale hobby esc. 

he is asking what the spec of the motor referring to. 

it referrs to max continuous draw. but as long as there is sufficient cooling it can go more than 70amps. 

personally i used 120amp before, and is watm to touch
 
if u use 6s battery=25v x 120a u can theoratically draw 3000w and on 10s batt 42x 120 = 5040W.

the motor obviously wont out put 5000w, but it can out put more than its spec sheet.

the problem lies on esc tho, because most of car esc made for 4 pole motor, it will cog and burn out due to insufficient detection of back emf.

if you want to usecar esc use prooven, branded esc
```

---
## \#5 Posted by: shizzdogg Posted at: 2018-01-05T10:36:47.891Z Reads: 60

```
Thanks makes sense. 

[quote="Luca1, post:3, topic:42832"]
You’ll get 2 700 watts if you plug your esc with a 10s battery  because you have a 70 A max intensity
[/quote]

So I guess that is why the Max Voltage is 10s for that particular motor?
```

---
## \#6 Posted by: shizzdogg Posted at: 2018-01-05T10:37:50.129Z Reads: 58

```
So 70A refers to the current the motor can draw before heating up?
```

---
## \#7 Posted by: onepunchboard Posted at: 2018-01-05T16:23:18.715Z Reads: 45

```
yeap

10 cha
```

---
## \#8 Posted by: squishy654 Posted at: 2018-01-05T17:01:53.686Z Reads: 37

```
Before the enamel melts off the wire and they short and then the magic smoke comes out of the motor...don't do that, they need the magic smoke to work well, keep it in the motor! lol
```

---
