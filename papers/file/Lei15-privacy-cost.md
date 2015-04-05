## [Cost-Effective and Privacy-Preseving Energy Management for Smart Meters](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6876215)


### Summary
In this paper, the authors study the battery load hiding approach and propose mechanism to tradeoff cost and privacy leakage.

### Model
- Battery Model
  - B_max: the battery capacity
  - B(t): the energy level of battery at time t
    - 0 <= B(t) <= B_max
  - P_B(t): the charging(>0)/discharging(<0) energy to/from battery during time slot t
    - P_B-min(t): the maximum discharging rate
    - P_B-max(t): the maximum charging rate
    - Thus: B(t+1) = B(t) + P_B(t)
  - C_B: operational cost of charging and discharging
- Load Model
  - L(t): the residential load generated at time slot t
  - L_max: upper bound of L(t)
  - P(t): Power drawned from the grid to serve the load
    - P(t) = L(t) + B(t)
  - P_max: upper bound of P(t)
    - P_max >= L_max
- Electricity Pricing Model
  - c(t): energy price at time t
  - c_max: upper bound of c(t)

### Objective
- Jointly optimize the cost of power and smart meter data privacy, while meeting the constraints. 
- Assumption: L(t) and c(t) are i.i.d. over slots.
  - Note that this assumption can be removed by using delayed Lyapunov drift and T slot drift techniques.
- Denote \bar(L) as the average load
  - then the objective is to minimize the variance of P(t)
  - **why**?


### TODO
- I don't understand why user privacy is modeled as the variance of P(t)
- I didn't the optimization technique they use
