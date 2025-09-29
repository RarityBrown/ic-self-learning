# Advanced Analog/RF/Mixed-Signal Topic for Graduate Student

为低年级研究生和学有余力的高年级本科生开始准备的高级主题，不过仍然是非科研性质，偏向于学习性质的内容。对于研究生层次的方向，因为行业内竞争和保密等原因，公开的教学资源更加稀少。除了本文，可以参考 analog 文件夹中分模块的介绍。

## 课程

| University             | Course No. | Year / WebSite                                               | Name                      | Teacher       | Slide     | Op-Amps             | ADC                                            |
| ---------------------- | ---------- | ------------------------------------------------------------ | ------------------------- | ------------- | --------- | ------------------- | ---------------------------------------------- |
| Boise State University | ECE614     | [2014](https://www.eecis.udel.edu/~vsaxena/courses/ece614/f14/Lectures.htm) | Advanced Analog IC Design | Vishal Saxena | available | CMFB + Differential | Switched-Capacitor, Comparators, Architectures |

## 常见模块

### 模拟/混合信号

#### Bootstrap

Move to ADDA

#### Dealing with Offset

##### Overview

- Kofi A. A. Makinwa @ TU Delft
  - ISSCC 2010 T6: Designing Smart Sensors
- Axel Thomsen @ Silicon Laboratories
  - ISSCC 2012 T8: Managing Offset and Flicker Noise

##### Chopper

- Kofi A. A. Makinwa @ TU Delft
  - Chopper Amplifiers Demystified 
    - [SSCS](https://resourcecenter.sscs.ieee.org/tags/chopper-amplifiers-demystified)
    - [中文讲解](https://zhuanlan.zhihu.com/p/20596750997)
- Qinwen Fan @ TU Delft
  - [Capacitively-Coupled Chopper Amplifiers](https://link.springer.com/book/10.1007/978-3-319-47391-8)

##### Auto-Zero

- Ali Sheikholeslami @ University of Toronto
  - [SSC-M](https://ieeexplore.ieee.org/document/7387869)
  - [中文讲解](https://zhuanlan.zhihu.com/p/24215780090)

##### DEM & correlated double sampling, etc.


#### Translinear loop

#### Reference

- [Current Reference Circuits: A Tutorial](https://ieeexplore.ieee.org/document/9314894) TCAS2
- [A Systematic Review of Voltage Reference Circuits: Spanning Room Temperature to Cryogenic Applications](https://ieeexplore.ieee.org/document/10786235) TCAS1

#### (Advanced) OpAmp


- Johan Huijsing @ TU Delft
  - book
    - *Operational Ampliers: Theory and Design (Third Edition)* 这老头好像研究了一辈子运放，所以这本书可以从题目中看出，就不是一本 Analog IC 的书，而是一本 OPAMP 的书
    - 书中的内容也涉及一些 chopper 之类的东西，没看过也看不懂

#### (Ultra) Low-Voltage Design / Sub-threshold Design

[A 60-dB Gain OTA Operating at 0.25-V Power Supply in 130-nm Digital CMOS Process](https://ieeexplore.ieee.org/document/6695792)

| Title                              | Year | Instructor     | Type     |
| ---------------------------------- | ---- | -------------- | -------- |
| Design of Voltage References       | 2013 | Wing-Hung Ki   | Tutorial |
| Designing Amplifiers for Stability | 2021 | Viola Schäffer | Tutorial |

### 射频

## 资料来源

### ISSCC

- ISSCC Tutorials, Short Course
  - 需要 SSCS Member，即需要付一点点费用，但是笔者认为物有所值，详见[SSCS](research.md#SSCS)
- ISSCCx (2015 only) & ISSCCedu (2018, 2019, 2020) & ISSCC Circuit Insights (2022, 2023, 2024, 2025)
  - 类似于公开课，但是 ISSCC 的委员会也不是很靠谱，几年一变名字。其中最靠谱的就是 2022 年，请来了一堆大佬（见下图）
  - 其他会议有类似的，但是也一样还不稳定，名字时常变化 [playlists](https://www.youtube.com/@IEEESolidStateCircuitsSociety/playlists)
    - VLSIx (VLSI Circuit Insights) 2016, VLSIedu (2019)
    - CICCx 2017, CICCedu (2019, 2020), CICC Educational Sessions
    - ESSERC Circuit Insights (2023, 2024)
    - ASSCC Circuit Insights (2024)

![image](https://github.com/user-attachments/assets/f13a2ac0-3435-45b9-a681-0cc53726c695)


|      | ISSCC                                                        | ESSERC | ASSCC |
| ---- | ------------------------------------------------------------ | ------ | ----- |
| 2025 | ![image](https://github.com/user-attachments/assets/d896dbb6-4ee7-44b7-bfb2-46ad9cfd5e37) |        |       |
| 2024 | ![image](https://github.com/user-attachments/assets/72dd7e55-d579-43c7-91d6-92734f54b6e6) | ![E2024](https://github.com/user-attachments/assets/23f15d87-ab41-4afd-a803-243469272110)  | ![A2024](https://github.com/user-attachments/assets/b20af13e-69ce-459b-aeb5-14e0c55f771b) |
| 2023 | ![image](https://github.com/user-attachments/assets/e184857f-699d-4402-a690-f0031094d8b3) |        |       |

- https://github.com/nishanchettri/ISSCC-Courses

### 其他付费学习资源

- https://store.hoomanreyhani.com/
- https://mead.ch/mead/
