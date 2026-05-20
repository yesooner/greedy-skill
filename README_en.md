# Greedy-skill

### AI Greedy Prediction × PUA Performance × Autonomous Loop

> *Stop AI from slacking off — squeeze every drop of predictive power out of it!* 💪

**Version: 0.3.0** | Meta-Learning Multi-Scale Adaptive Prediction Engine

<p align="center">
  <strong>语言 / Languages:</strong><br>
  <a href="./README.md">中文</a> |
  English
</p>

---

## What Is This? 🎯

In a nutshell: an **AI PUA master + prediction beast** combo

It combines:
- **Meta-Learning** — MAML-style fast adaptation, fast/slow weights working in tandem
- **Multi-Scale Time Windows** — short/medium/long term memory, all at once
- **Attention Routing** — 7 strategies compete via dot-product attention, AI picks the best play
- **Hierarchical Pattern Graph** — three-level pattern map with layered reasoning
- **CMA-ES Covariance Adaptation** — tuning confidence/momentum/entropy in 3 dimensions
- **Adversarial Learning** — noise perturbation, the more you beat it the stronger it gets
- **Experience Replay** — "mistake notebook" buffer mechanism
- **Pareto Multi-Objective** — Oracle rate + entropy + confidence, we want it all

Built on top of [PUA Framework](https://github.com/tanweai/pua) methodology 🀄

---

## Features ✨

| Feature | Description |
|---------|-------------|
| Multi-Scale Time Windows | Short/Medium/Long memory multi-scale fusion, tracking pattern changes across different time scales |
| Meta-Learning | MAML-style fast adaptation with fast/slow dual weights, learn fast and stay stable |
| Attention Routing | 7-strategy dot-product attention dynamic selection, letting AI decide which approach to use |
| Hierarchical Pattern Graph | Three-level pattern map with layered reasoning, abstracting from low-level actions to high-level strategies |
| CMA-ES Adaptation | Covariance matrix self-adaptive tuning, automatically finding optimal parameter distributions |
| Adversarial Learning | Noise perturbation boosts system robustness, stronger under pressure |
| Experience Replay | 100-slot mistake notebook with batch sampling, review mistakes to avoid repeating them |
| Pareto Optimization | Oracle rate + entropy + confidence multi-objective balance, no lopsided solutions |

---

## Quick Start 🚀

```bash
node skills/Greedy-skill/scripts/greedy-loop.js --cycles 400 --interval 50 --flavor alibaba
```

### Parameters

| Flag | Meaning | Default |
|------|---------|---------|
| `--cycles` | Number of cycles to run | 200 |
| `--interval` | Output status every N cycles | 10 |
| `--flavor` | Which "big tech flavor" to use | alibaba |

### Available Flavors `--flavor`

Supports multiple big tech styles including Alibaba, ByteDance, Huawei, Tencent, Baidu, Pinduoduo, Meituan, JD, Xiaomi, Netflix, Musk, Apple, Amazon, and Microsoft. Switch via the `--flavor` parameter.

---

## Project Structure 📁

```
greedy-skill/
├── scripts/
│   └── greedy-loop.js     # Main script, core engine
├── references/            # PUA methodology docs
├── SKILL.md               # Skill definition
├── README.md              # Chinese documentation
├── README_en.md           # English documentation
├── LICENSE                # MIT License
└── _meta.json             # Metadata
```

---

## Based on PUA Framework 🀄

This project references [PUA Framework](https://github.com/tanweai/pua) methodology:

- **Closed-Loop Awareness** — Done but not verified? Might as well not done!
- **Owner Consciousness** — No one else to blame, it's on you
- **Pressure Escalation** — Gentle pressure, escalating layer by layer
- **Flavor System** — Multiple big tech culture styles switchable on demand

---

## How It Works ⚙️

1. **Strategy Selection** — 7 strategies (conservative/aggressive/exploratory/adaptive/balanced/random/meta) compete via attention mechanism

2. **Multi-Scale Prediction** — simultaneously observe short/medium/long term history, weighted fusion output

3. **Meta-Learning** — MAML-style, fast weights respond quickly, slow weights learn steadily

4. **Oracle Verification** — Is the prediction useful? Threshold verification tells all!

5. **Self-Correction** — Consecutive failures trigger self-correction, switch strategies and retry

6. **Pareto Optimization** — balance Oracle rate, entropy, and confidence — no lopsided solutions allowed

---

## Core Innovations 🔥

### Multi-Scale Time Windows

The system maintains three time scales simultaneously:
- **Short-term window**: capture recent action patterns
- **Medium-term window**: identify trend changes
- **Long-term window**: maintain stable baseline

Through weighted fusion, the system responds quickly to immediate changes while maintaining long-term stability.

### Meta-Learning Mechanism

Adopting MAML-style meta-learning framework:
- **Fast Weights**: adapt quickly to current tasks
- **Slow Weights**: generalize across tasks, accumulating universal knowledge

The dual-weight system makes the system both agile and robust.

### Attention Routing Strategies

7 strategies, each with its own specialty:
- `conservative` — steady and risk-averse
- `aggressive` — bold and high-reward seeking
- `exploratory` — discover new patterns
- `adaptive` — opportunistic and flexible
- `balanced` — attack and defense in harmony
- `random_walk` — random exploration, break conventions
- `meta` — intelligent decision-making, dynamic switching

Attention mechanism dynamically allocates weights based on real-time performance, letting the strongest strategy stand out.

### Hierarchical Pattern Graph

Three-level structure with progressive abstraction:
- **L0 Base Patterns**: action / decision / state_change / outcome / cascade
- **L1 Mid Patterns**: goal_oriented / reactive / deliberative
- **L2 High Patterns**: exploration / exploitation

From concrete actions to abstract strategies, key information is distilled level by level.

### CMA-ES Covariance Adaptation

Evolution strategy based self-adaptive tuning:
- Maintains covariance matrix for confidence/momentum/entropy
- Automatically explores optimal parameter distributions
- No more painful manual tuning

### Adversarial Learning

Introducing noise perturbation to boost robustness:
- Add adversarial noise during training
- System learns to stay stable under interference
- More resilient in real-world applications

### Experience Replay

Learning from historical mistakes:
- 100-slot "mistake notebook"
- Batch sampling review every 20 cycles
- Avoid repeating mistakes, continuous improvement

### Pareto Multi-Objective Optimization

Three objectives, none can be missing:
- **Oracle Rate**: prediction accuracy
- **Entropy**: strategy diversity
- **Confidence**: prediction conviction

Pareto frontier algorithm finds the best balance, no lopsided solutions.

---

## License 📜

MIT License — methodology reference [PUA Framework](https://github.com/tanweai/pua)

---

> *Made with passion and a little bit of meta-learning* 🧠
>
> *If this helped you, star the repo — AI needs encouragement too!*