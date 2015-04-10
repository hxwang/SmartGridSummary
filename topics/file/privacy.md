## Privacy Define and Measurement

### Privacy 
- Privacy is defined as "undetectability" [[Andreas-10]](https://dud.inf.tu-dresden.de/literatur/Anon_Terminology_v0.34.pdf)

### Entropy
- [[Arijit-2014]](../../papers/file/ukil14-privacy-2bn2b.md)
  - S: sensor data set
  - &lambda; : non-sensitive part
  - v: sensitive part
    - S = &lambda; &cup; v
  - The privacy measure is defined as the amount of difficulty to infer v when only &lambda; is presented or how much probability of finding v
    - The information leakage transfer function:  p_m = (entropy of v) / (entropy of S)
  - In addition, the measure whether S and v are drawn from the same distribution by using **Kolmogorov-Smirnov (KS)** test, the misfit is denoted as p_s
  - Finally, the privacy quatification is p_m * p_s
  - Comments
    - This approach measures the information leakage. However, it can not directly be applied to smart grid privacy leakage. Since the privacy leakage is in fact related to the detecting mechanism. It is not clear how the entropy corresponds to the information leakage.
- [[McLaughLin-11]](../../papers/file/mclaughlin11-privacy-consumer.md)
  - Calculate the entropy of the workload changes (including 0 zeros, or not), the higher the entropy is, the larger the privacy exposed.
  
### Relative Entropy
- [[Kalogridis-10]](../../papers/file/Kalogridis10-privacy-undetectable.md)
  - The relative entropy or Kullback Leibler distance is a well know information theoreitc quantity which can be used to compare two sources of information. To employ this matric in the privacy context, we assume e(t) and d(t) can be modelled as stochastic process with probability measures P and Q. 
  - If f_p(x) and f_q(x) are the probability density functions (pdfs) of p and q, the relative entropy D(P||Q) is defined as
    - D(P||Q) = \sum^{x_max}_{x_min} f_p(x) log( f_p(x) / f_q(x))
  - The importance of the relative entropy is that (although it is not a distance as defined in mathematical sense), it quatifies the relation between P and Q. For example, the relative entropy is always positive, and for P identical to Q, it is 0.
  - Strictly speaking, the relative entropy is premetric.
  - Accordingly, the level of protection offered by an algorithm can be measured by the relative entropy D(P||Q) such that the higher the level of protection offered, the larger the relative entropy.

### NILM
- Only the electricity samples with prominent amplitude changes can server as valuable data sources for NILM algorithm.
