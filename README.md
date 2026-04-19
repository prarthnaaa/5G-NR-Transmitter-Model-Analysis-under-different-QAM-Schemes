````markdown
# Performance Analysis of 5G New Radio (5G NR) Transmitter Models Using QAM Modulation Schemes

A MATLAB Simulink-based project focused on evaluating the performance of 5G NR transmitter models using different QAM modulation schemes under ideal, impaired, and compensated operating conditions.

---

## 📌 Overview

5G New Radio (5G NR) requires high data rates, low latency, and reliable wireless communication. To achieve this, higher-order modulation techniques such as **16-QAM, 64-QAM, and 256-QAM** are widely used.

However, practical transmitter systems suffer from RF impairments such as:

- I/Q Imbalance  
- Phase Noise  
- Carrier Frequency Offset (CFO)  
- Power Amplifier Nonlinearity  
- Multipath Fading  
- AWGN Noise  

This project develops a simulation framework in **MATLAB Simulink** to analyze how these impairments affect system performance and how compensation techniques improve reliability.

---

## 🎯 Objectives

- Design a standard-compliant 5G NR transmitter model  
- Compare 16-QAM, 64-QAM, and 256-QAM modulation schemes  
- Analyze impact of real-world RF impairments  
- Implement suppression/compensation techniques  
- Measure system performance using standard metrics  
- Identify the most practical modulation scheme for real deployment  

---

## 🔍 Research Gaps

- Most existing studies analyze **single impairments only**, not combined real-world impairments.  
- Limited comparison of **16-QAM, 64-QAM, and 256-QAM** under identical conditions.  
- Gap between **ideal simulation models and practical hardware behavior**.  
- Few works evaluate **before-and-after compensation performance** clearly.  
- Limited use of **3GPP standard thresholds** for practical benchmarking.  

---

## 🛠 Tools & Technologies

- MATLAB  
- Simulink  
- 5G Toolbox  
- Communications Toolbox  
- RF Modeling Blocks  

---

## ⚙️ Simulation Parameters

| Parameter | Value |
|---------|-------|
| Carrier Frequency | 3.5 GHz |
| Bandwidth | 5 MHz |
| Subcarrier Spacing | 30 kHz |
| Duplexing | FDD |
| Number of Subframes | 10 |
| Modulation Types | 16-QAM, 64-QAM, 256-QAM |

---

## 📊 Performance Metrics Used

- **EVM (Error Vector Magnitude)** – Signal quality measurement  
- **PAPR (Peak-to-Average Power Ratio)** – Power efficiency indicator  
- **CCDF Curve** – Peak probability analysis  
- **Constellation Diagram** – Symbol accuracy visualization  
- **Spectrum Analysis** – Frequency domain behavior  

---

## 📈 Key Results

### Ideal Condition Performance

| Modulation | Obtained EVM (%) | 3GPP EVM Threshold (%) | Obtained PAPR (dB) | 3GPP PAPR Threshold (dB) |
|-----------|------------------|------------------------|-------------------|--------------------------|
| 16-QAM | 1.21 | ≤ 12.5 | 9.71 | ≤ 10 |
| 64-QAM | 1.24 | ≤ 8 | 9.80 | ≤ 10 |
| 256-QAM | 1.22 | ≤ 3.5 | 9.57 | ≤ 10 |

### Impairments + Compensation Performance

| Modulation | Obtained EVM (%) | 3GPP EVM Threshold (%) | Obtained PAPR (dB) | 3GPP PAPR Threshold (dB) |
|-----------|------------------|------------------------|-------------------|--------------------------|
| 16-QAM | 6.9 | ≤ 12.5 | 10.17 | ≤ 10 |
| 64-QAM | 6.6 | ≤ 8 | 9.83 | ≤ 10 |
| 256-QAM | 5.9 | ≤ 3.5 | 9.76 | ≤ 10 |

---

## 🔍 Major Findings

- **16-QAM** offered highest robustness against impairments.  
- **256-QAM** provided highest spectral efficiency but was highly sensitive.  
- **64-QAM** achieved the best trade-off between robustness and efficiency.  
- CFO and Phase Noise caused the most severe degradation.  
- Compensation improved EVM but could not fully restore ideal conditions.  

---

## 🧠 Compensation Techniques Used

- Carrier Synchronizer  
- I/Q Imbalance Compensator  
- Adaptive Correction Methods  

---

## 🌍 Real World Impact

This project supports:

- Smart Cities through reliable wireless communication  
- IoT networks with stable connectivity  
- Telemedicine and remote healthcare  
- Energy-efficient communication systems  
- Better spectrum utilization  

Aligned with:

- **SDG 9** – Industry, Innovation & Infrastructure  
- **SDG 7** – Affordable & Clean Energy  
- **SDG 11** – Sustainable Cities & Communities  

---

## 🏆 Conclusion

The project demonstrates that RF impairments significantly affect 5G NR transmitter performance. Among all tested schemes, **64-QAM is the most practical modulation technique**, offering the best balance between data rate, robustness, and implementation feasibility.

---

## 👩‍💻 Author

**Prarthna Puhan**
B.Tech Electronics and Communication Engineering
VIT Vellore

---

## 📜 License

Academic and research use only.

```
```
