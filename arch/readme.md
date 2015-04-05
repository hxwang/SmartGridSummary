## Architecture

### Smart Meter
- The smart meters are installed at each household and connected to the supplier through AMI.
- Smart meters make it possible to provide near real-time price incentives to customers which could potentially reduce the need for expensive peak capacity and energy. The successful adoption of smart metering and pricing could offer many benefits, including: reduction in wholesales prices, enhanced reliability, and environmental improvement. [[Wang-2012]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6203629)
- Benefits [[Mikhail-2010]](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=5403146)
  - Reduce data collection cost
  - improve large-scale load planning

### Supplier/Grid
- The energy supplier is either an actual power generator or a grid operation (e.g., a utility).
  - It has legitimae interst and priviledge to collect the identifiable consumption data. 

### Advanced Meter Infrastructure (AMI)
- AMI is composed of networked smart meters, but these smart meters not only collect register reads, the montly electricity consumption information for billing purposes, but also collect interval data (typically the minute-leve lor second-level electricity consumption information for billing purposes). [[Zhao-2014]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6847974)
  - On one hand, this fine-grained information enables trending, forecasting and fault detection analysis, which leads to a more efficient and robust grid system.
  - On the other hand, this information reveals important personal information - human behaviors. For example, by applying the None-Intrusive Load Monitoring (NILM) techniques, attackers can efficiently derivce the appliance usage patterns of the residents from the fine-grained energy usage profile. 

### None Intrusive Load Monitoring (NILM)
- NILM has been designed to aid electric utilities in the collection of appliance end user data. 
- This monitor requires only the information externally available from mwasurements of the load; no entry into the home is necessary to place sensors on separate appliances or branch circuits. No appliance survey or other cooperation from the residents is required. Mentionedi n [[Hard-1989]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=31557)

- NILM is originally designed to support constructin of smart homes, which learns the lifestyle of residents, monitors ageing and problematic appliances, and consequently provides safe environment for the alone elder people. [[Zhao-2014]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6847974)
- However, the NILM technique also enables malicious thrid parties to acquire the residents behavior patterns, which will reveal the vacant times, the number and the location of the residents insider a house, or even the ages and brands of appliances. This may cause severe security hazards. [[Zhao-2014]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6847974)
  - For example, if a burglar acquires this information, he immetiately knows when and where to break in. In fact, Rouf et al. have shown that they can spoof the neergy usage information from real world deployed meter systems as a thrid party to realized the analysis metioned abpve (identifying unoccuplied residences or people's routines).
- [Detailes about the attack](../topics/file/nilm.md)
