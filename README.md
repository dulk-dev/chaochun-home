# chaochun-home

[chaochun.cc](https://chaochun.cc) 个人主页。静态站点，部署在 Cloudflare Workers Assets。

首页 `index.html` 自上而下：

- 顶栏锚点：产品 / Skills / 文章
- Hero：口号、社交入口、黄便签
- 产品、Skills、文章：两列卡片，窄屏改成单列

长文在 Flowus。人物图在 `assets/`，卡片封面在 `assets/design/`。封面风格见 [`cover-design.md`](cover-design.md)。

正文字体是自托管的 Noto Sans SC / Noto Serif SC 子集（SIL OFL 1.1，见 `fonts/OFL.txt`）。

本地预览：

```bash
python3 -m http.server 4321
```

打开 <http://127.0.0.1:4321/>。

部署：

```bash
npx wrangler deploy
```
