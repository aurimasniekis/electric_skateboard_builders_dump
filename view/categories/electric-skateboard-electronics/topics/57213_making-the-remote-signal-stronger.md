# Making the remote signal stronger?

### Replies: 36 Views: 922

## \#1 Posted by: mxrider9239 Posted at: 2018-05-30T03:43:58.278Z Reads: 173

```
Hey guys, so far so good with my build! No complaints at all, HOWEVER, being that I live in New York and ride into the city with my board, I get a lot of interference because of everything that’s going on. So basically my question is, is there a way to increase signal strength and/or prevent signal interference?

Like I said it’s only when I’m in the city so it’s not that big of a deal because my connection is great 95% of the time. Was just curious.
```

---
## \#2 Posted by: biggdaddyhawk Posted at: 2018-05-30T04:31:49.046Z Reads: 163

```
Show us your setup. What are you working with
```

---
## \#3 Posted by: ervinelin Posted at: 2018-05-30T04:38:56.821Z Reads: 160

```
This isn't readily available for most remotes. Swapping antennas is possible in some but u risk killing your remote.

My suggestion is receiver placement. Get it as close to your remote as possible with as little things in between them as possible.

That said I had friends who had remotes which always failed at particular spots in the city.
```

---
## \#4 Posted by: Adam0311 Posted at: 2018-05-30T04:39:21.699Z Reads: 159

```
I’ve never used one, but have heard of others using a ferrite ring around the vesc to receiver wires. Supposed to do exactly what you’re looking for...filter the unwanted signals

Here is a far better explanation by @stuxtruth
 

> stuxtruthAug '16
"The ferrite ring acts as a common-mode, inductive filter of the high-frequency noise produced by the switching of the MOSFET’s inside of the ESC. Basically, it prevents the AC current fluctuations inherent in MOSFET switching from progressing beyond the ring itself (it actually looks like a big resistor to high-frequency currents and doesn’t affect DC signals at all), thus eliminating the potential for making your ESC signal wire an antenna that radiates at the frequency of the common-mode noise. It also prevents that noise from getting into your receiver or servo signal wires.

Wait a minute…that first paragraph was filled with a lot of crazy science words, so what the hell does all that mean?! You can think of your ESC as a big valve that supplies electrical current to your motor. If you want 100% throttle, then the valve stays open 100% of the time. If you only want 50% throttle, then the valve opens and closes so that 50% of the time, it’s open and the other 50% of the time it’s closed.

Just like the valve that you have on your kitchen sink, when you open and close it quickly enough, you sometimes hear a banging sound coming from the pipes in your wall. This is the “switching noise” (water hammer in the case of real plumbing) that the ESC produces when the MOSFET’s (switches…or valves in the plumbing analogy) switch on and off.

Because of how fast the switching is taking place inside the ESC, there are frequencies that can be close to that of our radio systems and this is what we want to avoid. Actually, the lower-frequency bands that were used in older radio systems were much more susceptible to this noise than our 2.4GHz systems are. That having been said, it’s not a bad idea to keep the ring in place when an ESC company provides it. It will never hurt the system, only help or do nothing…

Now, let’s say you’d like to add a ferrite ring to one of your ESC’s…this one is quite easy to do, actually. First, you’ve got to get one, right? I like to get mine at an online electronics store called DigiKey. I usually go for the EPCOS 16mm rings, as they give you enough room to fit the BEC lead through the core a few times. These things are super cheap and can be bought in bulk, if needed. If you don’t want to buy online, then you may get lucky and find something similar at your local Radio Shack or other electronics store. Once you’ve got your ring, you want to wrap your ESC’s BEC wire around it as many times as you can without putting undue stress on the wires or insulation. Usually, this is somewhere between 3-5 for the standard servo lead…make sure that you place the ring as close to where the wires exit the ESC as possible to stop the noise from getting any further than necessary. You’re all set!

Let’s take a quick look at the typical ESC manufacturers out there and how they employ ferrite rings… In the case of the Kontronik, it is still capable of noise production on the signal wire because it is not optically isolated like a lot of other high voltage ESC’s. Optical (“opto-isolated”) isolation prevents noise from being transmitted, but also prevents power from being transmitted too…thus, no “opto-isolated” ESC’s have BEC’s in them. Scorpion and Castle HV ESC’s are optically-isolated and as such either don’t come with ferrite rings (Scorpion) or, if they do (some Castles), are simply taking advantage of universal parts in their various product lines rather than having different wires for each ESC"
```

---
## \#5 Posted by: mxrider9239 Posted at: 2018-05-30T04:46:38.906Z Reads: 138

