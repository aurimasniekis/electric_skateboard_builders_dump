# Making simple wireless switch and brake light

### Replies: 7 Views: 716

## \#1 Posted by: LunarKim Posted at: 2018-03-22T04:50:47.765Z Reads: 145

```
My friend asked me if I could make a simple radio control device.

The preparations are mechanical switches and RC mini servos.

He wanted to control the 12V LED with this switch.

I simply fixed it to tell you how.

![20180322_081940|666x500](upload://4AeD9LwDTxBwY2MSG6X8QUxbJir.jpg)

He wanted to control only the LEDs, but I also connected the brake lights to the 2CH to test.

https://youtu.be/0kGwF8F1auk

If the servo arm is short, the controller may fire at the same time as it moves to the brake state.
It would be nice to connect the control module to the 12V LED.
```

---
## \#2 Posted by: MysticalDork Posted at: 2018-03-22T04:53:34.406Z Reads: 134

```
You could do that.... Or you could get one of these modules, and not have to worry about mechanical failure. https://www.pololu.com/product/2803
```

---
## \#3 Posted by: LunarKim Posted at: 2018-03-22T04:54:33.332Z Reads: 128

```
https://youtu.be/0kGwF8F1auk
```

---
## \#4 Posted by: MysticalDork Posted at: 2018-03-22T05:08:26.590Z Reads: 121

```
For my board I went a step further and used an attiny85 microcontroller to translate from an RC channel to a LED driver, that way I could have running lights and tail lights using the same LED, just different PWM levels.

I also used a spare channel for high beams and low beams on a headlight.

 I can give you the program if you're interested.
```

---
## \#5 Posted by: LunarKim Posted at: 2018-03-22T07:14:49.738Z Reads: 110

```
Good idea.
```

---
## \#6 Posted by: Bobby Posted at: 2018-04-19T04:19:29.746Z Reads: 65

```
Im interested please send so i can study and hopefully implement on my board
```

---
## \#7 Posted by: Scoo_B_SK8 Posted at: 2018-04-19T06:47:42.344Z Reads: 56

```
Nick Poole wrote a nice simple code...
https://www.sparkfun.com/tutorials/348
```

---
