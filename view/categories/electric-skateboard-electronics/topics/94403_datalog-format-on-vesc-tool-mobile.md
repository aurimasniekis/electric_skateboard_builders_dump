# Datalog Format on VESC Tool Mobile

### Replies: 4 Views: 146

## \#1 Posted by: bluegreen Posted at: 2019-05-20T08:24:08.663Z Reads: 54

```
The Mobile version of VESC tool has data logging (looks to be recent?).

It outputs a csv but without any headers and I wasn't able to find it documented anywhere so I looked into the source code to figure it out. For anyone else who stumbles on this problem this is the format:

|msecsSinceStartOfDay|v_in|temp_mos|temp_mos_1|temp_mos_2|temp_mos_3|temp_motor|current_motor|current_in|id|iq|rpm|duty_now|amp_hours|amp_hours_charged|watt_hours|watt_hours_charged|tachometer|tachometer_abs|position|fault_code|vesc_id|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|68209883|38.1|27.4|0|0|0|-81|0|0|0|0|0|0|0|0|0|0|0|0|235.8|0|4|




[details="The code:"]
        if (mRtLogFile.isOpen()) {
            auto t = QTime::currentTime();
            QTextStream os(&mRtLogFile);
            os << t.msecsSinceStartOfDay() << ";";
            os << v.v_in << ";";
            os << v.temp_mos << ";";
            os << v.temp_mos_1 << ";";
            os << v.temp_mos_2 << ";";
            os << v.temp_mos_3 << ";";
            os << v.temp_motor << ";";
            os << v.current_motor << ";";
            os << v.current_in << ";";
            os << v.id << ";";
            os << v.iq << ";";
            os << v.rpm << ";";
            os << v.duty_now << ";";
            os << v.amp_hours << ";";
            os << v.amp_hours_charged << ";";
            os << v.watt_hours << ";";
            os << v.watt_hours_charged << ";";
            os << v.tachometer << ";";
            os << v.tachometer_abs << ";";
            os << v.position << ";";
            os << v.fault_code << ";";
            os << v.vesc_id << ";";
            os << "\n";
            os.flush();
        }
[/details]


I'm using the flipsky nrf dongle:
https://flipsky.net/collections/accessories/products/core51822-ble4-0-bluetooth-2-4g-wireless-module-nrf51822-onboard-ws82013

I would really love to use metr but I guess that is only compatible with their dongle. Akmanaic didn't detect it either. If anyone knows how to make it work with an app that has GPS would be awesome, thanks!
```

---
## \#2 Posted by: bluegreen Posted at: 2019-05-20T22:09:17.181Z Reads: 32

```
Well I guess I know why nobody uses this or knows about it because it only works when the phone is unlocked. OKAY.
```

---
## \#3 Posted by: district9prawn Posted at: 2019-05-21T01:48:42.172Z Reads: 24

```
Thanks for posting this. I gave the datalogging a go but never got around to trying to figure out the csv.

And yes the datalogging is really new.
```

---
## \#4 Posted by: bluegreen Posted at: 2019-05-21T02:10:24.378Z Reads: 19

```
It's kind of useless while riding because the app has to be open. Could be good for diagnostics on the bench...

I hope some of the other apps will build in support for this module.
```

---
