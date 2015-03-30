## Concern

### 1. Electric Vehicles

#### Why become popular
- An emphasis on green technogloies and the price of gasoline is causing the number of electric vehicles to increase rapidly [[Zhou-2014]](http://arxiv.org/ftp/arxiv/papers/1402/1402.2489.pdf). 

#### Challenges
- To allow the user of electric vehicles to increase as rapidly as possible, it is necessary to find techniques to manage electric vehicle charging so that their oweners are not inconvenienced[[Zhou-2014]](http://arxiv.org/ftp/arxiv/papers/1402/1402.2489.pdf). . 

### Data Privacy
- [consumer's concern and the help of battery](http://spectrum.ieee.org/energy/the-smarter-grid/privacy-on-the-smart-grid)

### Security
- Smart Meter
  - **Data Transmission**: In smart grid systems, high-frequency measurement data (e.g., register readings and time interval consumption data), power quality data (e.g., voltage or current phase angle) and event data (e.g., outage alert) are collected from millions of smart meters and sent to the meter data repository at utilities. These data are expected to play a key role in supporting intelligent management applications (e.g., loading forecasting, demand management, outage management, energy theft detection, etc.) and improving smart grid stability and energy efficiency [[Yang-2014]](http://ieeexplore.ieee.org/xpl/login.jsp?tp=&arnumber=7007759&url=http%3A%2F%2Fieeexplore.ieee.org%2Fxpls%2Fabs_all.jsp%3Farnumber%3D7007759). 
  - **Security Issue**: 
    - **Trustworthiness in AMI data collection**: However, when the power grid evolves to become "smart", new security challenges have emerged. The security concern comes from the enlarged attack surface, for instance, smart meters are placed in physically insecure locations that are easily accessible to the adversaries, and thus are subject to attacks from physically tempering with meter reading (e.g., meter invasion) to manipulating measurement data in communication channel between meter processor and the embeded sensor. Moreover, the upgraded connectivity makes smart meters susceptible to cyber attacks in which adversaries may compromise smart meters or eavesdrop the communication.
    - **Data Privacy**: In smart grid, energy consumption data that contains rich information about end consumers is collected at a much higher frequency than before. Without proper protection, realtime fine-grained metering data may disclose sensitive informaiton about the consumers and expose them to a variety of privacy threats. For example, information about the lifestyle can be inferred from high-resolution metering data via nontrusive appliance load monitoring 9NLAM). In [[Molina-2010]](http://dl.acm.org/citation.cfm?id=1878446), the power consumption data is correlated to appliance usage to associate power events with automated appliances activities and inhabitant's activities. Such privacy-sensitive household data may be used by third-party industires to profile energy consumption patterns for maximizing their rvenue, or by malicious adversaries to derive the living patterns and conduct further intended attacks. For the sake of customers' privacy, personal data and consumption data in smart metering should be protected from unauthorzed sharing, disclosing or selling. [[Yang-2014]](http://ieeexplore.ieee.org/xpl/login.jsp?tp=&arnumber=7007759&url=http%3A%2F%2Fieeexplore.ieee.org%2Fxpls%2Fabs_all.jsp%3Farnumber%3D7007759)
    - **Data Sharing**: One major function of the smart grid system is to collect precise energy consumption data from resiential loads and smart meters so that a detailed view of energy usage will be provided to both utilities and consumers.
      - A multitudde of energy services are anticipated to be incorporated into the smart grid system to provide value-added services such as dynamic billing, load monitoring and forecasting, demand response, outsage and fraud detection, etc. To facilitate such applications, high resolution energy consumption is expected to be **shared** among various organizations in the industry and the governments, i.e., between the utilities and third-party service providers, which require access to the metering data at different levels of patial and temporal aggregation.


### Privacy
- Given the fact that metering data of individual homes/factories is accumulated every 15 min, it is possible to infer the pattern of electricity consumption of individual users. [[Wang-2012]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6203629)
- It would be possible for utilities to infer the type of appliances individual customers are using at every 15 min (i.e., when you are using your computer and when your garage door is activated). The compromise of cutomers' privacy would be significant if they are left unprotected [[Wang-2012]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6203629). 
- User privacy protection mechanisms in other fields are not applicable to smart grid. [[Wang-2012]](http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6203629)
- **Drawback bring by privacy issue**
  - The deployment of smart meters have encountered obstables from the public outcry. Some parts in North America and Europe have already banned the deployment of the smart meters. Furthermore, the disputes over the law aspects of AMI is also ongoing. Considering hte smart meter system's great benefits, addressing the privacy issues of smart metering data is crucial to the deployment of smart grid systems. 
