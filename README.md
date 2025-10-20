# 📝 Notion Blog

> 基于 **Astro + Notion API** 的轻量级博客框架 从 Notion 数据库自动拉取文章，快速搭建你的个人博客 🚀

## 🚀 Notion Blog 启动指南

本项目是基于 **Astro + Notion API** 的轻量级博客框架，支持从 Notion 数据库自动拉取文章。按照以下步骤即可快速启动。

### 1. 环境准备

在开始之前，请确保已安装以下工具：

- **IDE**：推荐 VS Code 或 [Trae]
- **Node.js**：版本 **20.19.0**（建议使用 nvm 管理 Node 版本）

### 2. 初始化项目

在任意目录下打开终端（Git Bash 或 PowerShell），执行以下命令：

bash

```
# 克隆项目模板
git clone git@github.com:fmxs/notion-blog.git

# 进入项目目录
cd notion-blog

# 安装依赖
npm install
```

### 3. 配置 Notion API

在项目根目录新建 `.env` 文件，并填入以下内容（替换为你自己的 Notion API 信息）：

env

```
NOTION_API_SECRET=你的Notion集成密钥
DATABASE_ID=你的Notion数据库ID
```

> 🔑 提示：
>
> - `NOTION_API_SECRET` 可在 Notion Developers 创建集成后获取。
> - `DATABASE_ID` 可在 Notion 数据库页面的 URL 中找到。

### 4. 本地运行

执行以下命令启动开发服务器：

bash

```
npm run dev
```

终端输出类似信息：

代码

```
Local:   http://localhost:4321/
```

打开浏览器访问 `http://localhost:4321/`，即可看到从 Notion 自动拉取的文章内容 🎉。