## Solutions to protect privacy

### Anomymization/Aggregation of metering data
- Anonymization
  - The metering data and customer identity are seperated by a third-party id [[Efthymiou-2010]](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=5622050). 
- Privacy-preserving metering data aggregation
  - Metering data is geographically encapsulated by aggreagting the metering data of co-located consumers [[Li-2011]](http://cae.ittc.ku.edu/papers/Li-IJSN.pdf). 
  - Rely on anonymization/escrow or aggregation techniques so that client's information can be aggregated and encrypted. Mentioned in [[Dimitriou-13]](http://dl.acm.org/citation.cfm?id=2480488)
- **Drawback**
  - This merely transfers doubts about trustworthiness from one party to another
  
### Modifying of metered data
- **Drawback**
  - This approach requires modification of the metering infrastructure, which may not be logistically and economically viable, with millions of smart meters already isntalled. 
  - Besides, the modification of usage data could result in inaccurate billing and grid controls, thereby undermine grid management. Mentioned in [[Yang15]](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6876215&tag=1)



### Battery Load Hiding
- Masking the power demand by adding or withdrawing to the meter visible energy demand with the help of recharable batteries or controllable load. 
  - [Battery Load Hiding](./blh.md)
