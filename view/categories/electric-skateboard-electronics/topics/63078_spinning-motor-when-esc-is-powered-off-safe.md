# Spinning motor when ESC is powered off safe?

### Replies: 3 Views: 185

## \#1 Posted by: chocol4te Posted at: 2018-07-27T17:19:12.550Z Reads: 70

```
I remember reading somewhere about either using the board or moving the motor when the ESC is not connected to a battery or off, but can't remember whether it was saying it is safe or unsafe to do.

Is it safe? I can see using one's board as a regular longboard could be useful at times.

I have an ESCape, if it is specific to the ESC.

Thanks!
```

---
## \#2 Posted by: AutoItKing Posted at: 2018-07-27T18:17:20.649Z Reads: 62

```
A spinning motor acts as a generator when not fed externally. You end up charging up the ESC circuit and sometimes enough to even turn it on. The Vedder firmware is pretty good at cutting off the charging but if it hasn't fully booted up yet there is a chance to blow something up. And of course as soon as it cuts off the motor it turns off again starting the cycle over. If you need to ride your board manually for any reason, disconnect the motor if it's easy, or pull the belt off (carry a skate tool with you). There is a chance you can generate enough voltage/energy to blow up your ESC, better safe than sorry.
```

---
## \#3 Posted by: chocol4te Posted at: 2018-07-27T19:35:20.154Z Reads: 49

```
Ahh, OK. Thanks! :D
```

---
