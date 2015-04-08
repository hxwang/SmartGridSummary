## Privacy Define and Measurement

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

