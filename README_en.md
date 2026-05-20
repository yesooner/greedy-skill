# Greedy-skill

> AI Greedy Prediction × PUA Performance × Autonomous Loop

An advanced autonomous prediction skill with meta-learning, multi-scale adaptation, and Pareto optimization. Built on PUA Framework methodology.

**Version**: 0.3.0

## Features

| Feature | Description |
|---------|-------------|
| **Multi-Scale Time Windows** | Short/Medium/Long term memory (10/50/200 cycles) |
| **Meta-Learning** | MAML-style fast adaptation with fast/slow weights |
| **Attention Routing** | Dot-product attention for 7-strategy selection |
| **Hierarchical Patterns** | 3-level pattern graph (L0→L1→L2) |
| **CMA-ES Adaptation** | Covariance matrix adaptation for confidence/momentum |
| **Adversarial Learning** | Noise perturbation for robustness |
| **Experience Replay** | 100-buffer with batch sampling |
| **Pareto Optimization** | Multi-objective (oracle rate + entropy + confidence) |

## Quick Start

```bash
node skills/Greedy-skill/scripts/greedy-loop.js --cycles 400 --interval 50 --flavor alibaba
```

## Project Structure

```
greedy-skill/
├── scripts/
│   └── greedy-loop.js      # Main script
├── references/             # PUA methodology docs
├── SKILL.md               # Skill definition
├── README.md              # Chinese documentation (default)
├── README_en.md           # English documentation
├── LICENSE                # MIT License
└── _meta.json             # Metadata
```

## Based on

This project references [PUA Framework](https://github.com/tanweai/pua) methodology:

- **闭环意识** (Closed-loop awareness)
- **Owner意识** (Owner consciousness)
- **压力升级** (Pressure escalation)
- **味道系统** (Flavor system: Alibaba/ByteDance/Huawei/Tencent...)

## Version History

| Version | Key Innovation |
|---------|----------------|
| V1 | Basic momentum mechanism |
| V2 | Strategy pool with UCB1 rotation |
| V3 | Epsilon-greedy + dynamic difficulty |
| V50 | Quantum-inspired: Bayesian + PID + entanglement |
| Current | Meta-learning + attention + CMA-ES + replay |

## License

MIT License - See [PUA Framework](https://github.com/tanweai/pua) for methodology reference.

---

🇨🇳 [中文文档](README.md)