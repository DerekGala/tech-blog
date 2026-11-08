# tech-blog

用 **Hugo** 构建、发布到 **GitHub Pages** 的静态博客。

- 站点地址：https://derekgala.github.io/tech-blog/
- 文章目录：`content/posts/<slug>.md`
- 部署：合并到 `main` 后由 `.github/workflows/deploy.yml` 自动构建部署

## 写一篇新文章

```bash
git checkout -b post/my-new-post
# 新建 content/posts/my-new-post.md
git add content/posts/my-new-post.md
git commit -m "post: my new post"
git push -u origin post/my-new-post
gh pr create --base main        # 或在网页上开 PR
```

合并进 `main` 后自动部署，无需手动构建。

## Frontmatter

只使用四个字段：

```yaml
---
title: 文章标题
date: 2026-11-08
tags: ["hugo", "github-pages"]
author: DerekGala
---
```

## 本地预览

```bash
hugo server -D
# http://localhost:1313/
```
