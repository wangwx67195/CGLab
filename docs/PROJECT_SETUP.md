# CGLab 工程初始化、多设备同步与工具选择

目标：尽可能**简单且跨设备**，不给第一节课引入 GUI、Vulkan、驱动或复杂依赖问题。

## 1. 建议技术栈

| 目的 | 首选 | 为什么 |
|---|---|---|
| 核心算法 | C++17 标准库 | 与 GAMES101 原始 C++ 作业相容；可直接接触内存布局和性能 |
| 构建 | CMake 3.16+（建议） | Linux/Windows/macOS 能统一管理各课可执行文件 |
| 编辑器 | VS Code 或其他 | 不绑定 IDE |
| 数学辅助 | **先自行实现简易 Vec2/Vec3/Mat，后按需引入 Eigen3** | 避免一开始被库掩盖数学含义 |
| 早期图片输出 | 二进制 PPM（P6） | C++ 标准库即可写出，不需要 OpenCV |
| 实验对照 | 图片浏览器、命令行、少量 pytest/Python（可选） | 工具服务于验证，而非代替算法 |
| 版本控制 | Git + GitHub | 进度文档、原始代码和少量结果跨设备同步 |

Windows 用户建议安装 C++ 编译器和 CMake，并使用 VS Code CMake Tools（可选）；具体安装方式根据平台现状确认，不硬编码环境路径。

## 2. 放到目标目录

本资料包解压后目录应是 `~/project/CGLab/`（若已有同名目录，请先备份并**人工合并**，不要覆盖已有进展）：

```bash
mkdir -p ~/project
unzip CGLab_learning_kit.zip -d ~/project
cd ~/project/CGLab
```

如本机习惯使用 `~/projects/`（复数），请遵从用户明确指定的 `~/project/CGLab`；不要帮用户悄悄改路径。

## 3. Git 仓库初始化（尚未建立时）

```bash
cd ~/project/CGLab
git init -b main
git add .
git commit -m "docs: initialize graphics learning lab"
```

在 GitHub 网站建立一个**空仓库** `CGLab`（不提前创建 README/.gitignore，以减少冲突），取得你自己账号下的地址，然后运行：

```bash
git remote add origin git@github.com:YOUR_ACCOUNT/CGLab.git
git push -u origin main
```

如果系统安装并登录 `gh`，也可以选择 `gh repo create CGLab --source=. --remote=origin --push --private`（是否公开由用户自己决定）。请根据登录状态、仓库是否已存在来选择，不要同时机械执行两种方案。

## 4. 第一次上课时创建代码与构建配置

不提供整份可复制的 C++ 题解和 CMake 脚手架。L01 学生应亲手建立：

- `src/lessons/L01_framebuffer/main.cpp`：实现 RGB 缓冲区、像素绘制和 PPM 写出。
- 根目录 `CMakeLists.txt`：先学会给 L01 定义一个名为 `cglab_l01` 的 executable target；建议 C++17。
- `tests/`：可先写手工检查脚本/说明，后续逐渐改为自动测试。
- `outputs/`：运行前确保目录存在，或在程序中检查创建目录是否成功；渲染文件不会默认上传 Git。

本课会实际用到的构建命令：

```bash
cmake -S . -B build
cmake --build build
```

可执行文件**准确路径取决于平台和 CMake generator**；首次构建后让 Agent 帮忙确认，而不是假定它一定在某个路径。

## 5. 推荐的 CMake 组织策略

- L01–L03：每课独立一个可执行程序；简单优先。
- L04 起：`src/core/` 中出现至少两处重复且稳定的基础类型时，再抽成库或公共源码。
- 不在第一天安装 OpenGL / Vulkan / CUDA；先把算法本身跑通。
- 大作业/参考代码放 `assets/official/` 或单独仓库，不要混同为学生原创实现。
- 需要 Eigen3 的课再引入；由 Agent 解释 API，避免把矩阵推导课程变成库调用演示。

## 6. 多设备同步建议

操作前检查：

```bash
git status
git remote -v
```

- 工作树干净时，按自己的工作流程 `git pull --rebase`（或普通 pull），确认无冲突后再开始。
- 写完后 `git add`、`git commit`、`git push`；只提交源代码、文档和挑选的小型结果。
- 未提交更改或提示冲突时**不要直接强行覆盖**；先理解差异，再选择提交、暂存或人工合并。
- `.gitignore` 排除 `build/`、`outputs/`、下载的大型第三方资源以及编辑器临时文件。`results/` 用于有意义的轻量成果。

## 7. 一条开课时给本地 Agent 的示范指令

> 你是 CGLab 的图形学老师，请先阅读根目录 `AGENTS.md`、`docs/LEARNING_PROGRESS.md`、`docs/LEARNING_PLAN.md` 和当前课程卡片。按照 `docs/AGENT_TEACHING_GUIDE.md` 开始本课：先讲必要原理和数学，再明确我需要亲手完成的代码任务与验收方法。不要直接写出完整核心算法代码；如果涉及 C++/CMake API，给我最小局部示例与常见错误。只有实际学习进度改变时，才根据 `docs/PROGRESS_MAINTENANCE.md` 更新进度。
