## Model


### Battery
- Motivation
  - Battery Energy Storage (BES) plays an increasingly important role in the modern deregularted electricity market. 
    - For instance, in cities such as San Francisco and New York, where power is costly, large commercial buildings are installed with batteries in their basements, for the purppose of storing electricity at night when prices are low, and tappling into the batteries during peak afternoons when prices are high [[Tan-2014]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7007733).

### Smart Meter
- The smart meters are installed at each household and connected to the supplier through AMI.
- Smart meters make it possible to provide near real-time price incentives to customers which could potentially reduce the need for expensive peak capacity and energy. The successful adoption of smart metering and pricing could offer many benefits, including: reduction in wholesales prices, enhanced reliability, and environmental improvement. [[Wang-2012]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6203629)

### Supplier/Grid
- The energy supplier is either an actual power generator or a grid operation (e.g., a utility).
  - It has legitimae interst and priviledge to collect the identifiable consumption data. 
  
### Third-Party
- There exist multiple third-party data consumers who are allowed to access smart metering data non-instrusively. 
- The supplier coolect terabytes of fine granular energy consumption measurements stemming from various consumer households, and provies access to energy service providers in two ways: [[Yang-2014]](http://ieeexplore.ieee.org/xpl/login.jsp?tp=&arnumber=7007759&url=http%3A%2F%2Fieeexplore.ieee.org%2Fxpls%2Fabs_all.jsp%3Farnumber%3D7007759)
  - 1. publishing pseudonymized consumption data to external stakeholders for secondary use
  - 2. answering queries of providers

### Electricity user
- Each proconsumer is equapped with 
  - a power and data management unit (called energy gateway, EG). interfacing the prosumer iteself with the micro grid and data conmmunication networks, controlling local energy sources and managing some controllable （i.e., shiftable) loads.
  - distributed energy sources (renewable energy sources, RESs, in the considered scenario). 
