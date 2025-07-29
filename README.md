# 🌐 A 120 Mbps WDM-Based VLC System for IoT Communication

**Presented by:**  
👨‍🎓 K. Venkat Sai Charan 
👨‍🎓 V. Kishore

**Department of Electronics and Communication Engineering**  
**Under the Guidance of:** Dr. B. Vasudevan, M.E., Ph.D.  
St. Joseph’s College of Engineering, Chennai, India  

---

## 📘 Abstract

As the Internet of Things (IoT) ecosystem continues to expand rapidly, the demand for high-speed, secure, and interference-free communication channels has become more pressing than ever. Traditional RF-based communication methods suffer from spectrum congestion, interference, and licensing limitations. To overcome these constraints, this project explores an alternative paradigm—**Visible Light Communication (VLC)** using **Wavelength Division Multiplexing (WDM)** and **RAGB LEDs** to design a system that can reliably deliver up to **120 Mbps** data for indoor IoT applications.

---

## 🎯 Objective

- Replace traditional RF-based IoT links with VLC-based systems to minimize spectrum congestion and interference.
- Develop a WDM-enabled VLC communication system with four parallel channels—Red, Amber, Green, and Blue LEDs.
- Simulate the entire transmission-reception pipeline using **OptiSystem v17**.
- Evaluate the effectiveness of **Return-to-Zero (RZ)** vs **Non-Return-to-Zero (NRZ)** encoding schemes.
- Design a cost-effective, power-efficient, and scalable indoor communication model.

---

## 🌐 Introduction

### What is IoT?

The **Internet of Things (IoT)** refers to a network of interconnected physical devices—ranging from home appliances to industrial machines—that collect and exchange data over the internet. By 2025, the number of connected IoT devices is projected to exceed **25 billion**, resulting in an unprecedented demand for data exchange infrastructure.

### Limitations of RF Communication in IoT

Although RF (radio frequency) communication has been the backbone of wireless technology, it is increasingly becoming inefficient for future IoT growth due to:

- **Limited RF Spectrum**: The radio spectrum is licensed and congested.
- **Electromagnetic Interference (EMI)**: Prone to interference from other RF devices.
- **Security Risks**: Radio signals can penetrate walls, making them vulnerable to attacks.
- **High Power Requirements**: RF systems are not as energy-efficient as VLC.

### Why VLC?

**Visible Light Communication (VLC)** is an optical wireless technology that uses the visible light spectrum (400–700 nm) for data transmission. VLC is ideal for indoor IoT systems due to:

- Unlicensed and abundant spectrum
- High security (light doesn’t pass through walls)
- Resistance to RF interference
- Dual-purpose: illumination + data communication
- Compatibility with energy-efficient LEDs

---

## 🧠 Theoretical Foundations

### Modulation Schemes

- **NRZ (Non-Return-to-Zero)**: A binary 1 is represented by a high voltage level, and 0 by a low voltage level. NRZ offers higher spectral efficiency and is suitable for high data rates.
- **RZ (Return-to-Zero)**: Data returns to zero between bits, reducing inter-symbol interference but consuming more bandwidth.

### Wavelength Division Multiplexing (WDM)

WDM is used to combine multiple LED light wavelengths into a single white light source. Each LED (Red, Amber, Green, Blue) transmits independent data, and the receiver uses **optical filters** to extract and demultiplex the signals.

### System Components

| Component | Description |
|----------|-------------|
| **LEDs (RAGB)** | Transmit independent data channels at 700nm, 600nm, 550nm, and 480nm |
| **WDM Multiplexer** | Combines multiple wavelengths into one white light beam |
| **Optical Bandpass Filter** | Isolates specific wavelengths at the receiver end |
| **Avalanche Photodiode (APD)** | Converts optical signal into electrical signal |
| **Low Pass Filter (LPF)** | Removes high-frequency noise |
| **BER Tester** | Measures bit error rate to evaluate performance |

---

