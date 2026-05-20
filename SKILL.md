---
name: Greedy-skill
description: "Greedy Prediction × PUA Performance × Autonomous Loop. Meta-Learning Multi-Scale Adaptive Prediction Engine with attention-based strategy routing, hierarchical pattern graphs, CMA-ES covariance adaptation, adversarial learning, experience replay, and Pareto optimization."
license: MIT
---

# Greedy-skill — Meta-Learning Multi-Scale Adaptive Prediction Engine

> Features: Meta-Learning | Multi-Scale | Attention Routing | Hierarchical Graph | CMA-ES | Adversarial | Experience Replay | Pareto Optimization

---

## 版本演进

| 版本 | 核心问题 | 解决方案 |
|------|---------|---------|
| V1 | 置信度 30%，单边衰减 | 引入动量 |
| V2 | 策略 100% conservative | 策略池 + 轮换 |
| V3 | 模式收敛过快，难度过低 | ε-greedy + 动态难度 + 模式衰减 |
| V50 | V3架构单一，无多维感知 | 量子增强: 多维动量 + 贝叶斯 + PID + 纠缠 + 混沌 |
| **Current** | **V50无元学习能力** | **元学习 + 多尺度 + 注意力 + CMA-ES + 对抗性 + 回放** |

---

## 十大核心创新

### 创新 1: 多尺度时间窗口

```
短记忆 (10轮): weight=0.5, alpha=0.9
中记忆 (50轮): weight=0.3, alpha=0.7
长记忆 (200轮): weight=0.2, alpha=0.5

多尺度置信度 = Σ(窗口置信度 × 窗口权重)
```

### 创新 2: 元学习 (MAML风格)

```
Fast权重: 快速适应当前任务
Slow权重: 跨任务泛化知识

元学习率: 0.01
每20轮从经验回放采样更新
```

### 创新 3: 注意力机制策略路由

```
Query向量: 8维随机向量
Key/Value向量: 每个策略独立的键值对
点积注意力: attention = softmax(Q·K/√d)·V

7策略: conservative | aggressive | exploratory | adaptive | balanced | random_walk | meta
```

### 创新 4: 层次模式图 (HMG)

```
Level 0: action | decision | state_change | outcome | cascade
Level 1: goal_oriented | reactive | deliberative
Level 2: exploration | exploitation

模式推理: L0 → L1 → L2 三层映射
```

### 创新 5: 协方差自适应 (CMA-ES启发)

```
3x3协方差矩阵: 置信度/动量/熵
均值向量: {confidence:0.7, momentum:0.5, entropy:0.5}
学习率: 0.1
```

### 创新 6: 对抗性自适应

```
对抗噪声: ε=0.05
噪声更新: noise = 0.9*noise + 0.1*new_noise
置信度扰动: confidence * (1 + noise)
```

### 创新 7: 经验回放

```
缓冲区大小: 100条
批采样: 10条/次
采样频率: 每20轮
元学习数据来源
```

### 创新 8: 多目标优化 (Pareto)

```
目标1: Oracle通过率 (target=75%, weight=0.4)
目标2: 熵 (target=50%, weight=0.3)
目标3: 置信度 (target=70%, weight=0.3)

Pareto前沿: 最多20个非支配解
```

### 创新 9: 连续动作空间 (策略梯度启发)

```
策略选择时考虑:
- UCB1置信度
- 熵奖励
- 混沌扰动
- 注意力分数
- 探索奖励
```

### 创新 10: 层次推理

```
输入: 基础模式 (action/decision/...)
推理: L0 → L1 → L2 三层映射
输出: 层次化预测 (level0 + level1 + level2)
```

---

## 核心架构

```
┌──────────────────────────────────────────────────────────────────┐
│                      Greedy-skill V300                           │
│                 Meta-Learning Multi-Scale Engine                │
├──────────────────────────────────────────────────────────────────┤
│  ┌────────────────────────────────────────────────────────────┐  │
│  │              多尺度时间窗口 (短/中/长)                        │  │
│  │         10轮(0.5) | 50轮(0.3) | 200轮(0.2)                   │  │
│  └────────────────────────────────────────────────────────────┘  │
│         ↓              ↓              ↓              ↓          │
│  ┌──────────┐  ┌──────────┐  ┌────────────┐  ┌──────────┐       │
│  │ 元学习   │  │ 注意力   │  │ CMA-ES    │  │ 对抗性   │       │
│  │ MAML    │  │ 策略路由  │  │ 协方差适应  │  │ 自适应   │       │
│  └──────────┘  └──────────┘  └────────────┘  └──────────┘       │
│         ↓              ↓              ↓              ↓          │
│  ┌────────────────────────────────────────────────────────────┐  │
│  │         经验回放 + Pareto优化 + 层次模式图                   │  │
│  │    replay:100 | pareto:20 | HMG:3层 | adversarial:0.05     │  │
│  └────────────────────────────────────────────────────────────┘  │
└──────────────────────────────────────────────────────────────────┘
```

---

## V50 vs V300 对比

| 指标 | V50 | V300 |
|------|-----|-----|
| **时间尺度** | 单尺度 | 多尺度 (3窗口) |
| **元学习** | 无 | MAML风格快速适应 |
| **策略选择** | 熵最大化+UCB1 | 注意力机制路由 |
| **策略数量** | 6 | 7 (+meta) |
| **模式关联** | 量子纠缠 | 层次模式图 |
| **协方差适应** | 无 | CMA-ES启发 |
| **对抗性** | 无 | 噪声扰动 |
| **经验回放** | 无 | 100条缓冲 |
| **多目标** | 无 | Pareto优化 |
| **理论基础** | 量子启发 | 元学习 + 层次推理 + 进化策略 |

---

## 使用指令

```bash
# 运行 Greedy-skill V300
node skills/Greedy-skill/scripts/greedy-loop.js --cycles 400 --interval 50 --flavor alibaba
```

---

## 技术规格

- **版本**: 0.3.0
- **架构**: Meta-Learning Multi-Scale Adaptive Prediction
- **依赖**: Node.js (无需额外包)
- **学习阶段**: exploration (30%) → exploitation (70%)
- **自修正**: 连续5次失败触发策略切换
- **经验回放**: 每20轮采样10条

---

*Greedy-skill V300 — 元学习 × 多尺度 × 注意力 × 层次图 × CMA-ES × 对抗性 × 经验回放 × Pareto优化*
*Powered by PUA Framework — tanweai/pua*