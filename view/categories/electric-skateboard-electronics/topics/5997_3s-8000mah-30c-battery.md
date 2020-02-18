# 3S 8000mah 30C battery

### Replies: 12 Views: 1197

## \#1 Posted by: anorak234 Posted at: 2016-07-12T18:53:22.930Z Reads: 152

```
I am considering a transportation build, which means small deck, small enclosure, and 1 battery if possible. I am hoping to take this to Germany (I know, German Esk8 laws, but I'm willing to take the risk) and for air travel the battery must be below 99 Wh. I found a battery with below 88.8 Wh, but it has 30C marked on it. I am not as knowledgable about the effects of Coulombs as I am when it comes to Volts or Amps. Here's the link: http://www.hobbyking.com/hobbyking/store/__16225__ZIPPY_Flightmax_8000mAh_3S1P_30C_Lipo_Pack.html 
Would 30C be doable? What would potential problems be? Any thoughts on this would be greatly appreciated
```

---
## \#2 Posted by: sl33py Posted at: 2016-07-12T19:08:56.228Z Reads: 149

```
hope this isn't too remedial.

Your C will only affect your charge rate, and discharge rate in Amps.  To determine discharge rate (or ability to discharge at a certain amperage) - take your Ah x C = amp discharge capacity.  usually they will state "constant" and "burst".

So this pack (which i have - working well after over a year), will discharge 30C (30x8Ah) 240A continuous, and 40c (40x8Ah) 320A burst.  I typically want a *minimum* of 100A continuous, as you want to only use a portion of the continuous discharge capability to extend pack life.  I've measured 45-60A peak usage on these in dual setup.

3s is not going to work well - i would at least get 6s (two of these) or get a larger 6s battery.  You would usually get batteries in teh # series you need after picking your ESC.  Most hobby ESC's max about 6s capability.  More than 6s gets expensive.  Well known options in this range are the FVT/XERUN and several others.  For more than 6s i'd recommend either DIYes options or VESC (my preferred).

HTH!
```

---
## \#3 Posted by: anorak234 Posted at: 2016-07-12T19:18:06.198Z Reads: 133

```
Thanks for the info @sl33py , it helps a lot! I'll try and find a battery for 5s or 6s thats under 100Wh if i can, do you have any recommendations?
```

---
## \#4 Posted by: sl33py Posted at: 2016-07-12T20:29:19.211Z Reads: 119

```
I'm a fan of two smaller/thinner batteries vs a single thicker one:

it's lower profile both for ground clearance, and less visible when riding (vs a big ass box below deck).

Here's an example (a poor one - my first test setup using painters tape to secure electronics) of single:
[img]https://lh3.googleusercontent.com/-DU7V3W_5PLU/Va3n4cktyqI/AAAAAAAAsp0/l3QwyIDu5XcCyJIci8dSfyNQHDsvQ1HrgCCo/s1600/2015-07-19%2B12.32.22.jpg[/img]
vs two:
[img]https://lh3.googleusercontent.com/-kPs33sPKzlw/Vb_dcirbVwI/AAAAAAAAlIA/NzRnTo6FBtoPlqxjEW9CZpgyPJLeqvd_gCCo/s1024/20150802_210037.jpg[/img]

So, if your limitation is 99Wh - your max will be two 4500mAh batteries (3s/11.1v nominal).  To determine Wh of a battery: (mAh)*(V)/1000 = (Wh) or simplified a 4500mAh battery is 4.5Ah, so (Ah)*(V)=Wh.  So dual 4.5Ah = 99.9Wh (4.5Ah * 11.1v = 49.5 x 2 = 99.9Ah).

In that case, i would get a pair of the smallest/thinnest/stealthiest 4500mAh batteries i could find.  Here are some to look at:
http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=10283 (~$30 ea x 2 = $60)
http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=63415  (~$27 x 2)
http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=17247 (~36 x 2)

or you can get a single 6s like this - just note instead of 23-30mm "thick" (C dimension), they are 44mm thick.

http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=11933 (~$60 ea)
[quote]Capacity: 4500mAh
Voltage: 6S1P / 6 Cell / 22.2V
Discharge: 25C Constant / 50C Burst
Weight: 687g (including wire, plug & case)
Dimensions: 168x49x_**44mm**_
Balance Plug: JST-XH
Discharge Plug: 4mm bullet-connector[/quote]

So while a single is enticing for simplicity - it will be nearly twice as thick.  so from the side more visible.

A super stealth setup would be a small enclosure like psychotiller makes - a single or dual batteries and ESC all enclosed.  Thinner and able to fit two 4500mAh batteries would give you low profile and 99Wh to maximize range.

I would not go below 6s.  At 99Wh you should be able to expect some decent range.

A *rough* rule of thumb (will definitely depend on your riding style, weight, and hills vs flats) is 10Wh = 1km.  So your 99Wh should get you ~10km/6mi.
```

---
## \#5 Posted by: anorak234 Posted at: 2016-07-12T20:32:13.613Z Reads: 98

```
Here we are! Two of these ought to cover it. Thanks for the help! http://www.hobbyking.com/hobbyking/store/__10283__Turnigy_4500mAh_3S_30C_Lipo_Pack.html
```

---
## \#6 Posted by: Skitzor Posted at: 2016-07-14T08:27:51.197Z Reads: 75

```
I'm trying to figure out the limitations as well,  I've found this chart from FAA. Your thoughts? 
Max 160Wh and 2 batteries means 320Wh to me but you'll have to be able to split them.
<img src="/uploads/db1493/original/2X/6/62d6f2d33d8f2ed7061f884cd76fe241ed79f1ea.PNG" width="690" height="154">
```

---
## \#7 Posted by: anorak234 Posted at: 2016-07-14T17:36:40.489Z Reads: 66

```
The thing is based on that chart you have to have airline approval to go above 1 battery and 99Wh. I doubt they'd ever accept it, probably easier to just stick with 99Wh
```

---
## \#8 Posted by: Skitzor Posted at: 2016-07-14T17:43:04.269Z Reads: 64

```
So If I made a new sticker on my space cell that's stating it's 99Wh I should be fine? Who's ever going to test that ^^
```

---
## \#9 Posted by: anorak234 Posted at: 2016-07-14T17:44:11.796Z Reads: 63

```
Yep you'd probably be fine... I don't think they have any way to test it
```

---
## \#10 Posted by: popopopop Posted at: 2016-07-14T18:59:14.230Z Reads: 62

```
Someone might look it up online real quick and double check. If it's wrong, you might be in a world of trouble depending on who's checking you.
```

---
## \#11 Posted by: anorak234 Posted at: 2016-07-14T19:00:53.569Z Reads: 60

```
Well I plan to keep it at 99Wh for travel anyways... Shouldn't be a problem if we don't lie about it
```

---
## \#12 Posted by: Blitz Posted at: 2018-01-05T15:15:47.247Z Reads: 19

```
I want to wire up 3 of them battreys in series Will the focbox handle and can i use 14awg 4mm
 (that would mean changeing the 5.5 to 4mm)
```

---
