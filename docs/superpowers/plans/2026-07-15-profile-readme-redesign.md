# GitHub 个人主页 README 美化实施计划

> **供自动化执行者使用：** 必须使用 `superpowers:executing-plans`，按任务逐步实施并核验。

**目标：** 将当前个人主页重构为由 Markdown、GitHub 支持的 HTML 和独立视觉资源组成的沉浸式交互技术作品集。

**架构：** 页面使用 Markdown 标题、段落、列表和简单 HTML 表格搭建；顶部横幅作为独立图片；项目、经历和统计保持为可编辑、可点击的独立内容。

**技术栈：** GitHub Flavored Markdown、HTML、Shields.io、PNG。

## 全局约束

- 不使用整页设计截图代替 README 内容。
- 不伪造真实项目演示 GIF。
- 所有文档和 Git 提交信息使用中文。
- 实现修改保留在工作区，不自动提交。

---

### 任务 1：准备独立视觉资源

**文件：**

- 创建：`assets/profile/hero-banner-v2.png`
- 创建：`assets/profile/spaceship-demo-cover.png`
- 创建：`assets/profile/exhibition-interaction-cover.png`
- 创建：`assets/profile/icon-interactive-exhibition.svg`
- 创建：`assets/profile/icon-realtime-graphics.svg`
- 创建：`assets/profile/icon-embedded-connected.svg`
- 创建：`assets/profile/icon-repository.svg`
- 创建：`.gitignore`

- [ ] 根据确认的效果图生成独立标题横幅与两张概念项目封面。
- [ ] 为互动展览、实时图形、嵌入式与互联制作独立 SVG 图标。
- [ ] 为精选仓库卡片制作统一仓库 SVG 图标。
- [ ] 将横幅复制到仓库资源目录。
- [ ] 忽略 `.superpowers/` 视觉讨论缓存。

### 任务 2：重构主页结构

**文件：**

- 修改：`README.md`

- [ ] 使用独立横幅、Markdown 标题和徽章构建头部。
- [ ] 将个人定位压缩为简介与三项核心能力。
- [ ] 分组整理技术栈。
- [ ] 新增由文本、链接和徽章组成的精选作品双列区域。
- [ ] 精简仓库与经历区域。
- [ ] 保留现有 GitHub Overview 与奖杯。

### 任务 3：验证 GitHub README 结构

**文件：**

- 检查：`README.md`
- 检查：`assets/profile/hero-banner-v2.png`

- [ ] 运行 `git diff --check`，预期无输出。
- [ ] 检查所有 HTML 表格标签成对出现。
- [ ] 检查横幅相对路径存在。
- [ ] 检查原有个人链接、项目链接和统计图片仍然存在。
- [ ] 确认 Git 状态只包含预期工作区修改。
