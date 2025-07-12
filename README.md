# 我的个人网站

这是一个使用纯HTML、CSS和JavaScript构建的现代个人网站，部署在GitHub Pages上。

## 功能特点

- 🎨 现代响应式设计
- 📱 移动设备友好
- ⚡ 快速加载
- 🌟 平滑滚动和动画效果
- 📧 联系表单
- 🚀 自动部署到GitHub Pages

## 技术栈

- HTML5
- CSS3 (Grid, Flexbox, Animations)
- JavaScript (ES6+)
- Font Awesome 图标
- Google Fonts

## 项目结构

```
├── index.html          # 主页面
├── styles.css          # 样式文件
├── script.js           # JavaScript文件
├── .github/
│   └── workflows/
│       └── deploy.yml  # GitHub Actions部署配置
└── README.md           # 项目说明
```

## 本地开发

1. 克隆仓库到本地
2. 在浏览器中打开 `index.html` 文件
3. 或者使用本地服务器（推荐）

使用Python启动本地服务器：
```bash
python -m http.server 8000
```

或使用Node.js：
```bash
npx serve .
```

## 自定义网站

要自定义这个网站，请修改以下内容：

### 个人信息
- 在 `index.html` 中更新姓名、职业和联系信息
- 修改技能标签和项目信息
- 更新社交媒体链接

### 样式
- 在 `styles.css` 中修改颜色方案和布局
- 调整字体和间距

### 功能
- 在 `script.js` 中添加更多交互功能

## 部署到GitHub Pages

1. 将代码推送到GitHub仓库
2. 在仓库设置中启用GitHub Pages
3. GitHub Actions会自动部署网站

### 启用GitHub Pages

1. 进入仓库的 Settings > Pages
2. 在 Source 下选择 "GitHub Actions"
3. 推送代码后，网站会自动部署

## 自定义域名（可选）

如果您有自定义域名：

1. 在仓库根目录添加 `CNAME` 文件
2. 文件内容为您的域名（如：example.com）
3. 在域名提供商处配置DNS记录

## 许可证

MIT License - 可自由使用和修改

## 贡献

欢迎提交Issue和Pull Request！

---

⭐ 如果这个项目对您有帮助，请给个星标！
