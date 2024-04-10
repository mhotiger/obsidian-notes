# Starting Simplest

2 inputs each to identical resistors connected together- averages two signals together. This can't really scale up to larger sets of inputs, and can't amplify any of the outputs. You'll always get max the highest value of the highest input. 

# Inverting amp

resistor to negative input, feedback resistor to the negative input, pos input to ground. 
I_in  = V_in/R1
No current flows in or out of the pop amp inputs. 
V_R2 = I_in
This setup is an inverting amplifier. 
V_out = -(V_in)

If we add another input resistor in parallel:
I_in1 = V_in/R1
I_in2 = V_in/R3
I_3 = Iin1 + Iin2


# Summing Mixer
Resistors in parallel feeding into the negative input of the op amp. negative feedback resistor. Positive to ground. 

# Preamp Stage
Buffer- input to negative of op amp, negative feedback without resistor, connected to inverting amplifier.
This gives us a high input impedance so we don't have to worry about it down the road. 
Then to a preamp inverting amp- input R1 1k,  R2 10k pot negative feedback, then to the summing amplifier. 