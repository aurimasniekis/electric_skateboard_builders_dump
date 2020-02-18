# Vesc, Arduino and Uart

### Replies: 6 Views: 1464

## \#1 Posted by: Agira Posted at: 2017-10-03T18:14:20.109Z Reads: 163

```
Hi, 

I finally decided to finish building my elongobard after too much time. At the moment i'm using a custom remote and recevier, basically two Arduino connected via Bluetooth. While waiting for my focbox to arrive, I'm trying to finalize the program, and now the troubles begin.
Three questions:

1. I've opted to use the uart through this library (https://github.com/RollingGecko/VescUartControl) and was thinking to use the nuchuck function controll the vesc. Does the nunchuck app to be activate or is the uart enough?

2. In the bdlc_tool code I found this command COMM_SET_RPM, from the coding seems to call the PID function and I suppose works like a cruise control.
Haven't found any sort of documentation/comment about. Is there any around about the various commands?

3. There is various firmware available, is there any better than the others?

Sorry if they are trivial questions, but no vesc yet so no testing.
Thanks a lot and sorry for my sketchy english. :)
```

---
## \#2 Posted by: niktwo17 Posted at: 2017-10-03T21:17:24.921Z Reads: 150

```
Hi,

you dont need to activate nunchuck mode. uart is enough.
by setting rpm you make your vesc achieve a specific speed while setcurrent controls the power of your board. are you talking about vesc firmware versions? basically you always want to use the newest one. however i dont know wether you can use rollinggeckos code with the new vesctool.
and one last thing, please use nrf24l01s for your remote. way more reliable than bluetooth.
```

---
## \#3 Posted by: Agira Posted at: 2017-10-04T07:42:34.507Z Reads: 129

```
[quote="niktwo17, post:2, topic:34689"]
you talking about vesc firmware versions? basically you always want to use the newest one
[/quote]

I mean different branches, the extended bdlc-tools version, the default one that come with the focbox (I read somewhere that comes with a modified version?), and the last vesc-tools one.
Does the new versions usually implement features of popular but older firmware?

[quote="niktwo17, post:2, topic:34689"]
please use nrf24l01s for your remote. way more reliable than bluetooth.
[/quote]

At the beginning that was the plan, but had a lot of problem with that chip. Way more than Bluetooth.  Way more. 
Probably had the clone version, need to find a good supplier. If I can, will take your advise. :)
```

---
## \#4 Posted by: florr Posted at: 2017-10-04T13:10:33.505Z Reads: 105

```
Hey!

two weeks ago, I've also build my first electric longboard - and I've also used an Arduino / uart communication to control my board.
The (newest?) HW 4.12 is arleady supported - you just need to select the VESC6 branch from RollingGecko. (I lost several hours until I noticed that..)
Something I've noticed when I was using the nrf24: the ack payload size is too large to transmit it. I've added a smaller struct - and now it's working pretty nice!
```

---
## \#5 Posted by: Agira Posted at: 2017-10-05T12:03:43.771Z Reads: 88

```
Thanks man! I was using the master branch, you saved me a lot of time for sure :grin:

I'd already disabled the ack payload, and they was working reasonably well at home. When I tested them in the basement (it's two floor under the ground so basically no external 2.4 GHz communication) the modules were losing connection in mere two meter. There was no explanation, maybe the radio wave bounce on the concrete wall and creating super strong interference?? No idea.
After that I throw them away and worked with Bluetooth, it turned out well for now. I will try again with the nrf24l01 when I could find genuine ones.
```

---
## \#6 Posted by: Pedrodemio Posted at: 2017-10-05T12:11:41.901Z Reads: 82

```
You don't need to use this function to use cruise control, if you use COMM_SET_CHUCK_VALUES ( I think it's that, long time since I looked) you can use a button that behaves like the C button on the nunchuck that enable cruise control

A word of advice from a bad experience, caution with it, if you use an nunchuck modeded as remote, the C and Z button can get stuck, leaving you with no immediate brakes, my board has few scratches because of that, since that I disabled cruise control
```

---
