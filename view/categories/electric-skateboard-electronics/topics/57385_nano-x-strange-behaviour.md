# Nano-X Strange behaviour

### Replies: 9 Views: 305

## \#1 Posted by: Kug3lis Posted at: 2018-05-31T18:56:28.421Z Reads: 93

```
Hey, guys I was riding at street then this started to happen at around 30mph... It feels like @Ackmaniac firmware protection kicks in after I apply brake like it looses signal or etc it doesn't even start move until I again apply full power...

Freaking scary shit, had to take UBER back home...

https://youtu.be/8dfoQfOvm7Q
```

---
## \#2 Posted by: Battosaii Posted at: 2018-05-31T18:59:04.933Z Reads: 92

```
That's weird, sometimes my Nano x dosnt bind correctly and it acts funny try rebinding it by jumping the pins on the reciever.
```

---
## \#3 Posted by: mmaner Posted at: 2018-05-31T19:12:04.397Z Reads: 80

```
Also you have to calibrate the remote every time you turn it on. As soon as you hit the power switch on the remote just run the throttle to the top and then the bottom and let it go back to the middle.
```

---
## \#4 Posted by: Kug3lis Posted at: 2018-05-31T19:14:21.146Z Reads: 80

```
I know, but this what happens when normally riding...
```

---
## \#5 Posted by: mmaner Posted at: 2018-05-31T19:33:53.297Z Reads: 74

```
Right, but if you don't calibrate it will accelerate and/or brake unpredictably. That may not be your issue, just wanted to tell you about it in case.
```

---
## \#6 Posted by: Kug3lis Posted at: 2018-05-31T19:57:10.331Z Reads: 67

```
Okay I had biggest wtf of the year today... I don't know how that stop still spinning was related to this but I found that one motor phase bullet was disconnected, because I saw error in faults saying over current then in real time I saw motor pulling 40A in air... So went to check bullets and then I saw what was and that wheel spins when I apply throttle I was like this:

https://media.giphy.com/media/lT4sgCJwC7B4c/giphy.gif
https://media.giphy.com/media/Ni4cpi0uUkd6U/giphy.gif
https://media.giphy.com/media/l3q2SaisWTeZnV9wk/giphy.gif
https://media.giphy.com/media/DowKEtWnLZcru/giphy.gif

So apparently VESC can spin motor with 2 phases I guess by seeing hall sensor data? Because I have no fucking idea how it was happening... And I am scared to try it again :D
```

---
## \#7 Posted by: barajabali Posted at: 2018-05-31T20:31:11.794Z Reads: 58

```
So non nano-x related then
```

---
## \#8 Posted by: JonathanLau1983 Posted at: 2018-05-31T20:39:34.754Z Reads: 54

```
The break was where the Focboxes motor phase wires meet the motor phase wires?
```

---
## \#9 Posted by: Kug3lis Posted at: 2018-05-31T23:32:11.539Z Reads: 42

```
bullet connector got disconnected... Yeah it's not nanox problem, but I thought it was, and now I think I know why it was behaving like that the master vesc which had this problem triggered overcurrent and I guess sent same message to slave that's why it was acting like that...
```

---
