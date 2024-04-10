# Passive Filters
No active components- not limited by slew rate, non linearity. Best for "roofing filters"- stops unwanted frequencies before they reach the first stage of electronics. 

# Active Filters

## Filter Characteristics
Second order bandpass responses are basically all the same. based on Q and gain. 
High pass and low pass can vary a lot- all have to compromise between a fast roll off, a flat response in the passband, and clean transient response. 
Butterworth is the most popular- very flat in the passband. 
Bessel gives a maximally linear phase response, but has a much slower roll off than the butterworth

# Sallen and Key
Pg 140 for diagram

A second order sallen and key filter is 2 stages of RC filter, passed into a follower, with the base of the first stage of RC tied to the output of the follower

Butterworth- C1= 2C2
Bessel- C1 = 1.335 C2


Cut off frequency- 1/(2 * pi * R * Sqrt(C1 * C2))

Q = 1/2 ( sqrt(C1/C2))


A high pass filter can come across difficulties in setting capacitor values. To help this, instead of using a unity gain stage follower, we add resistors to make the gain 1.586 (+4db) (gives us a Q of 0.707- critically damped) Then C1 and C2 can be the same value. 

A third order filter gives a steeper roll off. You can do this by using a simple RC first order, through a unity buffer, to a standard second order filter with a Q of 1. You can make it cheaper by stacking 3 stages of RC filter, with the second stage tied to the output of the unity gain buffer at the end of the chain. (pg 144)

Polypropylene capacitors are much more distortion free. 


## Multiple feedback bandpass filters

Figure pg 147

