# ⭐ 寻星star

> 如同流星飞跃天际 —— 循心 (heart) 的个人博客

一个基于 **Firefly**（Astro 静态博客主题）定制的个人网站，记录 Agent 开发学习之旅、项目实践与生活随笔。

## ✨ 功能

- 📝 **文章**：Markdown 写作，支持代码高亮、表格、目录、分享海报
- 📺 **追番页**：实时展示 Bilibili 追番（72 部）
- 📖 **番组计划**：展示 Bangumi 收藏履历（动画/游戏/音乐/书籍）
- 💬 **留言板**：Giscus 评论系统（GitHub Discussions 存储）
- 🎵 **音乐播放器**：内置歌单（4 首），支持本地音频 + 封面
- 🎀 **看板娘**：流萤 Spine 模型（崩坏：星穹铁道）
- 🗂️ 归档 / 分类 / 标签 / 搜索 / RSS / 相册 / 书签导航
- 🌙 亮暗主题切换（星空蓝紫主题色）

## 🛠️ 本地开发

```bash
pnpm install     # 安装依赖
pnpm dev         # 开发预览 http://localhost:4321
pnpm build       # 生产构建 → dist/
pnpm check       # 类型检查
pnpm preview     # 预览构建产物
```

## 📁 目录速览

```
src/
├── config/       # 站点配置中心（标题/个人资料/音乐/看板娘/页面开关…）
├── content/      # 内容仓库（posts 文章 / spec 固定页面）
├── pages/        # 页面路由
├── components/   # UI 组件
└── assets/       # 图片资源（头像、logo）
public/
└── assets/       # 静态资源（音乐、封面）
```

## 🏗️ 技术栈

- [Astro](https://astro.build/) 7.x + Svelte + Tailwind CSS
- 主题模板：[Firefly](https://github.com/CuteLeaf/Firefly)（MIT）
- 包管理器：pnpm

## 🚀 部署

支持 Cloudflare Pages / Vercel / Netlify 等静态托管（`pnpm build` 输出 `dist/`）。

## 📄 License

[MIT](LICENSE)
