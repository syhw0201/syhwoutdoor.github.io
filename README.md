# 🏔️ 深缘户外官网

> 深港徒步，跟八阿哥走 —— 安全带队，笑着出发，平安回家

## 📋 文件说明

| 文件 | 说明 |
|------|------|
| `index.html` | 网站首页（完整单页应用，包含所有区块） |
| `style.css` | 样式文件（户外绿色主题 + 橙色强调色） |
| `main.js` | 交互脚本（导航、标签切换、滚动动画等） |

## 🚀 部署教程（GitHub Pages 免费方案）

### 步骤1：创建 GitHub 账号
1. 访问 https://github.com
2. 注册一个账号（如果还没有）

### 步骤2：创建仓库
1. 点击右上角 "+" → "New repository"
2. 仓库名填：`syhwoutdoor.github.io`
3. 选择 "Public"（公开）
4. 勾选 "Add a README file"
5. 点击 "Create repository"

### 步骤3：上传网站文件
1. 进入刚创建的仓库
2. 点击 "Add file" → "Upload files"
3. 将 `index.html`、`style.css`、`main.js` 三个文件拖入上传区域
4. 点击 "Commit changes"

### 步骤4：启用 GitHub Pages
1. 进入仓库的 "Settings"（设置）
2. 左侧菜单点击 "Pages"
3. "Source" 选择 "Deploy from a branch"
4. "Branch" 选择 "main"，文件夹选择 "/ (root)"
5. 点击 "Save"

### 步骤5：绑定你的域名
1. 在 "Pages" 设置页面，找到 "Custom domain"
2. 输入你的域名：`www.syhwoutdoor.cn`（或 `syhwoutdoor.cn`）
3. 点击 "Save"
4. 勾选 "Enforce HTTPS"（强制HTTPS）

### 步骤6：域名解析（在腾讯云/阿里云操作）
1. 登录你的域名服务商（腾讯云/阿里云）
2. 找到域名解析设置
3. 添加以下记录：

| 主机记录 | 记录类型 | 记录值 |
|---------|---------|--------|
| @ | A | 185.199.108.153 |
| @ | A | 185.199.109.153 |
| @ | A | 185.199.110.153 |
| @ | A | 185.199.111.153 |
| www | CNAME | 你的用户名.github.io |

> 注意：IP地址是GitHub Pages的IP，可以去 https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site 确认最新IP

### 步骤7：等待生效
- GitHub Pages 部署通常需要 1-5 分钟
- 域名解析通常需要 10 分钟 - 48 小时
- 访问 `https://syhwoutdoor.cn` 查看效果

## 📝 内容定制说明

### 替换图片
目前网站使用的是占位图，你需要替换为真实图片：

1. **首页背景图**：在 `style.css` 中搜索 `.hero-bg`，替换背景图URL
2. **领队照片**：在 `index.html` 中搜索 "八阿哥带队实拍"，替换对应区域
3. **活动照片**：在 `index.html` 中搜索各个路线的 `.image-placeholder`，替换为真实照片
4. **微信二维码**：在 `index.html` 中搜索 "扫码添加微信"，替换为你的真实微信二维码图片

### 修改文案
直接编辑 `index.html` 文件中的文字内容即可。

### 修改配色
编辑 `style.css` 文件中的 CSS 变量：
```css
:root {
    --primary: #2D5A3D;        /* 主色调 - 绿色 */
    --accent: #E67E22;         /* 强调色 - 橙色 */
    ...
}
```

### 添加/删除活动线路
在 `index.html` 中找到对应区域的 `.routes-grid`，复制或删除 `.route-card` 卡片即可。

## 🎯 网站结构

```
首页
├── 导航栏（6个入口）
├── Hero区域（核心价值主张）
├── 三大核心价值
├── 关于我们（八阿哥介绍）
├── 安全保障（四三三法则）
├── 活动线路（香港/深圳/惠州）
├── 客户见证
├── 联系我们（加微信）
└── 页脚
```

## 📱 响应式支持

网站已适配：
- ✅ 桌面端（1200px+）
- ✅ 平板端（768px - 1199px）
- ✅ 手机端（< 768px）

## 🔧 技术特性

- 纯静态网站，无需服务器
- 响应式设计，适配各种设备
- 平滑滚动和视差效果
- 数字滚动动画
- 移动端菜单
- SEO友好（已添加meta标签）

## 📞 联系方式

- 企业邮箱：contact@syhwoutdoor.cn
- 微信：bagege-outdoor

---

**深缘户外 © 2024** - 深港徒步，跟八阿哥走
