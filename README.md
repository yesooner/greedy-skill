# 🎯 Greedy-skill

### AI 贪婪预测 × PUA 绩效 × 自主循环

> *让 AI 不再躺平，榨干最后一滴预测能力！* 💪

**版本 Version: 0.3.0** | 元学习多尺度自适应预测引擎 🧠

<p align="center">
  <strong>📝 语言 / Languages:</strong><br>
  中文 |
  <a href="./i18n/README.en.md">English</a>
</p>

---

## 🎉 这是什么神仙项目？

简单说：这玩意儿就是一个 **AI 版 PUA 大师 + 预测狂魔** 🚀

它融合了：
- 🧠 **元学习** — MAML 风格快速适应，fast/slow 权重双管齐下
- 🔍 **多尺度时间窗口** — 近 10 轮/50 轮/200 轮记忆通吃
- 🎯 **注意力路由** — 7 种策略点积注意力，AI 自己挑最佳打法
- 📊 **层次模式图** — 三级模式图 L0→L1→L2，层层递进
- 📈 **CMA-ES 协方差适应** — 置信度/动量/熵三维调参
- ⚔️ **对抗性学习** — 加噪声扰动，越锤越强
- 🔄 **经验回放** — 100 条缓冲区的"错题本"
- 🏆 **Pareto 多目标优化** — Oracle 通过率 + 熵 + 置信度全都要

底层基于 [PUA Framework](https://github.com/tanweai/pua) 方法论 🀄

---

## ✨ 功能特性一览

| 功能 | 描述 | Emoji |
|------|------|-------|
| 多尺度时间窗口 | 短/中/长期记忆 (10/50/200轮) | 🪟 |
| 元学习 | MAML 风格快速适应 | 🧠 |
| 注意力路由 | 7 策略点积注意力选择 | 🎯 |
| 层次模式图 | 3级模式图 (L0→L1→L2) | 📊 |
| CMA-ES 适应 | 协方差矩阵适应 | 📈 |
| 对抗性学习 | 噪声扰动提升鲁棒性 | ⚔️ |
| 经验回放 | 100条缓冲，批量采样 | 🔄 |
| Pareto优化 | 多目标优化 | 🏆 |

---

## 🚀 快速开始

```bash
node skills/Greedy-skill/scripts/greedy-loop.js --cycles 400 --interval 50 --flavor alibaba
```

### 参数说明

| 参数 | 含义 | 默认值 |
|------|------|--------|
| `--cycles` | 跑多少轮 | 200 |
| `--interval` | 隔几轮输出状态 | 10 |
| `--flavor` | 用哪家大厂味道 🍭 | alibaba |

### 可选味道 `--flavor`

| 味道 | Emoji | 风格 |
|------|-------|------|
| `alibaba` | 🟠 | 361/闭环/抓手 |
| `bytedance` | 🟡 | 坦诚/Always Day 1 |
| `huawei` | 🔴 | 狼性/军令状 |
| `tencent` | 🟢 | 赛马/小步快跑 |
| `baidu` | ⚫ | 技术信仰/基本盘 |
| `pinduoduo` | 🟣 | 本分/硬核 |
| `meituan` | 🔵 | 做难而正确的事 |
| `jd` | 🟦 | 正道成功/兄弟文化 |
| `xiaomi` | 🟧 | 极致性价比 |
| `netflix` | 🟤 | Keeper Test |
| `musk` | ⬛ | Hardcore/First Principles |
| `apple` | ⬜ | A Player/Think Different |
| `amazon` | 🔶 | Day 1/Customer Obsession |
| `microsoft` | 🪟 | 三圈影响力 |

---

## 🏗️ 项目结构

```
greedy-skill/
├── scripts/
│   └── greedy-loop.js     # 🚀 主脚本，核心引擎
├── references/            # 📚 PUA 方法论文档（各路大厂文化指南）
├── SKILL.md               # 🤖 Skill 定义
├── README.md              # 📖 中文文档（你在这里）
├── README_en.md           # 📖 English docs
├── LICENSE                # MIT 开源许可证
└── _meta.json             # 📦 元数据
```

---

## 📖 版本狂野历史

| 版本 | 核心创新 | 点评 |
|------|---------|------|
| V1 | 基础动量机制 | 🐣 刚学会走路 |
| V2 | 策略池 + UCB1 轮换 | 🐤 开始有想法了 |
| V3 | Epsilon-greedy + 动态难度 | 🐥 有点脑子了 |
| V50 | 量子增强: 贝叶斯 + PID + 纠缠 | 🦄 玄学加成拉满 |
| **Current** | 元学习 + 注意力 + CMA-ES + 回放 | 🐉 究极进化！ |

---

## 🀄 基于 PUA Framework

本项目灵感来自 [PUA Framework](https://github.com/tanweai/pua)，致敬以下方法论：

- 🔄 **闭环意识** — 做完不验证？等于没做！
- 👤 **Owner 意识** — 这事没别人，就你了
- 📈 **压力升级** — 温和施压，层层递进
- 🍭 **味道系统** — 阿里/字节/华为/腾讯... 各有各的调调

---

## 📊 运行效果预览

启动后你会看到这样的状态框 😍：

```
┌─────────────────────────────────────────────────────────┐
│  Greedy-skill Meta-Learning         [50/400]            │
├─────────────────────────────────────────────────────────┤
│  🟠阿里 exploitation 难度:1.15                           │
│  PUA:L2压力 动量值:68% 连续失败:0                      │
│  Oracle:72.5% 自修正:2次                                │
├─────────────────────────────────────────────────────────┤
│  置信度:71.3% 模式对齐:68.4%                            │
│  Alpha:28 Beta:12 熵:0.82                                │
└─────────────────────────────────────────────────────────┘
```

---

## ⚙️ 工作原理（文科生也能看懂版）

1️⃣ **策略选择** — 7 种策略（保守/激进/探索/自适应/平衡/随机/元）通过注意力机制竞争上岗

2️⃣ **多尺度预测** — 同时看最近 10 轮、50 轮、200 轮的历史，加权融合

3️⃣ **元学习** — MAML 风格，fast weights 快速响应，slow weights 稳步学习

4️⃣ **Oracle 验证** — 预测有没有用？跑一遍阈值验证说了算！

5️⃣ **自修正** — 连续失败 5 次？触发自我纠正，换策略重来！

6️⃣ **Pareto 优化** — Oracle 通过率、熵、置信度三点平衡，拒绝偏科

---

## 🤝 声明

 方法论致敬 [PUA Framework](https://github.com/tanweai/pua)

---



---

> *Made with 💪 and a little bit of 🧠*
> 
> *If this helped you, star ⭐ the repo — AI needs encouragement too!* 😎
