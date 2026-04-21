# Menghan Pages

这是一个最小版的个人静态页面发布目录，思路接近 `page.xueheng.site`：

1. 在本地生成 HTML、CSS、JS、图片或 PDF。
2. 用发布脚本复制到 `public/`。
3. 由 Caddy、GitHub Pages、Cloudflare Pages 或其他静态服务对外提供访问。

## 本地发布

```bash
sites/menghan/scripts/publish-local.sh faq-web-demo/index.html lianxh-2026-faq_20260421.html
```

发布后的文件会出现在：

```text
sites/menghan/public/lianxh-2026-faq_20260421.html
```

## Caddy 部署

把 `sites/menghan/public/` 上传到服务器的 `/var/www/menghan`，再参考
`Caddyfile.example` 配置 Caddy。

## 永久在线的选择

- GitHub Pages：适合免费、稳定、少维护的静态网页。
- Cloudflare Pages：适合绑定域名、CDN 和自动部署。
- VPS + Caddy：最像 `page.xueheng.site`，但需要一台长期在线服务器。

## GitHub Pages 发布

推荐仓库名：

```text
menghan
```

发布目录选择：

```text
main branch / root
```

发布后首页地址通常是：

```text
https://menghanyang88-jpg.github.io/menghan/
```
