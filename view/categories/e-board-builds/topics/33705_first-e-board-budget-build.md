# First e-board budget build

### Replies: 11 Views: 936

## \#1 Posted by: Nicoalix Posted at: 2017-09-22T10:44:08.010Z Reads: 129

```
Hi everyone!
First, for me it is hard to write English so I will use google translator, sorry errors.
My first idea was to make a mountain board, or al terrain board, but I understand that this should be a dual engine, and the budget increases considerably, practically double, so for now I discard this idea, and I have decided to make a single engine longboard for quiet ride, and maybe in the future, I can use these components to mount a mountain board partially.

These are the components that I have thought so far, I would appreciate any suggestions and warnings, since I am surely making some mistakes in the choices.

**-Motor  PROPDRIVE v2 5060 270KV - 45€**	
https://hobbyking.com/en_us/propdrive-v2-5060-270kv-brushless-outrunner-motor.html

**-90mm wheels	 - 29€**
https://www.amazon.com/dp/B012WNIU8G?m=A2DQMI7AS28KLN&ref_=v_sp_detail_page

**-Kit pulley, belt and motor mount  - 22€**
https://www.amazon.es/Electric-Skateboard-Longboard-Cintur%C3%B3n-Herramientas/dp/B073GWX3HK/ref=sr_1_1?ie=UTF8&qid=1506023151&sr=8-1&keywords=longboard%2Bdiy&th=1

**-Remote control and receptor - 22€**
https://www.amazon.es/Electric-Skateboard-Longboard-Cintur%C3%B3n-Herramientas/dp/B073GX83NH/ref=sr_1_1?ie=UTF8&qid=1506023151&sr=8-1&keywords=longboard%2Bdiy&th=1

**-VESC**
Thinking on diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
but I'm not sure if it's the best option, in this section I especially need suggestions.

**-Batteries**
I think 6s can be a good starting point, according to some calculations that I could do in ESK8 Calc, could get a top speed of 33.2 km / h.
Maybe 10s is a better option for the future? I hear suggestions here.
<img src="/uploads/db1493/original/3X/1/8/186ff8300fa6cd5f18939efe980d46a9acbdf8e1.jpg" width="667" height="500">

As you can see, in the electronic part is where I have more doubts and I need your experienced opinion.

**This is my current board**
https://www.hammondboards.com/longboard-hammond-ding-dong.html

**Thank you so much everyone!**
```

---
## \#2 Posted by: darkkevind Posted at: 2017-09-22T10:50:44.217Z Reads: 114

```
I wouldn't got with such a high KV for a small 50mm motor.

This would be better as it's lower KV:
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5065-236kv-brushless-outrunner-motor.html

Hoever this will probably be best:
https://www.banggood.com/Racerstar-5065-BR5065-140KV-6-12S-Brushless-Motor-With-Gear-For-Scooter-p-1110304.html

Also, be prepared to drill into your trucks to keep that motor mount stationary....
```

---
## \#3 Posted by: Nicoalix Posted at: 2017-09-22T10:53:59.668Z Reads: 112

```
Maybe a larger engine for single engine is more suitable? there is no problem in raising the budget for motor in 20-30 €
```

---
## \#4 Posted by: darkkevind Posted at: 2017-09-22T10:56:05.682Z Reads: 109

```
I'd go for the SK3 6364

This:
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html

Or this:
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html

That being said, I have the SK3 5065 236kv on a single drive build and it's ample for me...
```

---
## \#5 Posted by: Nicoalix Posted at: 2017-09-22T11:00:26.759Z Reads: 103

```
At first sk3 245kv was my first choice, then in this video I saw that the performance is quite similar, and given the budget, it seems that the NTM is winning
https://www.youtube.com/watch?v=ioFqJPht2kM
Maybe should not match the conclusions in a single engine configuration?
```

---
## \#6 Posted by: darkkevind Posted at: 2017-09-22T11:05:07.304Z Reads: 99

```
Those are smaller can motors and as you say, it's a dual drive so they're working together...
```

---
## \#7 Posted by: pat.speed Posted at: 2017-09-22T11:54:36.195Z Reads: 89

```
Do not buy that pulley kit, I bought a very similar one and have had nothing but trouble with it. Make sure you get HTD5 pulleys and belts
```

---
## \#8 Posted by: Nicoalix Posted at: 2017-09-22T12:15:37.022Z Reads: 86

```
Thanks, i keep the info.
They look good quality and the price is right.
Any place where you can buy only the mount at a viable price?
```

---
## \#9 Posted by: pat.speed Posted at: 2017-09-22T12:55:38.773Z Reads: 79

```
eBay, I have the mount and it works great after I changed the grub screws for m6 bolts and drill slots in the truck for the bolts
```

---
## \#10 Posted by: NickTheDude Posted at: 2017-09-22T14:02:03.309Z Reads: 72

```
Not sure how much of a budget you're on, but these general consensus on the best setup is 10S 170-230kV and a VESC. After that you can tune how much power you're looking for using amp limits on the VESC.
```

---
## \#11 Posted by: Nicoalix Posted at: 2017-09-22T21:00:19.838Z Reads: 64

```
What is the typical configuration for getting 10s? 5 x 2s?
It seems that the configurations with 3s, are more economical, with the same type of battery:
10s = 2s x 5 und = 78 €
12s = 3s x 4 und = 79 €
```

---
