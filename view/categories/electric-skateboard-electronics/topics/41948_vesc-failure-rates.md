# VESC failure rates?

### Replies: 21 Views: 1342

## \#1 Posted by: LAVAMAN Posted at: 2017-12-26T20:50:49.074Z Reads: 172

```
Has anyone ever tried to compile a list of overall failure rates of VESC's being sold on this forum? The reason I ask is that I think a fair % of failures are not user error, just bad quality and no QC (or inadequate QC) before being shipped to customers. I have read that several of the users on this forum have a box full of bad VESC's. I would be interested in knowing how many you have purchased in total, and of those how many were just bad or failed in less than a year and where they were purchased. I would not count those VESC's that (you know) failed because you made a mistake and did not follow the instructions (like adjusting the battery settings for the size of battery you are using) or were exposed to water etc. . Could you imagine if 80-90% of the bad VESC's were all coming from the same source (manufacturing facility or vendor). People who sell VESC's are probably not going to like this post. Just curious what you guys think.
```

---
## \#2 Posted by: Acido Posted at: 2017-12-28T08:03:55.941Z Reads: 138

```
If you push the limitis its likely to fail, if you dont, use reasonable settings there shouldnt be any problems
```

---
## \#3 Posted by: willpark16 Posted at: 2017-12-28T16:15:31.715Z Reads: 122

```
Yes just search it and you will find someone has
```

---
## \#4 Posted by: Exiledd_Top Posted at: 2017-12-28T17:06:42.962Z Reads: 116

```
@Deckoz and his crew managed get 23 vesc from TB and they were all bad he said or something along the lines they not lasting, some come same factory. From what am aware
```

---
## \#5 Posted by: Deckoz Posted at: 2017-12-28T17:15:52.297Z Reads: 106

```
Yea... 26.. 17 boards, mixed bldc/hybrid/foc. All dead within 2 months

I will say, there was 3 that lasted. Beyond those that failed. They were BLDC on 12s..

I find this fascinating that the bldc 10s all died. The current on 12s must be significantly less due to the increased voltage, allowing the fets and drv to stay cooler.
```

---
## \#6 Posted by: deucesdown Posted at: 2017-12-28T17:59:47.417Z Reads: 100

```
[quote="Deckoz, post:5, topic:41948"]
12s must be significantly less due to the increased voltage
[/quote]

Ah I failed at search but I believe @jinra tested, and found current to increase with voltage. It's as if higher voltage allows more current to flow.

Did all the vesc fail in similar ways?
```

---
## \#7 Posted by: LAVAMAN Posted at: 2017-12-28T18:00:34.564Z Reads: 96

```
Thanks for the info. I just sent my TB VESC to "The Board Tech" for an evaluation and repair. I hope it can be repaired. I hope it is worth repairing. I emailed Olins about when they might have their VESC's back in stock and have got no reply. FOC box is my other option. I hate throwing away $
```

---
## \#8 Posted by: Cobber Posted at: 2017-12-28T18:33:34.671Z Reads: 92

```
 Chaka might not be doing any DIY anymore dude, regardless you might not hear back from him dude?

https://www.electric-skateboard.builders/t/merry-christmas-and-goodbye/41826?u=cobber
```

---
## \#9 Posted by: LAVAMAN Posted at: 2017-12-28T18:59:01.371Z Reads: 89

```
Thanks, I must have been speed reading that post. I thought he was going to be focusing on Olins business in general, not just "completes".
```

---
## \#10 Posted by: Deckoz Posted at: 2017-12-28T19:20:58.184Z Reads: 89

```
[quote="deucesdown, post:6, topic:41948"]
found current to increase with voltage
[/quote]

For the same "load" the current will be less. However it's easy to surpass that load with the extra voltage. Think about acks firmware.

If you set the  max load watts to be 1512 watts per motor. 
On 10s motor max 42amps is  36v * 42 = 1512w
On 12s motor max 34a is 44.4v * 34a = 1512w~

Obviously if you don't limit your load...the motor will pull up to whatever you allow it. This is a good and a bad thing but you can play with it.

For example. Running a high motor Amp max without a watt limit. Let's choose a 100a motor max for simplicity. We have a duty cycle max of .95

Voltage = 42v
Motor max = 100a

At 0.25 duty cycle (42v*.25dc)*100a=1050w
 0.5 duty cycle (42v*.5dc)*100a=2100w
 0.75 duty cycle (42v*.75dc)*100a=3150w
 0.95 duty cycle (42v*.95dc)*100a=3990w

If you set a max watts. You can effectively make the board have really good dig acceleration while taming the top to be smooth. When your rolling at 20mph and reengaging the throttle puts you at about .35-.45 duty cycle. Having 100amps to the motor instantaneously is not ideal. Getting more like 20-45 is smooth. So let's pick 45a max for end throttle taper. 1750w is a nice middle wattage range for 6374 and will keep them running on the cooler side.

Our settings
Voltage = 42v 
Motor max = 100a
Max watts = 1750w

At 0.25 duty cycle (42v*.25dc)*100a=1050w
 0.5 duty cycle 1750w/(42v*.5dc)= 83a
 0.75 duty cycle 1750w/(42v*.75dc)=55.5a
 0.95 duty cycle 1750w/(42v*.95dc)=43.85a


Just something to think about..anyway amps go up as the voltage goes down...but you have a higher power(wattage) capability as the volts go up with the same amperage
```

