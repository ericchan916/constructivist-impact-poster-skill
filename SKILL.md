---
name: constructivist-impact-poster
description: 构成主义动势海报：用对角线张力、强对比与图形化动势，做一张决绝有力的运动感海报。根据【主标题】【短句】【场景】【版式】【主色强调】【画幅】生成一张简体中文海报。当用户提到「构成主义 / Constructivist / 动势海报」时使用。 Use when the user asks for a constructivist poster, diagonal impact poster, graphic campaign poster — produces one poster with only three visible Chinese lines: headline, supporting line, and footer「一张有戏 · 视觉习作」.
license: MIT
---

# 构成主义动势 · Constructivist Impact Poster

用对角线张力、强对比与图形化动势，做一张决绝有力的运动感海报。
An urgent geometric campaign-like poster with diagonal force, strong contrast, and graphic energy.

## 输入 · Inputs

```
【主标题】：
【短句】：
【场景】：
【版式】：（diagonal-dynamic，缺省 diagonal-dynamic）
【主色强调】：（红 / mustard / steel gray / deep navy（可选））
【画幅】：9:16（默认）
```

**缺失字段不要追问**：只给了主标题（或部分字段）时，由你根据主标题自行补全其余字段，并保证场景、版式、主色强调彼此协调、指向同一概念。画幅缺省为 9:16。
If any field is missing, fill it yourself coherently from the headline — never ask. Default aspect ratio 9:16.

## 使用方法 · How to use
1. 读取输入，补全缺失字段（内部完成，不输出分析）。
2. 按下方核心规则 + [prompt.md](prompt.md) 组合提示词，交给图像生成工具，**只输出一张**海报。
3. 若当前环境不能生图，输出下方「可直接粘贴的最终提示词」，已填好字段，供用户粘贴到 ChatGPT / 其他图像模型。

示例输入见 [examples/themes.md](examples/themes.md)。

## 核心规则 · Core rules

### 目标 · Intent
用对角线张力、强对比与图形化动势，做一张决绝有力的运动感海报。
Create an urgent, geometric, campaign-like poster with diagonal force, strong contrast, and graphic propaganda-inspired energy.

### 字体 · Typography
- Use bold condensed sans-serif or slab-like display type.
- Set type at strong angles or in assertive blocks.
- Use uppercase sparingly for impact.
- Keep details in stable horizontal areas.

### 配色 · Palette
- Red, black, cream, white, charcoal. Optional accents: mustard, steel gray, deep navy.
- 【主色强调】只取一个精确强调色，不要彩虹堆砌。

### 意象 · Imagery
- Use photo montage, silhouettes, geometric forms, arrows, rays, cropped figures, or symbolic objects.
- 【场景】描述应支撑字体与版式，不要喧宾夺主（除非风格本身以主体物件为第一阅读）。

### 质感 · Texture / Material
- Print grain, screenprint texture, paper aging, rough ink, overprint effects.

### 构图 · Composition
- Use diagonals to create momentum.
- Build contrast between massive shapes and precise text.
- Use geometric framing and directional emphasis.
- Make the message feel decisive and public.
- 版式从该风格允许的布局中选择：`diagonal-dynamic`；缺省 `diagonal-dynamic`。
- 单一焦点、清晰阅读顺序：主标题 → 焦点画面 → 短句 → 页脚。

### 文字锁定 · Text lock（一张有戏）
- 画面可见文字**只有三行**：【主标题】、【短句】、页脚「一张有戏 · 视觉习作」。
- 简体中文；每个字正确成形；不要英文乱码、假活动、假日期、假地址、假奖项、假价格、假 CTA、假品牌。
- 不要按钮/圆角胶囊/UI 容器；页脚就是普通小字排印。

### 避免 · Avoid
- Historical parody, excessive propaganda symbols, cluttered rays, unreadable angled details, and soft decorative styling.
- 额外假字、随机 logo、二维码、装饰堆砌、畸形字体、通用 AI 海报噪声、水印、UI。

### 执行 · Execution
不提问、不展示分析、不出多版本，直接输出一张海报。

## 可直接粘贴的最终提示词 · Ready-to-paste prompt template

```
【主标题】：{{主标题}}
【短句】：{{短句}}
【场景】：{{场景}}
【版式】：{{版式，缺省 diagonal-dynamic；可选 diagonal-dynamic}}
【主色强调】：{{主色强调}}
【画幅】：{{画幅，默认 9:16}}

Create exactly ONE polished professional {{画幅，默认 9:16}} portrait poster, static flat artwork, Chinese-mainland cultural/creative studio portfolio concept.
Language: Simplified Chinese. Headline: {{主标题}}. Supporting phrase: {{短句}}. Tiny plain footer: 一张有戏 · 视觉习作. Exact visible text ONLY these three phrases, every character correctly formed. No English clutter, random numbers, fake events, dates, addresses, awards, offers, prices, affiliations, calls to action or status labels. All content is fictional/conceptual creative brief, no real client claim.
If any field above is empty, fill it coherently from 【主标题】 so scene, accent and layout support one clear idea — do not ask questions.

SELECTED STYLE — STRICTLY THIS VISUAL SYSTEM, DO NOT MIX OTHER STYLES:
# Constructivist Impact
Intent: Create an urgent, geometric, campaign-like poster with diagonal force, strong contrast, and graphic propaganda-inspired energy.
Typography: Use bold condensed sans-serif or slab-like display type. Set type at strong angles or in assertive blocks. Use uppercase sparingly for impact. Keep details in stable horizontal areas.
Palette: Red, black, cream, white, charcoal. Optional accents: mustard, steel gray, deep navy. Use exactly one precise accent from 【主色强调】.
Imagery: Use photo montage, silhouettes, geometric forms, arrows, rays, cropped figures, or symbolic objects. Scene direction: {{场景}}.
Texture / Material: Print grain, screenprint texture, paper aging, rough ink, overprint effects.
Composition: Use diagonals to create momentum. Build contrast between massive shapes and precise text. Use geometric framing and directional emphasis. Make the message feel decisive and public. Use layout {{版式，缺省 diagonal-dynamic}} from allowed set (diagonal-dynamic). One dominant message, one focal point; reading order headline -> focal image -> supporting copy -> footer. Confident spacing; no overstuffed layout; no UI buttons/pills for the footer.

Avoid: Historical parody, excessive propaganda symbols, cluttered rays, unreadable angled details, and soft decorative styling. Also avoid fake extra text, logos, QR codes, decorative clutter, malformed typography, generic AI-poster noise, watermarks, UI chrome.

Do not ask questions. Do not show analysis or alternatives. Output the single finished poster only.
```
