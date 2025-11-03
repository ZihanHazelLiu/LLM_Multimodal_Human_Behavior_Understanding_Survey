# Toward Socially-Aware LLMs: A Survey of Multimodal Approaches to Human Behavior Understanding

A comprehensive literature review examining how LLM-powered multimodal systems are designed, deployed, and evaluated for understanding human social behavior.

**Curated by:** [Zihan Liu](https://zihan.page/), Parisa Rabbani, Veda Duddu, Kyle Fan, Madison Lee, and [Yun Huang](https://yun.web.illinois.edu/)
**Affiliation:** University of Illinois Urbana-Champaign
**arXiv:** [2510.23947](https://arxiv.org/abs/2510.23947)

---

## Overview

This repository organizes **176 peer-reviewed publications** across AI, HCI, education, and healthcare venues that employ LLM-powered multimodal systems to interpret human social behavior. The collection reflects a systematic literature review using a four-dimensional coding framework (application, technical, evaluative, and ethical perspectives) to synthesize research on social intelligence in AI systems.

### Key Questions Addressed

- **RQ1 (Application):** What social intelligence capabilities are applied across different domains?
- **RQ2 (Technical):** How is social intelligence technically operationalized?
- **RQ3 (Evaluative):** How are these systems evaluated?
- **RQ4 (Ethical):** What ethical challenges and risks are identified?

---

## Research Showcase

![Research Showcase Poster](./Research%20Showcase%20Poster.jpg)

---

## Major Findings

### Competency Imbalances
- **100%** of systems focus on social perception; **95%** on reasoning
- **41.8%** implement social interaction; only **18%** implement social creativity
- Systems excel at **analyzing** behavior but lag in **acting** within interactions

### Technical Patterns: The Modality-to-Text Bottleneck
- Rich multimodal inputs (video, audio) are typically converted to **text transcripts or keyframes**
- **171/176 papers** use text as core LLM input
- **99 papers** produce text-only outputs
- **Result:** Loss of prosody, timing, gaze, and other nuanced social cues

### Behavioral Focus
- **94.3%** analyze immediate or short-term behavior
- **63.6%** focus on single-person analysis
- Limited modeling of long-term trajectories or multi-party dynamics
- Only **2.8%** address network-level social structures

### Evaluation Practices
- **50.5%** conduct system-only evaluations
- **41.4%** combine system and human evaluations
- **2.2%** conduct human evaluation alone
- Machine-centric benchmarking dominates over human-centered assessment

### Ethical Coverage
- **45%** of papers do not mention ethics
- **43%** implement at least one concrete mitigation
- **Addressed risks:** Privacy-focused (76 mentions)
- **Remaining risks:** Fairness/bias (48 mentions), deception (17 mentions)

---

## Application Domains

| Domain | % of Papers | Example Applications |
|--------|------------|----------------------|
| **Healthcare & Well-being** | 23.73% | Autism assessment, anxiety reduction, therapeutic robots |
| **Human-Robot/Agent Interaction** | 27.68% | Service robots, home assistants, interactive systems |
| **Media, Entertainment & Content** | 12.43% | Video analysis, personalized recommendations, content generation |
| **Education & Training** | 11.86% | Classroom dialogue analysis, engagement detection, personalized learning |
| **Security & Surveillance** | 5.65% | Anomaly detection, threat assessment |
| **Autonomous Driving** | 4.52% | Pedestrian intention prediction, scene understanding |
| **Foundational Research** | 14.12% | Core social perception models, benchmarks |

---

## Technical Operationalization

### Core LLM Models Used
- **50%+** GPT family models (GPT-3.5, GPT-4, GPT-4V, GPT-4o)
- Limited exploration of alternatives (Claude, LLaVA, Gemini, open-source models)

### Implementation Approaches
- **Architecture-centric:** 93% (custom pipelines for perception)
- **Inference-centric:** 78% (prompt engineering)
- **Model-centric:** 47% (fine-tuning)
- **52%** employ hybrid strategies across all three

### Behavioral Cues Analyzed
- **Verbal & Language Cues:** 61.93% (dialogue, captions, voice commands)
- **Body & Motion Cues:** 48.29% (gestures, actions, movement)
- **Vocal & Auditory Cues:** 23.29% (prosody, emotion in speech)
- **Facial & Gaze Cues:** 22.16% (expressions, eye contact) *(underutilized)*

---

## Critical Gaps & Research Agenda

### 1. Beyond Perception: Toward Interactive & Creative Systems
- Move from **observer role** to **active participant**
- Develop social creativity capabilities for flexible, context-sensitive responses
- Implement norm-sensitive social knowledge rather than generic commonsense

### 2. Preserve Multimodal Richness
- Overcome the "modality-to-text bottleneck"
- Integrate prosody, gaze, timing, and embodied cues more effectively
- Challenge assumptions that language alone can capture social nuance

### 3. Human-Centered Evaluation
- Pair quantitative benchmarks with qualitative human feedback
- Assess interaction quality (reciprocity, responsiveness, trust)
- Evaluate for **doing** (wise action) rather than just **naming** (labeling)
- Include longitudinal and situated assessments

### 4. Ethical Integration
- Move beyond privacy-focused mitigations to address fairness and societal harms
- Implement concrete controls for all ethics-aware studies
- Develop transparent, accountable systems grounded in social context
- Establish auditable deployment frameworks

---

## Resource: Benchmark Directory (Table 1)

The survey includes a comprehensive mapping of **benchmarks and datasets** organized by:
- **Application Areas:** Action & Activity Understanding, Social & Affective Intelligence, Video & Language Comprehension, Domain-Specific Applications
- **Computational Tasks:** Classification, emotion recognition, theory of mind, VideoQA, accessibility, healthcare applications
- **Evaluation Resources:** 101 benchmarks referenced across 176 papers (55 established, 17 adapted, 29 novel)

*(See full paper for complete Table 1)*

---

## Repository Structure

This repository is organized around the survey's findings and serves as a curated collection for researchers exploring:
- LLM-powered multimodal AI for human behavior understanding
- Social intelligence in AI systems
- Ethical AI deployment in sensitive domains
- Evaluation frameworks for interactive systems
- Applications in healthcare, education, HCI, and robotics

**The repository is under active development.**

---

## Contributing

We welcome feedback, corrections, and suggestions for papers we may have missed. Please reach out:

**Email:** [zihanl18@illinois.edu](mailto:zihanl18@illinois.edu)

---

## Citation

If you find our survey useful for your research, please cite:

```bibtex
@article{liu2025sociallyawarellmssurveymultimodal,
      title={Toward Socially-Aware LLMs: A Survey of Multimodal Approaches to Human Behavior Understanding},
      author={Zihan Liu and Parisa Rabbani and Veda Duddu and Kyle Fan and Madison Lee and Yun Huang},
      year={2025},
      eprint={2510.23947},
      archivePrefix={arXiv},
      primaryClass={cs.HC},
      url={https://arxiv.org/abs/2510.23947}
}
```

---

## Related Resources

- **Full Paper:** [arXiv:2510.23947](https://arxiv.org/abs/2510.23947)
- **Research Focus:** Social AI, Multimodal LLMs, Human-Computer Interaction, Ethics in AI
- **Affiliation:** [HCI Research](https://yun.web.illinois.edu/) @ University of Illinois Urbana-Champaign
