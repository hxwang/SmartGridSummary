## [Cost-Effective and Privacy-Preseving Energy Management for Smart Meters](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6876215)


### Summary


### Model
- Battery
  - B_max: the battery capacity
  - B(t): the energy level of battery at time t
    - 0 <= B(t) <= B_max
  - P_B(t): the charging(>0)/discharging(<0) energy to/from battery during time slot t
    - P_B-min(t): the maximum discharging rate
    - P_B-max(t): the maximum charging rate
    - Thus: B(t+1) = B(t) + P_B(t)
  - C_B: operational cost of charging and discharging
