# Greedy-skill

### AI Greedy Prediction × PUA Performance × Autonomous Loop

> *Stop AI from slacking off — squeeze every drop of predictive power out of it!*

**Version: 0.3.0** | Meta-Learning Multi-Scale Adaptive Prediction Engine

<p align="center">
  <strong>语言 / Languages:</strong><br>
  <a href="./README.md">中文</a> |
  English
</p>

---

## What Is This?

In a nutshell: an **AI PUA master + prediction beast** combo

It combines:
- **Meta-Learning** — MAML-style fast adaptation, fast/slow weights working in tandem
- **Multi-Scale Time Windows** — remembers last 10/50/200 cycles, all at once
- **Attention Routing** — 7 strategies compete via dot-product attention, AI picks the best play
- **Hierarchical Pattern Graph** — three-level pattern map L0→L1→L2, layer by layer
- **CMA-ES Covariance Adaptation** — tuning confidence/momentum/entropy in 3 dimensions
- **Adversarial Learning** — add noise perturbation, the more you beat it the stronger it gets
- **Experience Replay** — 100-slot "mistake notebook" buffer
- **Pareto Multi-Objective** — Oracle rate + entropy + confidence, we want it all

Built on top of [PUA Framework](https://github.com/tanweai/pua) methodology

---

## Features

| Feature | Description |
|---------|-------------|
| Multi-Scale Time Windows | Short/Medium/Long memory (10/50/200 cycles) |
| Meta-Learning | MAML-style fast adaptation |
| Attention Routing | 7-strategy dot-product attention selection |
| Hierarchical Pattern Graph | 3-level graph (L0→L1→L2) |
| CMA-ES Adaptation | Covariance matrix adaptation |
| Adversarial Learning | Noise perturbation for robustness |
| Experience Replay | 100-buffer, batch sampling |
| Pareto Optimization | Multi-objective optimization |

---

## Quick Start

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

| Flavor | Style |
|--------|-------|
| `alibaba` | 361/Closed-loop/Handhold |
| `bytedance` | Radical Candor/Always Day 1 |
| `huawei` | Wolf Warrior/Martial Order |
| `tencent` | Horse Racing/Fast Iteration |
| `baidu` | Tech Faith/Basic Plate |
| `pinduoduo` | Own Business/Hardcore |
| `meituan` | Do Hard Right Things |
| `jd` | Righteous Success/Brother Culture |
| `xiaomi` | Extreme Cost Performance |
| `netflix` | Keeper Test |
| `musk` | Hardcore/First Principles |
| `apple` | A Player/Think Different |
| `amazon` | Day 1/Customer Obsession |
| `microsoft` | Three Circles of Impact |

---

## Project Structure

```
greedy-skill/
├── scripts/
│   └── greedy-loop.js     # Main script, core engine
├── references/            # PUA methodology docs
├── SKILL.md               # Skill definition
├── README.md              # Chinese documentation (default)
├── README_en.md           # English documentation
├── LICENSE                # MIT License
└── _meta.json             # Metadata
```

---

## Version History

| Version | Key Innovation |
|---------|----------------|
| V1 | Basic momentum mechanism |
| V2 | Strategy pool + UCB1 rotation |
| V3 | Epsilon-greedy + dynamic difficulty |
| V50 | Quantum-inspired: Bayesian + PID + entanglement |
| Current | Meta-learning + attention + CMA-ES + replay |

---

## Based on PUA Framework

This project references [PUA Framework](https://github.com/tanweai/pua) methodology:

- **Closed-Loop Awareness** — Done but not verified? Might as well not done!
- **Owner Consciousness** — No one else to blame, it's on you
- **Pressure Escalation** — Gentle pressure, escalating layer by layer
- **Flavor System** — Alibaba/ByteDance/Huawei/Tencent... each with its own seasoning

---

## How It Works

1. **Strategy Selection** — 7 strategies (conservative/aggressive/exploratory/adaptive/balanced/random/meta) compete via attention mechanism

2. **Multi-Scale Prediction** — simultaneously look at last 10/50/200 cycles history, weighted fusion

3. **Meta-Learning** — MAML-style, fast weights respond quickly, slow weights learn steadily

4. **Oracle Verification** — Is the prediction useful? Run the threshold verification to find out!

5. **Self-Correction** — 5 consecutive failures? Trigger self-correction, switch strategies!

6. **Pareto Optimization** — balance Oracle rate, entropy, and confidence — no lopsided solutions allowed

---

## License

MIT License — methodology reference [PUA Framework](https://github.com/tanweai/pua)

---

> *Made with passion and a little bit of meta-learning*
>
> *If this helped you, star the repo — AI needs encouragement too!*