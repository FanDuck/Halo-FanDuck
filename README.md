halo-theme-ethereal/├── .github/                     # GitHub 配置│   ├── ISSUE_TEMPLATE/          # Issue 模板│   ├── workflows/│   │   ├── ci.yaml              # 构建、版本检测与发布 Release│   │   ├── cd.yaml              # 发布时同步到 Halo 应用市场│   │   └── codeql.yml           # 代码安全扫描│   └── dependabot.yml           # 依赖自动更新├── .husky/                      # git 钩子├── .nvmrc                       # Node 版本├── i18n/                        # 国际化翻译文件│   ├── default.properties       # 默认语言（英文）│   ├── zh_CN.properties         # 简体中文│   └── zh_TW.properties         # 繁体中文├── public/                      # 静态资源│   ├── assets/                  # JS 脚本、图片等│   ├── fragments/               # Halo 页面片段│   └── gateway_fragments/       # 网关认证片段├── screenshot/                  # 主题截图├── scripts/                     # 构建脚本├── src/│   ├── components/              # 组件│   │   ├── *.astro              # Astro 静态组件│   │   ├── *.svelte             # Svelte 交互组件│   │   ├── control/             # 控件组件│   │   ├── misc/                # 杂项组件│   │   ├── photos/              # 照片相关组件│   │   └── widget/              # 侧边栏小组件│   ├── constants/               # 常量定义│   ├── env.d.ts                 # 环境类型声明│   ├── global.d.ts              # 全局类型声明│   ├── layouts/                 # 页面布局│   │   ├── Layout.astro         # 根布局│   │   └── MainGridLayout.astro # 主网格布局│   ├── pages/                   # 页面模板│   │   ├── index.astro          # 首页│   │   ├── post.astro           # 文章页│   │   ├── archives.astro       # 归档页│   │   ├── tags.astro           # 标签列表│   │   ├── tag.astro            # 标签详情│   │   ├── categories.astro     # 分类列表│   │   ├── category.astro       # 分类详情│   │   ├── photos.astro         # 图库列表│   │   ├── photo.astro          # 图库详情│   │   ├── moment.astro         # 瞬间详情│   │   ├── moments.astro        # 瞬间列表│   │   ├── links.astro          # 友情链接│   │   ├── friends.astro        # 朋友圈│   │   ├── equipments.astro     # 装备展示│   │   ├── portfolio.astro      # 项目集列表│   │   ├── portfolio-detail.astro # 项目集详情│   │   ├── wishes.astro         # 心愿便签│   │   ├── schedule-calendar.astro # 日程日历│   │   ├── schedule-calendar-card.astro # 日程日历卡片组件│   │   ├── timeline.astro        # 时间轴页面│   │   ├── skills.astro          # 技能页面│   │   ├── about.astro           # 关于页面│   │   ├── reward.astro          # 打赏页面│   │   ├── bangumis.astro        # 追番页面│   │   ├── layout.astro          # 插件前台页面契约布局模板│   │   ├── error/               # 错误页面│   │   │   └── 404.astro        # 404 页面│   │   └── page.astro           # 自定义页面│   ├── scripts/                 # 脚本源码│   │   ├── app.ts               # 初始化逻辑│   │   ├── assets/              # 经典脚本源码│   │   └── vendor/              # 第三方脚本│   ├── styles/                  # 全局样式│   ├── types/                   # TypeScript 类型定义│   │   ├── config.ts            # 主题配置类型│   │   └── searchResult.ts      # 搜索结果类型│   └── utils/                   # 工具函数│       └── photos/              # 相册相关工具├── AGENTS.md                    # AI 协作开发约定├── CHANGELOG.md                 # 更新日志├── CONTRIBUTING.md              # 贡献指南├── LICENSE                      # 许可证├── annotation-setting.yaml      # Halo 注解设置├── release.md                   # 发布说明├── astro.config.mjs             # Astro 构建配置├── nodemon.json                 # 开发热更新配置├── settings.yaml                # Halo 主题设置定义├── svelte.config.js             # Svelte 配置├── theme.yaml                   # Halo 主题元信息├── tsconfig.json                # TypeScript 配置├── pnpm-lock.yaml               # pnpm 依赖锁定文件├── pnpm-workspace.yaml          # pnpm 工作区配置└── package.json                 # 项目依赖与脚本
</details>

---

## 💻 开发

