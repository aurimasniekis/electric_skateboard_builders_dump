# ESC Programming For Nubes. S.O.S

### Replies: 6 Views: 1011

## \#1 Posted by: GinoDePolo Posted at: 2017-04-11T07:12:03.971Z Reads: 87

```
Hey eSk8 Squad,
I am doing my first ever build and I decided to choose all the parts individually and learn the mechanics. My current issue is the programming of the ESC. I have downloaded the software and I own the right programming card but I have no idea what values to put in all the categories. So lost. My current ESC is this https://hobbyking.com/en_us/trackstar-150a-genii-1-8th-scale-sensored-brushless-car-esc-pc-programmable.html with this program card https://hobbyking.com/en_us/trackstar-multi-function-smart-program-box.html
I realize this community is in love with the VESC but I couldn't quite get the budget that high, and yeah I do realize it is very close in price at this point but I digress. I do not really understand any of the terminology behind the programming software in reference to throttle or brakes or the different percentages and I definitely do not want to damage any of my other electronic parts...
My current Electronics:
Motor - Turnigy Sk3 280kv (https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html)
Batteries (2x) - https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack.html
Tx/Rx - https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html
ESC - Trackstar 150A Car ESC
Drive Train: 
Ratio - 2:6
Wheels - 83mm

I don't know if any of that information would help but I am just really having a hard time figuring it out. Any direction you guys can send me would be greatly appreciated :)
```

---
## \#2 Posted by: laurnts Posted at: 2017-04-11T07:57:22.286Z Reads: 74

```
There are some youtube videos how to program this ESC. I personally have that ESC with the programming card as well. However I already forgot how to do that and meanwhile my programming card is broken.

The setting is not as complex as VESC. It only adjust timing, brake strength, soft start, etc. It doesn't really affect your ESC basic operation unlike VESC with motor detection.
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-04-11T08:12:06.292Z Reads: 68

```
Basically, Car ESCs are plug and play, so you won´t damage anything if you connect it and go.
There are some nice features though, like adjusting the brakes or set a cutoff voltage, therefore just follow a tutorial somewhere.
```

---
## \#4 Posted by: lowGuido Posted at: 2017-04-11T08:49:30.185Z Reads: 60

```
make life easy for yourself and buy the programming card. its only $10 and it will save you a lot of hassle.
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2017-04-11T08:50:49.806Z Reads: 59

```
[quote="GinoDePolo, post:1, topic:20777"]
Hey eSk8 Squad
[/quote]

I love it...its catching on lol
```

---
## \#6 Posted by: Maxid Posted at: 2017-04-11T08:55:26.939Z Reads: 57

```
I always hated why the manufacturers have to make it so complicated that you can't just use an Arduino.
In the end it is just a PWM signal that is trasnmitted to the ESC - any Arduino should be capable of doing the job with the right sketch. Why can't they just upload that and have people use it instead of having to buy the programming card :frowning:
```

---
