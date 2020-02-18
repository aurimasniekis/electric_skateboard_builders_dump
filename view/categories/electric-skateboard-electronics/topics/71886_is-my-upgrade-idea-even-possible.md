# Is my upgrade idea even possible?

### Replies: 8 Views: 312

## \#1 Posted by: Dimotro Posted at: 2018-10-21T12:50:45.065Z Reads: 169

```
Good morning esk8 builders :) 

I've been having a cool idea on a upgrade for my build and have some questions if this is actually possible. 

I've got dual focboxes as vescs and noticed both vescs can output power to external devices. Now what really seemed like a cool idea is to integrate a smart speaker (Google home, alexa) in to my build and receive power from the vesc. This way I could just turn on my Hotspot on my phone and use all of the smart speaker functionality. 

However is this in any way possible? Or can't the vesc deliver sufficient power to such speaker for example? Any input is welcome! 😇

Thanks!
```

---
## \#2 Posted by: Acido Posted at: 2018-10-21T12:56:34.710Z Reads: 160

```
probably the vescs couldn't handle it
but you could put a step down converter directly on the battery and power wherever you want
```

---
## \#3 Posted by: Battosaii Posted at: 2018-10-21T12:57:09.815Z Reads: 153

```
Vesc doesn't have enough out put to power a speaker. It's ment to power small accessories like a blue tooth module.
```

---
## \#4 Posted by: Dimotro Posted at: 2018-10-21T13:17:08.280Z Reads: 133

```
Thanks for the input! That's about what I expected.

If I'd like to make this possible as an external system, what components would I need to make this work? So the speaker would have it's own separate battery source. The only nice thing to combine this is that the speaker would turn on together with my power switch. Any ideas? :)
```

---
## \#5 Posted by: totalgeek9224 Posted at: 2018-10-21T13:21:27.133Z Reads: 122

```
All you would really need is a buck converter to convert to whatever voltage you need, and then wire that after your switch so that the switch will also power the converter. 
Thats it :)
```

---
## \#6 Posted by: Andy87 Posted at: 2018-10-21T14:21:00.879Z Reads: 94

```
Idk which voltage your speakers need, but you can get something like this if it’s below 15V

https://alienpowersystem.com/shop/rc-ev-accessories/electronics/lien-hv-bec-14s-12amp-7-12-15V

Input goes to the batty direct, output you can link via your receiver of your remote and switch it on via ch3 or what ever your remote support.
```

---
## \#7 Posted by: mars Posted at: 2018-10-21T17:28:30.173Z Reads: 71

```
https://www.ebay.com/itm/Globe-Longboard-Skateboard-GSB-Pinner-Dark-Maple-w-Boombotix-Bluetooth-Speaker/391959285535?epid=7010187814&hash=item5b42980f1f:g:gVcAAOSwKOJbLBxR

On special....The board measures 9" x 41.25"
Works with any Bluetooth-enabled smart device compatible with any USB charger.
A 50mm driver and passive radiator so riders can feel bass under their feet.

All the bits you need....
```

---
## \#8 Posted by: mynamesmatt Posted at: 2018-10-21T21:18:07.194Z Reads: 47

```
https://www.ebay.com.au/itm/141871702338?ul_noapp=true
i use one of these in parallel with my vesc to charge remotes and phones etc. could also be used for a speaker idk why not?
```

---
