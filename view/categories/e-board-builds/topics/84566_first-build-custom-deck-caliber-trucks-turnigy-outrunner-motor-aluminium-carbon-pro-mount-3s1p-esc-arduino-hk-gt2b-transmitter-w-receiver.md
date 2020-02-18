# First build &#124; Custom Deck &#124; Caliber Trucks &#124; Turnigy outrunner motor &#124; Aluminium Carbon PRO Mount &#124; 3S1P &#124; ESC &#124; Arduino &#124; HK-GT2B transmitter w receiver

### Replies: 2 Views: 243

## \#1 Posted by: markus22133 Posted at: 2019-02-18T17:13:54.017Z Reads: 80

```
Hello everyone! I am currently building my first DIY electric skateboard. I started by doing some research and then proceeded to order all the main parts i needed (ESC, Motor, Batteries, Receiver/controller + mount). I just got the parts but i'm a bit overwhelmed, i am uncertain on how to connect everything and unsure if i need a spark arrestor or a solid state relay. Since i don&rsquo;t know anyone who is knows about DIY build and we don&rsquo;t really have a community for it here in Sweden i would really appreciate any help at all.

Now let&rsquo;s get into details:

So, firstly, i built a longboard (my old ones were to flexible) and attached my motor to my front truck with a mount, and then the motor pulley to the wheel pulley which i ordered from eskating.eu (really recommend, super nice people with amazing customer support). Now to the electrical components:

* Motor: Turnigy Aerodrive SK3 - 6364-213KV Brushless Outrunner Motor
* Batteries: 2x ZIPPY Flightmax 5000mAh 3S1P 20C
* ESC: TrackStar 150A GenII 1/8th Scale Sensored Brushless Car ESC - (PC Programmable)
* Transmitter/Reveiver: HK-GT2B 3CH 2.4GHz Transmitter and Receiver w/Rechargable Li-ion Battery
* Arduino uno (already had one so thought i could use instead of hobbykings programmable card)

I made a diagram before on how i tought i could connect everything:

![EL-Sk8|666x500](upload://sBBMnwmCqdRkWLjIm4zvlgj5eI.jpeg) 

My first question is if i need a spark arrestor or a a fail safe more than the one on the receiver? I also wonder if my build is balanced, i know my motor and esc can handle the voltage but do i need to add resistance? Im also unsure about my receiver, in the instruction book it says i need to charge it with a special charger which was not included but it seems logical that the arduino would power it. Do i need to to be charged and if so whats the easiest charger to get?
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-02-18T18:33:51.109Z Reads: 64

```
Your wiring looks good to me, I'd recommend looking into a "loop-key", its a brake in the positive wire between the battery and ESC using an anti spark connector (usually XT90s) so the battery cannot drain when the loop is removed and will not make sparks when the battery is reconnected.

Also, your voltage is EXTREMELY low...most skateboards will use 2 to 4 times as much voltage (6s to 12s).   You're gonna have enough amps for startup and your motor is a decent one, but your top speed will be abysmal unless you have massive wheels and a high gear ratio, which is not recommended

With standard wheels and gears you're looking at 9mph top speed

http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:3,%22motor-kv%22:213,%22system-efficiency%22:85,%22motor-pulley-teeth%22:15,%22wheel-pulley-teeth%22:36,%22wheel-size%22:90}|
```

---
