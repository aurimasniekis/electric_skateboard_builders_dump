# Speed to RPM finder

### Replies: 7 Views: 1070

## \#1 Posted by: scottkellum Posted at: 2016-09-24T16:12:31.573Z Reads: 109

```
https://scottkellum.github.io/Esk8-RPM-finder/

I just made a little tool to help find speed limits and translate them to RPM This should be useful if you want to limit the top speed of your board through the VESC. Hopefully my math is correct, it’s open source so feel free to contribute.
```

---
## \#2 Posted by: XIII Posted at: 2016-09-24T16:41:25.521Z Reads: 100

```
you need to multiply this rpm with 7 (pole pairs) to get your erpm. That is the value you can use in the vesc to limit your topspeed.
```

---
## \#3 Posted by: scottkellum Posted at: 2016-09-24T18:34:34.362Z Reads: 90

```
Thanks! I'll add that input when I get to a computer.
```

---
## \#4 Posted by: scottkellum Posted at: 2016-09-24T22:32:29.232Z Reads: 72

```
updated to calculate ERPM
```

---
## \#5 Posted by: treenutter Posted at: 2016-09-26T13:34:44.130Z Reads: 56

```
This is great @scottkellum! It might be useful to add a description of what gear ratio means for the tool. (the ratio is usually expressed as x:1 . I assume that x is the value that we plug in here.
```

---
## \#6 Posted by: scottkellum Posted at: 2016-09-26T13:59:37.084Z Reads: 51

```
Thanks! yup, I’ll try to clear that up a bit later.
```

---
## \#7 Posted by: mmaner Posted at: 2017-01-11T20:22:43.812Z Reads: 37

```
Such a great tool, I dont know how I missed that until now :).  Good job m8.
```

---
