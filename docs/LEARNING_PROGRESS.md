# CGLab 学习进展（唯一进度事实来源）

> 本文件只记录**真实学习过程**。下面是初始状态，不代表已经完成第一课。

## Current State

| 字段 | 当前值 |
|---|---|
| Current Lesson | **L01 · CPU 帧缓冲与首张图像** |
| Status | `not_started` |
| Last Updated | `2026-10-27`（初始课程规划建立） |
| Goal | 自己在 C++17 中管理 RGB 像素，生成有效的 P6 PPM 图像 |
| Next Action | **阅读 `docs/lessons/L01_framebuffer.md`，回答图像像素索引问题，再创建自己的 `main.cpp`** |

## Completed / 已有证据的进展

- [x] `planned`：已建立 GAMES101 → CGLab 的课程和文档结构（仅**规划完成**，不是学习成绩）。
- [ ] `observed`：L01 C++ 程序成功编译（尚未实施/验证）。
- [ ] `observed`：L01 输出有效 P6 PPM 图像（尚未实施/验证）。
- [ ] `observed`：四角颜色和中心矩形检查通过（尚未实施/验证）。
- [ ] `user_reported/observed`：学生能够解释帧缓冲索引与图像坐标约定（尚未确认）。

## Evidence / 证据

| 日期 | 类型 | 事实 / 命令 / 文件 | 结果 |
|---|---|---|---|
| 2026-10-27 | `planned` | `docs/LEARNING_PLAN.md`、`docs/lessons/L01_framebuffer.md` | 课程资料已准备；**未运行任何课程代码** |

## Open Questions / 当前疑点

- 待实际开始：C++17 编译器与 CMake 在当前设备上的实际版本、配置是否正常。
- 待学生确认：索引 `(y*width+x)*3` 和图像 `y` 轴向下的含义。

## Lesson History / 课程记录

| Lesson | 状态 | 最后记录 | 备注 |
|---|---|---|---|
| L01 | `not_started` | 2026-10-27 | 未开始；课程卡片已建立 |
| L02–L28 | `not_started` | — | 尚未开始；参见 `docs/LEARNING_PLAN.md` |

## Session Log / 学习会话摘记（追加，不覆盖）

| 日期 | 课次 | 发生了什么 | 下一步 |
|---|---|---|---|
| 2026-10-27 | 规划 | 创建教学路线、Agent 规则与进度文档；无代码实验 | 开始 L01 |

---

维护说明：参考 [`PROGRESS_MAINTENANCE.md`](PROGRESS_MAINTENANCE.md)，每次编辑必须区分 `observed`、`user_reported` 和 `planned`。没有运行证据，不得勾选测试通过。
