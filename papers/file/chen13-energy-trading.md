## [Energy Trading in the Smart Grid: From End-user's Perspective](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6810288)

### Summary

### Model
- End user
  - has battery
  - has renewable energy panel
  - can trade with the grid
- Dynamic energy price
- Model description
  - P(t): the energy price at time t
  - d(t): the energy demand of end user at time t
  - r(t): the harvested energy at time t
  - g(t): energy drawn from the grid at time t
    - d(t) = g(t) + b(t)
  - b_max: the maximum allowed amount of energy for charging the battery from the grid or discharging from the battery in one time slot
  - B(t): battery level at time t
    - B(t+1) = B(t) - b(t) + r(t)
    - constraints on b(t)
      - b(t) <= b_max
      - b(t) <= B(t)
    
### Algorithm
- does not require the knowledge of 
  - energy demands
  - electricity prices
  - renewable energy arrival process
  
