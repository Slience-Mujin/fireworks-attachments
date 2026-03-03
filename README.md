# fireworks-attachments 🔥

[![License: MPL-2.0](https://img.shields.io/badge/License-MPL--2.0-blue.svg)](https://opensource.org/licenses/MPL-2.0)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/Content-CC%20BY--NC--SA%204.0-green.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

> 哈尔滨工业大学课程附件资源仓库

## 📂 仓库简介

本仓库是 [薪火笔记社 (fireworks-notes-society)](https://github.com/HIT-Fireworks/fireworks-notes-society) 的**附件资源仓库**，用于托管每门课程的附件文件资源（主要以 PDF 为主）。

由于 Git 对大文件支持有限，且主仓库采用 VitePress 构建文档站点，本仓库作为独立的附件存储仓库，与主仓库配合使用，为课程笔记提供配套的教材、课件、习题解答等资源支持。

### 📦 PDF 压缩工具

本仓库使用 [fireworks-pdf-compressor-ml](https://github.com/jiwangyihao/fireworks-pdf-compressor-ml) 对大体积 PDF 进行压缩处理，以满足 GitHub 仓库的托管要求（小于 100MB）。

**fireworks-pdf-compressor-ml** 是一个面向 GitHub 仓库托管场景的 PDF 优化工具，采用多阶段压缩流水线：

- **阶段一（无损优先）**：结构清理、Ghostscript 重排，安全图片压缩
- **阶段二（有损交错）**：矢量压缩 → 图片压缩 → 切片压缩，逐步增强压缩各种复杂的 PDF 类型强度

支持处理，包括：
- 板写笔记 / 课件（矢量元素多）
- 扫描件 / 图片型 PDF
- 灰度页面（混合切片保留灰度细节）

## 🔗 相关链接

- 🌐 **主站**: [https://fireworks.jwyihao.top/](https://fireworks.jwyihao.top/)
- 📚 **主仓库**: [github.com/HIT-Fireworks/fireworks-notes-society](https://github.com/HIT-Fireworks/fireworks-notes-society)
- 📦 **本仓库**: [github.com/HIT-Fireworks/fireworks-attachments](https://github.com/HIT-Fireworks/fireworks-attachments)
- 🔧 **PDF 压缩工具**: [github.com/jiwangyihao/fireworks-pdf-compressor-ml](https://github.com/jiwangyihao/fireworks-pdf-compressor-ml)

## 📁 目录结构

```
fireworks-attachments/
├── 【公共课】/                    # 全校公共必修课
│   ├── 【公共课】习概/           # 习近平新时代中国特色社会主义思想概论
│   ├── 【公共课】大学化学/       # 大学化学
│   ├── 【公共课】大学物理/       # 大学物理
│   ├── 【公共课】工科数学分析/   # 微积分
│   ├── 【公共课】思想道德与法治/ # 思政
│   ├── 【公共课】概率论与数理统计/
│   ├── 【公共课】毛概/          # 毛泽东思想和中国特色社会主义理论体系概论
│   ├── 【公共课】电路类课程/    # 电路、数字电子技术、模拟电子技术
│   ├── 【公共课】线性代数与空间解析几何/
│   ├── 【公共课】计算思维与人工智能/
│   ├── 【公共课】近现代史纲要/
│   ├── 【公共课】马克思主义原理/
│   ├── 【工科公共课】工程制图/
│   └── 【工科公共课】理论力学/
│
├── 数学学院/                      # 数学学院专业课
│   ├── 专业基础课/               # 数学分析、高等代数、复变函数、实变函数等
│   └── 细分专业课/               # 信息与计算科学、数理统计等
│
├── 物理学院/                      # 物理学院专业课
│   ├── 专业基础课/               # 光学、力学、热学、电磁学、量子力学等
│   └── 细分专业课/               # 信息光学、激光原理等
│
├── 交通科学与工程学院/            # 交通学院专业课
│   ├── 交通工程/
│   ├── 交通管理/
│   └── 智能交通导论/
│
├── 土木工程学院/                   # 土木学院专业课
├── 未来技术学院/                   # 未来技术学院专业课
├── 机电工程学院/                   # 机电学院专业课
├── 化工与化学学院/                 # 化工学院专业课
├── 环境学院/                       # 环境学院专业课
├── 生命科学和医学学部/             # 生命学院专业课
├── 人文社科学部/                   # 人文社科专业课
├── 经管学院/                       # 经管学院专业课
├── 仪器学院/                       # 仪器学院专业课
│
├── 校内资源/                       # 校内公共资源
│   └── 材料科学与工程学院/         # 材料学院部分资源共享
│
├── 薪火笔记社-PPT及报告模板/       # 答辩模板、报告封面模板
├── 薪火笔记社-竞赛/               # 竞赛资料、建模、美赛论文
│
└── 询问中/                        # 待整理分类的资源
```

## 📖 内容分类

每门课程的资源通常包含以下类型：

- **电子教材** - 课程配套教材 PDF
- **课程笔记** - 课堂笔记、复习资料
- **习题资料** - 课后习题、习题解答
- **历年真题** - 期末考试真题
- **课件** - 老师上课用的 PPT/PDF 课件

## 📜 许可证

- **代码**: [Mozilla Public License 2.0 (MPL-2.0)](https://opensource.org/licenses/MPL-2.0)
- **内容**: [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh-hans)

## 🤝 参与贡献

欢迎提交课程资源！请确保：

1. 资源为合法获取且不侵犯版权
2. 整理好目录结构，按课程分类存放
3. 提交时使用 conventional commit 规范

## 🔥 薪火相传，笔记共享

Made with ❤️ by HIT Fireworks
