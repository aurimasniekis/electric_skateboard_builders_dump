# Trackstar 150A not calibrating

### Replies: 7 Views: 541

## \#1 Posted by: richi Posted at: 2017-10-29T08:33:02.399Z Reads: 59

```
Hello all,
great forum it has helped me alot along the way to building my Nephew a esk8, my problem is i have done all the wiring (in series ) but i cannot for the life of me get the esc to calibrate,
I'm running,
2x3s 5000 zippy's in series
a 150A turnigy trackstar
a 280kw 5055 turnigy aerodrive
a FS-GT2b controller,

when i turn this on i'm getting the solid bind but then only beeping and flashing green light from the ESC, does anyone know the problem as i really would like to get this project finished for Christmas (as it was a christmas present form last year!)
many thanks,
Rich.
```

---
## \#2 Posted by: JohnA Posted at: 2017-10-29T15:06:31.903Z Reads: 40

```
I’ve used the trackstars in a previous build, the only thing that comes to mine is to make sure that the receiver is plugged in to the signal wire and not the programming wire. And make sure it’s plugged in to the correct pins
```

---
## \#3 Posted by: richi Posted at: 2017-10-29T15:15:06.361Z Reads: 38

```
thanks for the reply, the  wiring coming off the esc to the receiver is correct, but it seems it's not reading any signal fom the controller at all, my only thought is that the controller is bad but as it's my first build i have nothing to test it againt, any ideas on how to test if the receiver is getting signals from the controller (it's definately binding but that's it!),
thanks.
```

---
## \#4 Posted by: JohnA Posted at: 2017-10-29T15:31:28.452Z Reads: 27

```
I’ve only used a GT2b and never had a problem. Maybe redo the binding process? If you have an arduino you could do a quick program to test it, or buy a cheap servo tester.
```

---
## \#5 Posted by: richi Posted at: 2017-10-29T16:13:36.925Z Reads: 24

```
Thanks John, sorted! i had the signal wire around the wrong way!! ah well learn from your mistakes and all that! thanks for your help, my next thing will to be getting a smaller controller as this fly B is massive!! any good/cheap(lol) suggestions,
Rich.
```

---
## \#6 Posted by: JohnA Posted at: 2017-10-29T16:17:02.563Z Reads: 26

```
Not a problem :), I would recomend the GT2B (not GT2E) because of its reliability. (30 bucks on amazon) And there are a lot of Case mods if you have access to a 3d printer like the  @MasterCho Case . But there are others people are happy with if you just use the search function
```

---
## \#7 Posted by: richi Posted at: 2017-10-29T17:35:00.788Z Reads: 21

```
So now to a new problem which i've just realised. in trying to get this calibrating i went back to a single battery and now i've wired it back to in series with my two in series but the trackstar 150A esc can only handle 21 volts and i have 22.6 as i'm in series what is the workaround here. is it possible to limit the volts getting to the esc? (it's already smoked maybe it's burnt up already:unamused:) 
thanks for the replies.
```

---
