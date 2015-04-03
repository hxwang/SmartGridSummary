## [Privacy for smart meters: Towards Undetable Appliance Load Signature](http://ieeexplore.ieee.org/xpl/login.jsp?tp=&arnumber=5622047)


### Summary
In this paper, the authors study the problem of protecting privacy of smart homes using battery storage device. In particular, the privacy is protected by charging/discharging battery to hide the real electricity usage. They design a simple **Best Effort (BE)** scheme to solve this problem with the objective of hiding the electricity changes in two successive time slots.

### Definition
- Privacy
  - Privacy is defined using **undetectability**, i.e., privacy is protected when, given a home load signature, we cannot sufficiiently distinguish whether an appliance load event exists or not.
  - They consider nay change (or no change) of appliance state, is "private" information, hence they wish to measure the degree of which the changes are detectable.

### Techniques
- Relative Entropy
  - when the power usage is the same with the output load, then the relative entropy is 0. 
  - The objective is to maximize entropy, thus to introduce more uncertainty.
  
### Algorithm
- **Best Effort (BE)** scheme
  - try the best effort to main the same level of electricity usage in two successive time slots
  - charge the battery only when the energy in the battery is not enough to maintain the same level electricity usage of current time slot and last time slot
  
### Question
- Why use relative entropy to represent the privacy? i.e., why the electricity changes in two successive time slots matter.
