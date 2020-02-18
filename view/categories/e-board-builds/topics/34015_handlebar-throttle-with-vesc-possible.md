# Handlebar throttle with vesc, possible?

### Replies: 2 Views: 615

## \#1 Posted by: flywithgriff Posted at: 2017-09-26T18:35:54.037Z Reads: 89

```
I am moving along with planning my electric mtb to scooter conversion. I would like to have a handle bar mounted throttle and still use the regen brakes as well. Any ideas how to do this with the vesc?
```

---
## \#2 Posted by: Martinsp Posted at: 2017-09-26T19:06:06.337Z Reads: 78

```
You could hack something like this servo tester together with an ebike throttle (they use hall sensors and magnets which would be harder to adapt i think) and use the potentiometer as a throttle with direct input to the VESC.

https://www.ebay.com/p/ESC-Ek2-0907-Updated-Servo-Tester-Server-Tech-Electronic-Speed-Controller/1086082019?iid=132116782422

EDIT: forgot to mention this. The tester gives the VESC the same input as regular receiver (PPM) so you can use all its features. You would somehow have to figure out how to make it so that the throttle returns/springs back to neutral position when released.
```

---
