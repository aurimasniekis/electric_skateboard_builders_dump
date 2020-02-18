# Focbox reporting wrong voltage and BMS overcharging

### Replies: 7 Views: 103

## \#1 Posted by: AxelF Posted at: 2019-07-22T10:23:11.064Z Reads: 30

```
Hi!

I just noticed a very concerning problem with my build. I got an Enertion Focbox (4.12), 10S Lipo battery and a Bestech charge/discharge 80A BMS.

So firstly, I just unplugged my balance connector to manually check on the individual cell voltages. All are reasonably balanced (+/- 0.05V), however, they are overcharged, with the max cell at 4.39V! Im using a 42V adapter to charge. Total pack voltage was roughly 43.7V.

Then I hook the board up to VESC tool, and the ESC is reporting 39.5V? What's going on here? Any help would be deeply appreciated, I really dont want to burn my house down :sweat_smile:
```

---
## \#2 Posted by: sayekim Posted at: 2019-07-22T10:31:22.352Z Reads: 28

```
Looks like you have set the balance charger to 11s?
```

---
## \#3 Posted by: AxelF Posted at: 2019-07-22T10:33:40.965Z Reads: 28

```
Unfortunately not, the BMS is a
http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D596.html
Fixed 10S.

EDIT: Might have found the source of the overcharging, my adapter suddenly gives 46V out (while not charging). However, the BMS should still have cut off the charging...
```

---
## \#4 Posted by: sayekim Posted at: 2019-07-22T10:41:59.820Z Reads: 25

```
Still odd that the esc reports a lower voltage. Where are you reading this voltage from the esc?
```

---
## \#5 Posted by: AxelF Posted at: 2019-07-22T10:45:46.583Z Reads: 25

```
Yep, very odd. Reading from the VESC tool, but also via UART to the my DaveGA monitor.
![image|683x500](upload://eHxNc7R3Ypll1JxkC9wPWg7iGM8.png)

EDIT2: False alarm. Turns out my multimeter is broken. When having the display illumination on, the meter reads way to high! Pack voltage now reads 39.2, more reasonable! Max cell at 3.96V, min cell at 3.91V.
```

---
## \#6 Posted by: Jumpman Posted at: 2019-07-22T11:05:43.470Z Reads: 24

```
Ha,ha.  Maybe try new batteries in your multimeter.
```

---
## \#7 Posted by: AxelF Posted at: 2019-07-22T11:07:20.563Z Reads: 24

```
Will do haha! Got my heart pounding real good when I saw those measurements :sweat_smile:
```

---
