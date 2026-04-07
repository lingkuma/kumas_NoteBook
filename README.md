# fugue一键搭建


# Logseq Publish 模板

这是一个基于 Logseq 的静态发布模板，适合把笔记仓库直接整理成个人博客或知识站点。日常内容仍然在 Logseq 里编辑和维护，仓库本身负责把这些页面转换成可部署的静态网站。

仓库的发布流程是：本地在 Logseq 中写作并提交后，推送到 `main` 分支；GitHub Actions 会自动调用 `logseq/publish-spa` 进行渲染，生成前端页面并发布到 `gh-pages` 分支；最后可以通过 Fugue 或 Vercel 这类静态托管服务完成上线。

如果你想搭建同样的流程，可以直接 fork 本项目，再参考 `pages/publish.md` 中的发布说明完成配置。

备注：README 中只保留纯文字说明，不放图片，因为图片内容不会被 Action 转换到最终页面，也不会被logseq追踪，这里的图片移动到其他页面也不会被转换。
其他页面中的图片可以正常使用。
