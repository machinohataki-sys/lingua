# Lingua PWA 部署指南

## 文件清单
- `index.html` — 主应用（React + 全部功能已内嵌）
- `manifest.json` — PWA 配置（APP名称、图标）
- `sw.js` — Service Worker（离线缓存）
- `icon-192.png` — 小图标
- `icon-512.png` — 大图标

## 部署到 GitHub Pages（免费，推荐）

### 第一步：注册 GitHub
1. 打开 https://github.com
2. 注册一个账号（免费）

### 第二步：创建仓库
1. 点右上角 "+" → "New repository"
2. 仓库名填：`lingua`
3. 勾选 "Public"
4. 点 "Create repository"

### 第三步：上传文件
1. 在新仓库页面点 "uploading an existing file"
2. 把这 5 个文件全部拖进去
3. 点 "Commit changes"

### 第四步：开启 GitHub Pages
1. 进入仓库 → Settings → Pages
2. Source 选 "Deploy from a branch"
3. Branch 选 "main"，文件夹选 "/ (root)"
4. 点 Save

### 第五步：访问
等 1-2 分钟后，打开：
https://你的用户名.github.io/lingua/

### 第六步：安装到手机
1. 手机 Chrome 打开上面的链接
2. Chrome 会弹出 "添加到主屏幕" 提示
3. 如果没弹出，点右上角 ⋮ → "添加到主屏幕"
4. 桌面出现 Lingua 图标，点击即用

## 注意事项
- GitHub Pages 是 HTTPS 的，PWA 必须 HTTPS 才能安装
- 离线功能：安装后，学词/复习/听力/辨音/词根 不需要网络
- AI 功能（查词/语境阅读/写作训练）需要网络 + API Key
- 数据保存在浏览器 localStorage 中，不会丢失（除非清除浏览器数据）
