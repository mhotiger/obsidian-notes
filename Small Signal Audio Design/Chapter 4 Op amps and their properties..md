Generally the most used op amps are the tl072 and 5532. (I bought a load of 5532 sweet)

# Properties
### Noise
Refer to the table on page 96 for a ranking of op amps and noise. There are two main styles based on the input type- BJT or JFET. Usually Jfets have more voltage noise and less current noise, and vice versa for the BJTs

### Slew Rate
Measures the rate at which the op amp output can change. Higher means faster, and therefore more accurate. After about 3 V/uS, the amp is fast wnough to keep up with the entire audio band, and much past this doesn't really help us any since we're only concerned about 20-20. 


### Input Offset Voltage
In the ideal, if the two opamp inputs are shorted, the output is zero. In reality it takes some voltage for them to operate, and so there's a small dc offset in that case. It can be enough to worry about, and should be dealt with. Details in chapter 11. 

### Bias Current
BJT input op amps have higher noise current and also bias current. When bias currents flow through varable resistors they make them noisy when moved. They can also cause significant DC offsets with high resistances. To compensate for this, we add a resistor the same value as the feedback resistor to the non inverting input. This also generates some Johnson noise, so to get rid of it we'll shunt it with a parallel capacitor. Diagram page 99. 


### Distortion
Distortion can be caused by a few things. Internal distortion is just related to the op amp itself and its construction. Not a lot to do about that. Slew limiting is related to the output swing rate of the op amp. We should be able ot design around this one. It shouldn't happen as long as we choose a component with a high enough slew rate to avoid it in the situation we designed for, with some extra margin for the clipping region. 
We've got some grace here, because for normal levels, we only need 2.3V/uS to get a full output 20k signal, but in practice, we wouldn't ever really see a FULL level 20k signal. There's almost always more energy in the bass frequencies than there is in the very high audio frequency band. Loading causes distortion, and varies chip to chip. The lowest load an op amp can drive is a compromise between number of op amps, cost, etc. As the load goes lower, so does the noise floor becuase we can choose lower resistor values for the feedback network, driving johnson noise down.  
