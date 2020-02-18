# Mini control Mod simple

### Replies: 14 Views: 1134

## \#1 Posted by: Lambjr088 Posted at: 2017-11-10T03:33:15.160Z Reads: 193

```
Hi there as mentioned on the title I have some pics and will try to explain on how I modded my mini controller from using disposable batteries to using a single lipo rechargeable battery with a lcd voltage meter to know when to recharge the controller.
 <img src="/uploads/db1493/original/3X/5/8/584f02d366472b589678de960a37e4de7f77cc47.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/9/7/9736ced351dfb0f0a0d58cb0c61df2b61ec8c225.jpg" width="281" height="500">
These are the parts I used. But you can choose to use something different. 
https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.ca%2Fulk%2Fitm%2F232496917174
https://m.fasttech.com/p/5054400
https://hobbyking.com/en_us/turnigy-nano-tech-1000mah-1s-15c-round-cell.html

I started by opening the control and removing the tray for the AA batteries to make space. Then I soldered the battery leads from the remote to the charging board here.
<img src="/uploads/db1493/original/3X/5/d/5dbc9daa25221acf02444d53dbc4e44b4a11580b.png" width="412" height="500">
After I soldered the battery to the board here with some copper wire here.
<img src="/uploads/db1493/original/3X/6/5/655dc94444ac45ae8b26460d980859d9f8e7bf55.png" width="474" height="500">
I soldered it this way to use the undervoltage cutoff from the board.
After that I turned on the remote to check if it was working while it was on I used a voltmeter to check where the negative and positive were on the switch located on the control to solder my lcd voltage display which were these. If you want to do the same please check your control to know which is (- and +) on you remote.
<img src="/uploads/db1493/original/3X/f/d/fdcbd40d152a43ec3dbb14f19a5858559f196226.png" width="494" height="500">
<img src="/uploads/db1493/original/3X/e/9/e9a0267d3ad224b9da2f4f4dea1f86c4278807a6.jpg" width="354" height="500"> 

After I made a hole for the display and hot glued everything down. Now my display' s edges came out too much so I filed it down which now shows white edges but it didn't mess up the display. You don't have to do that I just didnt like how it felt on my hand. Also the battery I am suggesting as opposed to the one I used is smaller and would go in slanted if you purchase it becasue of the cost. Currently the one I'm using is expensive at around $23 with international shipping and the one I suggested is arpund $8 with shipping. 
This is how I put it all together. If you have any questions please feel free to ask. I will try to answer as best as I can. Also if you can't make it yourself for any reason I will try to have some made but I can't promise many at this time because of financial issues. Thanks for taking your time to read this.
```

---
## \#2 Posted by: E1Allen Posted at: 2017-11-10T03:35:45.088Z Reads: 158

```
Nice. I have a portable fan that uses one 18650. It has micro USB charging and a low battery light as well.  Nice to know it works.
```

---
## \#3 Posted by: Lambjr088 Posted at: 2017-11-10T03:38:55.051Z Reads: 155

```
Have any pics of it? Would like to see it working with a 18650. Lol
```

---
## \#4 Posted by: scepterr Posted at: 2017-11-10T03:45:41.679Z Reads: 152

```
An alternative 1S battery gauge, just need to make 4 tiny holes instead of cutting a square out, less precision though of course. 
https://www.ebay.com/ulk/itm/282225781836
```

---
## \#5 Posted by: Lambjr088 Posted at: 2017-11-10T03:59:13.917Z Reads: 137

```
That would probably be more slick only you would know it is rechargeable lol nice. I used what I already had if not I would of used that lol.
```

---
## \#6 Posted by: E1Allen Posted at: 2017-11-10T04:06:24.608Z Reads: 138

```
<img src="/uploads/db1493/original/3X/3/c/3c6fcb784e3d22ba30971b99448b755085487799.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/e/2/e255ef82bde32e8ea5533da6fcd4a730745ec93f.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/b/7/b79d379007ecd174f80cd2fa1f539f0d40dcd7c9.JPG" width="375" height="500">

Only issue is the power knob controls the fan speed. I guess you could leave it on all the way and just wire it to the switch
```

---
## \#7 Posted by: rojitor Posted at: 2017-11-10T09:33:53.505Z Reads: 115

```


----------
:heart_eyes:


----------
```

---
## \#8 Posted by: deucesdown Posted at: 2017-11-10T15:45:01.261Z Reads: 100

```
Nice job!

So the remote's running off the lipo directly, all the way up to 4.2v, no magic smoke?
```

---
## \#9 Posted by: evoheyax Posted at: 2017-11-10T15:52:22.572Z Reads: 98

```
I love this work. You have inspired me to try the same also. Going to try some other modules to monitor battery voltage. Will post pictures when I get parts and do it.

I plan on cnc milling the controller case to get the best accuracy ;)
```

---
## \#10 Posted by: LukePL Posted at: 2017-11-10T16:14:20.949Z Reads: 93

```
[quote="deucesdown, post:8, topic:37903"]
So the remote's running off the lipo directly, all the way up to 4.2v, no magic smoke?
[/quote]

That is exactly my question! Would be great if it does.
```

---
## \#11 Posted by: Lambjr088 Posted at: 2017-11-10T16:54:17.453Z Reads: 77

```
@deucesdown @LukePL no magic smoke so far but I havent had a long run with it unfortunately it is too cold out here where I live to properly test it but it shows promise on a bench test. I would doubt it would smoke up since its only 1.2 volts higher than the AA batteries plus the charging board discharges at a max of 3amps but I doubt the control uses that much or even the display. 

  @evoheyax I would love to see pics of this once your done please post them on here too.
```

---
## \#12 Posted by: deucesdown Posted at: 2017-11-10T17:08:46.508Z Reads: 82

```
Lol I've been digging at a combo charger voltage-regulator. Waste of time if mini can take 4.2v...

Maybe lifepo4 wins here with nominal 3.3v and max 3.6v, if a $1 charging board can be found.

https://www.amazon.com/LiFePO4-Rechargeable-Battery-Security-Flashlights/dp/B01N79MGKO

https://www.ebay.com/itm/5V-Micro-USB-3-6v-Charger-Module-3-2V-LiFePO4-Battery-Charging-Board/272751010538?hash=item3f813a22ea:g:JpIAAOSwknJXyt9I

hmmmmm. 14500 is exactly AA size. if the board fits in the other AA bay, this is a very simple mod.

I should hook one up to a lab psu and see what voltage makes the smoke come out...
```

---
## \#13 Posted by: Lambjr088 Posted at: 2017-11-10T22:07:35.685Z Reads: 74

```
That test would actually be a wonderful one and the results will show us all how to really go about it and know what are real safe parameters for the remote
```

---
## \#14 Posted by: skslingo21 Posted at: 2017-11-12T19:09:51.279Z Reads: 64

```
Thank you, its great to see this mod broken down in simple steps!
You've made a great controller even lighter and more intuitive.
Your a step closer to charging right from the board too! :grinning:
Thank you for testing the 4.2V as well, I couldn't step up to the plate myself. 

Where you placed the voltage monitor, I installed a large rocker switch to replace the micro on/off switch which failed after some heavy use. :relaxed:
```

---
