## Architecture

### Smart Meter
- The smart meters are installed at each household and connected to the supplier through AMI.
- Smart meters make it possible to provide near real-time price incentives to customers which could potentially reduce the need for expensive peak capacity and energy. The successful adoption of smart metering and pricing could offer many benefits, including: reduction in wholesales prices, enhanced reliability, and environmental improvement. [[Wang-2012]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6203629)

### Supplier/Grid
- The energy supplier is either an actual power generator or a grid operation (e.g., a utility).
  - It has legitimae interst and priviledge to collect the identifiable consumption data. 

### Advanced Meter Infrastructure (AMI)
- AMI is composed of networked smart meters, but these smart meters not only collect register reads, the montly electricity consumption information for billing purposes, but also collect interval data (typically the minute-leve lor second-level electricity consumption information for billing purposes). [[Zhao-2014]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6847974)
  - On one hand, this fine-grained information enables trending, forecasting and fault detection analysis, which leads to a more efficient and robust grid system.
  - On the other hand, this information reveals important personal information - human behaviors. For example, by applying the None-Intrusive Load Monitoring (NILM) techniques, attackers can efficiently derivce the appliance usage patterns of the residents from the fine-grained energy usage profile. 

### None Intrusive Load Monitoring (NILM)
- NILM is originally designed to support constructin of smart homes, which learns the lifestyle of residents, monitors ageing and problematic appliances, and consequently provides safe environment for the alone elder people. [[Zhao-2014]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6847974)
- However, the NILM technique also enables malicious thrid parties to acquire the residents behavior patterns, which will reveal the vacant times, the number and the location of the residents insider a house, or even the ages and brands of appliances. This may cause severe security hazards.
  - For example, if a burglar acquires this information, he immetiately knows when and where to break in. In fact, Rouf et al. have shown that they can spoof the neergy usage information from real world deployed meter systems as a thrid party to realized the analysis metioned abpve (identifying unoccuplied residences or people's routines).
