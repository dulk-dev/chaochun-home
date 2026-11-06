# chaochun-home

[chaochun.cc](https://chaochun.cc) 个人主页。

静态站点，部署在 Cloudflare。人物图放在 `assets/`，不引用外部图床。

正文字体是自托管的 Noto Sans SC / Noto Serif SC 子集（SIL OFL 1.1，见 `fonts/OFL.txt`）。

```bash
npx wrangler deploy
```

设计稿在 [`design.html`](design.html)，不替换线上首页。本地预览：

```bash
python3 -m http.server 4321
```

打开 <http://127.0.0.1:4321/design.html>。
