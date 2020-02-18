# Help! issues with 6374 motor on foc(updated with video and pictures)

### Replies: 7 Views: 285

## \#1 Posted by: Guacamoleface Posted at: 2019-03-21T18:43:45.891Z Reads: 99

```
I have issues setting up my focbox(one of them), it will fail if I run the default parameters but If I change the first parameter (I:) that is default to 5 and I increase that to 10+ it will run the detection and get valid values.

However when I get to the next part after that - running sensor detection for hall sensors - it will now say "Bad FOC Hall Detection Result Received" - I tried going changing the prior values during foc detection to 15A on "I:" parameter but not much else. 

Don't dare to try anything else but decided it was better the hear here on the forum before I risk destroying something.

I checked hall sensor cables and also I use an adapter to make it fit to Foxbox connector and its an adapter from skating.eu. But as far as I saw it was in the correct order. Will supply pictures down below to show. 
Also my setup is dual focbox - 6374 Torqueboards motor, 10s4p 30Q, Not connected by can. And bluetooth Metr module. 

PS. The color swap from adapter to Focbox so don't get confused and use the adapter image as reference to what color goes to what.

@torqueboards tagging you here because here are some pictures you asked for in support :)  

https://youtu.be/9jXwbZwsu_w

![IMG_2796|375x500](upload://a9GzcqUn890LdmkUeRAaqPyVHRo.jpeg) ![IMG_2797|375x500](upload://uFEnuZvbgikDL7kNB2RLflEQOx7.jpeg) ![IMG_2802|666x500](upload://5oxNppNXszdoZPhgIyzSEC72QAo.jpeg) ![IMG_2803|375x500](upload://l2Q0gc9Ek7ZBOE9Af4sg0ScrIF1.jpeg) ![IMG_2812|375x500](upload://wlJOus8YvhPdYe5yRlhtUMD6DgG.jpeg) ![IMG_2813|375x500](upload://iH0kfwB3ZlH08uQBc4qxMTNqHCM.jpeg)![IMG_2847|666x500](upload://dp37GIJM5lg8r1xbgaaIf64EQeV.jpeg) ![IMG_2852|666x500](upload://gGVQXFIlc8IDG04Tr8D1spnzmtN.jpeg) ![IMG_2855|666x500](upload://kr7riwiZatNkrBv97ZCf5Adnmyf.jpeg)
```

---
## \#2 Posted by: Guacamoleface Posted at: 2019-03-22T18:14:34.414Z Reads: 67

```
Worth to mention I tried my other motor which went through fine, even swapped focboxes and issues still there on the problematic motor and no issues on other.
```

---
## \#3 Posted by: Eboosted Posted at: 2019-03-22T23:59:35.614Z Reads: 57

```
Then you need to change the motor, or if you can change the sensors and sensor wiring loom.
```

---
## \#4 Posted by: Guacamoleface Posted at: 2019-03-23T12:11:22.293Z Reads: 42

```
Thanks for reply @Eboosted . It has troubles in sensorless aswell. It requires 10-15a in parameters to just spin to do motor detection. I checked solder joints, and motor is barely used. Its magnets came lovar after just a couple km then it was idle for a while and got replacement magnets from @torqueboards and they are replaced and works fine but since then its had this issue aswell
```

---
## \#5 Posted by: torqueboards Posted at: 2019-03-23T14:08:31.932Z Reads: 33

```
@Guacamoleface I'll PM you
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2019-03-23T14:14:10.513Z Reads: 33

```
@Guacamoleface have you try to mesure it 2 time in a row? If it doesn’t work firt time try it again without changing anything.


Are those the default setting (current and voltage) ?
```

---
## \#7 Posted by: Guacamoleface Posted at: 2019-03-24T17:39:04.106Z Reads: 23

```
Yeah I tried a couple Times. 
Default for the motor detection yeah
```

---
