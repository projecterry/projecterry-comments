# Projecterry 文章评论

本仓库用于存储 [Projecterry 网站](https://projecterry.github.io/) 的文章评论。

评论由 [giscus](https://giscus.app/zh-CN) 连接到本仓库的 GitHub Discussions。网站源码保存在另一个私密仓库，本仓库只保存公开讨论和评论配置。

## 每篇文章一条讨论

- 所有文章共用本仓库。
- 文章通过页面路径 `pathname` 对应到 `Announcements` 分类中的独立讨论，启用严格匹配以避免串帖。
- 第一次发表评论或回应时，giscus 自动创建对应的讨论。
- 访客可以公开阅读评论，发表评论需要登录 GitHub。
- 网站维护者可以在 Discussions 中管理评论。

修改文章地址后，请同时迁移对应讨论的映射；仅修改文章标题不会改变评论归属。

## 网站设置

VitePress 的文章默认显示评论。需要关闭某页评论时，在该 Markdown 文件开头添加：

```yaml
---
comments: false
---
```

首页不显示评论，关于页面已单独关闭评论。