<a href="https://github.com/FanDuck/halo-theme-ethereal/graphs/contributors">
  <picture><source media="(prefers-color-scheme: dark)"srcset="https://shieldcn.dev/group/badge/PRs-Welcome!+github/FanDuck/halo-theme-ethereal/contributors+badge/Agent--friendly-AGENTS.md+github/dependabot/FanDuck/halo-theme-ethereal.svg?variant=secondary&amp;font=space-grotesk&amp;mode=dark" /><img alt="For Contributors"src="https://shieldcn.dev/group/badge/PRs-Welcome!+github/FanDuck/halo-theme-ethereal/contributors+badge/Agent--friendly-AGENTS.md+github/dependabot/FanDuck/halo-theme-ethereal.svg?variant=secondary&amp;font=space-grotesk&amp;mode=light" /></picture>
</a>

> 💡 **面向贡献者**：欢迎参与开发！贡献流程、代码约定与提 PR 规范请阅读 [`CONTRIBUTING.md`](./CONTRIBUTING.md)。
>
> 🤖 **面向 AI 协作者**：仓库根目录提供 [`AGENTS.md`](./AGENTS.md)，内含构建命令、目录约定、Halo/Thymeleaf 约定、常见坑与提交规范。使用 AI 编码工具（Codex / opencode / Cursor 等）贡献前请先阅读。
>
> ⚙️ 需要 **Node.js >= 22.12.0**（推荐 24.x，见仓库根目录 `.nvmrc`）和 **pnpm**

<p>
  <a href="https://nodejs.org/"><picture><source media="(prefers-color-scheme: dark)"srcset="https://shieldcn.dev/badge/Node.JS-%3E%3D%2022.12.0-30a043.svg?variant=secondary&amp;logo=nodedotjs&amp;logoColor=ffffff&amp;font=space-grotesk&amp;mode=dark" /><img alt="Node.js"src="https://shieldcn.dev/badge/Node.JS-%3E%3D%2022.12.0-30a043.svg?variant=secondary&amp;logo=nodedotjs&amp;logoColor=ffffff&amp;font=space-grotesk&amp;mode=light" /></picture></a>
  <a href="https://nodejs.org/"><picture><source media="(prefers-color-scheme: dark)"srcset="https://shieldcn.dev/badge/Recommendation-%3E%3D%2024.x-30a043.svg?variant=secondary&amp;logo=nodedotjs&amp;logoColor=ffffff&amp;font=space-grotesk&amp;mode=dark" /><img alt="Recommendation"src="https://shieldcn.dev/badge/Recommendation-%3E%3D%2024.x-30a043.svg?variant=secondary&amp;logo=nodedotjs&amp;logoColor=ffffff&amp;font=space-grotesk&amp;mode=light" /></picture></a>
  <a href="https://pnpm.io/"><picture><source media="(prefers-color-scheme: dark)"srcset="https://www.shieldcn.dev/badge/Package_mgr-pnpm-F69220.svg?logo=pnpm&amp;variant=branded&amp;size=sm&amp;mode=dark&amp;font=space-grotesk"><img alt="Package mgr · pnpm"src="https://www.shieldcn.dev/badge/Package_mgr-pnpm-F69220.svg?logo=pnpm&amp;variant=branded&amp;size=sm&amp;mode=light&amp;font=space-grotesk"></picture></a>
</p>

```bash
# 克隆项目
git clone [https://github.com/FanDuck/halo-theme-ethereal.git](https://github.com/FanDuck/halo-theme-ethereal.git)
cd halo-theme-ethereal

# 安装依赖
pnpm install

# 开发模式（监听文件变更自动重建）
pnpm dev

# 构建并打包为主题安装包（输出 zip 到 dist/）
pnpm build

# 仅构建主题模板（输出到 templates/）
pnpm build:only

# 代码格式化
pnpm format
🛠️ 技术栈技术用途类型安全静态页面生成与路由交互组件（Search、LightDarkSwitch）实用优先的样式框架Web 构建工具代码格式化工具页面过渡动画图标系统🙏 致谢Ethereal 的诞生离不开开源社区。非常感谢 jiewenhuang 开发的 halo-theme-fuwari，本项目在其基础上二次开发。由衷感谢以下开源项目：Halo：优秀的 Java 博客系统，本项目的运行平台Fuwari：原始 Astro 主题，本项目的设计基调halo-theme-fuwari：第一款将 Fuwari 风格移植至 Halo 的主题，本项目的直接上游Firefly：清新美观的 Astro 博客主题，本项目大量参考其设计Aemeath：基于 Firefly 二次创作的主题，本项目部分参考其设计Halo Sig：Halo 社区插件与工具链📄 许可证本项目基于 halo-theme-fuwari（MIT 许可）二次开发，遵守原始许可证条款，并采用 MIT License 开源发布。版权声明：Copyright (c) 2024 saicaca - fuwariCopyright (c) 2025 Jevon - halo-theme-fuwariCopyright (c) 2026 FanDuck - Halo-Theme-Ethereal根据 MIT 开源协议，你可以自由使用、修改、分发本项目的代码，但需保留上述版权声明。
