## [Demand-Side Management in a Smart Micro-Grid: A distributed approach based on bayesian game theory](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=7007722)

### Summary
- In this paper, the authors proposed a strategy allows to schedule shiftalbe loads in way to mitigate the PAR in load demand, while substantially preserving user privacy.
- Each consumer is endowed with *statistical information* about his and their future overall consumptions, so that he can select his actions on the basis of an expected payoff (i.e., a Bayesian approach is adopted).
  - This approach allows each prosumer to act in an autonomous fashion and to protect his privacy.

### Statistics Information
- As far as statistical information is concerned, we assume that the n-th prosumer is endowed with the knowledge of two different probability density function (pdfs), one related to the overall power flow in the microgrid, the other one to its own behavior. In particular, his statistical knowledge about the whole microgrid is condesed in the first order probability density function.
  - This pdf can be estimated by the microgrid supervisor and then its description (based on a parsimonious parametric representation of it) can be periodically broadcasted to all the prosumers.
  - The estimation of this pdf requires the exact knowledge of
    - the time instants in which any prosumer would like to instantly turn on its shiftable loads
    - the power absorption these activiation would ential. Thus it requires that each of the MG EGs memories the above mensioned data and periodially communicate them to the MG supervisor with a certain delay (so that the real time or day ahead load of prosumers remain unknown to potential eavesdroppers and provaciy is substantially perserved)
