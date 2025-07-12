# GitHub Pages 部署指南

## 快速部署步骤

### 1. 提交并推送代码到GitHub

首先，将所有文件提交到您的GitHub仓库：

```bash
git add .
git commit -m "添加个人网站文件"
git push origin main
```

### 2. 启用GitHub Pages

1. 访问您的GitHub仓库页面
2. 点击 "Settings" 选项卡
3. 在左侧菜单中找到 "Pages"
4. 在 "Source" 下拉菜单中选择 "GitHub Actions"
5. 点击 "Save"

### 3. 等待部署完成

- GitHub Actions会自动运行部署流程
- 您可以在 "Actions" 选项卡中查看部署状态
- 部署通常需要1-3分钟

### 4. 访问您的网站

部署完成后，您的网站将在以下地址可用：
```
https://yourusername.github.io/yourrepositoryname
```

## 自定义设置

### 更新个人信息

编辑 `index.html` 文件中的以下部分：

1. **姓名和标题**：
   ```html
   <h1 class="hero-title">你好，我是 <span class="highlight">您的姓名</span></h1>
   ```

2. **联系信息**：
   ```html
   <span>your.email@example.com</span>
   <span>github.com/yourusername</span>
   ```

3. **技能标签**：
   ```html
   <span class="skill-tag">您的技能</span>
   ```

4. **项目信息**：
   更新项目卡片中的标题、描述和链接

### 自定义颜色主题

在 `styles.css` 中修改CSS变量：

```css
:root {
    --primary-color: #2563eb;    /* 主色调 */
    --secondary-color: #64748b;  /* 辅助色 */
    --accent-color: #ffd700;     /* 强调色 */
}
```

### 添加自定义域名

如果您有自己的域名：

1. 在仓库根目录创建 `CNAME` 文件
2. 文件内容为您的域名（不包含 http://）
3. 在域名提供商处设置DNS记录指向GitHub Pages

## 故障排除

### 常见问题

1. **网站无法访问**
   - 检查GitHub Actions是否成功运行
   - 确认GitHub Pages已正确配置

2. **样式或脚本未加载**
   - 检查文件路径是否正确
   - 确保所有文件都已提交到仓库

3. **移动端显示异常**
   - 清除浏览器缓存
   - 检查CSS媒体查询

### 获取帮助

如果遇到问题：
1. 查看GitHub Actions的日志
2. 检查浏览器开发者工具的控制台
3. 参考GitHub Pages官方文档

## 进阶功能

### 添加Google Analytics

在 `index.html` 的 `<head>` 部分添加：

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_TRACKING_ID');
</script>
```

### 添加SEO优化

在 `<head>` 部分添加：

```html
<meta name="description" content="您的网站描述">
<meta name="keywords" content="关键词1, 关键词2, 关键词3">
<meta property="og:title" content="您的网站标题">
<meta property="og:description" content="您的网站描述">
<meta property="og:image" content="预览图片URL">
```

---

🎉 恭喜！您的个人网站现在已经部署在GitHub Pages上了！
