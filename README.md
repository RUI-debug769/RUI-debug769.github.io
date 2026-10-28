# RUI-debug769.github.io

个人博客 **MUR DOS LOG** 的 GitHub Pages 镜像。

- **镜像地址**：https://rui-debug769.github.io/
- **生产站点**：https://murdok.me （自有云服务器，Nginx 托管）
- **源码仓库**：https://github.com/RUI-debug769/backup-blog

本仓库**不存放源码**。`.github/workflows/pages.yml` 每次运行时会拉取 `backup-blog` 的 `main` 分支、执行 `pnpm build`，再把构建产物发布到 GitHub Pages。

触发方式：

- 手动：Actions → Mirror blog to GitHub Pages → Run workflow
- 定时：每周一 04:00 UTC 自动同步
- 外部：`repository_dispatch` 事件 `mirror`

> 说明：构建配置中的 canonical、sitemap 仍指向生产域名 `murdok.me`，镜像站点仅作可访问性备份，不作为 SEO 主入口。
