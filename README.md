# word-mystery-games · 单词剧本杀合集

> 把英语单词表变成剧情闯关游戏：说出咒语、审问嫌疑人、在倒计时里破案——单词是唯一的通关钥匙，玩着玩着就记住了。

**Turn vocabulary lists into murder-mystery adventures.** Single-file HTML games, zero dependencies, offline-friendly, mobile-first.

## 在线开玩

👉 **https://<你的GitHub用户名>.github.io/word-mystery-games/**

（把 `<你的GitHub用户名>` 替换成实际用户名；部署方法见文末「上架到自己的 GitHub」）

## 游戏列表

| # | 游戏 | 场景 | 词汇主题 | 文件 |
| --- | --- | --- | --- | --- |
| 1 | 急诊室之夜 | 深夜急诊室 | 医疗急救 | `games/er-night.html` |
| 2 | 美高派对疑云 | 美高 Friendsgiving 派对 | 派对社交 | `games/friendsgiving.html` |
| 3 | 厨房风暴 | 餐厅后厨 | 厨房烹饪 | `games/kitchen-storm.html` |
| 4 | 马戏团之夜：谁藏起了红鼻子 | 马戏团后台 | 外研版选必一 U1 | `games/circus-night.html` |
| 5 | 午夜编辑部：被掉包的退稿信 | 报社编辑部 | 外研版选必一 U2 | `games/midnight-archive.html` |

## 玩法机制

- 🗣️ **说出咒语**：对着屏幕拼读出目标单词，咒语门才会打开
- 🔍 **自由审问**：嫌疑人不会主动招供，问对问题才有线索
- ⏱️ **全局倒计时**：8 分钟内破案，时间压力让记忆更深刻
- ⚖️ **矛盾指认**：比对证词漏洞，指认真凶——指错了有"坏结局"
- 🏅 **单词徽章墙**：每掌握一个词点亮一枚徽章
- 📜 **结局证书 + 复盘页**：真结局需要剩余时间达标；复盘页列出本局所有单词，错词自动进"修炼洞窟"

## 三种打开方式

1. **在线玩**：打开上面的 GitHub Pages 链接，进大厅任选一部。
2. **本地玩**：下载任意一个 `games/*.html`，双击用浏览器打开即可，无需联网、无需安装。
3. **微信里玩**：把 html 文件直接转发到微信聊天/家长群，收到后点开 → 用浏览器打开就能玩（存档只存在本机浏览器里）。

## 目录结构

```javascript
├── index.html               # 合集大厅（纯静态入口页，零脚本）
├── games/
│   ├── er-night.html        # 急诊室之夜
│   ├── friendsgiving.html   # 美高派对疑云
│   ├── kitchen-storm.html   # 厨房风暴
│   ├── circus-night.html    # 马戏团之夜（U1）
│   └── midnight-archive.html# 午夜编辑部（U2）
└── README.md
```

## 技术说明

- 每部游戏都是一个**自包含单文件 HTML**：CSS/JS 全部内联，零 CDN、零外部资源，离线可玩
- 移动优先布局，手机、平板、电脑都能玩
- 全部脚本 IIFE 封闭运行，不与宿主页面冲突，可安全嵌入各类托管平台
- 大厅页零脚本纯静态，永远不会"卡住"

## 上架到自己的 GitHub

1. 新建一个名为 `word-mystery-games` 的公开仓库
2. 把本目录的 `index.html`、`README.md` 和整个 `games/` 文件夹上传到仓库根目录（保持结构不变）
3. 仓库 **Settings → Pages**，Source 选 `main` 分支 + `/(root)`，保存后等 1~3 分钟
4. 访问 `https://<你的用户名>.github.io/word-mystery-games/` 即可

> 注意：首页文件必须恰好叫 `index.html`（Windows 默认隐藏扩展名，小心存成 `index.html.html`）。

## 背景

这是 Elsa 英语追赶计划的游戏化学习产物：把教材词表和高频词织进悬疑剧情，让"背单词"变成"破案"。系列会持续更新（U3~U6 制作中）。

---

仅供学习交流使用。