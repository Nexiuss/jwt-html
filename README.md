# JWT 在线加密解密工具

一个安全便捷的 JSON Web Token (JWT) 在线处理工具，支持多种加密算法，所有操作均在浏览器本地运行，无需担心数据泄露。

## 🚀 功能特性

- **JWT 解析**：快速解析 JWT Token，展示 Header 和 Payload 信息
- **JWT 生成**：根据自定义 Payload 生成新的 JWT Token
- **多算法支持**：
  - HS256, HS384, HS512 (HMAC 算法)
  - RS256, RS384, RS512 (RSA 算法)
- **签名验证**：验证 JWT Token 签名的有效性
- **密钥状态**：实时显示密钥验证状态
- **本地运行**：所有数据处理均在浏览器中完成，不会上传到服务器
- **响应式设计**：适配桌面和移动设备

## 📦 技术栈

- **前端框架**：原生 HTML/CSS/JavaScript
- **样式框架**：Tailwind CSS 3.4.16
- **图标库**：Remix Icon
- **加密 API**：Web Crypto API

## 📖 使用说明

### 解析 JWT Token

1. 在「JWT Token」输入框中粘贴您的 JWT Token
2. 工具会自动解析并显示 Header 和 Payload 信息
3. （可选）输入密钥，验证签名的有效性

### 生成 JWT Token

1. 解析一个现有的 JWT Token 或手动编辑 Payload
2. 输入密钥
3. 修改 Payload 内容（必须是有效的 JSON 格式）
4. 工具会自动生成新的 JWT Token

### 验证签名

1. 输入 JWT Token
2. 输入对应的密钥
3. 查看「签名验证」区域的结果

## 🔧 如何运行

### 本地运行

1. 克隆或下载项目到本地
2. 直接在浏览器中打开 `index.html` 文件
3. 开始使用 JWT 工具

### 在线使用

（如果项目部署在服务器上，可以在此处添加访问链接）

## 📁 项目结构

```
jwt/
├── index.html          # 主页面
├── js/
│   └── tailwindcss-3.4.16.js  # Tailwind CSS 库
├── fonts/
│   ├── remixicon.css   # Remix Icon 样式
│   └── remixicon.woff2 # Remix Icon 字体文件
└── README.md           # 项目说明文档
```

## 🔒 安全性

- 所有数据处理均在浏览器本地完成，不会上传到任何服务器
- 支持 HTTPS 协议（如果部署在支持 HTTPS 的服务器上）
- 请妥善保管您的密钥信息，工具不会存储任何密钥

## 📝 注意事项

- 确保输入的 JWT Token 格式正确（由三部分组成，用点号分隔）
- Payload 必须是有效的 JSON 格式
- RSA 算法需要使用正确格式的 PEM 私钥
- 密钥验证失败可能是因为密钥不正确或算法不匹配

## 🤝 贡献

欢迎提交 Issue 和 Pull Request 来改进这个工具！

## 📄 许可证

MIT License

## 📞 联系方式

- 项目作者：JWT Tools
- 博客：[Nexiuss](https://nexiuss.github.io/)

---

© 2024 JWT Tools. All rights reserved.
