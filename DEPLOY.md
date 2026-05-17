# 部署指南

## 方式一：Vercel（推荐 ⭐）

1. 打开 https://vercel.com 并登录（可用 GitHub 账号）
2. 点击 "Add New Project" → 选择你的 GitHub 仓库
3. Framework Preset 选 **Other**（自动识别静态站点）
4. 点 **Deploy**，约 30 秒完成
5. 自动获得域名：`your-project.vercel.app`
6. 可在项目 Settings → Domains 绑定自定义域名

## 方式二：GitHub Pages

1. 打开 GitHub 仓库 → Settings → Pages
2. Source 选 **Deploy from a branch**
3. Branch 选 `main`，目录选 `/ (root)`
4. 点 Save，等待 1-2 分钟
5. 访问 `https://你的用户名.github.io/仓库名/`

> ⚠️ 如果使用 GitHub Pages 的项目站点（不是用户首页），由于路径原因，需要额外配置。建议直接用 Vercel，省心。

## 本地文件清单

需要部署的文件：
```
.
├── index.html              # 主页面
├── images/
│   └── horse-avatar.jpg    # 头像
├── styles/
│   └── main.css            # (未使用，可忽略)
├── .coze                   # 沙箱配置（部署时无需）
└── .git                    # Git 记录
```

部署时只需要 `index.html` 和 `images/` 目录。