---
## \#11 Posted by: Ixf Posted at: 2017-12-28T19:45:53.988Z Reads: 79

```
Damn.. wish I read this earlier.. bought 2, 2 dead, RMA limbo
```

---
## \#12 Posted by: LAVAMAN Posted at: 2017-12-28T20:44:04.762Z Reads: 74

```
If "The Board Tech" cannot fix mine then it will have to be FOC BOX or Miami Electric Boards. Olin's is out of the VESC business.
```

---
## \#13 Posted by: Jinra Posted at: 2017-12-29T00:57:01.981Z Reads: 64

```
I've never tested 12s as I don't have any power sources that provide that voltage.
```

---
## \#14 Posted by: deucesdown Posted at: 2017-12-29T01:55:40.228Z Reads: 62

```
Thanks for peeking in.

IIRC was it something like, you swapped out a 6s pack for 10s hoping to reduce amps, and actually the amps increased on 10s? I hope I'm not mixing you up with someone else.
```

---
## \#15 Posted by: Jinra Posted at: 2017-12-29T01:59:34.264Z Reads: 64

```
Yea i dont think that was me, I don't use 6s either. For the same wattage, current should be lower. However, more voltage = more speed as well which can take more current to overcome load from the additional speed.
```

---
## \#16 Posted by: deucesdown Posted at: 2017-12-29T02:18:29.214Z Reads: 63

```
I think I had a brain fail. What I was misremembering is related to temperature, not current.

http://www.electric-skateboard.builders/t/hummie-vs-devin-volts-conversion-to-amps/6910/76?u=deucesdown

@deckoz, I'm still processing your post. duty cycle refers to pwm, come on brain work!
```

---
## \#17 Posted by: Deckoz Posted at: 2017-12-29T03:26:05.025Z Reads: 59

```
Duty cycle is the percentage of work potential. Ie 50% duty cycle is 21 volts of the potential 42v of a 42v system.

The motor runs at the voltage of duty. Ie if you have telemetry and see 31% duty cycle on a 10s while your battery is at 39.83v

.31*39.83v = 12.34v is what voltage your motor is running at in that exact moment of time...

Does that make sense?
```

---
## \#18 Posted by: deucesdown Posted at: 2017-12-29T03:35:51.874Z Reads: 59

```
It makes sense, yeah, but I have to fit the PWM part into my brain for it to stick correctly. :)
```

---
## \#19 Posted by: overint Posted at: 2017-12-30T07:06:09.282Z Reads: 51

```
I have some maytech ones which are apparently bad, ended up getting focboxes instead. Would be interesting to know how the stack up.
```

---
## \#20 Posted by: marcoluz Posted at: 2017-12-30T09:55:00.934Z Reads: 46

```
Its a shame that we all spend hundreds of dollars and euros on vescs that they burn after just a few weeks of use. I don't get it. It's not supposed to be like that. They are not cheap. I don't care about the reason. I have bought only two vescs from maytech and they got down after 5 or 6 uses. And it wasnt my error believe me. They should cost 20 euros each for this sample rate of bad quality.
```

---
## \#21 Posted by: wafflejock Posted at: 2017-12-30T10:41:58.568Z Reads: 43

```
Haven't had a problem with my VESC from diy/torqueboards, granted this is my third but the first two were fried due to user (my own) errors.  That said I'm not pushing near any limits really I keep my amperage artificially limited to 30A on the battery 40A on the motor using the metr app and go lower if I'm giving the control over to someone else to try it out since no one expects the torque.  Also running BLDC mode never rolled the dice on FOC mode but on 10S and have been riding on it for over a year and again only had some fried ones early on from my own shorting things while powered in bad ways.
```

---
