# I need new parts for a setup I screwed up

### Replies: 3 Views: 340

## \#1 Posted by: Vivalize Posted at: 2017-10-17T17:56:38.273Z Reads: 60

```
Hey there, new builder here. A while ago I bought the parts for my first electric board utilizing:

2x5s lipos in series
https://hobbyking.com/en_us/turnigy-5000mah-5s-20c-lipo-pack.html

And a 260kV motor
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html

After burning through two cheap ESCs, I decided to take the plunge and get a VESC (an Enertion Focbox). After a lot of struggling, I was told that my motor was too high kV for my batteries when using the Focbox. So, two main questions:

1. What part would be easiest to replace to get this setup working? Could I replace the motor with a 190kV such as this one? http://www.michobby.com/product/maytech-6355-190kv-brushless-outrunner-motor-for-electric-skateboardse-bike/

2. I was also told by Enertion support that I would need to halve the max battery amperage parameter when configuring my vesc because I have two batteries in series (I would have to bring it down from 60A to 30A --- 60A being the max current of the Focbox). Is this true? My understanding was that the vesc+motor should pull 60A irrelevant of what the battery configuration is (and that those batteries should support that discharge rate).

Thanks for the help
```

---
## \#2 Posted by: Jinra Posted at: 2017-10-17T18:26:01.668Z Reads: 47

```
[quote="Vivalize, post:1, topic:35790"]
What part would be easiest to replace to get this setup working? Could I replace the motor with a 190kV such as this one? http://www.michobby.com/product/maytech-6355-190kv-brushless-outrunner-motor-for-electric-skateboardse-bike/
[/quote]

For that price you might as well get a tried and true motor from DIYES, APS, Ollin, or another SK3. For a single drive I recommend a 6374 motor instead.

[quote="Vivalize, post:1, topic:35790"]
I was also told by Enertion support that I would need to halve the max battery amperage parameter when configuring my vesc because I have two batteries in series (I would have to bring it down from 60A to 30A --- 60A being the max current of the Focbox). Is this true? My understanding was that the vesc+motor should pull 60A irrelevant of what the battery configuration is (and that those batteries should support that discharge rate).
[/quote]

No you only have to halve currents for dual VESC setups.
```

---
## \#3 Posted by: cwazy1 Posted at: 2017-10-17T18:52:05.450Z Reads: 37

```
If you only want a single motor, then go with a 6374. (also if you're 200+ pounds go with this)

collections/electric-skateboard-starter-collection/products/electric-skateboard-motor-6374-190kv-3150w

If you want to potentially go dual and not upgrade trucks, then stick with a 6355. 

collections/electric-skateboard-starter-collection/products/electric-skateboard-motor-6355-190kv
```

---
