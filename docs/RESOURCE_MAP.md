# GAMES101 · 官方课件、作业与来源核对表

> 建立日期：2026-10-27 · **课程素材请从原站下载，CGLab 不再分发原 PDF/ZIP。**

## 1. 最重要的官方入口

- [GAMES101 官方课程主页（22 讲大纲）](https://sites.cs.ucsb.edu/~lingqi/teaching/games101.html)
- [GAMES101 PPT 与视频目录（含百度网盘备份）](https://games-cn.org/graphics-intro-ppt-video/)
- [GAMES101 往期作业 0–8 汇总帖](https://games-cn.org/forums/topic/allhw/)
- [GAMES101 官方 BBS](https://games-cn.org/forums/forum/graphics-intro/)
- [Lecture 04 投影的补充手写推导（PDF）](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_04_supp.pdf)

**内容事实与 CGLab 取舍**：官网把课程定位为图形学原理导论，包含光栅化、几何表示、光的传播、动画和模拟，刻意不以 OpenGL 等特定 API 为重点。课程页列出 22 讲，并说明有 8 次小作业、1 次大作业；作业汇总帖列出编号 0 到 8 的发布链接。CGLab 将 22 讲重组为 **28 节自编项目课**，与官方讲次和作业不一一等价。

## 2. 22 讲官方讲义索引

下列标题依官方课表/课程 PPT 页面归纳；点击直达相应 PDF。若 PDF 因文件过大或网络原因打不开，请返回上方官方 PPT 与视频索引选备份。

| 原课程讲次 | 主题 | 课件 PDF |
|---|---|---|
| Lecture 01 | Overview of Computer Graphics（图形学概述） | [原课件 01](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_01.pdf) |
| Lecture 02 | Review of Linear Algebra（线性代数） | [原课件 02](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_02.pdf) |
| Lecture 03 | Transformation（基础变换） | [原课件 03](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_03.pdf) |
| Lecture 04 | Transformation Cont.（MVP / 投影） | [原课件 04](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_04.pdf) |
| Lecture 05 | Rasterization 1 (Triangles)（三角形光栅化） | [原课件 05](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_05.pdf) |
| Lecture 06 | Rasterization 2 (Antialiasing and Z-Buffering)（抗锯齿、深度） | [原课件 06](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_06.pdf) |
| Lecture 07 | Shading 1 (Illumination, Shading and Graphics Pipeline) | [原课件 07](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_07.pdf) |
| Lecture 08 | Shading 2 (Shading, Pipeline and Texture Mapping) | [原课件 08](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_08.pdf) |
| Lecture 09 | Shading 3 (Texture Mapping Cont.) | [原课件 09](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_09.pdf) |
| Lecture 10 | Geometry 1 (Introduction) | [原课件 10](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_10.pdf) |
| Lecture 11 | Geometry 2 (Curves and Surfaces) | [原课件 11](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_11.pdf) |
| Lecture 12 | Geometry 3 (Mesh Operations and Shadows) | [原课件 12](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_12.pdf) |
| Lecture 13 | Ray Tracing 1（求交与基本追踪） | [原课件 13](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_13.pdf) |
| Lecture 14 | Ray Tracing 2（加速结构） | [原课件 14](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_14.pdf) |
| Lecture 15 | Ray Tracing 3（辐射度量学 / 渲染方程） | [原课件 15](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_15.pdf) |
| Lecture 16 | Ray Tracing 4（蒙特卡洛 / 路径追踪） | [原课件 16](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_16.pdf) |
| Lecture 17 | Materials and Appearances（材质与外观） | [原课件 17](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_17.pdf) |
| Lecture 18 | Advanced Topics in Rendering（高级渲染） | [原课件 18](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_18.pdf) |
| Lecture 19 | Cameras, Lenses and Light Fields（相机与光场） | [原课件 19](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_19.pdf) |
| Lecture 20 | Color and Perception（颜色与感知） | [原课件 20](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_20.pdf) |
| Lecture 21 | Animation（动画与模拟基础） | [原课件 21](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_21.pdf) |
| Lecture 22 | Animation Cont.（数值积分、刚体与流体等） | [原课件 22](https://sites.cs.ucsb.edu/~lingqi/teaching/resources/GAMES101_Lecture_22.pdf) |

## 3. 官方作业发布帖与 CGLab 对齐关系

**提醒**：表中“主题”是常见的课程作业概括，用于确定学习路线；不是对每一份原作业 PDF 的逐条复现，也不是官方评分标准。正式原题、附带文件和细则以每个发布帖中的下载包为准。**作业 3 有更正包，优先使用更正版本。**

| 作业 | 主题概括 | 对应 CGLab | 官方出处 |
|---|---|---|---|
| PA0 | 入门准备与编程环境 | L01 开始前/期间（非同一题） | [作业 0 发布帖](https://games-cn.org/forums/topic/graphics-intro-hw0/) |
| PA1 | 旋转与投影 | L03–L04 | [作业 1 发布帖](https://games-cn.org/forums/topic/graphics-intro-hw1/) |
| PA2 | 三角形光栅化、Z-buffer、抗锯齿 | L05–L07 | [作业 2 发布帖](https://games-cn.org/forums/topic/graphics-intro-hw2/) |
| PA3 | 流水线和着色 | L08–L11 | [作业 3 更正公告](https://games-cn.org/forums/topic/%E4%BD%9C%E4%B8%9A3%E6%9B%B4%E6%AD%A3%E5%85%AC%E5%91%8A/) |
| PA4 | Bézier 曲线 | L14 | [作业 4 发布帖](https://games-cn.org/forums/topic/graphics-intro-hw4/) |
| PA5 | 光线与几何体求交 | L17–L18 | [作业 5 发布帖](https://games-cn.org/forums/topic/graphics-intro-hw5/) |
| PA6 | 包围盒层次与加速 | L19 | [作业 6 发布帖](https://games-cn.org/forums/topic/graphics-intro-hw6/) |
| PA7 | 路径追踪 | L21–L23 | [作业 7 发布帖（含常见问题）](https://games-cn.org/forums/topic/graphics-intro-hw7/) |
| PA8 | 质点弹簧系统 | L27 | [作业 8 发布帖](https://games-cn.org/forums/topic/graphics-intro-hw8/) |

### 资料使用建议

- 初学阶段**先做 CGLab 的小型自编任务**，已经理解数学与代码结构后，再在本课结尾打开对应原作业框架对照。
- 不要求先安装 2020 年课程虚拟机。先在自己的 Linux/Windows 上配置新环境；仅遇到特定依赖问题再向官方原框架回溯。
- 原作业的下载 ZIP 可能包含 C++ 源码、PDF 描述、资产和构建配置，按原站许可仅作学习参考；不要把它们当成个人原创代码提交。
- GAMES101 课程页面提到作业提交曾经结束，旧 SmartChair 链接与截止时间**不能默认仍有效**；CGLab 自己验收。

## 4. 核对范围与限制（重要）

在制定此路线时，核对了课程主页 22 讲主题、PPT/视频官方汇总、PA0–PA8 的官方发布页面，以及 Lecture 03、04、05 的可检索 PDF 文字与关键页图像、Lecture 04 补充手写推导。部分较大的课件（例如 Lecture 11、16、21）受在线浏览器文件大小限制，未逐页读取；原始作业 ZIP 只能从页面识别其链接，无法在当前检索环境直接解包逐项核对。因此 **28 节路线是基于官方大纲与部分原始材料的教学重组，而不是对全部课件和全部作业源代码逐行审阅**。后续实际进入某一课时，应打开对应原课件或已下载的原作业，核实细节。

特别注意：Lecture 05 中明确介绍 Frame Buffer、屏幕像素坐标和三角形像素中心采样，这也是先安排 L01 帧缓冲再安排 L05 光栅化的理由。

## 5. 课程结束后的参考方向（非当前必学）

- 想进一步学习几何处理：GAMES102。
- 想进一步学习物理模拟：GAMES103。
- 想学习现代实时渲染：GAMES202 / 现代图形流水线相关课程。

这些仅是未来选修建议；当前的 28 节优先夯实基础，不提前开额外项目。
