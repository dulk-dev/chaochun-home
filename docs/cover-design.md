# 封面生图说明

首页卡片左侧封面的风格备忘。源文件放在 `public/assets/design/`，页面里用 `/assets/design/`。不要外链临时图床。

右栏小角标可以另用 App 图标（见 `onion-mark.jpg`、`beeppace-mark.jpg`）。左侧大图是场景插画，不拿纯色块或单独图标充封面。

## 气质

暖米纸感的手绘插画。低对比，轻微纸纹或水彩颗粒。静物或很小的人物，主题物件一眼能认出来，四周留白。

不要写成实拍照片，也不要赛博、霓虹、暗黑界面。图里不要放可读的长句子；标牌、屏幕、书脊保持空白或只有色块。

## 色板

和页面变量对齐：

| 角色 | 色值 | 页面变量 |
| --- | --- | --- |
| 米纸底 | `#FBF8F0` 一带 | `--bg` |
| 墨绿 / 鼠尾草绿 | `#3F6E5A` | `--green` |
| 淡黄高光 | `#F6E38B` 一带 | `--mark` |
| 陶土 / 暖橙 | `#C96F4A` 一带 | 点缀 |
| 暖墨 | `#1C1915` | `--ink`，只用于细线 |

## 构图

略俯视或轻等轴的静物场景。主体占画面中部，不要贴边堆满。一张图只讲一件事。

卡片桌面布局里，这张图在左侧，宽度不少于整张卡的一半。窄屏改成上图下文，图本身仍要能看清主题。

## 现有封面

| 文件 | 一句话 |
| --- | --- |
| `onion.jpg` | 居家角落里的同心计时环，旁边是瑜伽垫、壶铃和水杯 |
| `beeppace.jpg` | 弯道跑道上均匀的节奏点，一只秒表落在路面 |
| `clarify.jpg` | 两人隔桌看一张打了勾的清单，像在把需求问清楚 |
| `duck.jpg` | 桌上的小黄鸭、笔记本和电脑；乱线被拉成一条直线 |
| `find-repos.jpg` | 人背对镜头，用放大镜在一排档案里找打勾的那本 |
| `subtitle.jpg` | 胶片框里两个人对话，下面是空白字幕条和播放三角 |
| `vibe.jpg` | 一张空白纸沿着坡道走到一座刚盖好的小屋 |
| `grok.jpg` | 圆头小机器人坐着读一叠笔记，上面贴着黄便签 |
| `ticket.jpg` | 桌上摊开一张空白旅行票根，旁边是一枚小邮票和折好的地图 |

## 输出

- 比例 4:3，长边约 1152、短边约 864
- JPEG，质量大约 80，放进 `public/assets/design/<name>.jpg`（页面里引用 `/assets/design/<name>.jpg`）
- 生图后看一眼：有没有误入的文字、水印、霓虹 UI

## Prompt 模板

把 `{SUBJECT}` 换成上面那种一句场景。色值保持不动，方便系列看起来是一套。

```text
Soft editorial illustration on warm rice paper. {SUBJECT}. Slightly elevated or lightly isometric still life, one clear subject, generous empty margin. Palette only: rice paper #FBF8F0, moss green #3F6E5A, pale yellow highlight #F6E38B, terracotta accent #C96F4A, warm ink lines #1C1915. Low contrast, light paper grain or watercolor texture, hand-drawn, not a photograph.

Negative: no photorealism, no neon cyberpunk, no dark mode, no cluttered UI screenshots, no watermark, no readable lorem text, no letters, no numbers, no logos, no pixel art.
```
