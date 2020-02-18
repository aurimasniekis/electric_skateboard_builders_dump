# What is low/high speed - motor min, battery min

### Replies: 5 Views: 200

## \#1 Posted by: Sebike Posted at: 2018-10-23T22:04:30.713Z Reads: 82

```
So, rumor has it that motor min has something to do with braking at low speed, while battery min is more related to regen braking at higher speeds.. 

But what defines high and low here? Is this related to vesc settings or hardware related? Does one come into effect as the other fades out, or how does it work. 

(I've read some thread explaining the relation between batt min and motor min, but I don't think it got into how one knows when one is more in effect than the other aso)

Share your knowledge and preach, brothers and sisters!!
```

---
## \#2 Posted by: professor_shartsis Posted at: 2018-10-23T22:23:12.556Z Reads: 77

```
the same braking torque limit at different speeds will be the same motor regen current... but this same amount of motor regen current will result in less regen battery current at lower speeds and more regen battery current at higher speeds. by limiting the battery current to less than the motor current, you limit the potential amount of current that could enter your battery by limiting the braking force at higher speeds.
```

---
## \#3 Posted by: dareno Posted at: 2018-10-23T22:28:02.353Z Reads: 73

```
That is the first time I've read one of your posts sir and fully understood it.  Hallelujah!  I feel smart now.  :nerd_face:
```

---
## \#4 Posted by: dareno Posted at: 2018-10-23T22:29:34.306Z Reads: 71

```
I still read you avatar as professor sharts though.  So maybe still stupid
```

---
## \#5 Posted by: Sebike Posted at: 2018-10-23T22:30:04.337Z Reads: 68

```
and I'm surprised there were no animated charts! Thank you for explaining! I'll let that sink in.
```

---