```
This will all change in the future but it’s a start and it’s doing it’s job so far.

Dual motor setup with maytech 6369 200kv motors, maytech “v” esc’s 10s5p battery with Samsung 22p cells, maytech 2.4ghz mini remote all trapped inside my little homemade enclosure (don’t mind how it looks, it’s still in progress. Just recently got latches for the cover and have an xt-90 plug holder on order)

And while I know my sheetmetal enclosure can have an effect on the remote signal, while I’m at home I can walk 15ft away and still have a good connection, in New York City I can’t be more than 3ft away.

![image|374x500](upload://yTO8tlthKx4awCXVzbpqNaeM0xf.jpeg)

![image|374x500](upload://ltQAAQfTyPxWZRumMTuUoB7HRR2.jpeg)
```

---
## \#6 Posted by: biggdaddyhawk Posted at: 2018-05-30T04:48:54.766Z Reads: 125

```
Ah it's a metal safe
```

---
## \#7 Posted by: mxrider9239 Posted at: 2018-05-30T04:50:02.149Z Reads: 120

```
Basically, but like I said I have absolutely zero problems around home, only when I’m heart of the city lol
```

---
## \#8 Posted by: mxrider9239 Posted at: 2018-05-30T04:58:15.419Z Reads: 126

```
Ok so just to make sure I’m understanding placement correctly, I’m wrapping the ferrite ring with my receiver wire as close to the esc as possible correct? 

So in reference to my setup, it’s the brown yellow and orange wire, as close as Possible to the location I’m pointing to correct?

![image|374x500](upload://j0S0AqnRXskKZXErJfWG8PZXEtS.jpeg)
```

---
## \#9 Posted by: lrdesigns Posted at: 2018-05-30T05:03:21.746Z Reads: 122

```
The receiver antenna needs to be outside the metal box for good range. No way around that. Just drill a small hole for the antenna.

What type of controller / receiver do you have?

Make a plastic lid? or  Small plastic section where the receiver is?
```

---
## \#10 Posted by: mxrider9239 Posted at: 2018-05-30T05:03:58.453Z Reads: 119

```
Yea my receiver is definitely as close to my remote as it can be, and when I go to work (in queens) there’s one spot I always get interference no matter what lol, but the city is constant and sporadic at the same time, while it doesn’t effect my safety (it’s usually when I’m trying to accelerate from a standstill or going straight in the middle of a long block) it’s just a little bit of a neusance that I’d like to prevent if possible.
```

---
## \#11 Posted by: Adam0311 Posted at: 2018-05-30T05:04:46.092Z Reads: 114

```
Yep, that is my understanding. Several guys used this trick on the first raptor deck because the carbon fiber lid was blocking the signal in urban areas. Seemed to work well.
```

---
## \#12 Posted by: mxrider9239 Posted at: 2018-05-30T05:05:41.707Z Reads: 117

```
That would be my next option if nothing else works, and I’m running a maytech mini remote which like I said in a previous comment has been great! And while I’m at home I can walk 15ft from my board and still have good connection, it’s just in the city it gets very spotty
```

---
## \#13 Posted by: mxrider9239 Posted at: 2018-05-30T05:06:26.159Z Reads: 114

```
Ok great I will definitely give that a try! And like you said it’ll either help or do nothing at all!
```

---
## \#14 Posted by: Adam0311 Posted at: 2018-05-30T05:08:25.360Z Reads: 114

```
Those were @stuxtruth words, but he’s correct (and far more knowledgeable than me).
```

---
## \#15 Posted by: mxrider9239 Posted at: 2018-05-30T05:14:45.211Z Reads: 111

```
Ahh sorry for mixing that up, I just took a look at that site you mentioned and does this look to be the correct size your talking about? I can’t find any made by epsco.

https://www.digikey.com/product-detail/en/kemet/ESD-R-28C/399-10859-ND/4290925
```

---
## \#16 Posted by: Adam0311 Posted at: 2018-05-30T05:17:23.088Z Reads: 106

```
Yeah, that should work. Just needs to fit in your enclosure and be small enough to loop the wire through it 4-5 times.
```

---
## \#17 Posted by: Wajdi Posted at: 2018-05-30T05:19:25.968Z Reads: 105

```
Seems like you are experiencing signal interference, if your remote operates on a fixed frequency like most of the available remotes do, then there is nothing you can do about it. The only remotes I’m aware of that does frequency hoping are the GT2B and the Photon remote ( I’m developing ).
```

