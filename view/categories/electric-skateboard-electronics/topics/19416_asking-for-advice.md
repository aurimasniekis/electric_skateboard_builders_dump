# Asking for advice

### Replies: 18 Views: 1481

## \#1 Posted by: OfficialRD Posted at: 2017-03-21T12:02:42.202Z Reads: 136

```
Been busy this whole weekend to read up on builds, set-ups and whats minimally necessary to get your board of the ground.

So the concoction i came up with:
Battery: 8000mah 22V 15C - (maybe buying two in parallel)
Motor: Turnigy Aerodrive SK3 - 6364-245kv
Wheels: 80mm (orangatang)
Board: 34" longboard (already have that)
Pinion: 15 
Spur: 34 or 36
ESC: [https://hobbyking.com/en_us/hobbywing-platinum-100a-v3-brushless-esc-w-10a-bec.html]
TX/RX: still undecided (tips are welcome!)

Just been wondering if this ESC is enough, because i have seen a lot of builds with 120A ESC.
```

---
## \#2 Posted by: Nowind Posted at: 2017-03-21T13:11:24.906Z Reads: 121

```
Hey.
If you wanna go with 6S i would advice to use a Hobbywing Quicrun ESC ... 150A, waterproof, good brakes, easy to setup with progbox...

Cheers
```

---
## \#3 Posted by: OfficialRD Posted at: 2017-03-21T13:27:00.428Z Reads: 111

```

Hey,@Nowind
Thanks for replying, but isnt the 150A a little to much if my max i can pull is only 120A in my setup? Also the VESC i have been seeying are 50A continuous. (dont know if i can compare a VESC with an ESC based on continuous Amp)
```

---
## \#4 Posted by: Bazingazunga Posted at: 2017-03-21T15:01:59.906Z Reads: 93

```
Perhaps, but too much is better than too little as you deffo know you aren't gonna fry it! Better to be safe than sorry 

Also id prob recommend 83mm -wheels  it'll just be easier to source them and a smoother ride.

Not sure if 15c might be a little low? Batteries aren't my forte i must admit.
```

---
## \#5 Posted by: OfficialRD Posted at: 2017-03-21T18:03:37.103Z Reads: 83

```
Hey, 
Thanks for your insight, but correct me if im wrong. For a DIY esk8 you need to know what your preferences are and what your surrounding factors are. Mine where pretty simple, wanted to go from A to B with a top speed of 35kmh. Live in a very flat piece of the world with super smooth roads. Not wanting to recharge the battery everyday so a reach of about 15km would be nice. 

After that i filled in the calculator what i needed so came up with the 245kv motor. Also a 8A 22V battery would give a about an hour at top speed with loaded weight and effienciency of 80%. Now to regulate that, i needed an ESC that would fit my motor that has an max output of 70A. And thats why i decided to go with a 100A ESC. Always heard get an ESC a little above your max output of the motor. 

On another note, my initial way of choosing my ESC were based of on the max output of my battery. In my case 8000*15 would be 120A. And then choosing the ESC. But my initial thoughts on this were pretty off (if im not mistaken). 

And the 83mm wheels here are way more expensive :( than the 80mm (can get a pair of 80mm for 50€)
```

---
## \#6 Posted by: NickTheDude Posted at: 2017-03-21T18:21:22.776Z Reads: 70

```
I would seriously recommend getting a VESC. The customization makes it worth it 100% and their not actually that much more expensive, especially on a single motor build. However the amp limit is much lower so in order to compensate I would increase voltage to 10S to achieve a similar power output. A 10S 5Ah pack would have slightly more range than the 6S 8Ah as well. Also, since the VESC has an ERPM limit (search the forums if you don't know about it) you should use a lower kV motor. Something around 190kV is perfect.

Also the ESC you posted is designed for helicopters so it wouldn't have adequate brakes. If you're dead set on using 6S then either this https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html or this https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-150a.html would be much better.

Also if your looking for a cheap tx/rx go for a GT2B. Their pretty common and are supposed to be very reliable. If you have access to a 3D printer you can print a new case for it to make it smaller if you want as well.
```

---
## \#7 Posted by: Nowind Posted at: 2017-03-21T19:00:44.272Z Reads: 70

```
There is no "too much" ...
i just suggest this because it is prooved in at least 10-20 E-MTB builds i know from and if it hold up in MTB it will last for sure in Street board...

They are more 6S ones which will work, but i personally trust most in Hobbywing.

Cheap and reliable... good for a budget build like yours too (-;

Hang Loose
Jenso
```

---
## \#8 Posted by: OfficialRD Posted at: 2017-03-21T20:24:36.360Z Reads: 63

