# 橘娃外挂系统 - 网页版

这是基于 Quartz 构建的静态网站，展示橘娃外挂系统的公开内容。

## 📁 公开内容

- **经验值** - 知识沉淀和学习笔记
- **弹药库** - 可复用的内容素材
- **学习课题** - 主题式学习资料

## 🚀 部署到 Cloudflare Pages

### 1. 推送到 GitHub

```bash
# 创建 GitHub 仓库后
git remote add origin https://github.com/你的用户名/仓库名.git
git branch -M main
git push -u origin main
```

### 2. Cloudflare Pages 配置

登录 [Cloudflare Dashboard](https://dash.cloudflare.com/) → Pages → Create a project

**构建配置：**
- **Framework preset**: None
- **Build command**: `npx quartz build`
- **Build output directory**: `public`
- **Node version**: 20

### 3. 本地预览

```bash
npx quartz build --serve
```

访问 `http://localhost:8080`

## 📝 说明

- 内容通过软链接从主外挂系统目录链接
- 修改主系统内容后，重新构建即可更新网站
- 不包含私密项目（BOSS）、收件箱、工坊等敏感内容
