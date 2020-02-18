# Looking for Support on my First DIY Eboard Build

### Replies: 5 Views: 529

## \#1 Posted by: OrthodoxName Posted at: 2018-06-01T00:58:59.259Z Reads: 112

```
I have wanted an electric longboard for a long time and have looked into building one. I have been researching which parts to buy and I think I have found a (maybe?) final list of parts... However, having little to no experience in this exact genre of electronics. I am posting here, hoping that some great souls may be willing to glance at my list and point out an problems with my selection of parts (i.e. unnecessarily large batteries for the limit of the VESC or A better 'bang-for-your-buck option on any specific part) The end goal is to get the board working well, while spending less than $400 all together. Opinions on parts are welcome as well. 

My planned list goes as follows: 
My currently owned full setup (deck and trucks) $0
[Turnigy Aerodrive SK3 - 6364-190KV Brushless Outrunner Motor $75](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html)
[Turnigy Skateboard Conversion Kit Spare Parts - Pulley Set with Belt $25](https://hobbyking.com/en_us/gear-set-with-belt.html)
[Turnigy Skateboard Conversion Kit Spare Parts - Motor Mount $10](https://hobbyking.com/en_us/motor-mount-5.html)
[Turnigy 5000mAh 5S 25C Lipo Pack w/XT-90 2x $45 (series) ](https://hobbyking.com/en_us/turnigy-battery-5000mah-5s-25c-lipo-pack-xt-90.html)
[ TORQUE ESC BLDC ELECTRONIC SPEED CONTROLLER $100](products/torque-esc-bldc-electronic-speed-controller?variant=722351915031)
[83mm Longboard Flywheels Wheels + ABEC 7 Bearings Spacers $25](https://www.amazon.com/Longboard-Flywheels-Wheels-Bearings-Spacers/dp/B07CJW7ZYF/ref=pd_sbs_468_1?_encoding=UTF8&pd_rd_i=B07CJW7ZYF&pd_rd_r=WDPAYDXHAECFDT3P0Y1A&pd_rd_w=9IWbZ&pd_rd_wg=DgFRG&refRID=WDPAYDXHAECFDT3P0Y1A)
[XCSOURCE 2.4GHz Radio Transmitter Remote Controller + 4 Channel Splash Proof Receiver + Binding Plug for Electric Skateboard OS917 $25](https://www.amazon.com/dp/B073GX83NH?tag=mike0939-20)
A XT90 Series Connector ~$10
A balance charger ~$25
```

---
## \#2 Posted by: Slak Posted at: 2018-06-01T10:11:01.368Z Reads: 83

```
Parts seems working with each others for me. Top speed should be around 50 Km/h (check with the calculator if you didn't, I haven't)

But there is no fuse (DANGER, DANGER) and no way to start/stop your board in your list (XT90S for example). And if the phase wires coming from the motor are not long enough and/or with wrong connectors (different from the ESC ones), you would need to buy new connectors and/or cables (12AWG is fine for motor phases).
```

---
## \#3 Posted by: dg798 Posted at: 2018-06-01T13:10:52.415Z Reads: 70

```
I would go with 90mm wheels. Also u need some sort of anti spark switch for turning on/off ur board
```

---
## \#4 Posted by: OrthodoxName Posted at: 2018-06-01T18:31:35.085Z Reads: 49

```
So adding a loopkey and a 100A 50+V fuse in line before it would be a good idea? Simple as that?
```

---
## \#5 Posted by: Slak Posted at: 2018-06-01T21:40:22.834Z Reads: 43

```
No if you do that, this fuse won't protect your esc ! Check its specs : "Current: Up to 240A for a few seconds or 50A continuous"
To be useful, a fuse is supposed to protect to weakest part of your circuit. It's usually the VESC and in your precise case it is (but always check).
Take your battery, if those 25C where real, it would mean 25-5=125A continous discharge. It's not 25C, less for sure but i can't say how much.

Get a Midi 50A fuse, solder inline and insulate or get a fuse holder for quick swap. You can go a bit lower in voltage. I use 60A/32V Midi fuse for my dual focbox (batt max of 30A each). They look like this : 
https://autoelectricsupplies.co.uk/image_uploads/101505_large.jpg


Antispark loopkey (XT90S connector) or antispark powerswitch with fuse holder. I personnally prefer XT90S but get informations on all-in-one pcb (antispark vedder like) if you prefer designed/sexy "on/off" button for your board.
```

---
