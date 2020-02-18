# Accurate speed tracking?

### Replies: 5 Views: 1366

## \#1 Posted by: Spek Posted at: 2016-10-02T17:52:49.846Z Reads: 130

```
I'm looking for a better way to view and track speed. My gps cuts out constantly using strava and other android apps. It often records a ride as a strait line point a to be, or 5 strait lines. So speed data is totally wrong. My road bike has Garmin Bluetooth magnetic sensors that are very accurate but pretty big for a skate wheel. Could the Vesc provide a speedo via Bluetooth using rpm and wheel circumference?
```

---
## \#2 Posted by: lox897 Posted at: 2016-10-02T21:56:58.919Z Reads: 133

```
Speedometer apps are quite accurate for real time data. If you want tracking throughout your ride, Strava and Map my ride is accurate for me. RPM could be turned into speed, don't know how that is done though.
```

---
## \#3 Posted by: Jinra Posted at: 2016-10-02T22:03:46.255Z Reads: 131

```
erpm divided by pole pairs (usually 7) = rpm

rpm * 60 = revolutions per hour

rph * 3.14159 (pi) * wheel diameter = mm/hour

mmph/gearing reduction (e.g. 2.4 for 2.4:1 reduction) = true mmph

then just convert mm to miles or kilometers in Google

This is pretty much how esk8 calculators like toddys and @makevoid work
```

---
## \#4 Posted by: Jinra Posted at: 2016-10-02T22:05:37.055Z Reads: 126

```
You can get one of these for iPhone app tracking

http://www.electric-skateboard.builders/t/introducing-rocket-boards-vesc-bluetooth-modules-for-sale/10422/30
```

---
## \#5 Posted by: Spek Posted at: 2016-10-02T22:54:44.052Z Reads: 98

```
It's usually pretty good except for my commute. I get a strait line from door to door. I I ride elsewhere strava works well.
```

---
