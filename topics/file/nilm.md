## Non-intrusive Load Monitoring (NILM)


### Objective
- NILM can be used to extract appliance profiles from load profiles. It is considered "non-instrusive" because it does this at the electric meter without instrumenting individual appliances. 
- NILM is an energy disaggregation approach. Energy disaggregation is the task of using an aggregate energy signal, such as that coming from a whole-home power monitor, to make inferences about the different invidual loads of the system. 

### Benefits
- Information about individual appliances is much more userful to consumers thatn simply total electricity usage.

### How it works
- Appliace Profile
  - An appliance profile consists of the types of appliances and the times during which each is operational during the day.
- NILM approach
  - Load profiling techniques classify devices by the changes in steady state load caused by their being turned "ON" and "OFF".
  - The approach is to decomposed load profile into a composite of invidual appliances features, i,e,m representative pairs of ON/OFF events.

### Model
- Appliances are treated as transmitters, and step changes are effectively treated as messages transmitted by the appliancesm so the load monitor is designed to act as an adaptive receiver.
