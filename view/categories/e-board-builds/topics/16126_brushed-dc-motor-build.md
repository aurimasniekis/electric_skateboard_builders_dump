# Brushed DC Motor build

### Replies: 3 Views: 2252

## \#1 Posted by: Toastertato Posted at: 2017-01-15T07:50:44.774Z Reads: 122

```
I'm thinking of starting my first E-Board build this summer, and want to see what your suggestions would be if I used a brushed DC motor to power my board instead.

I know, brushed motors have much lower efficiency, are heavier, and generally worse off for such applications. But recently, I got this motor from my school's robotics club. They were organizing for FRC and found a few "bad" motors that supposedly doesn't work anymore, so they let me keep it. It turns out the only problem with it was a loose connector, so it works perfectly fine now. Using this motor would save me $50 for a 320kv motor I was planning to buy.

Here is the motor: http://www.robotshop.com/en/banebots-first-cim-motor.html

I didn't think a brushed motor would work until I saw this video: https://www.youtube.com/watch?v=fbG35z_UZa0 

He used a brushed DC motor controlled by a MOSFET and an Arduino, which would save me another $100 for the VESC. His board seems pretty weak compared to the many other examples I've seen, but I think the size and power of my motor might be strong enough to work decently well.

Few problems I can see right off the bat is how I should power this motor. The typical 6s setup would probably be too much for the 12V motor to handle, so I'm thinking the slight over-volt of a 4s would work better  (Too much over-voltage might cause the motor to overheat too much). But if I do decide to upgrade to a BLDC, it would mean making an 8s battery system with the batteries I have which will make charging with the IMAX B6 a lot more complicated I assume. 

Another problem is the speed at which my board will be able to go at. If I use a 2:1 ratio with 83mm wheels at 60% efficiency ( http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":4,"motor-kv":442,"system-efficiency":60,"motor-pulley-teeth":15,"wheel-pulley-teeth":30,"wheel-size":83}| ), the theoretical top speed is 31 mph with a weighted down speed of about 19 mph. I heard that brushed motors have more torque than brushless, so a 2:1 ratio should still give it a reasonable amount of torque. It seems like my speed is slower than many of the other boards seen on this forum, so would this be a reasonable speed?

Also, I'm planning on making the board with a skateboard deck with longboard trucks on the ends (Apparently called a "schlongboard" ¯\_(ツ)_/¯). Would there be any issues I should watch out for by doing this?

I've never built anything of this sort before so suggestions and advices appreciated. Thanks!
```

---
## \#2 Posted by: wmj259 Posted at: 2017-01-15T19:01:27.058Z Reads: 73

```
I don't think the issue would be with a 6S as the VESC can control how much AMP/VOLT to send to the motor. But since you probably wont be using that, then you need to figure out a way to limit the voltage from a Arduino, you could use a Arduino Motorshield.
Please correct me if I am wrong, as the last time I used a Arduino was about 3 years ago.
```

---
## \#3 Posted by: Toastertato Posted at: 2017-01-15T19:46:43.269Z Reads: 63

```
I indeed do have to control the voltage that gets sent to the motor, which is where the MOSFET comes in. This MOSFET --> http://www.ebay.com/itm/5-PCS-5X-IRF3205-IR-MOSFET-N-CHANNEL-55V-110A-TO-220-USA-SHIP-/221970238492?hash=item33ae750c1c:g:gu0AAOSw5IJWcRY1 <-- can handle up to 110A supposedly. 

A motor shield most definitely would not be able to work in this application as it already heats up a lot at 2-3A, much less the 70A that the motor would draw at a normal load.

With just a MOSFET, I wouldn't be able to reverse (I don't think that matters much), but should I use a 6s battery and just limit the voltage that goes into my motor at full power?
```

---
