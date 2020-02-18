# Setting up dual focbox

### Replies: 5 Views: 900

## \#1 Posted by: zel Posted at: 2018-03-09T18:16:27.519Z Reads: 129

```
I am trying to set up my dual focbox and the remote is only controlling 1 motor. I am not sure if I set up the cam bus connector and input the right stuff into the bldc tool.

Here is a pic of the connections
![image|281x500](upload://8D33S4NQiOR3A9HTGcGn3tnj981.jpg)


Here are pics of the master focbox software:
![image|690x388](upload://5QLy1wuR19o7OZxAUYrAzr6CbHe.png)
![image|690x388](upload://4kZWpj1DatlwgRaIaCgYsgG7m1w.png)
![image|690x388](upload://1wUpbnSyXIs2RLMs13ZE29gfJ9x.png)

Pictures of the slave focbox software:
![image|690x388](upload://m5StbhtJkziaa14uYxLPw4Prbfv.png)
![image|690x388](upload://a5FpyQGmdnvJKuz8iumlNCuUB44.png)
![image|690x388](upload://qeO9mgea59JcrinPcmrrx13eGVj.png)

Let me know if you see anything or if you need any other pictures. Thanks.
```

---
## \#2 Posted by: DavidBanner Posted at: 2018-03-09T18:17:44.504Z Reads: 121

```
you need to select can fwd
```

---
## \#3 Posted by: zel Posted at: 2018-03-09T18:18:21.516Z Reads: 121

```
on the slave or master? or both?
```

---
## \#4 Posted by: DavidBanner Posted at: 2018-03-09T18:18:50.208Z Reads: 121

```
fwd the MASTER -> SLAVE
```

---
## \#5 Posted by: zel Posted at: 2018-03-09T18:19:58.253Z Reads: 116

```
alright thanks that fixed it.
```

---
