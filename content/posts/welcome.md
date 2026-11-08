---
title: 博客开张
date: 2026-11-08
tags: ["hugo", "github-pages", "blog"]
author: DerekGala
---

这是用 Hugo + GitHub Pages 搭建的第一篇文章。

## 发布流程

1. 在 `content/posts/` 下新建 Markdown 文件，frontmatter 只写四个字段：`title`、`date`、`tags`、`author`。
2. 提交到分支并发起 PR。
3. 合并进 `main` 后，GitHub Actions 自动构建并部署到 GitHub Pages。

## Frontmatter 模板

```yaml
---
title: 文章标题
date: 2026-11-08
tags: ["tag-a", "tag-b"]
author: DerekGala
---
```

正文从这行开始写。
