# Greedy-skill

### AI 贪婪预测 × PUA 绩效 × 自主循环

> *让 AI 不再躺平，榨干最后一滴预测能力！* 💪

**Version: 0.3.0** | 元学习多尺度自适应预测引擎

<p align="center">
  <strong>语言 / Languages:</strong><br>
  中文 |
  <a href="./README_en.md">English</a>
</p>

---

## 这是什么？ 🎯

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

底层基于 [PUA Framework](https://github.com/tanweai/pua) 方法论 🀄

---

## 功能特性 ✨

| 功能 | 描述 |
|------|------|
| 多尺度时间窗口 | 短/中/长期记忆多尺度融合，同时追踪不同时间尺度的模式变化 |
| 元学习 | MAML 风格快速适应，fast/slow 权重双管齐下，学得又快又稳 |
| 注意力路由 | 7 种策略点积注意力动态选择，让 AI 自己决定用哪种打法 |
| 层次模式图 | 三级模式图层层推理，从底层动作到高层策略逐级抽象 |
| CMA-ES 适应 | 协方差矩阵自适应调参，自动找到最优参数分布 |
| 对抗性学习 | 噪声扰动提升系统鲁棒性，在逆境中反而更强 |
| 经验回放 | 100 条缓冲区错题本，批量采样复盘，避免重复踩坑 |
| Pareto 优化 | Oracle 通过率 + 熵 + 置信度多目标平衡，拒绝瘸腿选手 |

---

## 快速开始 🚀

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

## 项目结构 📁

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

## 基于 PUA Framework 🀄

本项目参考 [PUA Framework](https://github.com/tanweai/pua) 方法论：

- **闭环意识** — 做完不验证？等于没做！
- **Owner 意识** — 这事没别人，就你了
- **压力升级** — 温和施压，层层递进
- **味道系统** — 多种大厂文化风格按需切换

---

## 工作原理 ⚙️

1. **策略选择** — 7 种策略（保守/激进/探索/自适应/平衡/随机/元）通过注意力机制竞争上岗

2. **多尺度预测** — 同时观察短期、中期、长期历史记忆，加权融合输出

3. **元学习** — MAML 风格，fast weights 快速响应，slow weights 稳步学习

4. **Oracle 验证** — 预测有没有用？跑阈值验证说了算！

5. **自修正** — 连续失败触发自我纠正，换策略重来

6. **Pareto 优化** — Oracle 通过率、熵、置信度三点平衡，拒绝偏科

---

## 核心创新 🔥

### 多尺度时间窗口

系统同时维护三个时间尺度的记忆：
- **短期窗口**：捕捉最近的动作模式
- **中期窗口**：识别趋势变化
- **长期窗口**：保持稳定的基线水平

通过加权融合，系统既能快速响应即时变化，又能保持长期稳定。

### 元学习机制

采用 MAML 风格的元学习框架：
- **Fast Weights**：快速适应当前任务，快速调整
- **Slow Weights**：跨任务泛化，积累通用知识

两层权重协同工作，让系统既敏捷又稳健。

### 注意力路由策略

7 种策略各有专长：
- `conservative` — 保守稳健，规避风险
- `aggressive` — 激进冒险，追求高回报
- `exploratory` — 探索新领域，发现新模式
- `adaptive` — 见机行事，随机应变
- `balanced` — 攻守兼备，稳中求进
- `random_walk` — 随机探索，打破常规
- `meta` — 智能决策，动态切换

注意力机制根据实时表现动态分配权重，让最强策略脱颖而出。

### 层次模式图

三层结构逐级抽象：
- **L0 底层模式**：action / decision / state_change / outcome / cascade
- **L1 中层模式**：goal_oriented / reactive / deliberative
- **L2 高层模式**：exploration / exploitation

从具体动作到抽象策略，逐层提炼关键信息。

### CMA-ES 协方差适应

基于进化策略的自适应调参：
- 维护置信度/动量/熵的协方差矩阵
- 自动探索最优参数分布
- 避免手动调参的痛苦

### 对抗性学习

引入噪声扰动提升鲁棒性：
- 在训练过程中添加对抗性噪声
- 系统学会在干扰下保持稳定
- 实际应用中更能抗压

### 经验回放

从历史错误中学习：
- 100 条容量的"错题本"
- 每 20 轮批量采样复盘
- 避免重复踩坑，持续进步

### Pareto 多目标优化

三个目标缺一不可：
- **Oracle 通过率**：预测准确性
- **熵**：策略多样性
- **置信度**：预测底气

Pareto 前沿算法找到最佳平衡点，拒绝偏科。

---

## 许可证 📜

MIT License — 方法论参考 [PUA Framework](https://github.com/tanweai/pua)

---

> *Made with passion and a little bit of meta-learning* 🧠
>
> *If this helped you, star the repo — AI needs encouragement too!*