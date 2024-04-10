Likely going to skim a little bit on this one

# Conductors
They aren't ideal. Copper is great, and that's why it's used everywhere. On pcbs it's really thin, and if you're dealing with a large load on a pcb, it's probably better to solder a wire on instead of relying on the pcb trace, or trying to use heavyweight copper on your pcb (it's expensive)
Pcb traces that are on interior layers need to be about 3 times as thick for the same current load as one on the surface since it has less opportunity to cool off. 

# Pcb Track to track crosstalk
Long parallel traces talk to each other- like a lot. You can mitigate it with a ground plane on either side of traces that need to have signal and be parallel. You should avoid having two different channels go through the same chip op amp- even if it's a dual channel and the crosstalk is supposed to be low, because of all the surrounding circuitry. 