# CGLab — 从零亲手实现计算机图形学算法 ^_^

> 一个**以 GAMES101 为主线、以学生亲手编码为核心**的项目式计算机图形学学习仓库。

## 我们的学习约定

- **算法自己写**：Agent 是老师与代码审阅者，不会替你完成核心课程代码。
- **每节课一个完整主题**：学完有一张图、一段动画、一个小实验或性能对照。
- **原理 → 数学 → 数据结构 → 代码 → 测试 → 复盘**。
- **不赶进度**：课程按学习质量推进，而非聊天轮数推进。
- **语言**：C++17 为主，CMake 构建；必要时利用 Python 做独立的数据可视化，不用黑盒代替算法。

## 从哪里开始

1. **人和 Agent 都先读** [`AGENTS.md`](AGENTS.md)。
2. 课程总体路线：[`docs/LEARNING_PLAN.md`](docs/LEARNING_PLAN.md)。
3. 当前进度：[`docs/LEARNING_PROGRESS.md`](docs/LEARNING_PROGRESS.md)。
4. 第一节课：[`docs/lessons/L01_framebuffer.md`](docs/lessons/L01_framebuffer.md)。
5. 教学互动规范：[`docs/AGENT_TEACHING_GUIDE.md`](docs/AGENT_TEACHING_GUIDE.md)。
6. 进度维护规范：[`docs/PROGRESS_MAINTENANCE.md`](docs/PROGRESS_MAINTENANCE.md)。
7. GAMES101 官方来源索引：[`docs/RESOURCE_MAP.md`](docs/RESOURCE_MAP.md)。
8. 跨设备的本地初始化：[`docs/PROJECT_SETUP.md`](docs/PROJECT_SETUP.md)。

## 代码和文档目录如何配合

- `src/lessons/LXX_<topic>/`：每课独立入口，自行写 `.cpp/.hpp`；可编译为单独 target。
- `src/core/`：真正反复使用的公共数据结构与算法。**先写每课，再在重构时提炼**，不要 L01 就搭一整个引擎。
- `tests/`：小规模确定性测试/边界测试。
- `assets/official/`：自行下载的 GAMES101 官方作业资料，仅供本地参考，默认不提交。
- `outputs/`：渲染输出、临时图、构建产物，默认不提交。
- `results/`：挑选的、轻量可复现的课程成果（可选择提交）。
- `docs/notes/`：手写数学推导、踩坑与结果分析。
- `.agents/skills/`：Codex 等 Agent 的可复用教学和进度技能。

> 仓库创建时**不预先提供任何课的完整 C++ 实现**；L01 的代码由你开始写。

## 课程出处与边界

本学习仓库为个人教学规划，**不是 GAMES101 官方课程、教材或自动评分系统**。

- [GAMES101 官网](https://sites.cs.ucsb.edu/~lingqi/teaching/games101.html)
- [官方 PPT / 视频索引](https://games-cn.org/graphics-intro-ppt-video/)
- [官方作业发布汇总](https://games-cn.org/forums/topic/allhw/)

官方课件与作业框架仍应从原站下载；该仓库以链接引用、独立编写原创代码，不批量再分发第三方课程文件。
