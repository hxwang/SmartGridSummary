## [Minimizing Private data disclosures in the smart grid](http://dl.acm.org/citation.cfm?id=2382242)

### Summary

### Model
- observed load change: e'(t)
- real load change: d'(t)
- Objective: to provent leaking of information in the demand load change 
  - One approach is to maintain the observed load as a constant, however, this approach will require a very large battery.

### Algorithm-Stepping Framework (SF)
- Objective: maximize the difference between the demand load and external load
- **Lazy-Stepping**
  - try to maintain the external load unchanged as long as possible

```python
t = 0
b = min(b_charge, b_discharge) # the maximum bettary power
e = [] # meter read
d = [] # demand
h = [] # coefficeny e[t] = h[t] * b
s = [] # charing signal 0 = discharge, 1 = charge

def lazy_steping(d):
  
```

- **Lazy-Charging**
  - try to keep charging the battery until the battery is full and then keep discharging the battery until it is empty
- **Random-Charging**
  - randomly choose whether to charge or discharge the battery

### Limitation of Existing Approach
- Best Effort (BE)
  - when charging or discarging will exceed the battery capacities
  - when even use the maximum charging/discharging rate, it may still fail to maintain a static load 
  
### TODO
- check how they compare the algorithms
