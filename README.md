# 笔记应用官方网站

这是笔记应用的官方网站，使用 GitHub Pages 托管。

## 📁 文件结构

```
docs/
├── index.html          # 主页
├── download.html       # 下载页面
├── pricing.html        # 打赏支持页面
├── css/
│   └── style.css      # 样式文件
├── js/
│   └── main.js        # JavaScript 脚本
├── images/            # 图片资源（需要手动添加）
│   ├── hero-screenshot.png      # 主页大图
│   ├── alipay-qrcode.png       # 支付宝收款码
│   ├── wechat-qrcode.png       # 微信收款码
│   └── screenshots/             # 产品截图
│       ├── 1.png
│       ├── 2.png
│       └── 3.png
└── README.md          # 本文件
```

## 🎨 需要添加的图片

在使用前，请添加以下图片到 `images/` 文件夹：

1. **主页大图** (`images/hero-screenshot.png`)
   - 推荐尺寸：1800x1200px
   - 应用主界面截图

2. **产品截图** (`images/screenshots/`)
   - 1.png - 主界面截图
   - 2.png - 深色模式截图
   - 3.png - 搜索功能截图
   - 推荐尺寸：1200x800px

3. **收款码** (`images/`)
   - alipay-qrcode.png - 支付宝收款码（200x200px）
   - wechat-qrcode.png - 微信收款码（200x200px）

## 🔧 自定义配置

### 1. 更新 GitHub 链接

在所有 HTML 文件中，将以下内容替换为你的实际信息：

```html
<!-- 替换这些链接 -->
https://github.com/你的用户名/仓库名
```

### 2. 更新下载链接

在 `download.html` 中，更新实际的下载链接：

```html
<!-- 替换为实际的 Release 下载链接 -->
https://github.com/你的用户名/仓库名/releases/latest/download/笔记应用-Setup-1.0.0.exe
```

### 3. 添加 Google Analytics（可选）

如果需要统计访问数据，在每个 HTML 文件的 `</head>` 前添加：

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## 🚀 部署到 GitHub Pages

### 方法一：通过 GitHub 网页设置

1. 提交代码到 GitHub
2. 进入仓库的 Settings
3. 找到 Pages 设置
4. Source 选择 `main` 分支的 `/docs` 文件夹
5. 点击 Save
6. 等待几分钟，访问 `https://你的用户名.github.io/仓库名/`

### 方法二：通过命令行

```bash
# 1. 添加所有文件
git add docs/

# 2. 提交
git commit -m "Add GitHub Pages website"

# 3. 推送到 GitHub
git push origin main
```

## 📝 维护指南

### 更新版本信息

当发布新版本时，需要更新以下位置：

1. `index.html` - 主页的版本号
2. `download.html` - 下载页面的版本号和更新日志
3. 下载链接指向最新的 Release

### 添加打赏记录

在 `pricing.html` 的打赏名单部分添加新记录：

```html
<div class="donor-item">
    <span class="donor-name">用户名</span>
    <span class="donor-amount">¥金额</span>
    <span class="donor-date">日期</span>
</div>
```

## 🎯 功能特性

- ✅ 响应式设计，支持移动端
- ✅ 现代化 UI 设计
- ✅ 平滑滚动动画
- ✅ 一键复制功能
- ✅ 通知提示
- ✅ SEO 优化

## 📞 联系方式

- 邮箱：laiwei9631@gmail.com
- 小红书：独立开发者小龙
- 微信公众号：来点狂想
- 团队主页：http://zhaowei.icu/

## 📄 许可证

MIT License
