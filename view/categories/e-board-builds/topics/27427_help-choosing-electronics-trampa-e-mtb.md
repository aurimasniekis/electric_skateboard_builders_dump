# Help choosing electronics (trampa e-mtb)

### Replies: 18 Views: 1236

## \#1 Posted by: Whitehawk Posted at: 2017-07-12T08:50:52.777Z Reads: 163

```
Hi guys,

I'm going to build a trampa e-mountainboard 8inch wheels with Jens (e-toxx) direct drive transmission (1:5 reduction).
I will build the battery myself (probably 18650).

I would like at least 35 or 40km/h top speed (+22mph), and enough torque to play with the board.

If I take 6S trackstar 150A ESC (most cheapest option), i will need ~200kv motors, but maybe the top speed will be too low ..
ESC 4.12 seem's not appreciate by everyone, and VESC6 cost a lot $$$ ..

What do you think guys ? What is the best ESC/VESC for you with a reasonable price ? :roll:

Thanks a lot !!
```

---
## \#2 Posted by: Okami Posted at: 2017-07-12T09:46:44.558Z Reads: 150

```
I would consider FOCBOX (aka vesc-x) as an option. I havent seen that many emtb builds with it but im sure there should be some.. it will of course cost more but at least theres gonna be more finetuning..

Though from what ive heard if you want to feel the 'dirt bike' experience, then it is better not to choose vesc but take some of the higher output 'regular escs'

I dont have calc data at the moment, but with 200kv your speed might be very close yes, Ive calculated myself that 213kv motor would be the best for 6s and ~40kph speeds but these 213kv motors are hard to find.

--
Im running 4:33 ratio, with 9inch wheels, 192kv motor and li-ion 6s battery, I think I can get about 36kph.. havent really measured final speed, as it might depend on battery level a bit too.. but it is above 30kph for sure.

Maybe @Duffman himself can chime in, perhaps he has went through a few escs to tell you the difference on what to choose the best.

--

As final note, if you can afford not to go with cheap 6s esc, I would advise to aim for at least 8s setup, Im pretty sure the feel might be way different. Though, try to collect some more info as I have very limited experience on how other setups feel besides my own but I know I dont really have high power setup because of limited voltage / esc. 

At 21.6v (li-ion) if you push about 80A, you can get ~ 1600W of power.

With 28 / 36v This number drastically increases close to / over 2000W of power.

You might not need it for constant riding but for acceleration boosts, wheelies and what not, this power can be very useful.
```

---
## \#3 Posted by: Cobber Posted at: 2017-07-12T10:03:21.832Z Reads: 133

```
Go for power like Okami said: there is no replacement for displacement:D
```

---
## \#4 Posted by: Whitehawk Posted at: 2017-07-12T14:01:16.229Z Reads: 121

```
What feeling do you prefer, esc or vesc ?
```

---
## \#5 Posted by: trancejunkiexxl Posted at: 2017-07-12T14:40:50.784Z Reads: 119

```
hi whitehawk im really interested in this as well.. dual esc but what amps? here is one i found for you *not sure it will be suitable, just want to help any way i can to figure out what is best,

http://www.ebay.com/itm/Castle-Creations-Talon-120-HV-120A-12S-ESC-Speed-Control-550-600-700-Heli-/131587364100?epid=1933280515&hash=item1ea337d504:g:JBcAAOSw0OJXLgYE
```

---
## \#6 Posted by: Okami Posted at: 2017-07-12T14:51:10.490Z Reads: 115

```
I might soon create some sort of esc comparison

For emtb, i think these are best candidates:

MAX6 / MAX8
FVT sleeping lion 120A, 12s
Roxxy esc (check NoWind builds)

Besides that:
Vesc 4, with heatsinks or even active cooling
Vesc-x (FOCBOX)
```

---
## \#7 Posted by: Whitehawk Posted at: 2017-07-12T16:16:06.962Z Reads: 108

```
Very powerfull ! But price is very high too =D
```

---
## \#8 Posted by: trancejunkiexxl Posted at: 2017-07-12T16:19:12.208Z Reads: 107

```
ya  after having vesc cuttout and getting injured me personally i am going to be very selective.. i am unsure about reliablility that would be my first concern..
```

---
## \#9 Posted by: Whitehawk Posted at: 2017-07-12T16:20:51.420Z Reads: 106

