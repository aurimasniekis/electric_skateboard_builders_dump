# How to wire voltmeter to fsesc 6.6

### Replies: 5 Views: 111

## \#1 Posted by: JoelMatousek Posted at: 2019-07-29T23:56:22.300Z Reads: 39

```
I have done some research and couldn't find anything. The only thing I have seen are people say it's not possible. I wanted to wire a voltmeter to the fsesc 6.6 so that it would turn on with the switch. I made a post here and got no answer, but for people now or in the future, this is how you do it.

It's pretty simple, solder the positive wire directly to the battery positive, then splice the ground wire on the UART port for the negative (or directly connect if nothing is already wired to it). For those who don't know, the UART port is the connector directly next to the leads that go to your motor, which is the biggest port on the vesc. The ground connector is the third pin from the motor leads.

I hope this helps someone as much as it would have helped me!
```

---
## \#2 Posted by: Blacksambo Posted at: 2019-07-30T00:00:18.008Z Reads: 38

```
got pictures please?
```

---
## \#3 Posted by: JoelMatousek Posted at: 2019-07-30T00:11:12.763Z Reads: 38

```
![20190729_201029|375x500](upload://6eFZa4HrYfBdmJpE0wRFpi4MCky.jpeg) ![20190729_200952|666x500](upload://k67sw4PAfwkzMSx55UE7s0oxL1e.jpeg)
```

---
## \#4 Posted by: JoelMatousek Posted at: 2019-07-30T00:12:07.051Z Reads: 36

```
Not the best pictures. But that first picture is the positive that goes to the voltmeter, and the second you can see the third pin from the left is the ground that I used
```

---
## \#5 Posted by: JoelMatousek Posted at: 2019-07-30T00:31:15.816Z Reads: 35

```
Let me know if you have any questions
```

---
