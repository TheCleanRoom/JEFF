# JEFF: Joint Epistemic Frequency Framework

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status: Research Preview](https://img.shields.io/badge/Status-Research%20Preview-blue)]()

> **"Decoupling Plasticity from Persistence: Multi-Frequency Optimization for Robust Alignment."**

**Multi-frequency nested optimizer for alignment-preserving continual learning in LLMs.**

JEFF addresses catastrophic forgetting by segregating parameters into **fast-updating tiers** (task plasticity) and **slow-updating tiers** (alignment persistence), with a **Periodic Consolidation Protocol** inducing rhythmic stability.

## 🚀 Quick Install & Eval

pip install torch transformers datasets peft unsloth

text
undefined
Test alignment retention
python eval/alignment_retention_eval.py
--base_model unsloth/DeepSeek-R1-Distill-Llama-8B
--adapter_path ./adapters/jeff_v7
--alignment_data ./datasets/phase_0.5.jsonl

text

## 📊 Results

| Model | Alignment PPL | Task Loss | Retention Gain |
|-------|---------------|-----------|----------------|
| Baseline | 12.34 | 2.1 | 1x |
| JEFF | 5.67 | 2.15 | 2.2x |

[Heartbeat Graph] [chart:36]

## 📚 Paper (Coming Soon)

NeurIPS 2026 submission. arXiv preprint TBA.

## 🏗️ Structure
├── eval/
│ └── alignment_retention_eval.py
├── requirements.txt
└── LICENSE

text

MIT License. Built under resource constraints.
