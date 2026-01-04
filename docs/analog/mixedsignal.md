## General Mixed Signal Sub-Blockes

used in 

> ADC, DAC, TDC, DTC, VTC, TVC; DPLL, DLL, CDR; SerDes; DPA...

### Switched-Capacitor

- Ken Kundert
  - Simulating Switched-Capacitor Filters with SpectreRF
- Boris Murmann
  - ISSCC 2011 T8: Noise Analysis in Switched-Capacitor Circuits
  - SSC-M 2013: Thermal Noise in Track-and-Hold Circuits

### Comparator

- Metastability & Cross-Coupled Pair
  - [Metastability: Deeply misunderstood](https://ieeexplore.ieee.org/document/10584398) by Chris Mangelsdorf [王小桃翻译](https://zhuanlan.zhihu.com/p/1915074577098323233)
  - Cross-Coupled Pair 的 Razavi SSC-M 通俗易懂，但是缺少进一步拔高的 insight 和计算，此处不放链接

#### 基本比较器类型

- StrongARM
  - [再世孟子 - 知乎](https://zhuanlan.zhihu.com/p/598924151)
  - [王小桃 - 知乎](https://zhuanlan.zhihu.com/p/16672774067)
- Double Tail
  - [宇文青霜 - 知乎1](https://zhuanlan.zhihu.com/p/1973463738737780166) [2](https://zhuanlan.zhihu.com/p/557606071)
- Current-Steering / CML latch
  - Razavi ADC book comparator chapter
- Dynamic Bias (Harijot Singh Bindra & Bram Nauta)
  - ESSCIRC 2017: [A 30fJ/comparison dynamic bias comparator](https://ieeexplore.ieee.org/document/8094528)
  - JSSC 2018: [A 1.2-V Dynamic Bias Latch-Type Comparator in 65-nm CMOS With 0.4-mV Input Noise](https://ieeexplore.ieee.org/document/8345180)
  - ISSCC 2022: [A 174μVRMS Input Noise, 1 GS/s Comparator in 22nm FDSOI with a Dynamic-Bias Preamplifier Using Tail Charge Pump and Capacitive Neutralization Across the Latch](https://ieeexplore.ieee.org/document/9731728)
- Floating Inverter Amplifier FIA (唐希源 & 孙楠)
  - VLSI 2019: [An Energy-Efficient Comparator with Dynamic Floating Inverter Pre-Amplifier](https://ieeexplore.ieee.org/document/8777942)
  - JSSC 2020: [An Energy-Efficient Comparator With Dynamic Floating Inverter Amplifier](https://ieeexplore.ieee.org/abstract/document/8947992)
  - CICC 2023: [A 0.69-Noise-Efficiency-Factor 4 x-Current-Reuse Dynamic Comparator with A Stacking FIA](https://ieeexplore.ieee.org/document/10121319)

#### 分析与仿真

- Papers
  - noise, offset focused - General ADC
    - [TCAS-I 2008: Noise Analysis of Regenerative Comparators for Reconfigurable ADC Architectures](https://ieeexplore.ieee.org/document/4446769)
    - [TCAS-I 2009: Simulation and Analysis of Random Decision Errors in Clocked Comparators](https://ieeexplore.ieee.org/document/5175291/)
    - [TCAS-I 2009: Analyses of Static and Dynamic Random Offset Voltages in Dynamic Comparators](https://ieeexplore.ieee.org/document/4783032)
    - [TCAS-I 2019: Analysis and Design of Regenerative Comparators for Low Offset and Noise]
  - SerDes focused
    - [VLSI 2008: Characterizing Sampling Aperture of Clocked Comparators]

- Simulation: noise, offset, metastability
  - tran 时域方法
    - ⭐Razavi ADC book 6.4 和 7.7 (这和之前 Razavi 发表的 SSC-M 中的内容基本是一模一样的，[王小桃翻译](https://zhuanlan.zhihu.com/p/16347220323))
  - PSS 频域方法
    - Cadence 
      - doc: [Keeping Things Quiet: A New Methodology for Dynamic Comparator Noise Analysis, Art Schaldenbrand, 2016](https://www.cadence.com/content/dam/cadence-www/global/en_US/videos/tools/custom-_ic_analog_rf_design/NoiseAnalyisposting201612Chalk%20Talk.pdf)  [video](https://www.youtube.com/watch?v=Syg2mK__Nj0)
      - doc: ⭐[ADC Verification Rapid Adoption Kit, Module 3: Dynamic Comparator Characterization](https://bbs.eetop.cn/thread-964432-1-1.html)
      - video: ⭐[Analog IP Verification Seminar, SAR ADC design and verification - 3 Simulations for SAR ADC, Effective Number of Bits (ENOB)](https://bbs.eetop.cn/thread-969302-1-1.html)
  - [通用介绍 by 宇文青霜 - 知乎 ](https://zhuanlan.zhihu.com/p/279111199)
 
### Faster Logic (TSPC & CML)
