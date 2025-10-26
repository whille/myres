# 资源下载中心

这是一个简单的静态文件下载服务，部署在 Vercel 上，用于提供音频学习包的下载。

## 项目结构

```
myres/
├── public/
│   ├── index.html          # 下载页面
│   └── downloads/
│       └── audio-package.zip  # 音频学习包
├── vercel.json            # Vercel 部署配置
└── README.md              # 项目说明
```

## 功能特性

- 🎵 提供音频学习包下载
- 📱 响应式设计，支持移动端
- ⚡ 基于 Vercel 的快速 CDN 分发
- 🔒 安全的文件下载服务

## 部署到 Vercel

### 方法一：通过 Vercel CLI

1. 安装 Vercel CLI：
   ```bash
   npm i -g vercel
   ```

2. 在项目根目录运行：
   ```bash
   vercel
   ```

3. 按照提示完成部署

### 方法二：通过 GitHub 集成

1. 将代码推送到 GitHub 仓库
2. 在 [Vercel Dashboard](https://vercel.com/dashboard) 中导入项目
3. 选择 GitHub 仓库并部署

## 配置说明

### vercel.json

- 使用 `@vercel/static` 构建器处理静态文件
- 配置了正确的 MIME 类型和缓存策略
- 设置下载文件的 Content-Disposition 头

### 文件服务

- 所有文件通过 `/public/` 路径提供服务
- 下载文件位于 `/downloads/` 路径下
- 支持直接文件访问和下载

## 访问地址

部署完成后，您可以通过以下地址访问：

- 主页：`https://your-project.vercel.app/`
- 直接下载：`https://your-project.vercel.app/downloads/audio-package.zip`

## 更新文件

要更新下载文件：

1. 替换 `public/downloads/` 目录中的文件
2. 提交更改到 Git
3. Vercel 会自动重新部署

## 技术栈

- HTML5 + CSS3
- Vercel Static Hosting
- 响应式设计
