# Advanced Analog/RF/Mixed-Signal Topic for Graduate Student

为低年级研究生和学有余力的高年级本科生开始准备的高级主题，不过仍然是非科研性质，偏向于学习性质的内容。对于研究生层次的方向，因为行业内竞争和保密等原因，公开的教学资源更加稀少。除了本文，可以参考 analog 文件夹中分模块的介绍。

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

Johan Huijsing @ TU Delft

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

### 其他

- https://store.hoomanreyhani.com/
- https://mead.ch/mead/

## Analog/Mixed-Signal/RF EDA

### SPICE & BSIM

### Spectre by Cadence: Kenneth S. Kundert @ UC Berkeley → Cadence 

- [Life After SPICE](https://ieeexplore.ieee.org/document/6051611)
- [Simulation of Nonlinear Circuits in the Frequency Domain](https://ieeexplore.ieee.org/document/1270223)
- [Steady-State Methods for Simulating Analog and Microwave Circuits](https://link.springer.com/book/10.1007/978-1-4757-2081-5)
- [The Designer’s Guide to Spice and Spectre®](https://link.springer.com/book/10.1007/b101824) 有许建超（西安交通大学）的电子译本
- [The Designer’s Guide to Verilog-AMS](https://link.springer.com/book/10.1007/b117108)
- [Introduction to RF simulation and its application](https://ieeexplore.ieee.org/document/782091)
- [Striving for small-signal stability](https://ieeexplore.ieee.org/document/900125)

### MATLAB & Simulink

- Mathworks 官方课程 / 功能介绍视频
  - 免费
    - [Simulink Onramp](https://matlabacademy.mathworks.com/details/simulink-onramp/simulink)
    - [Mixed-Signal Blockset](https://www.mathworks.com/products/mixed-signal.html)
      - [Mixed-Signal Data Analysis with MATLAB](https://www.mathworks.com/videos/series/mixed-signal-data-analysis-with-matlab.html)
      - [Understanding Phase Locked Loop with Mixed-Signal Blockset](https://www.mathworks.com/videos/pll-loop-parameter-estimation-68728.html)
      - ...
  - 付费
    - [Simulink for Analog Mixed-Signal Design](https://www.mathworks.com/learn/training/simulink-for-analog-mixed-signal-design.html)



### EDA List

| Full Custom (Analog)                  | Cadence                                         | Synopsys                            | [Siemens](https://www.sw.siemens.com/en-US/technology/electronic-design-automation-eda/) (Mentor) | Keysight                         | Empyrean 华大九天 |
| ------------------------------------- | ----------------------------------------------- | ----------------------------------- | ------------------------------------------------------------ | -------------------------------- | ----------------- |
| Solution                              | **Virtuoso Studio**                             | Custom Compiler                     | Tanner                                                       | Advanced Design System (ADS)     | Aether            |
| Platform (Environment)                | **Virtuoso Analog Design Environment (ADE)**    | PrimeWave Design Environment        | Solido Design Environment                                    |                                  |                   |
|                                       |                                                 |                                     |                                                              |                                  |                   |
| SPICE                                 | **Spectre** (Classic)                           | **PrimeSim HSPICE**, PrimeSim SPICE | Eldo, Solido SPICE                                           |                                  | ALPS              |
| 1st Gen FastSPICE                     | **Spectre APS**                                 |                                     | Analog FastSPICE (AFS) (*Berkeley Design Automation*)        |                                  |                   |
| 2nd Gen FastSPICE                     | **Spectre X**                                   | PrimeSim Pro                        | AFS eXTreme (AFS XT), Solido FastSPICE                       |                                  | **ALPS GT**       |
| RF SPICE (RF FastSPICE)               | **Spectre RF, Spectre FX**                      | PrimeSim SPICE                      | AFS RF                                                       |                                  | ALPS RF           |
| RC Extraction (2D EM Simulation)      | Quantus                                         | StarRC                              | Calibre xRC                                                  |                                  |                   |
| 2.5D EM Simulation (Planar 3D)        | **EMX** (*Integrand*)                           | RaptorH (RaptorX) (*Ansys*)         | Calibre xACT 3D                                              | RFPro\*, **ChannelSim (SerDes)** |                   |
| 3D EM Simulation (Full-Wave 3D)       | Clarity (for packaging)                         | **HFSS** (*Ansys*)                  | HLAS (for packaging)                                         | **EMPro**                        |                   |
| AMS Simulation                        | Spectre AMS + Xcelium                           | VCS AMS                             | Symphony, Questa ADMS                                        |                                  |                   |
|                                       |                                                 |                                     |                                                              |                                  |                   |
| Schematic / Layout Editor             | Virtuoso Schematic Editor XL / Layout Suite MXL |                                     | Tanner S-Edit / L-Edit                                       |                                  | Aether SE / LE    |
| Layout Automation                     | **Animate** (*Pulsic*)                          |                                     |                                                              |                                  |                   |
| Viewer                                | Virtuoso Visualization & Analysis (ViVA) XL     | Custom WaveView                     | Swave                                                        |                                  | iWave             |
| Cell                                  | Spectre Characterization Simulator              | PrimeLib                            | Solido Variation Designer                                    |                                  |                   |
|                                       |                                                 |                                     |                                                              |                                  |                   |
| Physical Verification (DRC, ERC, LVS) | Assura / Pegasus                                | IC Validator                        | **Calibre**                                                  |                                  |                   |

> \* FEM + Momentum 方法
>
> Planar 3D: 矩量法 (MoM - Method of Moments)
>
> Full-Wave 3D: 有限元法 (FEM - Finite Element Method) + 时域有限差分法 (FDTD - Finite Difference Time Domain)
>
> https://zhuanlan.zhihu.com/p/28550045
