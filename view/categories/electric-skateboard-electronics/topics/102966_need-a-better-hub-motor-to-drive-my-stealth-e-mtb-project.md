# Need a better hub motor to drive my stealth e-mtb project

### Replies: 3 Views: 167

## \#1 Posted by: Howiep Posted at: 2019-10-15T13:08:14.690Z Reads: 60

```
Hi guys, 

I am hoping somebody can please give me some advice on a hub motor to use for my e-mtb application. 

I’m working on a roller drive system with a single 63mm motor mounted under the cranks. The Turnigy 6354 140KV motor I’m using currently works well at speed, but quickly reaches the high-temp cut off when climbing hills. I tried integrating a heat sink to the mount but it didn’t do much at all. 

This setup is only intended to be an assist to pedalling, and as such I have limited the power to 300w. 

I know heat management is a problem for slow moving hub motors, but I expected a better result due to the low 300w power level. Though the system works well at speed, when crawling up long hills at ~10km/h the amps get up and we hit the 80°C cut-off within a few minutes. . 

![IMG_9127|666x500](upload://d0GHikLDVnFakxw9ZM5Em1viRMv.jpeg) 

![Roller-Dr-2|398x500](upload://2CaU7EWtfOxDFUvhDJFcPQl95Pz.jpeg) 

I want to be able to climb looong hills on a hot day at 10km/h (ideally less) with 300w of assist. Even dropping the KV down to ~90 I still need to pull between 30-45A for maybe half an hour or more. From what I’ve read here it seems that twin Hummie/Enertion/Meepo setups can climb hills pretty darn well. I’m hoping someone can recommend a motor that will work for me in this application - especially considering the moderate sustained current. I know some motors have less resistance/KM than others, so its not just a question of changing KV and amps to avoid heat saturation.

- I Already plan to upgrade to 10s battery, which will allow me to run a 80~100kv motor and still keep top speed around 40km/h. 
- I only have 80mm of width to play with so his may rule out some super long motors. 
- At the moment the VESC temp barely gets above ambient. Hopefully a motor that can pull higher continuous amps doesn’t shift the problem there. 
- Ideally I’d like to buy a single motor, and need to be able to remove any urethane outer to add my tyre roller. 



Current Setup: 
- Flipsky VESC 4.12 in aluminium heat sink case. Set to 300w/45A max. 
- Turnigy SK8 6354 140kv motor
- Zippy 7s lipo battery


Thanks in advance for any help. As I’ve worked through this project I’m always amazed to see so much expertise in the one place.
```

---
## \#2 Posted by: Movation Posted at: 2019-10-17T04:01:59.544Z Reads: 33

```
Powered bike hubs are so cheap now. i helped a mate build a 1200watt mtb with a 250watt police mode. The hub was relatively cheap under $600AU but for hills a befang style chain drive is much better at it uses your bikes gears. Also if you up the voltage it wont pull as much current and generate less heat.
```

---
## \#3 Posted by: Howiep Posted at: 2019-10-17T04:50:58.098Z Reads: 31

```
Thanks for your help. There are certainly some good options out there, but IMO none can achieve the low weight and handling characteristics I'm looking for - The current kit adds only 2kg of weight all included, and can be removed in about a minute. 

As you mentioned, bike hub motors struggle with hills, and also add undesirable unsprung weight. 

Mid-drive kits are also heavier and less efficient due to the gear reduction needed to match the rpm of our big dumb human legs. They are also harder on the drivetrain, need special cranks/BB/spider, and no regenerative braking, 

So I really want to pursue this roller drive system, but just need a motor that can handle the heat a bit better than my Turnigy SK8.
```

---
