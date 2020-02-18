# Vesc Maximum Brake Force

### Replies: 1 Views: 157

## \#1 Posted by: Flo Posted at: 2018-08-28T19:03:30.247Z Reads: 54

```
Just a toppic to exchange about brake force experience. I am using the vesc6 with a bicycle rear hub motor. So I really want the VESC to break as strong as possible in order to prevent brake pad wear out! Up to now I always used 
setBrakeCurrent(0-100%*MaxBrakeCurrent)  
to break. Braking performance was not too good with my direct drive hub motor. Now I tried:
setRPM(0-100%*actualRPM)
I found out that braking through commanding a lower RPM is way stronger than setting the brake current. I am happy with the result but I'm wondering if that is how vesc6 is supposed to behave? Any opinions on that?
```

---