## 🛠 Tools & Simulation

### OptiSystem v17

All simulations were performed using **OptiSystem v17**, a professional-grade optical communication simulation tool by Optiwave. It enables the planning, testing, and modeling of advanced optical networks and components.

Simulation includes:

- LED source configuration
- NRZ/RZ encoding
- WDM multiplexing
- Optical link propagation
- Receiver-side demultiplexing
- BER performance analysis

---

## 📊 Results & Analysis

| Transmission Rate | Encoding Scheme | BER Performance |
|-------------------|------------------|------------------|
| 10 Mbps per LED   | NRZ              | Low BER          |
| 20 Mbps per LED   | NRZ              | Acceptable BER   |
| 30 Mbps per LED   | RZ               | Higher BER       |

**Key Observations:**

- **NRZ** consistently performs better than **RZ** in terms of BER.
- Increasing APD surface area improves signal reception.
- The combined data throughput from 4 LED channels reaches up to **120 Mbps**, sufficient for dense IoT environments.
- Noise from ambient light is minimized using **optical filters** and **RC-based high-pass filtering**.

---

## 📚 Literature Review Highlights

- **FBMC in VLC** – Introduced multilevel modulation for increased spectral efficiency.
- **OFDM with Fractional Sampling** – Achieved high gains in multipath VLC environments.
- **WDM-Ro-VLC for Radio Applications** – Demonstrated high-speed VLC using multiplexing.
- **Surveys on VLC** – Emphasized VLC’s potential in secure, indoor communication.
- **LEDs as Transmitters & Receivers** – Suggested LED-based transceivers with ambient light mitigation.

---

## 🔮 Future Enhancements

- 🧠 **ML-Driven Adaptive Modulation**: Optimize transmission dynamically based on channel conditions.
- 📱 **Mobile App Integration**: For monitoring and control of IoT endpoints.
- 🌦 **Environmental Awareness**: Use sensors for weather-adaptive light communication.
- 🚗 **Vehicular VLC (V2X)**: Expand the technology to car-to-car and car-to-infrastructure communication.
- 🔁 **Bi-directional VLC**: Enable full-duplex communication using separate light spectrums.

---

## 🧾 Conclusion

This project validates the feasibility of deploying **WDM-based VLC systems** for high-speed, interference-free, and secure indoor IoT applications. By leveraging **low-cost RAGB LEDs**, **simple modulation**, and **multiplexing techniques**, the system achieves a combined throughput of **120 Mbps**—sufficient for modern IoT requirements in smart homes, healthcare, industrial automation, and beyond.

---

## 📘 References

1. Kumar, S., Singh, P. (2020). Filter Bank Multicarrier Modulation for VLC. *Wireless Pers Commun.* [DOI](https://doi.org/10.1007/s11277-020-07347-6)  
2. Kalikulov, N. et al. (2020). Multipath Diversity for OFDM-Based VLC. *Wireless Pers Commun.* [DOI](https://doi.org/10.1007/s11277-020-07171-y)  
3. Chaudhary, S. et al. (2019). A 3×25 Mbps WDM-Ro-VLC System. *WACOWC.* [DOI](https://doi.org/10.1109/wacowc.2019.8770208)  
4. Kumar, S., Singh, P. (2019). A Survey of VLC: Potential and Challenges. *Wireless Pers Commun.* [DOI](https://doi.org/10.1007/s11277-019-06616-3)  
5. Kadirvelu, S., Baba, V. (2018). VLC Using LED Receiver under Ambient Light. *Opt Quant Electron.* [DOI](https://doi.org/10.1007/s11082-017-1280-4)

---

## 🙏 Acknowledgments

We extend our sincere gratitude to **Dr. B. Vasudevan** for his expert mentorship, and to the **Department of ECE, St. Joseph’s College of Engineering**, for the infrastructure and academic support.

---

## 📬 Contact

For simulation files, collaborations, or queries:  
📧 kvsc1511@gmail.com
