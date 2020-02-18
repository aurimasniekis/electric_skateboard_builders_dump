# Motor goes in reverse

### Replies: 10 Views: 736

## \#1 Posted by: fuzzyspikez Posted at: 2018-03-31T20:44:13.740Z Reads: 114

```
Hey there, just finished my build and came to take it for a spin and the motor was going in reverse. Anyone know what’s wrong?
```

---
## \#2 Posted by: Colson003 Posted at: 2018-03-31T20:45:07.406Z Reads: 115

```
Are you using a VESC? If not just swap two phase wires.
```

---
## \#3 Posted by: Apolo Posted at: 2018-03-31T20:45:26.831Z Reads: 112

```
Switch any two of the 3 motor wires and run motor detection again
```

---
## \#4 Posted by: abenny Posted at: 2018-03-31T20:46:58.903Z Reads: 110

```
even if you are using a vesc..just switch the position of any 2 of the 3 phase wires
```

---
## \#5 Posted by: Colson003 Posted at: 2018-03-31T20:48:20.944Z Reads: 107

```
If using a VESC it’s just a box you tick. You can switch one wire but then you’ll need to do the motor detection again.
```

---
## \#6 Posted by: abenny Posted at: 2018-03-31T20:49:25.369Z Reads: 106

```
ah..TIL...i havent used the vesc software i still use the bldc tool
```

---
## \#7 Posted by: Colson003 Posted at: 2018-03-31T20:50:37.741Z Reads: 103

```
Now that I think about it it’s only while running FOC that you’d need to redo the motor detection.
```

---
## \#8 Posted by: ZackoryCramer Posted at: 2018-03-31T21:23:29.310Z Reads: 87

```
Is there a way to reverse the motor rotation using software?
Switching the phase wires seemed like a hastle. :peach:
```

---
## \#9 Posted by: Jammeslu Posted at: 2018-03-31T22:23:16.170Z Reads: 75

```
I know there is a box to tic on the Vesc-tool firmware. Dont think so on the BLDC tool
```

---
## \#10 Posted by: fuzzyspikez Posted at: 2018-04-01T06:57:17.341Z Reads: 56

```
Thanks, I just had the phase wires plugged in incorrectly.
```

---
