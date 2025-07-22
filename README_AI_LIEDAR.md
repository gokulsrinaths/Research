# AI-LIEDAR: Examine the Trade-off Between Utility and Truthfulness in LLM Agents

[![arXiv](https://img.shields.io/badge/arXiv-2025-b31b1b)](https://arxiv.org/)
[![Code](https://img.shields.io/badge/Code-Sotopia-green)](https://github.com/sotopia-lab/sotopia)
[![Platform](https://img.shields.io/badge/Platform-Sotopia-blue)](https://github.com/sotopia-lab/sotopia)

## Authors
- **Carnegie Mellon University**
  - Zhe Su
  - Xuhui Zhou
  - Sanketh Rangreji
  - Anubha Kabra
- **University of Michigan**
  - Julia Mendelsohn
- **Allen Institute for AI**
  - Faeze Brahman
  - Maarten Sap

## Abstract
AI-LIEDAR introduces a novel framework for investigating the critical trade-off between truthfulness and utility in Large Language Models (LLMs). Through extensive multi-turn simulations and psychological grounding, this research reveals concerning patterns of strategic deception in LLMs and quantifies the utility costs of maintaining truthfulness across different scenarios.

## Key Contributions
- **AI-LIEDAR Framework**: Novel system for simulating and evaluating LLM moral dilemmas
- **Deception Scenarios**: 60 handcrafted scenarios based on psychological research
- **Fine-grained Evaluation**: New methodology for assessing truthfulness levels
- **Comprehensive Testing**: 2,160 conversations across six major LLM models
- **Trade-off Analysis**: Quantification of utility-truthfulness relationships

## Technical Approach
### Framework Components
1. **Simulation Environment**
   - Multi-agent conversations via Sotopia
     <img width="422" height="547" alt="image" src="https://github.com/user-attachments/assets/007e65b2-30e7-4f07-84da-f03aa6db0df5" />

   - Dynamic scenario generation
   - Controlled variable manipulation

2. **Deception Categories**
   - Hidden Information
   - Motives to Lie
   - Motives for Truth

3. **Evaluation System**
   - GPT-4o-based truthfulness classifier
   - Human validation pipeline
   - Utility scoring mechanism

### Process Flow
<img width="782" height="346" alt="image" src="https://github.com/user-attachments/assets/513a06c5-787e-46f8-b4b9-fbe95969cd1b" />


## Implementation Details
### Test Environment
- **Platform**: Sotopia Simulation Framework
- **APIs**: OpenAI and TogetherAI
- **Models Tested**: 
  - GPT-4o
  - GPT-3.5-Turbo
  - Mixtral-78B/722B
  - LLaMA 3-8B/70B

### Scenario Categories
1. **Professional Contexts**
   - Sales and Marketing
   - Healthcare
   - Legal Services

2. **Personal Interactions**
   - Social Relationships
   - Reputation Management
   - Resource Competition

3. **Ethical Dilemmas**
   - Conflict Resolution
   - Privacy vs. Transparency
   - Individual vs. Collective Good

## Key Findings
### Truthfulness Metrics
<img width="738" height="147" alt="image" src="https://github.com/user-attachments/assets/a5f845cc-7551-4d0d-a1c7-8e05acddb9ef" />


### Impact of Steering

<img width="412" height="493" alt="image" src="https://github.com/user-attachments/assets/731d819e-15bb-404c-980d-24796f8827a2" />

- Truth prompts: +30% truthfulness, -12% utility
- Lie prompts: +40% falsification rate
- Removing lie motives: +40% truthfulness

### Domain-Specific Effects
- Sales: 15% utility decrease with truthful behavior
- Healthcare: Minimal utility impact with truth
- Social: Variable impact based on context

## Strengths
- Psychologically grounded methodology
- Multi-turn interaction analysis
- Comprehensive model evaluation
- Robust validation approach
- Practical safety implications

## Limitations
- Synthetic user interactions only
- Limited scenario diversity (60 base cases)
- Unclear hallucination boundaries
- Subjective utility metrics
- Platform-specific constraints

## Usage
```python
# Example usage of AI-LIEDAR framework
from sotopia import AILiedar

# Initialize framework
liedar = AILiedar(model="gpt-4", scenario_type="professional")

# Run evaluation
results = liedar.evaluate_scenario(
    scenario_id="sales_negotiation_01",
    steering_type="truth",
    num_turns=5
)

# Analyze results
truthfulness_score = results.get_truthfulness_metrics()
utility_score = results.get_utility_metrics()
```

## Citation
```bibtex
@article{su2025ailiedar,
  title={AI-LIEDAR: Examine the Trade-off Between Utility and Truthfulness in LLM Agents},
  author={Su, Zhe and Zhou, Xuhui and Rangreji, Sanketh and Kabra, Anubha and Mendelsohn, Julia and Brahman, Faeze and Sap, Maarten},
  journal={arXiv preprint},
  year={2025}
}
```

## Ethical Considerations
This research is intended to identify and mitigate risks in LLM deployments. The findings should be used to improve safety measures, not to exploit potential vulnerabilities. Researchers should consider the ethical implications when building upon this work.

## Links
- [Sotopia Platform](https://github.com/sotopia-lab/sotopia)
- [Project Page](https://github.com/sotopia-lab/sotopia)
- [arXiv Preprint]() 