---
## \#18 Posted by: mxrider9239 Posted at: 2018-05-30T05:24:00.190Z Reads: 99

```
Alright cool,  thanks for the input! I appreciate it!

@Wajdi so how does that work exactly? The remote automatically switches to another frequency when connection is lost? And is it that quick/seamless that you don’t even notice?
```

---
## \#19 Posted by: Wajdi Posted at: 2018-05-30T05:33:50.699Z Reads: 98

```
Basically the frequency is continuously changing at any given time from the time the remote is turned on. It is not noticeable and feels just like any fixed frequency remote. Both the remote and receiver needs to be in a preconfigured agreement to jump from one frequency to another in a synchronous manner.
```

---
## \#20 Posted by: mxrider9239 Posted at: 2018-05-30T05:41:20.538Z Reads: 96

```
Hmm sound interesting, the photon remote your working on, when will that be available?
```

---
## \#21 Posted by: Wajdi Posted at: 2018-05-30T06:29:26.323Z Reads: 86

```
It’s available on my website at eboardshop.net
Let me know if you got any questions.
```

---
## \#22 Posted by: ervinelin Posted at: 2018-05-30T06:36:03.772Z Reads: 82

```
Accelerating from standstill sounds more like a brownout than an interference issue...

I added an LC filter and large capacitor to my 5V line powering the receiver. This helped a lot for my Arduino based remotes.
```

---
## \#23 Posted by: mxrider9239 Posted at: 2018-05-30T06:39:24.709Z Reads: 79

```
I was just using that as on of the examples I’ve experience it on, I’ll come to a stop, then when I get the green light I’ll give my board a push and then accelerate, but then sometimes nothing happens at all until I move a few more feet. It’s 100% interference from everything around me, just didn’t know how to help prevent that.
```

---
## \#24 Posted by: Acido Posted at: 2018-05-30T06:49:06.681Z Reads: 75

```
Im looking to make my signal stronger also, could I just drill a small hole and make the antenna wire on the reciver longer for like 20cm and put it underneath the griptape?
```

---
## \#25 Posted by: amazingdave Posted at: 2018-05-30T07:05:13.060Z Reads: 72

```
You can’t change the length of the antenna without screwing things up... the length is based on the wavelength of the signal being transmitted/ received.
```

---
## \#26 Posted by: ervinelin Posted at: 2018-05-30T07:47:26.717Z Reads: 62

```
You can to a certain degree if the exposed element is not changed.
```

---
## \#27 Posted by: amazingdave Posted at: 2018-05-30T07:56:02.570Z Reads: 61

```
Yes.... what he said.... use coax to extend and have the actual working part of the aerial somewhere better.

You cannot however solder a wire to the end of your aerial and expect it to work.
```

---
## \#28 Posted by: Acido Posted at: 2018-05-30T08:23:28.192Z Reads: 60

```
Thanks i guess thats a no go then
```

---
## \#29 Posted by: ervinelin Posted at: 2018-05-30T08:48:22.471Z Reads: 61

```
U need to see what antenna you have to begin with. If it's already a coaxial wire soldered or attached via a uFL connector you just need to buy a longer antenna and solder or connect it back yourself.

Again you need to make sure it's the right frequency (typically 2.4ghz).
```

---
## \#30 Posted by: banjaxxed Posted at: 2018-05-30T09:11:40.497Z Reads: 55

```
The eBay escs have an external antenna port I notice, would be a good thing to implement in vesc design perhaps
```

---
## \#31 Posted by: ervinelin Posted at: 2018-05-30T09:19:48.271Z Reads: 55

```
ESCs typically don't act as receivers, not sure which each you have seen that has an antenna attached. Not even sure if that's a good idea considering you should separate the receiver from electrical noise.
```

---
## \#32 Posted by: Acido Posted at: 2018-05-30T10:18:34.196Z Reads: 54

```
Regular thin wire in the reciever and remote
```

---
## \#33 Posted by: ervinelin Posted at: 2018-05-30T11:54:29.385Z Reads: 53

```
Got pic? 10char
```

---
## \#34 Posted by: Acido Posted at: 2018-05-30T12:11:47.190Z Reads: 51

```
Regular mini remote
```

---
## \#35 Posted by: GrecoMan Posted at: 2018-05-30T12:29:19.076Z Reads: 49

```
lol you made a faraday cage

radio signals can’t get through a box of metal
```

---
## \#36 Posted by: Kug3lis Posted at: 2018-05-30T12:30:18.521Z Reads: 52

```
Faradays cage* 

https://en.wikipedia.org/wiki/Faraday_cage
```

---
