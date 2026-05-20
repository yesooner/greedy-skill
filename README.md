# Greedy-skill

> AI 贪婪预测 × PUA 绩效 × 自主循环

高级自主预测技能，集成元学习、多尺度适应和Pareto优化。基于PUA Framework方法论。

**版本 Version**: 0.3.0

## 功能特性

| 功能 | 描述 |
|------|------|
| **多尺度时间窗口** | 短/中/长期记忆 (10/50/200轮) |
| **元学习** | MAML风格快速适应，fast/slow权重 |
| **注意力路由** | 7策略点积注意力选择 |
| **层次模式图** | 3级模式图 (L0→L1→L2) |
| **CMA-ES适应** | 协方差矩阵适应 (置信度/动量) |
| **对抗性学习** | 噪声扰动提升鲁棒性 |
| **经验回放** | 100条缓冲，批量采样 |
| **Pareto优化** | 多目标 (Oracle率 + 熵 + 置信度) |

## 快速开始

```bash
node skills/Greedy-skill/scripts/greedy-loop.js --cycles 400 --interval 50 --flavor alibaba
```

## 项目结构

```
greedy-skill/
├── scripts/
│   └── greedy-loop.js      # 主脚本
├── references/             # PUA 方法论文档
├── SKILL.md               # Skill 定义
├── README.md              # 中文文档 (默认)
├── README_en.md           # English documentation
├── LICENSE                # MIT 许可证
└── _meta.json             # 元数据
```

## 基于

本项目参考 [PUA Framework](https://github.com/tanweai/pua) 方法论：

- **闭环意识** (Closed-loop awareness)
- **Owner意识** (Owner consciousness)
- **压力升级** (Pressure escalation)
- **味道系统** (Flavor system: 阿里/字节/华为/腾讯...)

## 版本历史

| 版本 | 核心创新 |
|------|---------|
| V1 | 基础动量机制 |
| V2 | 策略池 + UCB1轮换 |
| V3 | Epsilon-greedy + 动态难度 |
| V50 | 量子增强: 贝叶斯 + PID + 纠缠 |
| Current | 元学习 + 注意力 + CMA-ES + 回放 |

## 许可证

MIT License - 方法论参考 [PUA Framework](https://github.com/tanweai/pua)

---

🇺🇸 [English Documentation](README_en.md)