```
Just found that : https://hobbyking.com/fr_fr/turnigy-sentilon-v4-100a-5-12s-hv-bulletproof-speed-controller-w-rpm-sensor.html

What do you think ?
```

---
## \#10 Posted by: trancejunkiexxl Posted at: 2017-07-12T16:23:15.528Z Reads: 105

```
i would wait awhile for people to chime in who have done a couple of builds, might save you some cash and time in long run.. having bought a bunch of parts i regret not waiting a bit longer
```

---
## \#11 Posted by: sMATTEr Posted at: 2017-07-13T04:23:07.891Z Reads: 99

```
I've pretty much just completed my first build. A trampa with TB 6374 motors, Max6 esc, e-toxxx Direct drive and a 8s Lipo setup. 

I would definitly not go for 6s. For me the Torque of a MTB is critical and with 6s you're not going to get it. I'm actually thinking of doing 12s with Roxxy's to get more power.

I've done 45km/h with my setup. Probably enough for most :slight_smile:<img src="/uploads/db1493/original/3X/6/b/6bd6718c01847011ca432114821062e343931625.PNG" width="281" height="500">

So, got for atleast 8s and use a quality esc.😊
```

---
## \#12 Posted by: Whitehawk Posted at: 2017-07-13T07:33:02.342Z Reads: 88

```
I've got a quotation for a couple 12S sleeping lion ESC : 210$
But they are not very know on the market so .. hard to have an idea about reliability
```

---
## \#13 Posted by: benwong Posted at: 2017-07-13T07:53:42.312Z Reads: 90

```
@Whitehawk i am using sleeping lion 12S now. So far running well. 
There is two version of firmware, one have strong torque kick in and powerfull. 
Another is smoother acceleration. It depend what terrain you go for. I am using smoother version and feel better control of the throttle compare to another one. 
Running 12S lipo 136KV motor with 14:66 ratio. Max speed i yet count and not ready for full speed yet since no confidence on this board. (new in MTB). but estimated can get 35kph
While you connect remote wire by using y splitter, remember remove one of the positive wire of remote wire. 

 <img src="/uploads/db1493/original/3X/f/e/fe597ad15dad22a635b7fcbc3a9cb9a688b1fd5f.jpg" width="690" height="460">
```

---
## \#14 Posted by: Whitehawk Posted at: 2017-07-13T08:32:53.197Z Reads: 86

```


Thanks for informations @benwong , you should have a lot of torque with 136kv motors !

I will maybe try those sleeping lion =)
```

---
## \#15 Posted by: benwong Posted at: 2017-07-13T08:38:32.638Z Reads: 83

```
yup, crazy torque, not a good thing also. every time acceleration u will jerking there like a newbie riding on Eboard. 

Try to seek for others advise before sleeiping lion, because I only playing around this ESC without compare to others.
```

---
## \#16 Posted by: Okami Posted at: 2017-07-13T11:05:43.272Z Reads: 80

```
Im wondering could u solve the problem if u had more.finetuned remote

Ive been thinking about whenever it would be possible to.modulate signal coming from remote..

It would.make life easier for.other riders too.i think

----

On a side note - thanks for explaining difference.between 2 current firmwares. This gives a, new insight about sleeping lion escs

Also - interesting to note.that 12s is indeed way too powerful, ive always thought it is a good idea to start with either 8s or 10s, i think @Nowind himself mentioned that lower voltages are smoother than 12s for example, this probably affects how sensitive the.motor is, as higher voltage can increase rpm quite rapidly, i believe.. not like 6s for example, where everything happens way slower
```

---
## \#17 Posted by: 2Old2Sk8 Posted at: 2018-09-28T14:29:44.852Z Reads: 29

```
[quote="benwong, post:13, topic:27427"]
While you connect remote wire by using y splitter, remember remove one of the positive wire of remote wire.
[/quote]

@benwong Sorry to revive this old thread.  Just wondering why you say you need to remove one of the positive wires?  I get that you only need one to power the receiver, but does it cause a problem if they are both supplying power?  Seems like it would be better to have both as you would have redundancy in case one ESC shuts down...
```

---
## \#18 Posted by: benwong Posted at: 2018-09-28T15:24:07.314Z Reads: 28

```
@2Old2Sk8 if dinnt remove one of the positive wire, it will have 2 positive (2power) to one receiver. this is told by ESC supplier. I have burn one of the ESC before he told me this.
```

---
