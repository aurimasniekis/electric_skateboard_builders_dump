# Downhill braking. Enertion remote vs GT2B?

### Replies: 13 Views: 1973

## \#1 Posted by: michaelcpg Posted at: 2016-05-06T02:30:01.143Z Reads: 171

```
Hey guys,

I've had my board running for a couple weeks now. Apart from the deck, the setup is essentially exactly the same as a Raptor Mono. So far the board has been excellent but I do have one issue that is fairly significant due to the fact that my daily commutes include a lot of long steep hills.

I'm currently using the Enertion remote and to be honest, the braking feels much too twitchy for my liking when riding down hills. Especially considering that I do a lot of riding on the footpath due to many of the hills being main roads into the city as well as the fact that I'm often riding during rush hour traffic.

When I say 'twitchy' I mean that quite often when I'm braking fairly heavily, loosening off on the brake only slightly will result in a complete loss of braking until I either fully take my finger off the brake and then reapply brake or otherwise push the trigger close to all the way forward so I'm essentially using max braking power.

While this is usually manageable, it's just not going to be good enough for me as a long term solution as it can make going down steep hills quite nerve wracking... I've changed some of the remote settings in the VESC (as instructed by several tutorials) and have switched the VESC to use FOC mode which has helped to some extent but not enough for it to be practical/safe enough for daily riding.

Would buying an RC remote such as the GT2B in a custom enclosure be likely to result in a much smoother braking experience? 
I'm also considering getting hall sensors to help smoothen the braking experience as well but this isn't something I've done too much research into just yet so I'm not sure exactly what sort of effect I should expect from this.

Any thoughts or other tips to improve downhill braking smoothness would be greatly appreciated :)
```

---
## \#2 Posted by: treenutter Posted at: 2016-05-06T03:14:32.968Z Reads: 161

```
@michaelcpg I'm sure you can get better performance out of the remote you've got. Lots of others here are using it without those issues. 

It sounds like maybe your ppm input limits aren't set properly. Have you used BLDC tool to set the min and max pulsewidth? You can also try adjusting some of the braking force settings. 

That said, I use a modded gt2b and it has been the best controller I've used so far. Not a single dropout, connects instantly, and responds how I expect it to every time. If you're having problems and they are related to your controller, it's worth a try.
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-05-06T03:28:49.654Z Reads: 148

```
I've set the max and min pulsewidth settings for my remote which did help to some extent. Where can I find the settings for adjusting braking force? 
As I said mentioned though, the issue is less about the actual force of the braking and more with the (not so) smooth transition between different levels of braking.

Where do people buy their modded GT2B's these days anyway?
```

---
## \#4 Posted by: treenutter Posted at: 2016-05-06T04:15:38.199Z Reads: 140

```
[quote="michaelcpg, post:3, topic:2936"]
Where do people buy their modded GT2B's these days anyway?
[/quote]

Get a Flysky gt2b from anywhere you like... Hobbyking or Amazon. Download the badwolf mod from thingyverse and print it at shapeways or another 3D printing shop. 

@FLATLINEcustoms is now making a mod (not sure if it's available yet) and  @chaka sells complete badwolf mods.
```

---
## \#5 Posted by: onloop Posted at: 2016-05-06T04:26:31.923Z Reads: 136

```
check this out

http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
```

---
## \#6 Posted by: michaelcpg Posted at: 2016-05-06T04:30:23.872Z Reads: 127

```
Thanks @onloop. I've read through this and have set the battery current settings to those recommended for the space cell but it seems more to be an issue with the sensitivity of the hand controller.

Cheers @treenutter, might have to nicely ask my mate if I can use his 3D printer :)
```

---
## \#7 Posted by: onloop Posted at: 2016-05-06T04:43:09.129Z Reads: 124

```
lower the regen current & modify the PPM settings.

You should be able to get it perfect!
```

---
## \#8 Posted by: michaelcpg Posted at: 2016-05-06T04:55:57.436Z Reads: 121

```
When you say lower the regen current are you referring to Batt min (regen)? I've currently got it set to 12A, couldn't lowering it more than that potentially damage the cells?
Any particular PPM settings I should try modifying? As I've already mentioned I've modified the min and max pulsewidth settings based on a tutorial you linked in another thread. I haven't come across any information on what effect changing the other settings have though.
```

---
## \#9 Posted by: onloop Posted at: 2016-05-06T04:58:07.929Z Reads: 117

```
bat min regen
motor min regen


these are negative values


e.g -12 change to -8


this will be weaker brakes.
```

---
## \#10 Posted by: michaelcpg Posted at: 2016-05-06T05:00:04.768Z Reads: 108

```
Ok I might try this as a temporary solution, however I was actually eventually planning on adding another 10 cells to the battery to make a 10s4p pack largely due to the fact that the braking currently isn't strong enough in some situations, so I'll probably have to look at other more permanent solutions.
```

---
## \#11 Posted by: Adam0311 Posted at: 2016-05-06T05:05:39.813Z Reads: 107

```
I ride up and down a 19% grade several times a week...with both raptor dual and mono...no issues. Min the regen like @onloop says and play with the ppm bandwidth and deadband some more, bench test while plugged into BLDC tool until you find a setting that feels progressive enough when braking.
```

---
## \#12 Posted by: Adam0311 Posted at: 2016-05-06T05:11:16.946Z Reads: 106

```
Sounds like you just need a dual. Mono set up is great, but it just doesn't have the traction or power of the dual.
```

---
## \#13 Posted by: michaelcpg Posted at: 2016-05-06T05:39:20.415Z Reads: 100

```
Yea you're right, the plan is to get another 6374 motor eventually :)
```

---
