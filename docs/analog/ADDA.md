# ADDA

## Modules

### Bootstrap

todo

### Switch-Capacitor & Comparator

Move to [Mixed Signal](mixedsignal.md)

## 通用学习资源

ADDA 方向部分大学是有本科生选修课的

后文中 `⚡` 代表高速 (Nyquist) ADDA, `🎯` 代表高精度 (Oversampling) ADDA, `⭐` 代表精选/推荐/必读资源

### Introduction

```mermaid
graph LR

  SAR["2016 T5: Basics of SAR ADCs: Circuits & Architectures"] --> FoM
  %% Fundamentals["2023 T3: Fundamentals of Data Converters"] --> FoM
  FoM["2022 SC3: Introduction to ADCs/DACs: Metrics, Topologies, Trade Space, and Applications"]
  
  FoM --> NS["2019 T5: **Noise-Shaping** in Data Converters"]
  FoM --> TI["2020 T5: Fundamentals of **Time-Interleaved** ADCs"]
  FoM --> CT["2024 T7: Fundamentals of **Continuous-Time** ADCs"]
```

- A Brief History of Data Conversion: A Tale of Nozzles, Relays, Tubes, Transistors, and CMOS
- FUNDAMENTALS OF SAMPLED DATA SYSTEMS, ADI
- Pieter Harpe @ TU/e
  - ISSCC 2016 [T05](https://resourcecenter.sscs.ieee.org/education/short-courses/sscstut20160090) - Basics of SAR ADCs Circuits & Architectures

### Boris Murmann @ Stanford → UH Mānoa

- 一句话介绍: ADC FoM 表格的经典 maintainer
- courseware
  - Stanford EE315A, EE315B
- conference
  - 2013 CICC T: A/D Converter Circuit and Architecture Design for High-Speed Data Communication
  - 2022 ISSCC SC: Introduction to ADCs/DACs: Metrics, Topologies, Trade Space, and Applications ⭐
- https://github.com/bmurmann/ADC-survey

### Manar El-Chammas ⚡ @ TI → Omni Design

- conference
  - ICECS 2011 T: Time-Interleaved ADCs Theory and Design
  - NEWCAS 2012 T: The World of Time-Interleaved ADCs from theory to design
  - ISSCC 2017 F6: Design Techniques for Multi-GSs and High Performance Pipelined ADCs
  - AUB Talks Semantic Communications 2024: The hardware behind the algorithms: A look at energy-efficient transievers and accelerators
- book
  - 2024 High-Performance and High-Speed Pipelined ADCs (z-lib + tor)

### Pieter Harpe @ TU/e

- conference
  - 2016 ISSCC [T05](https://resourcecenter.sscs.ieee.org/education/short-courses/sscstut20160090) - Basics of SAR ADCs Circuits & Architectures ⭐⭐
  - 2016 SSC-M: [Successive Approximation Analog-to-Digital Converters: Improving Power Efficiency and Conversion Speed](https://ieeexplore.ieee.org/document/7743043)
  - Low-power SAR ADCs
    - 2019 ESSCIRC Paper: [Low-power SAR ADCs: trends, examples and future](https://ieeexplore.ieee.org/document/8902871)
    - 2019 ESSCIRC Video: [Low-Power SAR ADCs Presented by Pieter Harpe - YouTube](https://www.youtube.com/watch?v=BE9onmrGZhY)
    - 2019 OJSSCS Paper: [Low-Power SAR ADCs: Basic Techniques and Trends](https://ieeexplore.ieee.org/document/9908164)
  - 2022 ISSCC SC3: High Precision and Low Power ADCs
  - 2024 CICC: [Energy Efficient ADC Design Techniques](https://ieeexplore.ieee.org/document/10529035)
  - 2025 ASSCC: [Circuits for Data Conversion](https://www.youtube.com/watch?v=dDKxcVIHDjg&list=PLvYonHCKSWainhipdNmCATbT_zvK1rlnB&index=2)
 
### Marcel J.M. Pelgrom @ TU Delft / NXP → Retired ⭐

- 一句话介绍: ADC 领域的真正专家
- book
  - 2022 Springer: Analog-to Digital Conversion, Fourth Edition ⭐⭐
  - 2023 Springer: Multi-Gigahertz Nyquist Analog-to-Digital Converters
- conference
  - 2020 SSCS-EDS South Brazil Distinguished Talk: [ADC Performance Limits - The Fundamentals](https://www.youtube.com/watch?v=doTHd0W9QhA)

### Behzad Razavi @ UCLA

- book
  - 2025 Cambridge: Analysis and Design of Data Converters ⭐⭐
- journal
  - 2013 JSSC: Design considerations for interleaved ADCs
- courseware (not recommended)
  - 2012 EE215D: https://www.seas.ucla.edu/brweb/teaching/215D_S2012/

### 邱云 Yun Chiu @ UT Dallas

- courseware
  - 2025 EECT 7327: https://personal.utdallas.edu/~yxc101000/courses/7327/handout.html
- conference
  - mwscas 2012: Recent Advances in Multistep Nyquist ADC’s
  - ISSCC 2023 T3: Fundamentals of Data Converters

### Ahmed M. A. Ali ⚡ @ ADI → Apple (High Speed)
    
- book
  - 2016 IET: High Speed Data Converters 《高速数据转换器设计》
- conference
  - CICC 2018 T: High Speed Pipelined ADCs: Fundamentals and Variants
  - ISSCC 2021 T05: Calibration Techniques in ADCs

### 陳碩偉 Mike Shuo-Wei Chen @ USC

- 一句话介绍: 现代异步 SAR-ADC (比较器 Valid 信号作为自驱动时钟) 的提出者; ISSCC, JSSC 2006
- conference
  - CICC 2018 T: Evolutions of SAR ADC: From high resolution to high speed regime
- paid
  - hoomanreyhani 2021: Advanced Data Converters

### Michael P. Flynn @ UMich 

- conference
  - CICC 2015: ADC Trends and Impact on SAR ADC Architecture and Analysis
  - ASSCC 2017 T1: ADC hybrids and ADC morphing
  - ISSCC 2018 edu: Evolutional of the SAR ADC

### Aaron Buchwald ⚡ @ Entropic → Inphi → Aeonsemi

- conference
  - ISSCC 2010 T3: Specifying and Testing ADCs
  - CICC 2015: Practical considerations for application specific time interleaved ADCs
  - VLSI 2016 SC3: ADCs for PAM-X / QAM-X Backplane and Optical Data Links
  - CICC 2017 S2-1: A Supposedly Clever Thing I’ll Never Do Again
  - CICC 2018 T2: Time Interleaved ADCs Requirements vs. Application
- journal
  - 2016: High-speed time interleaved ADCs

### Keysight ⚡

John P. Keane

- conference
  - ISSCC 2020 T5: Fundamentals of Time-Interleaved ADCs ⭐

Kenneth C. Dyer

- conference
  - 2016 ISSCC F2: Calibration and Dynamic Matching in Data Converters
- journal
  - 2018 SSC-M: Calibration and Dynamic Matching in Data Converters: Part 1, Part 2

### Walt Kester @ ADI

- book
  - 2005 ADI: Data Conversion Handbook
- MT series ADI
  - MT-001 to MT-031

### 孙楠, 李福乐, 揭路, 唐希源 @ THU, PKU ⭐

- courseware / slides
  - https://bbs.eetop.cn/thread-953294-1-23.html
  - https://bbs.eetop.cn/thread-954969-2-90.html
  - https://bbs.eetop.cn/thread-943698-8-29.html
- conference
  - ASSCC 2025 T1: Noise-Shaping SAR ADC: Design, Development, and Deployment
- journal
  - [Low-Power SAR ADC Design: Overview and Survey of State-of-the-Art Techniques](https://ieeexplore.ieee.org/document/9761973)

### 陈知行⚡ @ University of Macau

- conference
  - CICC 2024: The Race for the Extra Pico Second without Losing the Decibel: A Partial-Review of Single-Channel Energy-Efficient High-Speed Nyquist ADCs
- paid
  - hoomanreyhani 2024: Extreme SAR ADCs

### Paid

- eeeknow.com 移知
  - 高速异步 SAR ADC 设计实战 ⭐
  - 30 天学会 Sigma-Delta(Σ-Δ) ADC 设计
  - Current Steering DAC 的 Matlab 建模与电路设计
- icdesign.com
  - 比较器
  - SAR ADC
  - Current Steering DAC

### Others

- UC Berkeley
  - UCB EE 247 (old), EE 240C (new)
- 朱樟明 @ XIDIAN
  - 《低功耗 CMOS 逐次逼近型模数转换器》
- Allen
  - 第二版

### Cadence

- ADC Verification Rapid Adoption Kit [eetop download](https://bbs.eetop.cn/thread-964432-1-1.html) ⭐
- Analog IP Verification Seminar, SAR ADC design and verification [eetop download](https://bbs.eetop.cn/thread-969302-1-1.html) [link2](https://pan.baidu.com/s/1TNBDKtl22S0xxORziXMdsg?pwd=sjxj)

### MATLAB

https://www.mathworks.com/help/msblks/examples.html?category=data-converters&exampleproduct=all
https://www.mathworks.com/help/msblks/ug/adc-tutorial.html


https://www.mathworks.com/help/msblks/ug/successive-approximation-adc.html
https://www.mathworks.com/help/msblks/gs/DesignAndEvaluateSARADC.html


- Mixed-Signal Blockset (msblks)
  - [data-converters.html](https://www.mathworks.com/help/msblks/data-converters.html)
    - [saradc.html](https://www.mathworks.com/help/msblks/ref/)
   

## Nyquist ADC (⚡高速)

### Flash ADC

### SAR ADC

| Title                                                        | Author                 | Year | IEEE/Google Scholar |
| ------------------------------------------------------------ | ---------------------- | ---- | ------------------- |
| [A 10-bit 50-MS/s SAR ADC With a Monotonic Capacitor Switching Procedure](https://ieeexplore.ieee.org/document/5437496) | Chun-Cheng (Jason) Liu | 2010 | 1000/1500           |


### Pipeline ADC

#### Amp

##### Ring Amp by [Benjamin Hershberg](https://ieeexplore.ieee.org/author/37399879200)

- Benjamin Hershberg @ Intel
  - CICC 2020: Ringamp - The Scalable Amplifier We’ve All Been Waiting For?
    - video: [Ring Amplifier (Ringamp) Tutorial - YouTube](https://www.youtube.com/watch?v=uPFCcgjS5Zk)
    - slides: [PowerPoint Presentation](https://www.benjamin.hershberg.com/wp-content/papercite-data/slides/2020-cicc-invited-talk.pdf)
    - (the very first) paper: [Ring Amplifiers for Switched Capacitor Circuits, 2012, JSSC](https://ieeexplore.ieee.org/document/6373760)
  - Personal website: https://www.benjamin.hershberg.com/

### Clocking

The Speed–Power Trade-Off in the Design of CMOS True-Single-Phase-Clock Divider

## Oversampling ADC (🎯高精度)

### ΣΔ Modulation


## Sensor Interface & Biomedical IC


| University | Course No. | Year / WebSite                                              | Name                | Teacher         | Video | Slide |
| ---------- | ---------- | ----------------------------------------------------------- | ------------------- | --------------- | ----- | ----- |
| TU Delft   | EE1320     | [2013](https://ocw.tudelft.nl/courses/measurement-science/) | Measurement Science | Michiel Pertijs | OCW   | OCW   |
|            |            |                                                             |                     |                 |       |       |


- Kofi Makinwa & Michiel Pertijs @ TU Delft
  - ESSCIRC 2007 PLENARY: Smart sensor design: The art of compensation and cancellation
  - ISSCC 2008 Tutorial: CMOS Temperature Sensors
  - ISSCC 2010 Short Course: Designing Smart Sensors (in Standard CMOS)
  - ISSCC 2014 Tutorial: Design of Physical-to-Digital Converters
  - VLSI 2016 VLSIx Circuit Insights: Smart Sensor Design
- Fan Qinwen @ TU Delft
  - Webinar 2022: Evolution of precision amplifiers

### Chopping & Auto-Zeroing & Dynamic Element Matching (DEM)

- Kofi Makinwa @ TU Delft
  - ISSCC 2007 Tutorial: Dynamic-Offset Cancellation Techniques in CMOS
  - ISSCCedu 2016: Chopper Amplifier Demystified
  - ESSCIRCedu 2018: Auto-Zeroing Demystified
  - IEEE Sensors 2018: Capacitively-Coupled Chopper Instrumentation Amplifiers: an Overview
  - ISSCC 2022 Circuit Insights: Coping with Variability
  - ESSCIRC 2023 Circuit Insights: The Power of Averaging


[Chopping Amp in Cadence Virtuoso](https://www.youtube.com/watch?v=gF8sOlK7TM8)


## 参考

- https://www.zhihu.com/question/429625678
- https://www.zhihu.com/question/553117936 ⭐
- https://www.zhihu.com/question/502632221
- https://www.zhihu.com/question/478487601
- https://www.zhihu.com/question/590222455
- https://www.zhihu.com/question/433785533

资料收集原则：尽量只收集 2010 年及以后的资料，理由：

1. 再经典的资料也会过时的
