# Research Communication: Academic Writing and Presentation

## Basic

- *How to Do Research in IC Design?*，胡诣哲
  - [Slides2024](https://bbs.eetop.cn/thread-962980-1-1.html) [Slides2025](https://bbs.eetop.cn/thread-992963-1-1.html) 

## Schematic & Diagramming

- *通过 Visio, Excel 和 Powerpoint 绘制电路图和仿真图*, 胡诣哲
  - [Slides & Samples](https://bbs.eetop.cn/thread-983425-5-1.html)

## Presentation

- Use Phrases, Not Sentences

### multipage

- *Giving Great Technical Talks*, Kofi Makinwa
  - [Slides](https://ei.et.tudelft.nl/docs/Makinwa_-_Giving_Great_Talks_2023.pdf)
- *Effective Technical Presentations: The How-To Guide*, Danielle Griffith, SSCS Webinars For Young Excellence
  - [YouTube Video](https://youtu.be/TW6m4jZd4yk?t=314)
- *ISSCC Regular Presentations (Template & Guide)* & *VLSI PowerPoint Guidelines and Template*
  - [2024 VLSI](https://archive.vlsisymposium.org/24web/author-instructions/) [2025 VLSI](https://www.vlsisymposium.org/authors/)
- *Giving a good ISSCC presentation, November 2007: Tips on how to prepare and give a good ISSCC talk*, Jan Van der Spiegel

做学术 slide 后的检查：

- [ ] 字体通用性
- [ ] 页码, 2 of *number of pages* 记得加上总页数
- [ ] 嵌入字体（有时反而不工作，需要再研究一下）
- [ ] 纯图片版 pptx
  - 自动工具？
- [ ] pdf 版
- [ ] `[Name, 2017, Boardcom, JSSC]`
- https://www.zhihu.com/question/6408584014/answer/1944745698500273497

### single page

#### One-Pager

#### Plan

Gantt Diagram

## Design Review

- *You Stink at Design Reviews!*, Chris Mangelsdorf
  - [SSC-M](https://ieeexplore.ieee.org/document/10752736)


Put in slides (for analog): 

- Results
  - Waveform screenshot
  - Average power, peak current
  - Schematic (testbench & DUT) / Layout screenshot
- Testbench settings
  - Path to testbench
  - `config` screenshot
  - `maestro` screenshot
  - `lock` and rename the final `history` simulation data

## Paper & Conference

- *Do's and Don'ts of Writing a Good Paper Recommendations from a Former Editor in Chief*, Bram Nauta, SSCS Webinars For Young Excellence
  - [YouTube Video](https://youtu.be/atxWbgOX454?t=305)
  - [Slides](https://resourcecenter.sscs.ieee.org/education/webinars/sscsweb3099)
- *Writing a good ISSCC paper, June 2024: Tips on how to increase the chances of paper acceptance*, Jan Van der Spiegel
  - [Slides](https://submissions.mirasmart.com/ISSCC2025/PDF/ISSCC2025_WritingGoodISSCCPaper.pdf)
- todo: 论文图表设计的色彩搭配理论，并结合色彩纠正和配色方案的定量分析


# Journals, Conferences and Symposiums List

## IEEE: Institute of Electrical and Electronics Engineers

> IEEE 电气电子工程师学会是全球最大的技术专业组织，涵盖电气、电子、计算机等众多工程领域。

### SSCS: Solid-State Circuits Society

> SSCS 固态电路学会是 IEEE 旗下的一个专业学会，专注于固态电路和系统（其实简而言之就是 IC）。ISSCC 是 SSCS 主办的年度会议，被公认是 IC 设计领域的最顶级学术会议。

SSCS 的 Student Member 中国区一年 $14+$5.5（IEEE + [SSCS](https://www.ieee.org/membership-catalog/productdetail/showProductDetailPage.html?product=MEMSSC037) Student Member 打包购买），支持支付宝、微信付款，非常建议购买，因为 SSCS Student Member 可以免费观看所有的 ISSCC Tutorials 和 ISSCC Short Course 视频，这些视频是非常好的学习资源。当然也有一些省钱的操作，比如在[三月后](https://cn.ieee.org/membership_join/)购买 Student Member 只收半年的钱。

然后话说回来，ieeetv.ieee.org 上的视频链接是直接走 IEEE 网站的流量，不做鉴权的。比如说 [ISSCC 2016](https://ieeetv.ieee.org/ondemand/2016-isscc-tutorials/1702/basics-of-sar-adcs-circuits-architectures-video) 显示需要会员才能播放，但是买会员后 F12 一看发现直接就是 .mp4 公开的链接。而 sscs.ieee.org 的[视频](https://resourcecenter.sscs.ieee.org/education/short-courses/sscstut20160090)则走的是 Amazon 的 CDN，至少不是一个 F12 就可以无权限访问的。不过有权限了以后还是随便下载，改天搞个爬虫，，，

注册会员后记得到邮件设置去[关闭](https://github.com/RarityBrown/ieee-unsubscribe)所有不需要的邮件，不然 IEEE 三天两头你发邮件，整个邮箱像 IEEE 的垃圾堆一样。

期刊：JSSC, SSC-L

会议：ISSCC

#### VLSI

VLSI often refers to the following two:

- *Symposium on VLSI Technology and Circuits*
  - Symposium on VLSI Technology + Symposium on VLSI Circuits (VLSIC, VLSI Circuits)
  - VLSI Technology and Circuits
  - ISSCC > VLSI
- *Transactions on VLSI Systems*
  - TVLSI ≲ TCASII

NOT *International Conference on VLSI Design* (VLSID) or *Computer Society Annual Symposium on VLSI* (ISVLSI)

### 总结

对于 IC 设计领域而言：

| 学会 (Society)                                     | 顶刊   | 次顶刊           | 其他刊               | 顶会                                                        | 次顶会                                                       |
| :------------------------------------------------- | :----- | ---------------- | -------------------- | :---------------------------------------------------------- | ------------------------------------------------------------ |
| **SSCS** (Solid-State Circuits Society)            | JSSC   | SSC-L            | OJ-SSCS              | ISSCC (9月初截稿, 2月开会), <br />VLSI (2月初截稿, 6月开会) | ESSERC (4月截稿, 9月开会), <br />CICC (11月截稿, 4月开会), <br />ASSCC (6月截稿, 11月开会) |
| **CAS** (Circuits and Systems Society)             | TCAS-I | TCAS-II, TBioCAS | TVLSI, OJCAS, TCASAI | ISCAS                                                       | [ISICAS](https://www.zhihu.com/question/559252881/answer/2716642993), BioCAS |
| **MTT-S** (Microwave Theory & Techniques Society)  | TMTT   |                  |                      | RFIC Symposium (1月中截稿, 6月开会), <br /> IMS          |                                                              |
| **PELS** (Power Electronics Society)               | TPEL   |                  |                      | APEC                                                        |                                                              |
| **CEDA** (Council on Electronic Design Automation) | TCAD   |                  |                      | DAC                                                         | ICCAD                                                        |

对于 IC 器件和工艺领域而言：

todo
