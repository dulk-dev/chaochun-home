# chaochun-home

[chaochun.cc](https://chaochun.cc) 个人主页。Astro 静态站，部署在 Cloudflare Workers Assets。

首页自上而下：顶栏锚点（产品 / Skills / 文章）、Hero（口号、社交入口、黄便签）、三个分区的两列卡片。长文在 Flowus。

## 技术栈

- [Astro](https://astro.build) 5，`output: "static"`
- 自托管 Noto Sans SC / Noto Serif SC 子集（`public/fonts/`，许可 `OFL.txt`）
- Cloudflare Workers Assets（`wrangler.jsonc` 指向 `dist/`）

## 本地

```bash
npm install
npm run dev
```

生产构建：

```bash
npm run build
npx astro preview
```

打开构建结果是 `dist/index.html`。部署：

```bash
npx wrangler deploy
```

## 目录

```text
public/fonts/          自托管字体
public/assets/         人物图和卡片封面
src/pages/index.astro  首页
src/components/        顶栏、便签、分区、卡片
src/data/              导航和三区卡片数据
src/styles/            色板和全局样式
docs/site-style.md     色板、字体、版式
docs/cover-design.md   封面怎么画
docs/ip/               人物三视图，不进页面
```
