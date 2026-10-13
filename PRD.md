# PRD：NEC GitHub 组织首页改造

## 1. 项目背景

NEC（New Energy Coder Club，新能源开发者社区）的 GitHub 组织首页原先使用默认模板，信息展示较为简单，缺乏品牌感和导航入口。为了提升社区在 GitHub 上的专业形象，并方便访客快速了解社区、找到核心仓库和参与方式，需要对组织 profile README 进行全面改造。

## 2. 项目目标

- 提升 NEC GitHub 组织首页的视觉专业度和品牌识别度。
- 清晰展示社区定位、核心领域、核心仓库和快速入口。
- 降低新访客了解社区和参与贡献的门槛。
- 建立可维护、可扩展的组织首页内容结构。

## 3. 改造范围

仅涉及 `.github` 仓库（即本仓库）中的组织 profile 文件：

- `profile/README.md`：组织首页主内容
- `profile/assets/banner.svg`：组织首页 banner 图

## 4. 改造内容

### 4.1 顶部 Banner

- 在 `profile/README.md` 顶部居中展示组织 banner。
- Banner 文件路径：`profile/assets/banner.svg`。
- Banner 设计要求：
  - 尺寸：1200×400
  - 风格：蓝绿渐变，体现新能源与科技感
  - 内容：NEC 大标题、中文名称、英文口号

### 4.2 徽章区

在标题下方展示一排 shields.io 徽章，统一使用 `flat-square` 风格：

- 🏠 组织主页（GitHub Hub）
- 🌐 社区官网
- 📚 主仓库
- License

### 4.3 关于我们

用表格展示社区聚焦的四个方向：

| 方向 | 内容 |
|------|------|
| 机器人竞赛 | CURC / RoboCon 赛事资料与开源工程 |
| 新能源嵌入式 | 电控、电机驱动、光伏储能实战项目 |
| 知识沉淀 | 学习路线、技术文档、赛事规则 |
| 开源协作 | 模板化项目结构、贡献者成长体系 |

### 4.4 核心仓库

用表格列出组织核心仓库：

| 仓库 | 说明 | 技术栈 |
|------|------|--------|
| new_energy_coder_club | 社区主仓库 | Markdown / 资料库 |
| newenergycoder.club | 社区官网 | React + Vite |

### 4.5 快速入口

单独设置「快速入口」区域，汇总关键链接：

- 组织主页
- 社区官网
- 主仓库
- 本仓库（.github profile 仓库）

### 4.6 加入我们

列出加入社区的方式：

- 访问官网
- 阅读贡献指南
- 通过官网「加入我们」页面

### 4.7 贡献者墙

使用 contrib.rocks 自动生成主仓库贡献者头像墙，感谢社区贡献者。

### 4.8 社区理念

底部居中展示社区理念：

> **连接 · 启发 · 赋能**  
> *Connect, Inspire, Empower*

## 5. 文件结构

```
.github/
└── profile/
    ├── README.md
    └── assets/
        └── banner.svg
```

## 6. 验收标准

- [x] 组织首页显示自定义 banner，无错位或乱码。
- [x] 徽章区链接可点击，样式统一。
- [x] 关于我们、核心仓库、快速入口、加入我们、贡献者墙、社区理念各区域完整。
- [x] 在桌面端和移动端 GitHub 页面均可正常浏览。
- [x] `profile/README.md` 已推送至 `main` 分支。

## 7. 实施记录

| 时间 | 操作 | 提交 |
|------|------|------|
| 2026-10-13 | 创建 `profile/README.md` 并美化 | `2387651` |
| 2026-10-13 | 添加 GitHub Hub 和快速入口 | `cf16695` |
| 2026-10-13 | 添加 banner、贡献者墙、调整徽章样式 | `dac3d1b` |

## 8. 后续优化方向

- 加入 GitHub 数据徽章（Stars、Forks、Followers）。
- 加入技术栈/工具图标墙。
- 加入社交媒体链接（微信公众号、B站等）。
- 根据社区发展更新核心仓库列表。
- 设计并替换为更精致的品牌 banner（含 Logo、插画元素）。

## 9. 相关链接

- 组织首页：https://github.com/new-energy-coder-club
- 社区官网：https://www.newenergycoder.club
- 主仓库：https://github.com/new-energy-coder-club/new_energy_coder_club
