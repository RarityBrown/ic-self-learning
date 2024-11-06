# Digital IC Learning Resouces

- 虽然大概率以后就是做 analog 的了，但是和 digital 因电源时钟离不开 analog 类似，analog 因接口测试离不开 digital，所以也得学习啊
- 国内高校普遍使用 *Digital Integrated Circuit: A Design Perspective* 这本又老又底层的书，对于 Verilog 和 Architecture 的内容介绍几乎为零，从现代的角度看与其说是 design perspective 的，不妨说是 EDA perspective 的。另一本国内高校普遍使用的 Verilog 书过度关注于语法，而且太老，不适合用于学习
- 建议的 prerequisite 和 EECS 151 一致：数电、计组，也非常建议考虑用 AI 辅助学一学 Verilog 基础的语法
- 本文目前主要关注数字前端，如果有空可能会放一些数字后端的东西，不过这个似乎也是 EDA perspective 的东西，没有什么“知识”

## HDL Language

- Verilog 而不是 VHDL：ref: *Language Wars in the 21st Century: Verilog versus VHDL*
- Verilog 而不是 Chisel 等 HLS：~~不要被做体系结构的人拐跑了（说的就是一生一芯）~~
- Verilog 而不是 SystemVerilog：面向初学者的 SystemVerilog 的优质课程或教材较少，往往假设读者有 Verilog 背景；而且面向验证的内容多，面向设计的内容少
  - [RTL Modeling with SystemVerilog for Simulation and Synthesis by Stuart Sutherland](https://www.sutherland-hdl.com/books_and_guides.html) 作者去世
  - 当然，如果准备在数字方向上深造的话近年来可能还是 SystemVerilog 为主了，当然，这只是我一个数字外行人的想法罢了

## Courses

- EECS 151/251A by John Wawrzynek, UC Berkeley（BiliBili 上有转载）
- ELEC 4200 by Ujjwal Guin, Auburn University（顺带一提，Google 联想 Tim Cook 是校友，这学校感觉很不出名啊，也是因为 Google 到 slides 后一看内容感觉很好才发现的）

## Books

EECS 151/251A 第一节课就提到，没有特别适用的书，*Digital Design and Computer Architecture* 太浅而 *A Design Perspective* 太底层。另一个国内比较主流的选择是 *Advanced Digital Design with the Verilog HDL*，我总体读下来感觉代码有得挺好，但也有部分 HDL 代码存在不可综合等问题，不过总体而言还是比前两本书适合不少了。搜索相关参考书的关键词应当是 Digital Design 而不是 Digital IC，后者容易进入数字后端所关注的重点。

总体而言建议的重点参考资料是：

|                                                              | 英/中文版 电子版   | 英文版出版年份 | 深度（难度）                     |
| ------------------------------------------------------------ | ------------------ | -------------- | -------------------------------- |
| Advanced Digital Design with the Verilog HDL, 2nd edition    | 扫描版；扫描版     | 2011           | ★★★★★                            |
| Digital Design: A Systems Approach                           | 扫描版；扫描版     | 2012           | ★★★★<br />(Part IV 即第 14 章后) |
| Digital Design: Principles and Practices, 5th edition        | 原版；扫描版       | 2018           | ★★★                              |
| Digital Design and Computer Architecture, RISC-V edition     | 原版；非 RISC-V 版 | 2021           | ★★★                              |
| Digital Logic Circuit Analysis and Design, 2nd edition       | 找不到；无翻译     | 2020           | to read                          |
| HDL Compiler for Verilog User Guide (Synopsys)               | 最新公开版本       | 2023           | ★★★★                             |
| Advanced Chip Design, Practical Examples in Verilog          | 不售               | 2013           | to read                          |
| [Cliff Cummings' Verilog & SystemVerilog Papers](http://www.sunburst-design.com/papers/) |                    |                | ★★★★★                            |

这些资料（几乎）不涉及晶体管级而且不仅仅介绍 HDL 语法。另外，第一本书的作者最近去世了，可能再也不会更新版本了；其他几本书的情况也是类似，作者往往都七老八十，人走几年后书也就随风飘散了。真是期待哪一天能大一统，联合起来搞上下两册书，一本入门一本精进就完美了。毕竟数字设计已经如此成熟，而且相较于模拟自由度也不高。

- Advanced Digital Design with the Verilog HDL, 2nd edition: 采用 ASM 图作为状态机的表示，不是很主流。

- Digital Design: A Systems Approach
  - Part IV Synchronous sequential logic
    - Sequential logic
    - Timing constraints
    - Datapath sequential logic
    - Factoring finite-state machines
    - Microcode
    - Sequential examples
- Digital Design: Principles and Practices
  - 

一些与 FSM 编码格式相关的资料：

- [有限状态机 FSM 设计 by Qian Gu](https://qian-gu.github.io/posts/ic/fsm-design.html)：总结程度高，上手就能用，不过隐去了一些细节
- [状态机设计 by foveryoung](https://bbs.eetop.cn/thread-273600-1-1.html)：其参考文献丰富、深刻，有时间值得全部阅读


一些比较新的可参考的资料：

- [Digital VLSI Design with Verilog: A Textbook from Silicon Valley Polytechnic Institute](https://link.springer.com/book/10.1007/978-3-319-04789-8) by John Michael Williams
- [FPGA-Based Prototyping Methodology Manual](https://www.synopsys.com/company/resources/synopsys-press/fpga-based-prototyping-methodology-manual.html) by Synopsys
- [FPGA Prototyping by SystemVerilog Examples: Xilinx MicroBlaze MCS SoC Edition](https://www.wiley.com/en-us/FPGA+Prototyping+by+SystemVerilog+Examples%3A+Xilinx+MicroBlaze+MCS+SoC+Edition-p-9781119282662) by Pong P. Chu

以及一些国内的书：

- 数字 IC 设计入门
- 数字系统设计与 Verilog HDL

还有一本比较有特色的书：

Designing Video Game Hardware in Verilog


## 一些其他资源

一些刷题网站：

- https://verilogoj.ustc.edu.cn/oj/
- HDLBits
- 牛客


一些 GitHub 大学资源：

- https://github.com/hustrlee/HUST-Verilog-Course


一些知乎资源：

- https://www.zhihu.com/question/21892919
- https://www.zhihu.com/question/54815861
- https://www.zhihu.com/question/403640698


一些工具资源

- [StarVision PRO (concept.de)](https://www.concept.de/StarVision.html)
- https://www.sigasi.com/
- https://github.com/Digital-EDA/Digital-IDE
- 使用 yosys 的在线综合网站：https://digitaljs.tilk.eu/
