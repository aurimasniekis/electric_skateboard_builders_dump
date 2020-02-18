# Detail Explanation of Motor Electrical Specs

### Replies: 1 Views: 1074

## \#1 Posted by: rbstv Posted at: 2016-10-01T12:06:58.252Z Reads: 123

```
Hi newbie here, 
I have some background in electrical stuff, but I don't specialize in power applications. I haven't actually built a board yet, but planning to start and experiment.

I'm trying to run some numbers for the electronics, motor speed, efficiency and such, and have a few questions regarding the motor model. I'll post what I know, please correct me if there are inaccuracies stated, and feel free to contribute, I would be very interested in hearing about the true performance specs of motors you guys have on hand for comparison purposes.

From what I understand KV is the no-load rpm per volt applied. For brushless motors though, the controller and the commutation method adds a layer of complexity.

I plan to use FOC anyway so let's assume perfect sine wave output, which will drive it like a 3-phase AC motor with a biased neutral voltage. Speed is a function of frequency but let's assume the FOC perfectly matches output frequency to instantaneous rpm via detected back EMF. Effectively torque is induced until magnitude of back EMF at some max rpm reaches the voltage applied.

When KV is defined for brushless motors, which applied voltage is referring to?  Is it the 3-phase line-to-line Voltage or the per phase voltage? Since its a wave, is the voltage measured in RMS voltage, amplitude voltage, or peak to peak voltage?

I think normally people use the RMS Line to Line Voltage since it's most easily measured with a multimeter. If that's the case, let's assume a battery pack of Vbat. Looking through ESC circuits, each phase has 2 power transistors that connects to Vbat and ground, generating any voltage in-between via PWM. The voltage amplitude of the biggest sin wave per phase would then be Vbat/2, the Vrms per phase would be sqrt(2) factor less so Vbat/(2sqrt2), and line to line Vrms would be Vbat*sqrt3/(2sqrt2). So if we had a battery voltage of Vbat, max line to line Vrms applied to motors is around 0.61*Vbat. Which is the value that should be multiplied by KV. This is contrary to how other examples of max no-load speed is calculated on this forum where people multiply Vbat directly with KV. What am I misunderstanding in these calculations?

Also when DIY people measure KV of their motors, is it generally just let it freespin and measure the rpm divided by applied voltage? Or extrapolate back to ideal point by compensating for voltage drop across internal resistance using the small no-load current? Or maybe just ballpark the number via the number of windings?

The internal resistance of the motor is a critical parameter that I don't see mentioned here much for some reason. For the most part everyone is using copper coils so I don't expect a huge variation for similar motor designs, but it is easily measured and useful know. Particularly for determining battery configuration, as it would be ideal to match the voltage and current output capability of the battery to the ratio fixed by the internal resistance of the motor. For example at a fixed voltage, the motor resistance determines the max current draw(at stall), so I can buy a certain C rating battery accordingly. I think the standard measurement is line to line resistance, which is twice the per phase resistance in wye-configuration. 

The power rating of a motor should be determined by thermal limitations so it's not as much of a hard electrical constraint, generally keep it not so hot such that magnets lose their field, windings burn, polyurethane melts, etc. The weakest link should fail at some temperature( anyone have a figure for this breakdown temperature in general?). Measuring continuous power rating isn't hard, just fix a room temperature, spin the motor under constant load, vary the load until the equilibrium temperature settles comfortably below the maximum, and measure the constant power draw, which is also translatable to current draw via P=I^2R. I guess active and passive cooling mechanisms also affect things.

I heard that the ballpark estimate is every 10Wh is will take you around 1km. If traveling at 30km/h constantly, 1 km would take 1/30 hrs. So on average 300W constant power rating is the bottom line (total motors combined). Personally I would be comfortable with maybe power rating of twice that.

Efficiency:
For a given motor, constant electrical power = constant current = constant torque. Larger current = Larger torque.
Mechanical power output is torque*rpm. So efficiency depends on how fast a motor is spinning. 
Specifically electrical efficiency is (instantaneous rpm/max rpm). Hence stall = 0% efficiency and all heat, while max rpm is the most electrically efficient with all output mechanical power used to overcome friction to maintain speed.

The most efficient acceleration curve should be slow and smooth. This is because the max rpm is determined by voltage applied to motor, which is controlled by the ESC as a moving target to adjust current rpm. The larger the difference between current speed and target speed, the less the efficiency, but it also causes more current draw and hence more torque to compensate.    

While riding, the main source of mechanical load is climbing hills and wind drag. There is also the force required to accelerate a mass, but lets assume steady state constant velocity to avoid differential equations. Climbing hill is inefficient because rpm is low causing low efficiency while drawing high power to sustain torque. Cruising fast is inefficient because wind drag is a function of velocity squared, so the power dissipated to drag is proportional to square of speed. 

To design for the most efficient power flow. The the easiest way is to gear down and lower rpm, which will increase electrical efficiency, give more torque for hill climbing, and reduce wind drag losses since max speed is reduced. But going slow is lame.

The other way is to make a more efficient motor. Derivations aside, the ratio of electrical loss to mechanical output is approximately proportional to: motor resistance*KV^2.

The lower this value more efficient the motor. Reducing resistance requires thicker coils, reducing KV requires more windings, so the trade off for efficiency is size and weight. The trend is bigger motors are generally more efficient and run cooler.  

The max speed can be increased by increasing KV, with the trade off being efficiency. The other method to increase speed is to increase applied voltage, which does not affect the electrical loss ratio. Ideally it is more efficient to get top speed using higher voltage while using as low of a gear as possible(low KV). However, if you go too high in voltage, the switching loss from the power mosfets come to dominate(this is because the large drain terminals have substantial capacitance, and energy stored in capacitor is 1/2CV^2). I recall 60Vish was a good sweet spot which is why VESC have that cap.

Personally, top speed of around 35km/h is fine.
The most convenient battery pack to build is 12s, so around 50Vish max, 44.4V nominal.
I'm thinking dual hub motors, so KV selection is constrained. For a standard 83mm dia wheel, 80-90KV rpm/(line-to-line Vrms) would land me in my speed target using FOC.
The resistance of this one chinese hub motors I've seen states 0.7ohms, nobody else seems to put internal resistance as spec. Equivalently (max power/ max current ^2) would derive a similar value. Anyway, the lower the more efficient but also means larger max torque and higher C rating battery requirements.
Heat dissipation / continuous power draw rated for 300W each motor is good enough for me, I'm pretty light anyway, but definitely higher the better.
```

---
