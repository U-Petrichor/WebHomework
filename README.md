<div align="center">
  
![漫步者旅游攻略](https://cdn.jsdelivr.net/gh/U-Petrichor/WebHomework@main/image/logo.png)
  
</div>

# 🧳 漫步者旅游攻略

> 一个精美的多国旅游攻略静态网站，提供详尽的旅行路线规划、景点介绍和实用信息。

## ✨ 项目特色

- 🎨 **精美UI设计**：采用模糊背景、渐变效果和现代化设计风格
- 🎯 **3D轮播效果**：攻略中心采用3D透视轮播，支持键盘导航和左右箭头切换
- 📅 **时间轴布局**：详细攻略页面使用时间轴展示每日行程，左右交替布局
- 🗺️ **交互式地图**：嵌入Google Maps，实时查看旅行路线
- 📱 **响应式设计**：完美适配桌面端、平板和移动设备
- 🎭 **自定义字体**：使用特色中文字体增强视觉体验
- ⚡ **流畅动画**：悬停效果、过渡动画和交互反馈

## 📂 项目结构

```
WebHomework/
├── index.html             # 首页（Hero全屏首屏）
├── pages/
│   ├── guides-hub.html    # 攻略中心（3D轮播展示）
│   ├── guide-norway.html  # 挪威8日游玩攻略（时间轴布局）
│   └── contact.html       # 联系与反馈页面
├── css/
│   └── style.css          # 全局样式文件
├── font/
│   ├── AaYouLongXingShu-2.ttf      # Aa游龙行书字体
│   └── XingQiuManYouJiHua-2.ttf    # 星球漫游记字体
├── image/
│   ├── logo.png           # 网站图标
│   ├── banner.jpg         # 首页横幅
│   ├── background.jpg     # 背景图片
│   └── [景点图片...]      # 各景点相关图片
├── screenshots/           # 网页截图（用于README展示）
│   ├── homepage.png       # 首页截图
│   ├── guides-hub.png     # 攻略中心截图
│   ├── guide-norway.png   # 挪威攻略截图
│   └── contact.png        # 联系反馈页面截图
└── README.md              # 项目说明文档
```

## 🚀 快速开始

### 本地预览

使用Python内置HTTP服务器：

```bash
# Python 3.x
python -m http.server 3000 --bind 127.0.0.1

# 或指定端口
python -m http.server 8000
```

然后在浏览器中访问：`http://127.0.0.1:3000` 或 `http://localhost:3000`

> **⚠️ 重要提示**：挪威攻略页面中嵌入了 Google Maps 交互式地图，需要连接外网才能正常显示地图。如果无法访问外网，地图区域将显示为空白或加载失败提示。

### 使用其他本地服务器

**Node.js (使用 http-server)**
```bash
npx http-server -p 3000
```

**PHP**
```bash
php -S localhost:3000
```

> **💡 最佳浏览效果**：为了获得最佳的视觉体验，建议将浏览器窗口大小调整为屏幕的 **90%**。这样可以确保页面元素完整显示，3D轮播效果和响应式布局都能达到最佳展示效果。

## 📖 页面说明

### 🏠 首页 (`index.html`)

- **Hero全屏首屏**：大图背景，欢迎文案
- **欢迎模块**：功能介绍和行动按钮
- **景点画廊**：两列阶梯式布局，展示全球著名景点
  - 悬停效果：图片放大，标题详情展开
  - 支持点击查看大图

<div align="center">
  
![首页截图](https://cdn.jsdelivr.net/gh/U-Petrichor/WebHomework@main/screenshots/homepage.png)
  
*首页展示 - Hero全屏首屏与景点画廊*

</div>

### 📚 攻略中心 (`pages/guides-hub.html`)

- **3D轮播展示**：
  - 当前激活项居中显示
  - 左右侧项目模糊缩小（3D透视效果）
  - 支持左右箭头或键盘方向键切换
  - 底部统一CTA按钮，根据攻略状态动态显示文案
  
- **攻略内容**：
  - 挪威8日游玩攻略（完整内容）
  - 日本7日经典路线（敬请期待）
  - 法国南部5日游（敬请期待）
  - 投稿新攻略入口

- **APP推荐**：挪威攻略中包含实用APP推荐框

<div align="center">
  
![攻略中心截图](https://cdn.jsdelivr.net/gh/U-Petrichor/WebHomework@main/screenshots/guides-hub.png)
  
*攻略中心 - 3D轮播效果与APP推荐*

</div>

### 🗺️ 挪威攻略 (`pages/guide-norway.html`)

- **时间轴布局**：
  - 左侧：时间轴内容区域（8天行程，左右交替）
  - 右侧：固定地图面板（Sticky定位）
  - ⚠️ **地图加载**：右侧地图使用 Google Maps 嵌入，需要连接外网才能显示
  
- **每日行程**：
  - 标题使用Aa游龙行书字体
  - 包含行程描述、详细清单和景点图片
  - 左侧图片悬停放大效果
  - 列表项采用淡蓝色背景框

- **交互特性**：
  - 内容框悬停上浮效果
  - 标题悬停颜色变化

<div align="center">
  
![挪威攻略截图](https://cdn.jsdelivr.net/gh/U-Petrichor/WebHomework@main/screenshots/guide-norway.png)
  
*挪威攻略 - 时间轴布局与交互式地图*

</div>

### 💬 联系反馈 (`pages/contact.html`)

- **关于作者**：团队介绍
- **反馈表单**：包含多个表单字段
  - 文本输入、邮箱、下拉选择
  - 单选框、复选框
  - 文本域
  - 提交按钮

<div align="center">
  
![联系反馈页面截图](https://cdn.jsdelivr.net/gh/U-Petrichor/WebHomework@main/screenshots/contact.png)
  
*联系反馈页面 - 关于作者与反馈表单*

</div>

## 🎨 设计亮点

### 字体系统

- **Aa游龙行书**：用于时间轴Day标题
- **星球漫游记**：用于首页标题、攻略中心标题、挪威攻略主标题
- **ZCOOL KuaiLe**：备用标题字体
- **Noto Sans SC**：正文内容字体

### 色彩方案

- 主色调：`#3498db` (蓝色)
- 深色：`#333`
- 浅色背景：`#f4f4f4`
- 半透明模糊背景增强视觉层次

### 动画效果

- 3D轮播：透视变换、模糊效果
- 悬停动画：卡片上浮、图片缩放
- CTA按钮：摇晃动画吸引注意
- 平滑过渡：所有交互都有流畅的过渡效果

## 🛠️ 技术栈

- **HTML5**：语义化标签，结构清晰
- **CSS3**：
  - Flexbox & Grid布局
  - 3D Transform和Perspective
  - CSS变量
  - 动画和过渡效果
  - 媒体查询（响应式设计）
- **JavaScript**：轮播交互逻辑、键盘导航
- **Google Fonts**：Web字体支持

## 📱 响应式支持

- **桌面端**：完整功能展示，3D轮播效果
- **平板设备**：适配中等屏幕，优化布局


## 🌟 功能特性

- ✅ 全站统一导航栏（Sticky定位）
- ✅ 模糊背景效果（除首页外所有页面）
- ✅ 3D轮播交互（支持键盘导航）
- ✅ 时间轴行程展示
- ✅ 交互式地图嵌入（⚠️ 需要外网访问 Google Maps）
- ✅ 表单验证和反馈
- ✅ 响应式图片加载（lazy loading）
- ✅ 网站图标（Favicon）支持
- ✅ 无障碍访问（ARIA标签）

## 📝 开发说明

### 添加新攻略

1. 在 `pages/` 目录创建新的攻略HTML文件
2. 参考 `guide-norway.html` 的时间轴结构
3. 在 `guides-hub.html` 的轮播中添加新项目
4. 更新相关的图片资源

### 自定义样式

主要样式定义在 `css/style.css`：
- CSS变量定义在 `:root` 中
- 各页面样式按模块分组
- 媒体查询在相应模块末尾

### 字体替换

如需替换字体：
1. 将字体文件放入 `font/` 目录
2. 在 `style.css` 添加 `@font-face` 声明
3. 更新对应的 `font-family` 属性

## 👥 开发团队

© 2025 王何佳、叶于琳、吾米提·加帕尔的Web开发技术基础-实操性作业3

## 📄 许可证

本项目仅用于学习和教育目的。

## 📸 截图说明

README中展示的网页截图位于 `screenshots/` 目录：

- `homepage.png` - 首页完整展示
- `guides-hub.png` - 攻略中心3D轮播效果
- `guide-norway.png` - 挪威攻略时间轴布局
- `contact.png` - 联系反馈页面


## 🙏 致谢

- Google Fonts 提供免费Web字体
- 所有景点图片来源于网络，仅用于学习展示
- 感谢所有为旅游攻略提供灵感的旅行者们

---

**享受你的旅程，探索世界的美好！** 🌍✈️
