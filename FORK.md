# 关于这个 Fork

这是 `cmliu/CF-Workers-WebSSH` 的个人 Fork，用于 Cloudflare Workers 自动部署。

- 上游更新会自动同步到本仓库（`.github/workflows/sync-upstream.yml`，每周一次，也可手动触发）。
- 每次推送到 `main` 分支，Cloudflare Workers Builds 会自动构建并部署。
- 本地补丁（与上游的差异）：
  - 手机端快捷键悬浮按钮的触屏检测修复（部分手机浏览器谎报 `pointer: fine`）。
  - `wrangler.toml` 中 `preview_urls = false`（关闭预览 URL）。
- 如果上游更新与本地补丁冲突，同步工作流会失败并提醒手动解决。