```
As a developer, having the option of customization makes me very happy. Only prob is the VESC are not that readily availbe in the Netherlands. Ill try and google it, hopefully ill find such a gem for a decent price ;). 

What have you done to me, been learning a lot about the ERPM, from there i went on the frequency and followed up on the turns and poles in a motor. Quite the eye opener. Thanks! Just a little calculation to see if i understand ERPM: voltage*kv rating*pole pairs 
--> 37*190*7=49210 compaired to
--> 22.2*245*7=38073 ERPM 

So the VESC just limits the voltage or does it limit the frequency?

Aah didnt know you could calculated duration of a battery by Watts, yeah i would get a slightly higher range but wouldnt that mean, if i were to take a 190kV, the ratio of my pullies have to be adjusted to get the same topspeed? Oh wait thats where the ERPM limiter comes in to play. 

And lastly, found the TX/RX you were talking about. Was also thinking about using the ardiuno i have lying around. 

Tl:dr: figured some shit out, had some moments of clarity, still a little bit unsure if i got it all correct but will follow up on your advice (a little bit).
```

---
## \#9 Posted by: OfficialRD Posted at: 2017-03-21T20:32:41.580Z Reads: 53

```
I totally take your word for it! Also you will need way more torque on those builds. 

And you got me, going for a budget board :P thats why i choose (relatively) the cheapest battery for my buck 

u2
```

---
## \#10 Posted by: NickTheDude Posted at: 2017-03-21T20:38:32.142Z Reads: 52

```
Yep that math is right, the VESC doesn't actually limit your ERPM (unless you program it to), but Vedder (the guy that designed it) wrote in a blog post that heat starts to build up quickly if you exceed 60k ERPM. So it's important to pick a kV and voltage combo that doesn't exceed 60K.

If it did exceed 60K, for example 245kV and 10S, you would need to program the VESC to limit the ERPM to 60K to make sure it doesn't overheat.

Also, I've heard that BLDC motors are most efficient in higher RPMs, so limiting your ERPM is essentially limiting the motors efficiency.

And yeah you'd have to adjust your gearing a little, 15/36 would be about right for 35km/h.
```

---
## \#11 Posted by: OfficialRD Posted at: 2017-03-21T20:58:44.588Z Reads: 43

```
Yeah, i read up on that to. So to its better to go higher on the Volts than on the Amps to get the desired duration/reach. But that means you have to spend a little more on (V)ESC and battery. (there goes my budget build)

About that sweet spot for effeciency. Is there a way to calculate that theoretically? And or is it already been done, cant find stats for that online other than Vedders.

Thanks for replying
```

---
## \#12 Posted by: NickTheDude Posted at: 2017-03-21T21:13:47.084Z Reads: 41

```
No idea how to calculate it, there have been a few threads about it but most of it is just speculation I believe :(
```

---
## \#13 Posted by: Bazingazunga Posted at: 2017-03-22T12:00:04.060Z Reads: 34

```
Yeah thats what i was trying to say when i said better too have too big than too little - if you had some water to put in a bucket, would you rather guess how much is there and get a bucket just big enough, or have a big one guaranteed to not be too small!
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-03-22T12:10:03.912Z Reads: 37

```
Some infos about motor and battery efficiency, maybe there are some things that´ll help you out ;)

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#15 Posted by: OfficialRD Posted at: 2017-03-22T20:53:52.005Z Reads: 31

```
Yeah already read that one, im thinking i almost read every thread in here :speak_no_evil:
```

---
## \#16 Posted by: slugit Posted at: 2017-03-23T00:53:21.267Z Reads: 29

```
Hi there... 1st post, so ill do my best...
Im retrofitting a chinese mountainboard as one of the controllers failed...
I have 2 vedder 4.12 vesc, intending to connect via cannbus...
Now for the problem..!
I had them wired for power, but not interconnected, had them (loosely, yes i know, stupid) assembled in the case in a sort of square, L to reverse L format,caps at 90deg...
Connected the power, all good....
Then i went to plug in the usb...
There was a tiny little spark as one of the capacitor legs touched one of the last 2 pins of the 'P1' connector either pin 'MP' or '5v' (cant quite read all the letters/positioning..)
The LED went out, no comms over USB...
Can anyone tell me what ive probably killed, and what i need to replace..?
```

---
## \#17 Posted by: mmaner Posted at: 2017-03-23T01:26:46.966Z Reads: 25

```
Pics would go a long way twords definitely g what help you need.
```

---
## \#18 Posted by: saul Posted at: 2017-03-23T12:58:11.180Z Reads: 18

```
[quote="OfficialRD, post:15, topic:19416"]
Yeah already read that one, im thinking i almost read every thread in here :speak_no_evil:
[/quote]

I doubt that there are tons... lol
but from you parts I can tell you're trying to built to a budget, thinking you can upgrade later.
in the end it cost much more and you end up with redundant and useless parts...

get a vesc, at least 8s battery. and you have a really nice board that can can still be customized.
it will cost around $500 in parts but perform like $1000 complete.
```

---
