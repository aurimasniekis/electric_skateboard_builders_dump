# Soldered bullet connectors on to VESC&hellip; what could possibly go wrong? :)

### Replies: 10 Views: 559

## \#1 Posted by: skelstar Posted at: 2018-12-23T17:52:28.174Z Reads: 200

```
So I was struggling to get the phase wires out of my enclosure and I saw a post _somewhere_ where someone had soldered the bullet connectors straight to the VESC phase outputs.

The 90 degree configuration would suit my enclosure "form factor" so I thought I would give it a go as well. 

![IMG_20181223_145500|666x500](upload://OtKJvCmNgGySXiUZamAW3azaXn.jpeg) 

I understand that there is a bit of mechanical strain on the soldered bullets in this arrangement so I am screwing the board down at a very similar point/plane.

![IMG_20181223_145522|666x500](upload://sA7A31wjagxSIh2e701MuvDCtlu.jpeg) 

My only real concern is the amount of heat in those FETs, but after a quick _Google_ (after I implemented the design and did a test-ride of course) it seems that the nylon washers are good to about 220 degrees C (sustained).

![image|561x500](upload://5aVFfyEKIEHGUm2xYJ3d0jZZOQJ.jpeg) 

![image|690x376](upload://fzoKbFpzlYYkN1n52bQGrhrvRPx.jpeg) 

![image|619x500](upload://idfW0iIqfYEjOgDbgBARRicke5F.jpeg) 

The reason I made this "slide in insert" was so I could remove the end enclosure (the green bit) while leaving the electronics intact. Maybe a huge waste of time, but I _love_ designing (hopefully) elegant solutions (I'm a software developer).

Any thoughts/concerns I've missed? 

Next steps (other than making the other end work the same way):
a) get some fibre/temperature-appropriate washers to replace the nylon ones.
b) secure the other end of the VESC better.

Few more pics: https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/8657?u=skelstar
```

---
## \#2 Posted by: b264 Posted at: 2018-12-23T23:15:56.488Z Reads: 140

```
This looks like it may have trouble dealing with heavy vibrations.  At a minimum I would use silicone and cable ties to make it one with that side wall -- silicone between it and the wall, then a few days later after it cures, use cable ties to torque that onto the green side. (You'd have to make a couple holes in it to feed the cable ties through)  You do NOT want those 90 degree bullet connectors flexing under vibration.

But I don't know, those are just my thoughts for what they're worth
```

---
## \#3 Posted by: skelstar Posted at: 2018-12-23T23:21:25.355Z Reads: 140

```
Fair advice.You're right. I'm keeping an eye on it. Thinking out at least packing out the big-ass capacitor end of the VESC to stop it from acting like a lever. 

Might design a cable-tie mount into to the next iteration of the green (and red) part of the enclosure.
```

---
## \#4 Posted by: skelstar Posted at: 2018-12-25T21:36:34.832Z Reads: 99

```
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/8716?u=skelstar

So FWIW I thought I would document this.

I liked the idea of the banana connectors for the phase wires to be more secure/more modular so I quickly printed this arrangement.

1. Obviously have to adjust the clearances a bit better, but that's mostly in the white part with the sockets protruding from it about 1-2mm too much (hence the gap between the white and yellow parts).
2. Not happy with the colours. Yellow was just in the printer, and the ivory-white I have surplus of. Might make the white part the same colour as the main enclosure section (darkish grey) and the phase connector will be _red_ I reckon.
3. Connection at the other end of the phase wires are going to have to be right-angled too. Not really enough room, and I'm going to swap out the trucks for Calibre IIs and a longer bracket from one of the forum members (https://www.janux-esk8.com/product-page/dual-idlers-motor-mount) which means even less room.

![IMG_20181226_094944|666x500](upload://AvpO4MSg6pDyd6oEJBIk7xDG8ze.jpeg)![IMG_20181226_102429|666x500](upload://j7vBGJLA9CxLqgtXkqMUlF7p0tJ.jpeg)![IMG_20181226_102819|666x500](upload://q6n3LU17OCEwxVF6Brv8UEgqozV.jpeg)!
```

---
## \#5 Posted by: skelstar Posted at: 2018-12-25T22:27:04.015Z Reads: 71

```
![IMG_20181226_105923|666x500](upload://yOhgzrUqyt0cnHdig0zixppiwdl.jpeg) ![IMG_20181226_112130|375x500](upload://1KtgbqxLybGmjR5N2oDldFFLgbK.jpeg) ![IMG_20181226_112527|375x500](upload://3df7GBBQeU1DDLiXBpw7j7tZj6y.jpeg)

OMG that gap in the phase connector (yellow-white connection)!
```

---
## \#6 Posted by: skatardude10 Posted at: 2018-12-25T22:58:14.781Z Reads: 62

```
It looks like you got some underextrusion and delamination there. What kind of printer do you have? Have you calibrated your e-steps?
```

---
## \#7 Posted by: skelstar Posted at: 2018-12-25T23:00:18.220Z Reads: 64

```
Heavily modified Tevo Tarantula. Despite the calibrated e-steps it will be the 0.8mm nozzle (Volcano hotend). I'm fine with it. Once I get my V6 0.4mm nozzle on there I will be redoing. Prototyping at the moment.
```

---
## \#8 Posted by: skatardude10 Posted at: 2018-12-25T23:01:54.142Z Reads: 62

```
Nice, 0.8, the layers do look thicc! I bet that prints fast, I probably should up to 0.6mm at some point.
```

---
## \#9 Posted by: skelstar Posted at: 2018-12-25T23:03:39.731Z Reads: 62

```
That green bit takes 1 hour (mental), dark gray enclosure in other photos are more like 2.5 hours. Stupid fast if you're printing 0.4mm nozzles predominantly.

_Love_ printing big/fast when prototyping. Lots to learn when going big though.
```

---
## \#10 Posted by: skelstar Posted at: 2018-12-25T23:21:19.244Z Reads: 60

```
(btw - that gap in the green part is because my chamfer is too aggressive and it's a crack. Sorted in v77 that I printed later).
```

---
