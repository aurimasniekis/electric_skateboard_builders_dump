# Board cutting out

### Replies: 2 Views: 105

## \#1 Posted by: MrDGOrman Posted at: 2019-05-22T15:59:24.218Z Reads: 48

```
Hi everyone,

So I went to use my board today and as soon as I went over something rough the board would cut out. Well, not the board itself, but the ability to go/stop wasn't possible. Here's what I've found so far:

* The FOCBOX doesn't turn off. It still has power but the green light no longer lights up. If I turn the board off and on again, it'll work fine.
* The ability to go may return, it may not.
* My Bluetooth dongle from Trampa won't allow me to connect (via Vesc Project app) after the incident unless I turn the board off, fully close the app and try again.

I connected the Bluetooth module yesterday and it asked me to do a firmware update, which I did. I updated all my settings (bat/motor max/min etc) and I'm curious if a new software version has automatically applied something that I'm not aware of which may cause the board to turn off as a precaution? Also, what buadrate should I use for the Trampa module? It's currently set to 115200.

I think it could be one of the following in its respective order:
1. A setting has changed during the update which is causing it.
2. My receiver is failing.
3. My FOCBOX is failing, AGAIN.

Thoughts would be appreciated!
```

---
## \#2 Posted by: MrDGOrman Posted at: 2019-05-22T16:37:06.429Z Reads: 38

```
So I've done some further testing and it would appear that when the NRF/Bluetooth dongle isn't connected the board rides without any problems. However, if it's connected, it cuts out. My guessing it's trying to send too much information at once?

Remote is handled through the Nano-X, RT data is with the dongle.

Is my buadrate correct or should I reduce it?
```

---
