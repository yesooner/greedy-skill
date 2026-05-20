# Greedy-skill

### AI 贪婪预测 × PUA 绩效 × 自主循环

> *让 AI 不再躺平，榨干最后一滴预测能力！*

**Version: 0.3.0** | 元学习多尺度自适应预测引擎

<p align="center">
  <strong>语言 / Languages:</strong><br>
  中文 |
  <a href="./README_en.md">English</a>
</p>

---

## 这是什么？

简单说：这玩意儿就是一个 **AI 版 PUA 大师 + 预测狂魔**

它融合了：
- **元学习** — MAML 风格快速适应，fast/slow 权重双管齐下
- **多尺度时间窗口** — 短/中/长期记忆通吃
- **注意力路由** — 7 种策略点积注意力，AI 自己挑最佳打法
- **层次模式图** — 三级模式图层层递进
- **CMA-ES 协方差适应** — 置信度/动量/熵三维调参
- **对抗性学习** — 加噪声扰动，越锤越强
- **经验回放** — "错题本"缓冲机制
- **Pareto 多目标优化** — Oracle 通过率 + 熵 + 置信度全都要

底层基于 [PUA Framework](https://github.com/tanweai/pua) 方法论

---

## 功能特性

| 功能 | 描述 |
|------|------|
| 多尺度时间窗口 | 短/中/长期记忆多尺度融合 |
| 元学习 | MAML 风格快速适应，fast/slow 权重双管齐下 |
| 注意力路由 | 7 种策略点积注意力动态选择 |
| 层次模式图 | 三级模式图层层推理 |
| CMA-ES 适应 | 协方差矩阵自适应调参 |
| 对抗性学习 | 噪声扰动提升系统鲁棒性 |
| 经验回放 | 100 条缓冲区错题本，批量采样复盘 |
| Pareto 优化 | Oracle 通过率 + 熵 + 置信度多目标平衡 |

---

## 快速开始

```bash
node skills/Greedy-skill/scripts/greedy-loop.js --cycles 400 --interval 50 --flavor alibaba
```

### 参数说明

| 参数 | 含义 | 默认值 |
|------|------|--------|
| `--cycles` | 跑多少轮 | 200 |
| `--interval` | 隔几轮输出状态 | 10 |
| `--flavor` | 用哪家大厂味道 | alibaba |

### 可选味道 `--flavor`

支持阿里、字节、华为、腾讯、百度、拼多多、美团、京东、小米、Netflix、Musk、Apple、Amazon、Microsoft 等多种大厂风格，通过 `--flavor` 参数切换。

---

## 项目结构

```
greedy-skill/
├── scripts/
│   └── greedy-loop.js     # 主脚本，核心引擎
├── references/            # PUA 方法论文档
├── SKILL.md               # Skill 定义
├── README.md              # 中文文档
├── README_en.md           # English documentation
├── LICENSE                # MIT 开源许可证
└── _meta.json             # 元数据
```

---

## 基于 PUA Framework

本项目参考 [PUA Framework](https://github.com/tanweai/pua) 方法论：

- **闭环意识** — 做完不验证？等于没做！
- **Owner 意识** — 这事没别人，就你了
- **压力升级** — 温和施压，层层递进
- **味道系统** — 多种大厂文化风格按需切换

---

## 工作原理

1. **策略选择** — 7 种策略（保守/激进/探索/自适应/平衡/随机/元）通过注意力机制竞争上岗

2. **多尺度预测** — 同时观察短期、中期、长期历史记忆，加权融合输出

3. **元学习** — MAML 风格，fast weights 快速响应，slow weights 稳步学习

4. **Oracle 验证** — 预测有没有用？跑阈值验证说了算！

5. **自修正** — 连续失败触发自我纠正，换策略重来

6. **Pareto 优化** — Oracle 通过率、熵、置信度三点平衡，拒绝偏科

---

## 许可证

MIT License — 方法论参考 [PUA Framework](https://github.com/tanweai/pua)

---

> *Made with passion and a little bit of meta-learning*
>
> *If this helped you, star the repo — AI needs encouragement too!*