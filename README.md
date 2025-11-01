# WebTest

多国旅游攻略静态网站（首页、攻略中心、具体攻略页与联系反馈页）。

目录结构（简要）：
- `index.html` 首页（Butterfly 首屏 Hero）
- `pages/guides-hub.html` 攻略中心（卡片网格布局）
- `pages/guide-china.html` 中国10日游模板（行程日块样式）
- `pages/contact.html` 反馈与信息（完整表单）
- `css/style.css` 全局样式与组件样式

本地预览：
```bash
python -m http.server 3000 --bind 127.0.0.1
```

后续协作：
- 在远程平台（如 GitHub/GitLab）创建仓库 `WebTest`
- 将本地仓库推送到远程（见下方“推送指引”）