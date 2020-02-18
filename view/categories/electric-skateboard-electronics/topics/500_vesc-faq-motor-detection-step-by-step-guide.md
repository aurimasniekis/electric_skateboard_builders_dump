# VESC FAQ &#124; Motor Detection Step-by-step Guide

### Replies: 3 Views: 10325

## \#1 Posted by: onloop Posted at: 2015-11-16T23:57:07.688Z Reads: 1191

```
It is important to set correct motor-dependent parameters in the sensor(less) tab. Otherwise, the motor will run poorly or not at all.

<img src='/uploads/db1493/original/1X/aa42f2525c52a702e51e32b3bd142d5e413afc24.png'>

The important motor-dependent parameters are “Integrator limit” and “BEMF Coupling”, and they can be measured by clicking the "Start Detection" Button at the bottom left of page.

**INSTRUCTIONS**

 1. Connect the motor without any load and make sure that it can spin up freely.
 2. Make sure that no other input such as PPM is used. If it is, it will stop the motor immediately when the detection tries to start it and the detection will fail.
 3. Click the “Start detection” button. The motor should spin up, release throttle and then run slowly for a moment.
 > If the motor doesn’t spin up properly, Adjust “Current” and “Min ERPM” until it does. In general, small motors should have lower current and higher ERPM and larger motors the other way around. 
Current usually is in the range 1A to 6A and min ERPM usually is in the range 300 to 1200.
If spinning up works but running slowly afterwards doesn’t work (the motor just stutters), try increasing “Low duty” to 0.1 or so. Increasing low duty will make it easier for the motor to run slowly during the test, but the result will become less accurate.

 4. Manually put the obtained values into the boxes. I usually round “integrator limit” down to the closest multiple of 5 and “BEMF Coupling” down to the closest multiple of 50. Having them slightly lower than the detection result is good in most cases, so that’s why I round them downwards like that. Getting these parameters perfectly right is not too critical though.
 5. The next parameters to adjust are “Min ERPM” and “Min ERPM for integrator limit”.
> What they should be depends on the application and is in most cases not too important. In general lowering them will work better if the load has much inertia. I have Min ERPM around 200 and Min ERPM for integrator limit around 1000 for all my applications.
You can probably keep the same parameters I have, but if you want to tweak your startup you can experiment with them.
It is important that “Min ERPM” always is lower than “Max ERPM at full brake” and “Max ERPM at full brake in current control mode” on the “Limits” page.

 6. Commutation mode should always be “Integrate”.
 7. The other parameters are for RPM-based timing advance and some other things that aren’t necessary to adjust in the normal case, so I won’t explain them here yet.


HERE IS THE VIDEO SHOWING THE ABOVE STEPS
https://youtu.be/17CSl1iXYE8?t=7m32s
```

---
## \#3 Posted by: cnd Posted at: 2018-02-23T15:31:15.915Z Reads: 262

```
This might be a good place to tell us what ERPM means.
At a guess, I think it means "electrical", which is probably some multiplier of the physical RPM based on some characteristic of the how the motor is built (poles?).
Judging form how my motor won't work when I put RPM numbers into the ERPM box, it does seem clear that this is not an actaul RPM number at least?
```

---
## \#4 Posted by: GrecoMan Posted at: 2018-02-23T15:52:23.741Z Reads: 231

```
there are tons of forums readily available in other threads, just search.

but no, erpm =/= rpm. it means electrical rpm.
```

---
