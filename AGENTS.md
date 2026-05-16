# AGENTS.md

## 项目概览

西柚的个人主页，科技深空风单页应用。展示个人信息、工作经历、教育背景、关注方向、技能标签和联系方式。

## 技术栈

- 原生 HTML + CSS + JavaScript
- Tailwind CSS v4 (CDN)
- Lucide Icons (CDN)
- Google Fonts (Inter + Noto Sans SC)

## 目录结构

```
/
├── index.html          # 主页面（所有内容）
├── images/
│   └── horse-avatar.jpg  # 头像图片
├── styles/
│   └── main.css         # 预置样式（未使用）
└── .coze                # 项目配置
```

## 构建与运行

- 开发：`python -m http.server 5000 --bind 0.0.0.0`
- 端口：5000
- 热更新：修改 HTML 后手动刷新浏览器

## 代码风格

- 使用 Tailwind CSS 原子化类名
- 自定义 CSS 变量在 `@theme` 中定义
- 中文内容使用 Noto Sans SC，英文使用 Inter