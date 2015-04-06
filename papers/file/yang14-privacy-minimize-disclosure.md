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
C = [] # current battery capacity

def update_battery():
  e[t] = h[t] * b
  b_t = e[t] - d[t]
  C[t] = C[t-1] + b_t

def lazy_steping(type):
  
  # battery change
  b_t = e[t-1] - d[t] 
  
  if C[t-1] + b_t  > CH:
    # battery is full
    h[t] = h[t-1] - 1
    s[t] = 0
  elif C[t-1] + b_t < CL:
    # battery is empty
    h[t] = h[t+1] + 1
    s[t] = 1
  elif d[t] <= (h[t-1]-1)*b or d[t] >= (h[t-1]+1)*b
    # demand changes too much
    h[t] <- f(h[t-1]) # update h[t] accordingly
    if type == "LS1":
      s[i] = randint() % 2
    if type == "LS2":
      s[i] = 1 if C[t-1] < (CL + CH)/2 else 0
  else:
    h[t] = h[t-1]
    s[t] = s[t-1]
    
 update_battery()
 

def lazy_charging():
  if s[t-1] ==1 and C[t-1] + b > CH:
    s[t] = 0
  elif s[t-1] == 0 and C[t-1] - b < CL:
    s[t] = 1
  else
    s[t] = s[t-1]
  
  # update h[t] according to charging signal
  h[t] <- f(h[t-1]) 
  
  update_battery()

def random_charging():
  p = (C[t-1] - CL) / (CH - CL)
  if random.nextDouble() < p:
    s[t] = 0
  else
    s[t] = 1
  
  # update h[t] according to charging signal
  h[t] <- f(h[t-1]) 
  
  update_battery()
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
