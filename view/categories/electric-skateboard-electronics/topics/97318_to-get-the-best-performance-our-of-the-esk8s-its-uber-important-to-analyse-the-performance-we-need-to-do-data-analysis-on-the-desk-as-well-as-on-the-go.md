# To get the best performance our of the esk8s, its uber important to analyse the performance.. We need to do data analysis on the desk as well as on the go

### Replies: 10 Views: 259

## \#1 Posted by: thurbolt Posted at: 2019-06-26T08:00:10.509Z Reads: 108

```
![datalogger|480x360](upload://mHHKZ6BFnWu9ApEKDqrqHkHe3fB.jpeg) 

Hello my friends this is Kanber, its nice to be in this forum.

To get the best performance our of the esk8s, its uber important to analyse the performance.. Battery, Motors, Drivers, Voltage, Current, Heat, Speed, vibration and more.. We need to do it on the desk as well as on the go.

I investigated the previous topics but, couldnt see a good solution. Did I miss something ??

How you guys do that ? What do you use ? What type of affordable DATA LOGGERs are on the market for this purpose ? Is it worth designing and building an affordable DATALOGGER for esk8 performance analysis ?

Very Best regards
```

---
## \#2 Posted by: meesie Posted at: 2019-06-26T11:19:03.742Z Reads: 80

```
METR modules are very good. they have a designated app for on your phone
```

---
## \#3 Posted by: thurbolt Posted at: 2019-06-27T08:31:46.519Z Reads: 67

```
Thanks @meesie yes many friends suggested that modules and the app, they are good indeed. 

But still, what I am offering is a versatile datalogger that , with apropriate sensors and connections, users can use it in anyway they like freely. Let me try to explain, the branded onboard data output can give you parameter a, b, c on platform x… I still think that the options are limited there… What I am thinking is a datalogger that you can use on platform x, y, z, t… and get parameters, a, a1, a2, b, b1, b2, c,d,e,f,g,h,j… with wider, versatile, programable options…

Another example… We always use some electronic circuits for different purposes right, on them there is an lcd showing some data values… One user can say that ok the datas I see on the lcd is enough… Another user may want to use a multimeter to see more, to check if the values on lcd are accurate… Another user may want to use oscilloscope… Another one may want to go far deeper… This is like that…
```

---
## \#4 Posted by: Acido Posted at: 2019-06-27T10:02:28.299Z Reads: 57

```
I think that you are kinda overthinking all of this...

Metr/other modules are really small and they already have logs which can be exported and analysed easily

Do you plan on like adding 20 sensors to your board or?
```

---
## \#5 Posted by: Sn4pz Posted at: 2019-06-27T11:10:24.732Z Reads: 59

```
Agreed, METR modules provide all the relevant information in a great package, and even integration with (some) other electronics. 

I don't really know how much more 'relevant information' we need other than what the METR offers, *especially* when the module provides a time stamp on all of the data, so there's no need to guess why the data / your board was behaving a certain way

That being said, the "cheap man's metr" would either be a regular hm-10 module which are literally a few dollars, or even Frank's module if you want to spend a few extra dollars on vesc integration 🤷

Having variance in the market is good, but this just seems a little redundant
```

---
## \#6 Posted by: thurbolt Posted at: 2019-07-05T06:20:56.203Z Reads: 34

```
Hello my friends @Acido @Sn4pz, thanks for the detailed replies. What you've said is true. Yet, I still believe that there will be DIY'ers who wants to see and log as many parameters as they can on the board, from any point they like, while driving or on the desk, while adding some new components and testing..  

There is a common problem with onboard systems and data monitors, they log the parameters from certain spots (test points) on the circuit. You cannot change that, you cannot get data from another point that you like on the circuit or on any other part. Another thing is that, you cannot be sure if the onboard system is correct or not, or how correct it actually is (there may be something that prevents it from functioning). If there is smt wrong right after the the onboard systems test point, or if the sensors of the onboard system malfunctions, you will see that everything is ok.. but the real situation might be different..

Your feedback is important guys, thanks again and please lets keep our contact. Iam working on a datalogger for another customer for another industry, when finished I ll bring it here and lets see if anybody in esk8 community wants to use it or not.

Kind regards
Kanber
```

---
## \#7 Posted by: meesie Posted at: 2019-07-05T10:58:29.247Z Reads: 26

```
[quote="thurbolt, post:6, topic:97318"]
desk
[/quote]

please just say board. makes it a whole lot easier
```

---
## \#8 Posted by: thurbolt Posted at: 2019-07-05T12:13:28.786Z Reads: 25

```
[quote="thurbolt, post:6, topic:97318"]
while driving or on the desk
[/quote]

I meant "while riding the electric skateboard or working on the electric skateboard while its on the desk"

![42450436-1-tf|280x280](upload://qEiuHjuBMv5mY34vfsTP9NxYNiR.jpeg)
```

---
## \#9 Posted by: Darkie02 Posted at: 2019-07-05T15:11:27.191Z Reads: 21

```
How about you tell us the advantages of what you looking to offer over what we all ready use? A dog has no idea how a car works he just gets in and know it’s walkie. The VESC all ready has all sorts of sensors and inputs we use that. no idea what more could be useful it’s a OS project and a lot of the ideas have all ready been implemented 

The only one I can think of is PPW issues. is it the signal VESC, reviver, brown out 5v power issue, Interference. Just feels you keep trying things until it’s solved it.
```

---
## \#10 Posted by: thurbolt Posted at: 2019-07-06T11:00:28.254Z Reads: 13

```
Thanks @Darkie02 , I noted the PPW issue.. Let me first develop the prototype and then we talk on the real thing. I will inform you, lets keep contact.
```

---
