## [Protecting Consumer Privacy from Electric Load Monitoring](http://www.cse.psu.edu/~smclaugh/cse598e-f11/papers/mclaughlin-ccs.pdf)

### Summary
In this paper, the authors propose an NILL scheme for protecting consumer privacy from electric load monitorng.  

### Algorithm
- **Non-intrisive Load Leveling (NILL)** scheme

```Python

k_ss = find_init_kss(profile[t0:t1])
k_l = max_charge_rate
k = k_ss
mode = ss
tr = 0 #recovery mode start time
a = 0.8

def find_init_kss(d):
  k = 0
  # find smallest k that L <= K*(t-t0) - D + Hc(t0) <= H
  return k
  
def find_kh(d):
  k_h = average(d) * 0.8
  return k_h

def switch_to_ss(d, t):
  mode = ss
  k = k_ss = a * sum(d[tr:t]) / (t-tr) + (1-a)*k_ss
  
def switch_to_h(d, t):
  mode = h
  k_h = find_kh(d[t-p:t])
  k = k_h
  tr = t
        
def switch_to_l(d, t):
  mode = l
  k = k_l
  tr = t
  
def update_battery(d, c, t):
  b = k - d
  c[t] = c[t-1] + b
  
def simulate(d):
  t = 0
  while (true):
    if mode == ss:
      if c[t] < L and d[t] > k_ss:
        switch_to_l(d, t)
      if c[t] > H and d[t] < k_ss:
        swtich_to_h(d, t)
    elif mode == h:
      if d[t] - k_h > 5:
        switch_to_ss(d, t)
    elif mode == l:
      if c[t] > 0.8:
        switch_to_ss(d, t)
    
    update_battery(d, c, t)
    t = t + 1
```

### TODO
- Discuss how NILM works
- Discuss how NILL works
