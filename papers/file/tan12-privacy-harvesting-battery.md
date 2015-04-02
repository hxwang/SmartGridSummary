## [Smart Meter Privacy in the Presence of Energy Harvesting and Storage Devices](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6486062)

### Summary
In this paper, the authors study the trade-off between energy efficiency and user privacy for homes configured with recharagle battery and energy harvester. They conclude that larger recharagle battery, energy harvesting rate can help reduce privacy leakage.

### Model
![](../figs/sm.PNG)

- X_i: the total amount of energy demand of the appliances at time i
- Y_i: the amount of energy the system request from utility provider
- Z_i: the amount of harvesting energy at time i
- b_i: the amount of energy in battery at time i


### Algorithm
- use *equivocation* to measure the uncertainty
- define information leakage rate, wasted energy rate
- They model the problem as a Finite State Machine and using markov chain theory to solve it.

### Weakness
- they seems to exhaust enumerate all possible states, which may be untractable for large settings.

### Extension
- consider dynamic energy price
