# Simple Guide for VESC Telemetry Monitor?

### Replies: 12 Views: 1147

## \#1 Posted by: Marty Posted at: 2017-04-26T18:07:19.796Z Reads: 164

```
Would love to outfit my board with a VESC Telemetry Monitor (a small OLED Display) in the TX.
I know how it "therotecially" works but thats where it ends ;-)
The are a lot of Libraries for this kind of I know - but honestly - is somewhere a complete guide of how to do it ?
Here are also a lot of posts about the different ones - they all look nice but nowhere a description of how to do this.
I dont mind if it would be via NRF or BT.
I know its your hard own work what you did - but no one here to share their codes, schematic or am I just to stupid to find them or do this my own ? ;-)
Thanks already in advance
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-04-26T18:09:31.514Z Reads: 158

```
take a look ate vedder web site, most of the info that you're looking is probably there.

[Vedder.se](http://vedder.se/)
```

---
## \#3 Posted by: Marty Posted at: 2017-04-27T10:53:58.686Z Reads: 136

```
oh I did have a look there - but was looking for a "simple explained" solution - I am not very deep into coding etc ;-)
```

---
## \#4 Posted by: Vieo Posted at: 2017-04-27T11:15:26.840Z Reads: 128

```
You'll need to know how to code - http://vedder.se/2015/10/communicating-with-the-vesc-using-uart/

I think there some solutions people have made where a BT link to a iOS/Android app

Ardunio example: https://github.com/RollingGecko/VescUartControl
```

---
## \#5 Posted by: lox897 Posted at: 2017-04-27T12:57:59.963Z Reads: 117

```
I've got it running currently with rolling gecko's code, a 0.96" OLED, custom case, and thumb wheel. Planning to open source all my designs when I'm finished testing
```

---
## \#6 Posted by: Vieo Posted at: 2017-04-27T13:28:08.037Z Reads: 117

```
You got a picture of this?
```

---
## \#7 Posted by: lox897 Posted at: 2017-04-27T18:55:14.558Z Reads: 109

```
Here's one of it on the bread board: <img src="/uploads/db1493/original/3X/b/c/bc5c10721c0c4f56d05882cc96fc914615505f7b.PNG" width="516" height="499">

And the case I designed for it:
<img src="/uploads/db1493/original/3X/c/a/caf48eec02f4dfee1a1076fc8bc0904903adbe31.PNG" width="517" height="500">
```

---
## \#8 Posted by: evoheyax Posted at: 2017-04-27T19:00:49.920Z Reads: 100

```
I always wanted to have a display like that on my remote or board, but I found the iphone route much easier. I plan on making a holder that is attached via the truck holes so you can attach your phone to your board to see the data without having to hold it. Seems like a simpler solution then programming these displays.
```

---
## \#9 Posted by: flatsp0t Posted at: 2017-04-27T21:15:03.524Z Reads: 93

```
I am not sure if i would want my phone cms away from my feet and the groud while rideing on a vibrating and shaky board. They are kind of expensive these days.
```

---
## \#10 Posted by: Challlsss Posted at: 2017-04-27T21:49:56.507Z Reads: 90

```
Just a thought, what if you made a square hole with a router in the board, and countersink the edges. Then use Plexiglas or whatever clear material on top as a cover.... 

Then small holes along countersunk edges of deck and along edges of Plexiglas, and glue neodymium magnets into those holes and BAM! you got yourself the ultimate Iphone case in your longboard :slight_smile:
```

---
## \#11 Posted by: evoheyax Posted at: 2017-04-27T23:58:38.257Z Reads: 86

```
That's a valid concern. It would have to hold the phone very securely, which is possible. The gimbel I use for my iphone for example a great example of a holding mechanism that would be hard for a phone to come out of.

In general, your phone should have a case + screen protector that will prevent any damage in most cases anyways. Your board shouldn't be flipping over, and it's not hard to avoid stepping on it.

Again, valid concerns, but I think theres easy safe guards to prevent the worst nightmare of your phone getting damaged.
```

---
## \#12 Posted by: Marty Posted at: 2017-04-29T21:08:24.712Z Reads: 59

```
oh yes - thats exactly what I was talking about - the small OLED display in the remote - perfect !
would love to see how you made this - that is right the stuff I was looking for
great work !!
```

---
