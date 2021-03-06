## Solutions to protect privacy

### Summary
- A typical approach to privacy in smart meter data is aggregation along dimensions of space (using neighborhood gateways), time (using battery storage), or precision (using noise addition). [[Sraj-11]](../../papers/file/sraj11-utility-privacy.md)
  - **Limitation**: these solutions seek to support utility and privacy in different ways; however, they do not have a robust theoretical basis for both privacy and utility. 
- Why need a theoreitcal framework of  utility-privacy [[Sraj-11]](../../papers/file/sraj11-utility-privacy.md)
  - We need a privacy framework that not only address the capabilities of current non-intrusive load monitoring (NALM) techniquesbut is also extensible to future ones. 
  - A theoretical famework enables us to examine the costs of lost privacy against the benefits of data diseemination, namely, the tradeoff between privacy and utility.
  - It would be desire to give each customer the ability to decide the tradeoff and also to give the electricity provider the ability to incentivize the customer to participate in such a bargain by offering intersing points of tradeoff.
  
### Anomymization/Aggregation of metering data
- Anonymization
  - The metering data and customer identity are seperated by a third-party id [[Efthymiou-2010]](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=5622050). 
- Privacy-preserving metering data aggregation
  - Metering data is geographically encapsulated by aggreagting the metering data of co-located consumers [[Li-2011]](http://cae.ittc.ku.edu/papers/Li-IJSN.pdf). 
  - Rely on anonymization/escrow or aggregation techniques so that client's information can be aggregated and encrypted. Mentioned in [[Dimitriou-13]](http://dl.acm.org/citation.cfm?id=2480488)
- More about aggregation
- **Drawback**
  - This merely transfers doubts about trustworthiness from one party to another
  
### Modifying of metered data
- **Drawback**
  - This approach requires modification of the metering infrastructure, which may not be logistically and economically viable, with millions of smart meters already isntalled. 
  - Besides, the modification of usage data could result in inaccurate billing and grid controls, thereby undermine grid management. Mentioned in [[Yang15]](http://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=6876215&tag=1)



### Battery Load Hiding
- Masking the power demand by adding or withdrawing to the meter visible energy demand with the help of recharable batteries or controllable load. 
  - [Battery Load Hiding](./blh.md)
