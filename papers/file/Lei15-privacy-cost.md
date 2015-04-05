## [Cost-Effective and Privacy-Preseving Energy Management for Smart Meters](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6876215)


### Summary


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
