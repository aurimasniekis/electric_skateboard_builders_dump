# Robotics drive chassis with scooter motors

### Replies: 6 Views: 330

## \#1 Posted by: murdomeek Posted at: 2019-02-15T01:34:21.130Z Reads: 121

```
Hey guys,

I am making a robotics project for school.  The robot is suppose to go around on a farm helping out farmers with simple tasks.  I have used these 48v 500w geared hub motors (intended for escooters).  I am using 4 of these and also got their matching escooter controller from the same manufacturer: 
 https://www.alibaba.com/product-detail/High-Efficiency-24v-250w-36v-500w_60671676498.html?spm=a2700.8443308.0.0.5d3c3e5fhPVagh


HOWEVER
After hooking everything up and testing it successfully on the workbench, the robot is too heavy to start from standstill.  Right now the robot is ~250lbs, but is meant to support up to 500+lbs.  After I give it a nudge/kick, the motors can keep the robot moving.  

The school has budget for some more expensive motors + controllers.  However, all the e-scooter/ moped hub motors that I have searched up has motors intended to go up to 60kmh+.  But we only need 10km/h MAX for our application.  And since its a hub motor, we cant gear down externally.  I would also ideally like to stick with hub motors for the simplicity of installation and there's no chain/belts for rocks/dirt to interfere with.   

Without custom winding my own hub motors, what other suggestions do you guys have?  I've also looked up some ebike wheels, but the tires are too thin (even for fat tires)

Thanks in advance!
```

---
## \#2 Posted by: Benjamin899 Posted at: 2019-02-15T02:32:07.026Z Reads: 105

```
thats weird. Do these motors have sensors? And what type of battery do you use?
```

---
## \#3 Posted by: DerelictRobot Posted at: 2019-02-15T02:45:57.775Z Reads: 97

```
What kind of ESC? What are your motor/battery current settings? 

You're looking at realistically like a 300-350w effective power per motor, with those tires. it's a lot of initial current draw as those hub motors are not geared and likely underpowered for anything heavier.
```

---
## \#4 Posted by: murdomeek Posted at: 2019-02-15T03:55:51.364Z Reads: 89

```
the standard esc's for scooter/bikes: https://lunyee.en.alibaba.com/product/60823249808-806956300/ebike_36V48V_500W_800W1000W_Sine_wave_Parallel_Controller_for_double_drive_BLDC_hub_Motor.html?spm=a2700.icbuShop.41413.14.7e351b11JdrmoI

I am using lead acid 48v 18.5ah  (4x 12v in series) with a 120a fuse switch
and yes, the ESC's have sensor support.

Thats what I thought too.  But these are suppose to be for "electric scooters" which can support the weight of a person with one motor. And I have 4 motors :/
```

---
## \#5 Posted by: DerelictRobot Posted at: 2019-02-15T05:44:06.713Z Reads: 69

```
So you're encountering a few issues compounded here. While I wouldn't recommend a 500lb payload with those motors, ever, 250 should be doable under short term usage. 

An SLA battery of that size is not really well suited for this application. Generally speaking they're intended source about 2-5amp discharge. With your batteries in series you don't gain anything but voltage, which does nothing to help your batteries ability to provide enough current. You can theoretically pull about 15amp from it, but at that rate you'll get about 14Ah total capacity with the rest lost to heat. 

Your system might actually perform better in a 2S2P configuration over 4S1P if only because your issue isn't voltage, it's current, and when those motors are first spinning up they're at a very low duty cycle (voltage) anyway, so the higher top end voltage just gives you a higher top speed you'll never get to. Most of these motors will operate just fine at 40%+ duty cycle, it's getting up to that point that can be sluggish without enough amps. But, that's a bandaid fix.

Ultimately without a programmable ESC like a vesc you're somewhat blind to the settings of the motor and battery configuration. Better batteries would probably be the quickest way to fix this but that's assuming the ESCs can give enough current. 

I'd advise either more batteries in parallel or a lithium-ion pack in addition to a programmable ESC so you have some insight on what's going on there. 

To recap: I think you're limited by the current output of your battery + not being able to tune in your settings on your ESC. You need current to get those motors rolling from a dead stop, especially with those big tires. Push up the PSI as well, it'll help with roll resistance.
```

---
## \#6 Posted by: murdomeek Posted at: 2019-02-15T06:03:15.220Z Reads: 54

```
Thanks for the informative reply!
I'll look into lithium ion packs.  I was under the impression that these SLA batteries can provide more than 15 amps.

I would probably upgrade the controllers to VESC's as well to tune the settings.

I've found a website with similar motors that might be able to do some custom windings options: http://www.cnqsmotor.com/en/article_read/QSMOTOR%2010inch%20500W%20-%203000W%204000W%20205%2048V%20-%2096V%20BLDC%20direct%20drive%20electric%20wheel%20Hub%20Motor/526.html

might go with 1000w or 1500w upgrade in that case
```

---
