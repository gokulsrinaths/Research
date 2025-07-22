# Cooperate or Collapse: Emergence of Sustainable Cooperation in a Society of LLM Agents

[![NeurIPS 2024](https://img.shields.io/badge/Conference-NeurIPS%202024-blue)](https://neurips.cc/Conferences/2024)
[![Code](https://img.shields.io/badge/Code-GovSim-green)](https://github.com/giorgiopiatti/GovSim)

## Authors
- Giorgio Piatti (ETH Zürich)
- Zhijing Jin (ETH Zürich, MPI, University of Toronto)
- Max Kleiman-Weiner (University of Washington)
- Bernhard Schölkopf (MPI for Intelligent Systems)
- Mrinmaya Sachan (ETH Zürich)
- Rada Mihalcea (University of Michigan)

## Abstract
This research investigates how societies of LLM-based agents can sustainably govern shared resources in multi-agent environments. Through the introduction of GOVSIM, a novel multi-agent simulation framework, we explore the emergence of cooperation and sustainable resource management among LLM agents.

## Key Contributions
- **GOVSIM Framework**: A multi-agent, multi-turn LLM simulation for studying cooperation
- **Comprehensive Benchmarking**: Evaluation of 15+ LLMs across 3 sustainability scenarios
- **Universalization Impact**: Demonstrated how moral reasoning improves cooperative outcomes
- **Communication Analysis**: Quantified the value of agent dialogue in achieving sustainability
- **Open Source**: Full environment and agent prompts available for research

## Technical Approach
### Framework Components
- Multi-agent system with shared resource environments
- Phase-based architecture: Harvest → Discuss → Reflect
- Support for moral reasoning and memory reflection
- Transparent action visibility among agents

### Scenarios
1. Fishery Management
2. Pasture Sustainability
3. Pollution Control

## Key Results
- GPT-4 achieved >50% survival rate in sustainability scenarios
- Agent communication reduced resource overuse by 22%
- Universalization-based reasoning increased survival time by 4 months on average
- Most LLMs require explicit prompting for long-term consequence consideration

## Strengths
- Novel multi-agent benchmark grounded in moral philosophy
- Strong empirical methodology with comprehensive ablations
- Highlights current limitations in LLM reasoning capabilities
- Open-source implementation for reproducibility

## Limitations
- Simplified resource dynamics (single resource type per scenario)
- Limited to language-based agents (no physical/multimodal simulation)
- Assumes ideal prompt adherence
- API cost constraints affected some robustness testing

## Citation
```bibtex
@inproceedings{piatti2024cooperate,
  title={Cooperate or Collapse: Emergence of Sustainable Cooperation in a Society of LLM Agents},
  author={Piatti, Giorgio and Jin, Zhijing and Kleiman-Weiner, Max and Schölkopf, Bernhard and Sachan, Mrinmaya and Mihalcea, Rada},
  booktitle={Advances in Neural Information Processing Systems},
  year={2024}
}
```

## Links
- [GitHub Repository](https://github.com/giorgiopiatti/GovSim)
- [NeurIPS 2024](https://neurips.cc/Conferences/2024) 