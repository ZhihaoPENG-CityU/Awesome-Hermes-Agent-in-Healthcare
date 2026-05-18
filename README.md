<h1 align="center">
  <strong>Awesome-Hermes-Agent-in-Healthcare</strong>
</h1>
<!-- Hermes-style healthcare agents: memory, skills, tools, and self-evolution -->
<p align="center">
  <sub>Curated papers &amp; open-source resources · Healthcare Agent · Memory · Skill · Self-evolution</sub>
</p>

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <!-- <a href="https://github.com/ZhihaoPENG-CityU/Awesome-Hermes-Agent-in-Healthcare/stargazers"><img src="https://img.shields.io/github/stars/ZhihaoPENG-CityU/Awesome-Hermes-Agent-in-Healthcare?style=social" alt="GitHub stars"></a> -->
  <a href="#-contributing"><img src="https://img.shields.io/badge/Contributions-Welcome-brightgreen?style=flat-square" alt="Contributions welcome"></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Healthcare-Agent-0f766e?style=flat-square" alt="Healthcare Agent">&nbsp;
  <img src="https://img.shields.io/badge/Memory-1d4ed8?style=flat-square" alt="Memory">&nbsp;
  <img src="https://img.shields.io/badge/Skill-6d28d9?style=flat-square" alt="Skill">&nbsp;
  <img src="https://img.shields.io/badge/Self--Evolution-b91c1c?style=flat-square" alt="Self-evolution">
</p>

<p align="center">
  A curated list of <strong>papers</strong> and <strong>open-source resources</strong> on
  <strong>Hermes-style healthcare agents</strong>:
  agentic systems that combine <strong>clinical reasoning</strong>,
  <strong>long-term memory</strong>, <strong>reusable skills</strong>,
  <strong>tool use</strong>, and <strong>self-evolution</strong>
  for healthcare, medicine, and biomedical research.
</p>

<table align="center">
  <tr>
    <td align="center" width="25%"><b>Agent</b><br/><sub>Clinical reasoning, tools, workflows</sub></td>
    <td align="center" width="25%"><b>Memory</b><br/><sub>Patient, case, episodic, retrieval</sub></td>
    <td align="center" width="25%"><b>Skill</b><br/><sub>Skill libraries, tool use, distillation</sub></td>
    <td align="center" width="25%"><b>Evolution</b><br/><sub>Reflection, feedback, continual improvement</sub></td>
  </tr>
</table>

<br/>

---

<a id="contents"></a>

## 📌 Contents

- [Scope](#-scope)
- [Taxonomy](#-taxonomy)
- [Tags](#-tags)
- [Hermes-Style Healthcare Agent Papers](#-hermes-style-healthcare-agent-papers-2023now)
- [Survey Papers](#-survey-papers)
- [Historical Agent-Based Healthcare](#classic-agent-based-health-care-20022008)
- [By Topic](#-by-topic)
- [Related Repositories](#-related-repositories)
- [Acknowledgements](#-acknowledgements)
- [Contributing](#-contributing)
- [Contact Us](#-contact-us)

---

## 🎯 Scope

This repository curates research on **Hermes-style healthcare agents**: agentic systems that can reason over clinical or biomedical tasks, use tools, accumulate memory, acquire reusable skills, and improve through feedback or self-evolution.

**In scope:**

- Healthcare agents for diagnosis, EHR workflows, care planning, patient interaction, clinical operations, biomedical discovery, and medical imaging workflows.
- Agent memory, including patient memory, clinical trajectory memory, episodic memory, retrieval memory, and long-context case memory.
- Agent skills, including tool-use skills, skill libraries, workflow skills, skill retrieval, skill distillation, and medical skill audits.
- Self-evolving or self-improving agents, including reflection, feedback learning, experience replay, closed-loop improvement, and continual adaptation.
- Evaluation and governance for healthcare agents, including clinical benchmarks, hallucination detection, safety rails, physician alignment, privacy, and regulatory frameworks.

**Related but secondary:**

- General agent, memory, skill, or self-evolution methods that are clearly transferable to healthcare.
- Medical VLM or multimodal systems when they include agentic reasoning, tool use, memory, or self-improvement.
- Historical pre-LLM healthcare agent systems, kept mainly as background context.

---

## 🧬 Taxonomy

| Track | Focus |
|------|-------|
| **Healthcare Agents** | Clinical consultation, EHR agents, diagnosis agents, care planning, biomedical research agents, and healthcare workflow automation. |
| **Memory for Healthcare Agents** | Patient-specific memory, case memory, longitudinal records, retrieval-augmented memory, and clinical trajectory modeling. |
| **Skills and Tool Use** | Medical tool use, workflow skills, skill libraries, skill retrieval, skill audit, and reproducible clinical workflows. |
| **Self-Evolving Healthcare Agents** | Reflection, feedback learning, self-improvement, closed-loop clinical agents, and biomedical agents that evolve from experience. |
| **Evaluation, Safety, and Governance** | Clinical benchmarks, hallucination detection, physician agreement, privacy, safety rails, audits, and regulatory frameworks. |
| **Related Foundations** | General-purpose agent, memory, skill, and self-evolution papers that provide reusable methods for healthcare agents. |

---

<a id="tags"></a>

## 🏷️ Tags

Entries are curated with a primary scope tag and, when useful, one or more capability tags. Prefer concise combinations such as `[Core][Memory]`, `[Core][Skill][Evolution]`, or `[Foundation][Eval]`.

| Tag | Meaning |
|-----|---------|
| **`[Core]`** | Primary focus: healthcare or biomedical agents with memory, skills, tool use, self-evolution, or agent evaluation. |
| **`[Memory]`** | Agent memory, patient memory, case memory, longitudinal clinical records, retrieval memory, or trajectory modeling. |
| **`[Skill]`** | Skill learning, skill libraries, skill retrieval, tool-use skills, workflow skills, or skill distillation. |
| **`[Evolution]`** | Self-improvement, reflection, feedback learning, continual adaptation, experience replay, or agent self-evolution. |
| **`[Eval]`** | Benchmarks, safety evaluation, hallucination detection, physician agreement, governance, audit, or regulatory frameworks. |
| **`[Foundation]`** | General agent, memory, skill, or self-evolution methods that are strongly transferable to healthcare agents. |
| **`[Background]`** | Healthcare or biomedical multimodal work that is useful context but is not primarily agentic. |
| **`[Archive]`** | Historical healthcare agent systems or background works kept for literature context. |

> **Note:** Tags are **curatorial**, not quality judgments. Use `[Core]` for healthcare-agent work, then add capability tags like `[Memory]`, `[Skill]`, `[Evolution]`, or `[Eval]` when they describe the main contribution.

---

## 📝 Hermes-Style Healthcare Agent Papers (2023–Now)

> **Default order (time):** Within each `###` calendar year, entries are **newest first**, using the numeric order of the first `arxiv.org/abs/` or `arxiv.org/pdf/` id `YYMM.NNNNN` when present (e.g. `2605.*` before `2604.*` before `2603.*`). Entries with a bioRxiv/medRxiv `/10.1101/YYYY.MM.DD` path use that calendar date; bullets without any such id sort at the **end** of that year. Papers whose arXiv id implies another calendar year are grouped under the matching `###` heading. Venue tags use **`(*Venue'YY_MM*)`** when the month is known from links, otherwise the short **`(*Venue'YY*)`** form (no `_MM`).
>
> **Tags:** See [Tags](#-tags) for the Hermes-oriented tag definitions.
>
> **Other sort orders:** Plain GitHub Markdown has **no** interactive sort controls. Keep new additions in time order and use the taxonomy above to keep the list browsable.
>
> **Out-of-scope entries** (relative to [Scope](#-scope) **In scope**) are wrapped in HTML comments (`<!-- … -->`): they stay in the file for reference but are **hidden** on GitHub-rendered Markdown.

### 2026

<!--
  - [Foundation] (*arXiv'26_05*) **GraphFlow: An Architecture for Formally Verifiable Visual Workflows Enabling Reliable Agentic AI Automation**
    [[📝 Paper](https://arxiv.org/abs/2605.14968)]

-->
<!--
  - [Foundation] (*arXiv'26_05*) **Holistic Evaluation and Failure Diagnosis of AI Agents**
    [[📝 Paper](https://arxiv.org/abs/2605.14865)]

-->
- [Core] (*arXiv'26_05*) **Agentifying Patient Dynamics within LLMs through Interacting with Clinical World Model**
  [[📝 Paper](https://arxiv.org/abs/2605.14723)] [[💻 Code](https://github.com/FreedomIntelligence/SepsisAgent)]

- [Foundation][Memory][Evolution] (*arXiv'26_05*) **SAGE: A Self-Evolving Agentic Graph-Memory Engine for Structure-Aware Associative Memory**
  [[📝 Paper](https://arxiv.org/abs/2605.12061)]

- [Foundation][Evolution][Eval] (*arXiv'26_05*) **On-Policy Self-Evolution via Failure Trajectories for Agentic Safety Alignment (FATE)**
  [[📝 Paper](https://arxiv.org/abs/2605.11882)]

- [Foundation][Eval] (*arXiv'26_05*) **Agent-ValueBench: A Comprehensive Benchmark for Evaluating Agent Values**
  [[📝 Paper](https://arxiv.org/abs/2605.10365)]

- [Core][Eval] (*arXiv'26_05*) **AgentRx: A Benchmark Study of LLM Agents for Multimodal Clinical Prediction Tasks**
  [[📝 Paper](https://arxiv.org/abs/2605.10286)] [[💻 Code](https://github.com/nyuad-cai/AgentRX)]

- [Foundation] (*arXiv'26_05*) **MCP-Cosmos: World Model-Augmented Agents for Complex Task Execution in MCP Environments**
  [[📝 Paper](https://arxiv.org/abs/2605.09131)]

- [Core][Eval] (*arXiv'26_05*) **Measuring What Matters: Benchmarking Generative, Multimodal, and Agentic AI in Healthcare**
  [[📝 Paper](https://arxiv.org/abs/2605.08445)]

- [Foundation] (*arXiv'26_05*) **MASPO: Joint Prompt Optimization for LLM-based Multi-Agent Systems**
  [[📝 Paper](https://arxiv.org/abs/2605.06623)] [[💻 Code](https://github.com/wangzx1219/MASPO)]

<!--
  - [Foundation] (*arXiv'26_05*) **SkillOS: Learning Skill Curation for Self-Evolving Agents**
    [[📝 Paper](https://arxiv.org/abs/2605.06614)] [[💻 Code](https://github.com/EvolvingAgentsLabs/skillos)]

-->
- [Core] (*arXiv'26_05*) **NeuroAgent: LLM Agents for Multimodal Neuroimaging Analysis and Research**
  [[📝 Paper](https://arxiv.org/abs/2605.06584)]

- [Core] (*arXiv'26_05*) **A Versatile AI Agent for Rare Disease Diagnosis and Risk Gene Prioritization**
  [[📝 Paper](https://arxiv.org/abs/2605.06226)]

- [Foundation] (*arXiv'26_05*) **TheraAgent: Self-Improving Therapeutic Agent for Precise and Comprehensive Treatment Planning**
  [[📝 Paper](https://arxiv.org/abs/2605.05963)]

<!--
  - [Foundation] (*arXiv'26_05*) **MemTier: Tiered Memory Architecture and Retrieval Bottleneck Analysis for Long-Running Autonomous AI Agents**
    [[📝 Paper](https://arxiv.org/abs/2605.03675)]

-->
- [Core] (*arXiv'26_05*) **CuraView: A Multi-Agent Framework for Medical Hallucination Detection with GraphRAG-Enhanced Knowledge Verification**
  [[📝 Paper](https://arxiv.org/abs/2605.03476)]

- [Core] (*arXiv'26_05*) **Healthcare AI GYM for Medical Agents**
  [[📝 Paper](https://arxiv.org/abs/2605.02943)] [[💻 Code](https://github.com/minstar/Healthcare_GYM)]

- [Core] (*arXiv'26_05*) **An Empirical Study of Agent Skills for Healthcare: Practice, Gaps, and Governance**
  [[📝 Paper](https://arxiv.org/abs/2605.02709)]

<!--
  - [Foundation] (*arXiv'26_05*) **ARA: Agentic Reproducibility Assessment for Scalable Support of Scientific Peer-Review**
    [[📝 Paper](https://arxiv.org/abs/2605.02651)] [[💻 Code](https://github.com/AndresLaverdeMarin/agentic_reproducibility_assessment)]

-->
- [Core] (*arXiv'26_05*) **PhysicianBench: Evaluating LLM Agents in Real-World EHR Environments**
  [[📝 Paper](https://arxiv.org/abs/2605.02240)]

- [Core] (*arXiv'26_05*) **Virtual Speech Therapist: A Clinician-in-the-Loop AI Speech Therapy Agent for Personalized and Supervised Therapy**
  [[📝 Paper](https://arxiv.org/abs/2605.01101)]

- [Background] (*arXiv'26_04*) **LLM as Clinical Graph Structure Refiner: Enhancing Representation Learning in EEG Seizure Diagnosis**
  [[📝 Paper](https://arxiv.org/abs/2604.28178)]

- [Core] (*arXiv'26_04*) **Modeling Clinical Concern Trajectories in Language Model Agents**
  [[📝 Paper](https://arxiv.org/abs/2604.27872)]

- [Background] (*arXiv'26_04*) **Iterative Multimodal Retrieval-Augmented Generation for Medical Question Answering**
  [[📝 Paper](https://arxiv.org/abs/2604.27724)]

- [Core] (*arXiv'26_04*) **Detecting Clinical Discrepancies in Health Coaching Agents: A Dual-Stream Memory and Reconciliation Architecture**
  [[📝 Paper](https://arxiv.org/abs/2604.27045)]

- [Background] (*arXiv'26_04*) **MedSynapse-V: Bridging Visual Perception and Clinical Intuition via Latent Memory Evolution**
  [[📝 Paper](https://arxiv.org/abs/2604.26283)]

- [Background] (*arXiv'26_04*) **Case-Specific Rubrics for Clinical AI Evaluation: Methodology, Validation, and LLM-Clinician Agreement Across 823 Encounters**
  [[📝 Paper](https://arxiv.org/abs/2604.24710)]

- [Core] (*arXiv'26_04*) **NeuroClaw Technical Report: Closed-Loop Agentic AI for Executable and Reproducible Neuroimaging Research**
  [[📝 Paper](https://arxiv.org/abs/2604.24696)] [[🌐 Project](https://cuhk-aim-group.github.io/NeuroClaw/index.html)] [[💻 Code](https://github.com/CUHK-AIM-Group/NeuroClaw)]

<!--
  - [Foundation] (*arXiv'26_04*) **Skill Retrieval Augmentation for Agentic AI**
    [[📝 Paper](https://arxiv.org/abs/2604.24594)] [[💻 Code](https://github.com/oneal2000/SR-Agents)]

-->
- [Foundation] (*arXiv'26_04*) **FastOMOP: A Foundational Architecture for Reliable Agentic Real-World Evidence Generation on OMOP CDM Data**
  [[📝 Paper](https://arxiv.org/abs/2604.24572)] [[💻 Code](https://github.com/fastomop)]

- [Core] (*arXiv'26_04*) **Agentic Clinical Reasoning over Longitudinal Myeloma Records: A Retrospective Evaluation Against Expert Consensus**
  [[📝 Paper](https://arxiv.org/abs/2604.24473)]

- [Core] (*arXiv'26_04*) **Agentic AI Platforms for Autonomous Training and Rule Induction of Human-Human and Virus-Human Protein-Protein Interactions**
  [[📝 Paper](https://arxiv.org/abs/2604.23924)]

<!--
  - [Foundation] (*arXiv'26_04*) **ClawTrace: Cost-Aware Tracing for LLM Agent Skill Distillation**
    [[📝 Paper](https://arxiv.org/abs/2604.23853)] [[💻 Code](https://github.com/epsilla-cloud/clawtrace)]

-->
- [Core] (*arXiv'26_04*) **EndoGov: A knowledge-governed multi-agent expert system for endometrial cancer risk stratification**
  [[📝 Paper](https://arxiv.org/abs/2604.23802)]

- [Eval] (*arXiv'26_04*) **Vibe Medicine: Redefining Biomedical Research Through Human-AI Co-Work**
  [[📝 Paper](https://arxiv.org/abs/2604.23674)]

<!--
  - [Background] (*arXiv'26_04*) **VeriLLMed: Interactive Visual Debugging of Medical Large Language Models with Knowledge Graphs**
    [[📝 Paper](https://arxiv.org/abs/2604.23356)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **From Research Question to Scientific Workflow: Leveraging Agentic AI for Science Automation**
    [[📝 Paper](https://arxiv.org/abs/2604.21910)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **Transient Turn Injection: Exposing Stateless Multi-Turn Vulnerabilities in Large Language Models**
    [[📝 Paper](https://arxiv.org/abs/2604.21860)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **AEL: Agent Evolving Learning for Open-Ended Environments**
    [[📝 Paper](https://arxiv.org/abs/2604.21725)] [[💻 Code](https://github.com/WujiangXu/AEL)]

-->
- [Core] (*arXiv'26_04*) **Trustworthy Clinical Decision Support Using Meta-Predicates and Domain-Specific Languages**
  [[📝 Paper](https://arxiv.org/abs/2604.21263)]

- [Core] (*arXiv'26_04*) **Agentic AI for Personalized Physiotherapy: A Multi-Agent Framework for Generative Video Training and Real-Time Pose Correction**
  [[📝 Paper](https://arxiv.org/abs/2604.21154)]

<!--
  - [Foundation] (*arXiv'26_04*) **Co-Evolving LLM Decision and Skill Bank Agents for Long-Horizon Tasks**
    [[📝 Paper](https://arxiv.org/abs/2604.20987)] [[🌐 Project](https://wuxiyang1996.github.io/COSPLAY_page/)] [[💻 Code](https://github.com/wuxiyang1996/cos-play)]

-->
- [Eval] (*arXiv'26_04*) **Can "AI" Be a Doctor? A Study of Empathy, Readability, and Alignment in Clinical LLMs**
  [[📝 Paper](https://arxiv.org/abs/2604.20791)]

- [Foundation] (*arXiv'26_04*) **Learning to Evolve: A Self-Improving Framework for Multi-Agent Systems via Textual Parameter Graph Optimization**
  [[📝 Paper](https://arxiv.org/abs/2604.20714)]

- [Core] (*arXiv'26_04*) **MedSkillAudit: A Domain-Specific Audit Framework for Medical Research Agent Skills**
  [[📝 Paper](https://arxiv.org/abs/2604.20441)]

- [Core] (*arXiv'26_04*) **From Fuzzy to Formal: Scaling Hospital Quality Improvement with AI**
  [[📝 Paper](https://arxiv.org/abs/2604.20055)]

- [Core] (*arXiv'26_04*) **AblateCell: A Reproduce-then-Ablate Agent for Virtual Cell Repositories**
  [[📝 Paper](https://arxiv.org/abs/2604.19606)]

<!--
  - [Foundation] (*arXiv'26_04*) **A Self-Evolving Framework for Efficient Terminal Agents via Observational Context Compression**
    [[📝 Paper](https://arxiv.org/abs/2604.19572)]

-->
<!--
  - [Foundation] (*ACL'26_04*) **From Experience to Skill: Multi-Agent Generative Engine Optimization via Reusable Strategy Learning**
    [[📝 Paper](https://arxiv.org/abs/2604.19516)] [[💻 Code](https://github.com/Wu-beining/MAGEO)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **MDAgent: A Multi-Agent Framework for End-to-End Molecular Dynamics Research**
    [[📝 Paper](https://arxiv.org/abs/2604.18622)]

-->
- [Foundation] (*arXiv'26_04*) **First, Do No Harm (With LLMs): Mitigating Racial Bias via Agentic Workflows**
  [[📝 Paper](https://arxiv.org/abs/2604.18038)]

- [Core] (*arXiv'26_04*) **Neuro-Symbolic Resolution of Recommendation Conflicts in Multimorbidity Clinical Guidelines**
  [[📝 Paper](https://arxiv.org/abs/2604.17340)]

- [Core] (*arXiv'26_04*) **From Clinical Intent to Clinical Model: An Autonomous Coding-Agent Framework for Clinician-driven AI Development**
  [[📝 Paper](https://arxiv.org/abs/2604.17110)] [[💻 Code](https://github.com/zhaozh10/clinical-automata)]

<!--
  - [Foundation] (*arXiv'26_04*) **GenericAgent: A Token-Efficient Self-Evolving LLM Agent via Contextual Information Density Maximization**
    [[📝 Paper](https://arxiv.org/abs/2604.17091)] [[💻 Code](https://github.com/lsdefine/GenericAgent)]

-->
- [Core] (*arXiv'26_04*) **Agentic Large Language Models for Training-Free Neuro-Radiological Image Analysis**
  [[📝 Paper](https://arxiv.org/abs/2604.16729)]

- [Foundation] (*arXiv'26_04*) **DeepER-Med: Advancing Deep Evidence-Based Research in Medicine Through Agentic AI**
  [[📝 Paper](https://arxiv.org/abs/2604.15456)]

- [Core] (*arXiv'26_04*) **RadAgent: A Tool-Using AI Agent for Stepwise Interpretation of Chest Computed Tomography**
  [[📝 Paper](https://arxiv.org/abs/2604.15231)] [[🌐 Project](https://rad-agent.github.io/)]

<!--
  - [Foundation] (*arXiv'26_04*) **Autogenesis: A Self-Evolving Agent Protocol**
    [[📝 Paper](https://arxiv.org/abs/2604.15034)]

-->
- [Eval] (*arXiv'26_04*) **Can LLMs Score Medical Diagnoses and Clinical Reasoning as well as Expert Panels?**
  [[📝 Paper](https://arxiv.org/abs/2604.14892)]

- [Background] (*arXiv'26_04*) **Rethinking Patient Education as Multi-turn Multi-modal Interaction**
  [[📝 Paper](https://arxiv.org/abs/2604.14656)]

- [Core] (*arXiv'26_04*) **Evo-MedAgent: Beyond One-Shot Diagnosis with Agents That Remember, Reflect, and Improve**
  [[📝 Paper](https://arxiv.org/abs/2604.14475)]

<!--
  - [Background] (*arXiv'26_04*) **Seeing Through Experts' Eyes: A Foundational Vision Language Model Trained on Radiologists' Gaze and Reasoning**
    [[📝 Paper](https://arxiv.org/abs/2604.14316)]

-->
- [Background] (*arXiv'26_04*) **Enhancing Reinforcement Learning for Radiology Report Generation with Evidence-aware Rewards and Self-correcting Preference Learning**
  [[📝 Paper](https://arxiv.org/abs/2604.13598)]

- [Core] (*arXiv'26_04*) **QuarkMedSearch: A Long-Horizon Deep Search Agent for Exploring Medical Intelligence**
  [[📝 Paper](https://arxiv.org/pdf/2604.12867)]

- [Core] (*arXiv'26_04*) **CARIS: Coding-Free and Privacy-Preserving MCP Framework for Clinical Agentic Research Intelligence System**
  [[📝 Paper](https://arxiv.org/abs/2604.12258)]

- [Core] (*arXiv'26_04*) **Development, Evaluation, and Deployment of a Multi-Agent System for Thoracic Tumor Board**
  [[📝 Paper](https://arxiv.org/abs/2604.12161)]

- [Core] (*ACL'26_04*) **Dialectic-Med: Mitigating Diagnostic Hallucinations via Counterfactual Adversarial Multi-Agent Debate**
  [[📝 Paper](https://arxiv.org/abs/2604.11258)]

<!--
  - [Foundation] (*arXiv'26_04*) **Mem^2Evolve: Towards Self-Evolving Agents via Co-Evolutionary Capability Expansion and Experience Distillation**
    [[📝 Paper](https://arxiv.org/abs/2604.10923)] [[💻 Code](https://buaa-irip-llm.github.io/Mem2Evolve)]

-->
- [Core] (*arXiv'26_04*) **CAMYLA: Scaling Autonomous Research in Medical Image Segmentation**
  [[📝 Paper](https://arxiv.org/abs/2604.10696)] [[🌐 Project](https://yifangao112.github.io/camyla-page/)]

- [Core] (*arXiv'26_04*) **Constraint-Aware Corrective Memory for Language-Based Drug Discovery Agents (CACM)**
  [[📝 Paper](https://arxiv.org/abs/2604.09308)]

<!--
  - [Foundation] (*arXiv'26_04*) **SEA-Eval: A Benchmark for Evaluating Self-Evolving Agents Beyond Episodic Assessment**
    [[📝 Paper](https://arxiv.org/abs/2604.08988)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **Multi-Agent Decision-Focused Learning via Value-Aware Sequential Communication (SeqComm-DFL)**
    [[📝 Paper](https://arxiv.org/abs/2604.08944)]

-->
- [Eval] (*arXiv'26_04*) **Grounding Clinical AI Competency in Human Cognition Through the Clinical World Model and Skill-Mix Framework**
  [[📝 Paper](https://arxiv.org/abs/2604.08226)]

<!--
  - [Foundation] (*arXiv'26_04*) **SEARL: Joint Optimization of Policy and Tool Graph Memory for Self-Evolving Agents**
    [[📝 Paper](https://arxiv.org/abs/2604.07791)]

-->
- [Core] (*arXiv'26_04*) **EMSDialog: Synthetic Multi-person Emergency Medical Service Dialogue Generation from Electronic Patient Care Reports via Multi-LLM Agents**
  [[📝 Paper](https://arxiv.org/abs/2604.07549)]

- [Core] (*arXiv'26_04*) **Joint Optimization of Reasoning and Dual-Memory for Self-Learning Diagnostic Agent**
  [[📝 Paper](https://arxiv.org/pdf/2604.07269)]

- [Core] (*arXiv'26_04*) **LungCURE: Benchmarking Multimodal Real-World Clinical Reasoning for Precision Lung Cancer Diagnosis and Treatment**
  [[📝 Paper](https://arxiv.org/pdf/2604.06925)]

- [Foundation] (*arXiv'26_04*) **SymptomWise: A Deterministic Reasoning Layer for Reliable and Efficient AI Systems**
  [[📝 Paper](https://arxiv.org/pdf/2604.06375)]

- [Core] (*arXiv'26_04*) **Evidence-Based Actor-Verifier Reasoning for Echocardiographic Agents**
  [[📝 Paper](https://arxiv.org/pdf/2604.06347)]

- [Core] (*arXiv'26_04*) **MAT-Cell: A Multi-Agent Tree-Structured Reasoning Framework for Batch-Level Single-Cell Annotation**
  [[📝 Paper](https://arxiv.org/abs/2604.06269)] [[💻 Code](https://github.com/jiangliu91/MAT-Cell-A-Multi-Agent-Tree-Structured-Reasoning-Framework-for-Batch-Level-Single-Cell-Annotation)]

- [Core] (*arXiv'26_04*) **From Exposure to Internalization: Dual-Stream Calibration for In-context Clinical Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2604.06262)]

- [Core] (*arXiv'26_04*) **BAAI Cardiac Agent: An intelligent multimodal agent for automated reasoning and diagnosis of cardiovascular diseases from cardiac magnetic resonance imaging**
  [[📝 Paper](https://arxiv.org/abs/2604.04078)] [[💻 Code](https://github.com/plantain-herb/Cardiac-Agent)]

<!--
  - [Foundation] (*arXiv'26_04*) **SKILLFOUNDRY: Building Self-Evolving Agent Skill Libraries from Heterogeneous Scientific Resources**
    [[📝 Paper](https://arxiv.org/abs/2604.03964)]

-->
- [Core] (*arXiv'26_04*) **XrayClaw: Cooperative-Competitive Multi-Agent Alignment for Trustworthy Chest X-ray Diagnosis**
  [[📝 Paper](https://arxiv.org/pdf/2604.02695)]

<!--
  - [Foundation] (*arXiv'26_04*) **CoEvoSkills: Self-Evolving Agent Skills via Co-Evolutionary Verification**
    [[📝 Paper](https://arxiv.org/abs/2604.01687)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **CORAL: Towards Autonomous Multi-Agent Evolution for Open-Ended Discovery**
    [[📝 Paper](https://arxiv.org/abs/2604.01658)] [[💻 Code](https://github.com/Human-Agent-Society/CORAL)]

-->
- [Core] (*arXiv'26_04*) **CARE: Privacy-Compliant Agentic Reasoning with Evidence Discordance**
  [[📝 Paper](https://arxiv.org/abs/2604.01113)]

- [Core] (*arXiv'26_04*) **PsychAgent: An Experience-Driven Lifelong Learning Agent for Self-Evolving Psychological Counselor**
  [[📝 Paper](https://arxiv.org/abs/2604.00931)]

- [Core] (*arXiv'26_04*) **Can Large Language Models Self-Correct in Medical Question Answering? An Exploratory Study**
  [[📝 Paper](https://arxiv.org/abs/2604.00261)]

- [Core] (*arXiv'26_04*) **A Safety-Aware Role-Orchestrated Multi-Agent LLM Framework for Behavioral Health Communication Simulation**
  [[📝 Paper](https://arxiv.org/abs/2604.00249)]

- [Core] (*arXiv'26_04*) **Agentic AI for Clinical Urgency Mapping and Queue Optimization in High-Volume Outpatient Departments: A Simulation-Based Evaluation**
  [[📝 Paper](https://arxiv.org/abs/2604.00215)]

- [Core] (*bioRxiv'26_04*) **A Unified Agent-Enabled Platform for Drug Repurposing across Molecular, Phenotypic, and Clinical Scales**
  [[📝 Paper](https://www.biorxiv.org/content/10.64898/2026.04.19.719462v1)]

- [Core] (*medRxiv'26_04*) **Artificial Intelligence Agents in Mental Health: A Systematic Review and Meta Analysis**
  [[📝 Paper](https://www.medrxiv.org/content/10.64898/2026.04.21.26351365v1)]

- [Eval] (*medRxiv'26_04*) **Dissecting clinical reasoning failures in frontier artificial intelligence using 10,000 synthetic cases**
  [[📝 Paper](https://www.medrxiv.org/content/10.64898/2026.04.22.26351488v1)]

- [Eval] (*medRxiv'26_04*) **HAARF: Healthcare AI Agents Regulatory Framework**
  [[📝 Paper](https://www.medrxiv.org/content/10.64898/2026.04.09.26350519v1)] [[💻 Code](https://github.com/Task-force-for-AI-agents-in-Healthcare/haarf)]

- [Core] (*arXiv'26_04*) **One Panel Does Not Fit All: Case-Adaptive Multi-Agent Deliberation for Clinical Prediction (CAMP)**
  [[📝 Paper](https://arxiv.org/abs/2604.00085)]

<!--
  - [Foundation] (*arXiv'26_03*) **Cognitive Friction: A Decision-Theoretic Framework for Bounded Deliberation in Tool-Using Agents**
    [[📝 Paper](https://arxiv.org/abs/2603.30031)]

-->
- [Core] (*arXiv'26_03*) **Perfecting Human–AI Interaction at Clinical Scale: Turning Production Signals into Safer, More Human Conversations**
  [[📝 Paper](https://arxiv.org/abs/2603.29893)]

- [Core] (*arXiv'26_03*) **Symphony for Medical Coding: A Next-Generation Agentic System for Scalable and Explainable Medical Coding**
  [[📝 Paper](https://arxiv.org/abs/2603.29709)]

<!--
  - [Foundation] (*arXiv'26_03*) **Meta-Harness: End-to-End Optimization of Model Harnesses**
    [[📝 Paper](https://arxiv.org/pdf/2603.28052)]

-->
- [Core] (*arXiv'26_03*) **Improving Clinical Diagnosis with Counterfactual Multi-Agent Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2603.27820)]

- [Core] (*arXiv'26_03*) **Self-evolving AI agents for protein discovery and directed evolution**
  [[📝 Paper](https://arxiv.org/abs/2603.27303)] [[💻 Code](https://github.com/ai4protein/VenusFactory2)]

- [Core] (*arXiv'26_03*) **MediHive: A Decentralized Agent Collective for Medical Question Answering**
  [[📝 Paper](https://arxiv.org/abs/2603.27150)]

<!--
  - [Foundation] (*arXiv'26_03*) **AIRA_2: Overcoming Bottlenecks in AI Research Agents**
    [[📝 Paper](https://arxiv.org/pdf/2603.26499)]

-->
<!--
  - [Foundation] (*arXiv'26_03*) **Reflect to Inform: Boosting Multimodal Reasoning via Information-Gain-Driven Verification**
    [[📝 Paper](https://arxiv.org/pdf/2603.26348v1)]

-->
- [Core] (*arXiv'26_03*) **SkinGPT-X: A Self-Evolving Collaborative Multi-Agent System for Transparent and Trustworthy Dermatological Diagnosis**
  [[📝 Paper](https://arxiv.org/abs/2603.26122)]

- [Core] (*arXiv'26_03*) **Doctorina MedBench: End-to-End Evaluation of Agent-Based Medical AI**
  [[📝 Paper](https://arxiv.org/pdf/2603.25821)]

<!--
  - [Foundation] (*arXiv'26_03*) **UI-Voyager: A Self-Evolving GUI Agent Learning via Failed Experience**
    [[📝 Paper](https://arxiv.org/pdf/2603.24533v1)]

-->
- [Core] (*arXiv'26_03*) **CarePilot: A Multi-Agent Framework for Long-Horizon Computer Task Automation in Healthcare**
  [[📝 Paper](https://arxiv.org/abs/2603.24157)] [[🌐 Project](https://akashghosh.github.io/Care-Pilot/)] [[💻 Code](https://github.com/AkashGhosh/CarePilot)]

- [Core] (*arXiv'26_03*) **GSEM: Graph-based Self-Evolving Memory for Experience Augmented Clinical Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2603.22096)]

<!--
  - [Foundation] (*arXiv'26_03*) **When Models Judge Themselves: Unsupervised Self-Evolution for Multimodal Reasoning**
    [[📝 Paper](https://arxiv.org/pdf/2603.21289v1)]

-->
<!--
  - [Foundation] (*arXiv'26_03*) **MemMA: Coordinating the Memory Cycle through Multi-Agent Reasoning and In-Situ Self-Evolution**
    [[📝 Paper](https://arxiv.org/abs/2603.18718)]

-->
<!--
  - [Foundation] (*arXiv'26_03*) **AgentFactory: A Self-Evolving Framework Through Executable Subagent Accumulation and Reuse**
    [[📝 Paper](https://arxiv.org/abs/2603.18000)] [[💻 Code](https://github.com/zzatpku/AgentFactory)]

-->
<!--
  - [Foundation] (*arXiv'26_03*) **SkillEvolver: Dynamic Skill Lifecycle Management for Agentic RL**
    [[📝 Paper](https://arxiv.org/abs/2603.17187)] [[💻 Code](https://github.com/aiming-lab/MetaClaw)]

-->
- [Core] (*arXiv'26_03*) **OpenHospital: A Thing-in-itself Arena for Evolving and Benchmarking LLM-based Collective Intelligence**
  [[📝 Paper](https://arxiv.org/abs/2603.14771)] [[💻 Code](https://github.com/ZJU-LLMs/Agent-Kernel/tree/main/demo/OpenHospital)]

- [Core] (*arXiv'26_03*) **EviAgent: Evidence-Driven Agent for Radiology Report Generation**
  [[📝 Paper](https://arxiv.org/pdf/2603.13956)]

- [Core] (*arXiv'26_03*) **TheraAgent: Multi-Agent Framework with Self-Evolving Memory and Evidence-Calibrated Reasoning for PET Theranostics**
  [[📝 Paper](https://arxiv.org/abs/2603.13676)]

<!--
  - [Foundation] (*arXiv'26_03*) **CreativeBench: Benchmarking and Enhancing Machine Creativity via Self-Evolving Challenges**
    [[📝 Paper](https://arxiv.org/pdf/2603.11863)]

-->
- [Core] (*arXiv'26_03*) **Emulating Clinician Cognition via Self-Evolving Deep Clinical Research**
  [[📝 Paper](https://arxiv.org/abs/2603.10677)]

- [Core] (*arXiv'26_03*) **Skill-Evolving Grounded Reasoning for Free-Text Promptable 3D Medical Image Segmentation**
  [[📝 Paper](https://arxiv.org/abs/2603.08215)]

<!--
  - [Foundation] (*arXiv'26_03*) **EvoScientist: Towards Multi-Agent Evolving AI Scientists for End-to-End Scientific Discovery**
    [[📝 Paper](https://arxiv.org/pdf/2603.08127)]

-->
- [Core] (*arXiv'26_03*) **Med-Evo: Test-time Self-evolution for Medical Multimodal Large Language Models**
  [[📝 Paper](https://arxiv.org/abs/2603.07443)]

- [Core] (*arXiv'26_03*) **Evolving Medical Imaging Agents via Experience-driven Self-skill Discovery (MACRO)**
  [[📝 Paper](https://arxiv.org/abs/2603.05860)]

<!--
  - [Foundation] (*arXiv'26_03*) **Tool-Genesis: A Task-Driven Tool Creation Benchmark for Self-Evolving Language Agent**
    [[📝 Paper](https://arxiv.org/pdf/2603.05578)]

-->
<!--
  - [Foundation] (*arXiv'26_03*) **AutoSkill: Experience-Driven Lifelong Learning via Skill Self-Evolution**
    [[📝 Paper](https://arxiv.org/abs/2603.01145)] [[💻 Code](https://github.com/ECNU-ICALK/AutoSkill)]

-->
<!--
  - [Background] (*arXiv'26_03*) **How Well Do Multimodal Models Reason on ECG Signals?**
    [[📝 Paper](https://arxiv.org/abs/2603.00312)]

-->
- [Eval] (*arXiv'26_02*) **The Doctor Will (Still) See You Now: On the Structural Limits of Agentic AI in Healthcare**
  [[📝 Paper](https://arxiv.org/abs/2602.18460)]

- [Eval] (*arXiv'26_02*) **Agentic AI, Medical Morality, and the Transformation of the Clinic**
  [[📝 Paper](https://arxiv.org/abs/2602.16553)]

- [Core] (*arXiv'26_02*) **Closing Reasoning Gaps in Clinical Agents with Differential Reasoning Learning**
  [[📝 Paper](https://arxiv.org/abs/2602.09945)]

<!--
  - [Foundation] (*arXiv'26_02*) **S1-NexusAgent: a Self-Evolving Agent Framework for Multidisciplinary Scientific Research**
    [[📝 Paper](https://arxiv.org/abs/2602.01550)]

-->
<!--
  - [Foundation] (*arXiv'26_02*) **Position: Agentic Evolution is the Path to Evolving LLMs**
    [[📝 Paper](https://arxiv.org/pdf/2602.00359v2)]

-->
- [Core] (*bioRxiv'26_02*) **PantheonOS: An Evolvable Multi-Agent Framework for Automatic Genomics Discovery**
  [[📝 Paper](https://www.biorxiv.org/content/10.64898/2026.02.26.707870v1)] [[🌐 Project](https://pantheonos.stanford.edu)] [[💻 Code](https://github.com/aristoteleo)]

- [Core] (*arXiv'26_01*) **EvoClinician: A Self-Evolving Agent for Multi-Turn Medical Diagnosis via Test-Time Evolutionary Learning**
  [[📝 Paper](https://arxiv.org/abs/2601.22964)] [[💻 Code](https://github.com/yf-he/EvoClinician)]

- [Core] (*arXiv'26_01*) **Route, Retrieve, Reflect, Repair (R⁴): Self-Improving Agentic Framework for Visual Detection and Linguistic Reasoning in Medical Imaging**
  [[📝 Paper](https://arxiv.org/abs/2601.08192)] [[💻 Code](https://github.com/faiyazabdullah/MultimodalMedAgent)]

- [Core] (*arXiv'26_01*) **IBISAgent: Reinforcing Pixel-Level Visual Reasoning in MLLMs for Universal Biomedical Object Referring and Segmentation**
  [[📝 Paper](https://arxiv.org/abs/2601.03054)]

- [Core] (*arXiv'26_01*) **ClinicalReTrial: A Self-Evolving AI Agent for Clinical Trial Protocol Optimization**
  [[📝 Paper](https://arxiv.org/abs/2601.00290)]

- [Core] (*bioRxiv'26_01*) **Agentomics: An Agentic System that Autonomously Develops Novel State-of-the-art Solutions for Biomedical Machine Learning Tasks**
  [[📝 Paper](https://www.biorxiv.org/content/10.64898/2026.01.27.702049v1)]

- [Core] (*AACR Annual Meeting'26*) **Agentic AI as the Cancer Researcher: Autonomous Discovery in Oncology**
  [[🌐 Program](https://www.aacr.org/meeting/aacr-annual-meeting-2026/program/)]

- [Core] (*CEEM'26*) **From Non-Agentic LLMs to Multi-Agent Systems in Emergency Medicine: A Scoping Review**
  [[📝 Paper](https://doi.org/10.15441/ceem.26.136)]

- [Core] (*Cambridge Open Engage'26*) **Artificial Epidemiology: How Self-Evolving Clinical AI Manufactures Disease Prevalence from Administrative Coding Artifacts**
  [[📝 Paper](https://doi.org/10.33774/coe-2026-ssm1q)]

- [Core] (*Expert Syst. Appl.'26*) **CARE: A clinical agentic reasoning engine to enhance real-World diagnostic accuracy via structured medical reasoning**
  [[📝 Paper](https://doi.org/10.1016/j.eswa.2026.131476)]

<!--
  - [Foundation] (*GitHub'26*) **EverOS: Build, evaluate, and integrate long-term memory for self-evolving agents**
    [[💻 Code](https://github.com/EverMind-AI/EverOS)]

-->
<!--
  - [Foundation] (*GitHub'26*) **NanoResearch: Co-Evolving Skills, Memory, and Policy for Personalized Research Automation**
    [[💻 Code](https://github.com/OpenRaiser/NanoResearch)]

-->
- [Eval] (*Health Inf Sci Syst'26*) **Enhancing LLM-based medical decision-making by test-time knowledge acquisition**
  [[📝 Paper](https://doi.org/10.1007/s13755-026-00449-8)]

<!--
  - [Foundation] (*ICLR'26 Rejected*) **SkillEvo: An Experience Learning Framework with Reinforcement Learning for Skill Evolution**
    [[📝 Paper](https://openreview.net/forum?id=S1cIE9pe3k)]

-->
- [Core] (*Nat. Health'26*) **A multi-agent framework combining large language models with medical flowcharts for self-triage**
  [[📝 Paper](https://www.nature.com/articles/s44360-026-00112-2)] [[💻 Code](https://github.com/digihealthucsd/Multi-agent-self-triage-system)]

- [Core] (*Nat. Med.'26*) **An agentic framework for autonomous scientific discovery in cancer pathology**
  [[📝 Paper](https://www.nature.com/articles/s41591-026-04357-y)]

- [Core] (*Nature Biomedical Engineering'26*) **BioMedAgent: A Self-Evolving LLM Multi-Agent Framework for Autonomous, Tool-Aware Biomedical Data Analyses**
  [[📝 Paper](https://www.nature.com/articles/s41551-026-01634-6)] [[🌐 Project](http://biomed.drai.cn)] [[💻 Code](https://github.com/BOBQWERA/BioMedAgent)]

<!--
  - [Foundation] (*arXiv'26*) **MAGE: Multi-Agent Self-Evolution with Co-Evolutionary Knowledge Graphs**
    [[🌐 arXiv](https://arxiv.org/search/?searchtype=all&query=MAGE%3A%20Multi-Agent%20Self-Evolution%20with%20Co-Evolutionary%20Knowledge%20Graphs&abstracts=show&order=-announced_date_first&size=25)]

-->
- [Core] (*npj Digital Medicine'26*) **EvoMDT: A Self-Evolving Multi-Agent System for Structured Clinical Decision-Making in Multi-Cancer**
  [[📝 Paper](https://www.nature.com/articles/s41746-025-02304-8)] [[💻 Code](https://github.com/KesselZ/EvoMDT)]

- [Core] (*bioRxiv'26_07*) **STELLA: Towards a Biomedical World Model with Self-Evolving Multimodal Agents**
  [[📝 Paper](https://www.biorxiv.org/content/10.1101/2025.07.01.662467v2)]

- [Core] (*bioRxiv'26_06*) **OriGene: A Self-Evolving Virtual Disease Biologist Automating Therapeutic Target Discovery**
  [[📝 Paper](https://www.biorxiv.org/content/10.1101/2025.06.03.657658v2)]

### 2025

- [Core] (*arXiv'25_10*) **Evolving Diagnostic Agents in a Virtual Clinical Environment**
  [[📝 Paper](https://arxiv.org/abs/2510.24654)]

- [Core] (*bioRxiv'25_10*) **LabOS: The AI-XR Co-Scientist That Sees and Works With Humans**
  [[📝 Paper](https://www.biorxiv.org/content/10.1101/2025.10.16.679418v2)] [[💻 Code](https://github.com/zaixizhang/LabOS)] [[🌐 Project](https://ai4labos.com/)]

- [Foundation] (*ICLR'26_10*) **EvoTest: Evolutionary Test-Time Learning for Self-Improving Agentic Systems**
  [[📝 Paper](https://arxiv.org/abs/2510.13220)] [[💻 Code](https://github.com/yf-he/EvoTest)]

<!--
  - [Foundation] (*ICLR'26_10*) **CoT-Evo: Evolutionary Distillation of CoT for Scientific Reasoning**
    [[📝 Paper](https://arxiv.org/abs/2510.13166)] [[💻 Code](https://github.com/Irving-Feng/CoT-Evo)]

-->
- [Core] (*arXiv'25_10*) **RareAgent: Self-Evolving Reasoning for Drug Repurposing in Rare Diseases**
  [[📝 Paper](https://arxiv.org/abs/2510.05764)]

- [Core] (*ICLR'26_10*) **Doctor-R1: Mastering Clinical Inquiry with Experiential Agentic Reinforcement Learning**
  [[📝 Paper](https://arxiv.org/abs/2510.04284)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10006814)] [[💻 Code](https://github.com/thu-unicorn/Doctor-R1)]

- [Core] (*ICLR'26_09*) **KnowGuard: Knowledge-Driven Abstention for Multi-Round Clinical Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2509.24816)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10008150)] [[💻 Code](https://github.com/IcecreamArtist/KnowGuard)]

- [Core] (*arXiv'25_09*) **MedLA: A Logic-Driven Multi-Agent Framework for Complex Medical Reasoning with Large Language Models**
  [[📝 Paper](https://arxiv.org/abs/2509.23725)]

- [Core] (*arXiv'25_09*) **A Co-evolving Agentic AI System for Medical Imaging Analysis (TissueLab)**
  [[📝 Paper](https://arxiv.org/abs/2509.20279)] [[🖥️ Platform](https://tissuelab.org)]

- [Core] (*arXiv'25_09*) **MACD: Multi-Agent Clinical Diagnosis with Self-Learned Knowledge for LLM**
  [[📝 Paper](https://arxiv.org/abs/2509.20067)]

- [Core] (*arXiv'25_09*) **Evaluation of Causal Reasoning for Large Language Models in Contextualized Clinical Scenarios of Laboratory Test Interpretation**
  [[📝 Paper](https://arxiv.org/abs/2509.16372)]

<!--
  - [Foundation] (*arXiv'25_09*) **Evolving-RL: End-to-End Optimization of Experience-Driven Self-Evolving Capability**
    [[📝 Paper](https://arxiv.org/abs/2509.15194)] [[💻 Code](https://github.com/YujunZhou/EVOL-RL)]

-->
- [Eval] (*medRxiv'25_08*) **Automation Bias in Large Language Model Assisted Diagnostic Reasoning Among AI-Trained Physicians**
  [[📝 Paper](https://www.medrxiv.org/content/10.1101/2025.08.23.25334280v2)]

- [Core] (*arXiv'25_08*) **HealthFlow: A Self-Evolving AI Agent with Meta Planning for Autonomous Healthcare Research**
  [[📝 Paper](https://arxiv.org/abs/2508.02621)] [[💻 Code](https://github.com/yhzhu99/HealthFlow)]

- [Core] (*arXiv'25_06*) **Integrating Dynamical Systems Learning with Foundational Models: A Meta-Evolutionary AI Framework for Clinical Trials**
  [[📝 Paper](https://arxiv.org/abs/2506.14782)]

- [Core] (*ICLR'26_06*) **Language Agents for Hypothesis-driven Clinical Decision Making with Reinforcement Learning**
  [[📝 Paper](https://arxiv.org/abs/2506.13474)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10011252)] [[💻 Code](https://github.com/dharouni/LA-CDM)]

- [Core] (*arXiv'25_06*) **CounselBench: A Large-Scale Expert Evaluation and Adversarial Benchmarking of Large Language Models in Mental Health Question Answering**
  [[📝 Paper](https://arxiv.org/abs/2506.08584)]

- [Core] (*arXiv'25_06*) **Agentomics-ML: Autonomous Machine Learning Experimentation Agent for Genomic and Transcriptomic Data**
  [[📝 Paper](https://arxiv.org/abs/2506.05542)] [[💻 Code](https://github.com/BioGeMT/Agentomics-ML)]

- [Core] (*arXiv'25_06*) **MedAgentGym: A Scalable Agentic Training Environment for Code-Centric Reasoning in Biomedical Data Science**
  [[📝 Paper](https://arxiv.org/abs/2506.04405)]

- [Core] (*ICLR'26_06*) **MMedAgent-RL: Optimizing Multi-Agent Collaboration for Multimodal Medical Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2506.00555)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10011724)]

- [Core] (*arXiv'25_05*) **Silence is Not Consensus: Disrupting Agreement Bias in Multi-Agent LLMs via Catfish Agent for Clinical Decision Making**
  [[📝 Paper](https://arxiv.org/abs/2505.21503)]

- [Core] (*arXiv'25_05*) **MedSentry: Understanding and Mitigating Safety Risks in Medical LLM Multi-Agent Systems**
  [[📝 Paper](https://arxiv.org/abs/2505.20824)] [[💻 Code](https://github.com/KaiChenNJ/MedSentry)]

- [Core] (*arXiv'25_05*) **DoctorAgent-RL: A Multi-Agent Collaborative Reinforcement Learning System for Multi-Turn Clinical Dialogue**
  [[📝 Paper](https://arxiv.org/abs/2505.19630)]

<!--
  - [Foundation] (*arXiv'25_05*) **Nature's Insight: A Novel Framework and Comprehensive Analysis of Agentic Reasoning Through the Lens of Neuroscience**
    [[📝 Paper](https://arxiv.org/abs/2505.05515)] [[💻 Code](https://github.com/BioRAILab/Awesome-Neuroscience-Agent-Reasoning)]

-->
- [Core] (*MICCAI'25_03*) **MedAgentSim: Self-Evolving Multi-Agent Simulations for Realistic Clinical Interactions**
  [[📝 Paper](https://arxiv.org/pdf/2503.22678)] [[💻 Code](https://github.com/MAXNORM8650/MedAgentSim)]

- [Core] (*ICLR'26_03*) **MedAgent-Pro: Towards Evidence-based Multi-modal Medical Diagnosis via Reasoning Agentic Workflow**
  [[📝 Paper](https://arxiv.org/abs/2503.18968)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10008810)] [[💻 Code](https://github.com/jinlab-imvr/MedAgent-Pro)]

- [Core] (*arXiv'25_03*) **MDTeamGPT: A Self-Evolving LLM-based Multi-Agent Framework for Multi-Disciplinary Team Medical Consultation**
  [[📝 Paper](https://arxiv.org/abs/2503.13856)] [[🌐 Project](https://kaichennj.github.io/MDTeamGPT-Main/)]

- [Core] (*arXiv'25_03*) **MAP: Evaluation and Multi-Agent Enhancement of Large Language Models for Inpatient Pathways**
  [[📝 Paper](https://arxiv.org/abs/2503.13205)]

- [Core] (*arXiv'25_02*) **PathFinder: A Multi-Modal Multi-Agent System for Medical Diagnostic Decision-Making Applied to Histopathology**
  [[📝 Paper](https://arxiv.org/pdf/2502.08916)]

<!--
  - [Foundation] (*arXiv'25_02*) **EvoAgent: Self-evolving Agent with Continual World Model for Long-Horizon Tasks**
    [[📝 Paper](https://arxiv.org/abs/2502.05907)] [[💻 Code](https://github.com/siyuyuan/evoagent)]

-->
- [Core] (*Advanced Science'25*) **Autonomous Self-Evolving Research on Biomedical Data: The DREAM Paradigm**
  [[📝 Paper](https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.202417066)]

<!--
  - [Foundation] (*EMNLP'25 Demo*) **EvoAgentX: An Automated Framework for Evolving Agentic Workflows**
    [[📝 Paper](https://aclanthology.org/2025.emnlp-demos.47/)] [[💻 Code](https://github.com/EvoAgentX/EvoAgentX)]

-->
- [Core] (*IEEE ICASSP'25*) **SeM-Agents: A Self-Evolving Framework for Multi-Agent Medical Consultation Based on Large Language Models**
  [[📝 Paper](https://ieeexplore.ieee.org/abstract/document/10889517)]

- [Foundation] (*IJISAE'25*) **Self-Evolving LLM Ecosystems for Precision Medicine**
  [[📝 Paper](https://ijisae.org/index.php/IJISAE/article/view/7793)]

- [Core] (*NeurIPS'25 Workshop*) **HealthAlign-Agents: Self-Play Reflective Prompting for Culturally Aligned Health Communication in Low-Resource Languages**
  [[📝 Paper](https://neurips.cc/virtual/2025/135933)]

### 2024

- [Core] (*arXiv'24_12*) **KG4Diagnosis: A Hierarchical Multi-Agent LLM Framework with Knowledge Graph Enhancement for Medical Diagnosis**
  [[📝 Paper](https://arxiv.org/abs/2412.16833)]

- [Core] (*arXiv'24_10*) **Adaptive Reasoning and Acting in Medical Language Agents**
  [[📝 Paper](https://arxiv.org/abs/2410.10020)]

- [Core] (*arXiv'24_09*) **Depression Diagnosis Dialogue Simulation: Self-improving Psychiatrist with Tertiary Memory**
  [[📝 Paper](https://arxiv.org/abs/2409.15084)]

- [Core] (*arXiv'24_05*) **AgentClinic: A Multimodal Agent Benchmark to Evaluate AI in Simulated Clinical Environments**
  [[📝 Paper](https://arxiv.org/abs/2405.07960)] [[🌐 Project](https://agentclinic.github.io)] [[💻 Code](https://github.com/samuelschmidgall/agentclinic)]

- [Core] (*arXiv'24_05*) **Agent Hospital: A Simulacrum of Hospital with Evolvable Medical Agents**
  [[📝 Paper](https://arxiv.org/abs/2405.02957)]

- [Core] (*ACM-BCB'24_04*) **ClinicalAgent: Clinical Trial Multi-Agent System with LLM-based Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2404.14777)] [[💻 Code](https://github.com/LeoYML/clinical-agent)]

- [Core] (*arXiv'24*) **Towards Conversational Diagnostic AI (AMIE)**
  [[📝 Paper](https://www.nature.com/articles/s41586-025-08866-7)]

### 2023

<!--
  - [Foundation] (*arXiv'23_12*) **ReST meets ReAct: Self-Improvement for Multi-Step Reasoning LLM Agent**
    [[📝 Paper](https://arxiv.org/abs/2312.10003)]

-->
<!--
  - [Foundation] (*arXiv'23_06*) **SELFEVOLVE: A Code Evolution Framework via Large Language Models**
    [[📝 Paper](https://arxiv.org/abs/2306.02907)]

  ---


-->
## 📚 Survey Papers

> Survey and perspective papers use `[Eval]` when they focus on evaluation, governance, safety, or clinical deployment.

- [Eval] (*npj AI'26*) **AI agent in healthcare: applications, evaluations, and future directions**
  [[📝 Paper](https://www.nature.com/articles/s44387-026-00076-4)]

- [Eval] (*arXiv'26_05*) **Beyond Individual Intelligence: Surveying Collaboration, Failure Attribution, and Self-Evolution in LLM-based Multi-Agent Systems**
  [[📝 Paper](https://arxiv.org/abs/2605.14892)]

- [Eval] (*J. Med. Syst.'26*) **When Chatbots Become Agents: The Next Phase of Healthcare AI**
  [[📝 Paper](https://doi.org/10.1007/s10916-026-02402-4)]

- [Eval] (*arXiv'26_02*) **Agentic AI in Healthcare & Medicine: A Seven-Dimensional Taxonomy for Empirical Evaluation of LLM-based Agents**
  [[📝 Paper](https://arxiv.org/abs/2602.04813)]

- [Eval] (*arXiv'26_05*) **An Empirical Study of Agent Skills for Healthcare: Practice, Gaps, and Governance**
  [[📝 Paper](https://arxiv.org/abs/2605.02709)]

- [Eval] (*medRxiv'26_04*) **Artificial Intelligence Agents in Mental Health: A Systematic Review and Meta Analysis**
  [[📝 Paper](https://www.medrxiv.org/content/10.64898/2026.04.21.26351365v1)]

- [Eval] (*CEEM'26*) **From Non-Agentic LLMs to Multi-Agent Systems in Emergency Medicine: A Scoping Review**
  [[📝 Paper](https://doi.org/10.15441/ceem.26.136)]

- [Eval] (*arXiv'25_08*) **A Comprehensive Survey of Self-Evolving AI Agents: A New Paradigm Bridging Foundation Models and Lifelong Agentic Systems**
  [[📝 Paper](https://arxiv.org/abs/2508.07407)] [[💻 Code](https://github.com/EvoAgentX/Awesome-Self-Evolving-Agents)]

<!--
  - [Eval] (*arXiv'25_07*) **A Survey of Self-Evolving Agents: What, When, How, and Where to Evolve on the Path to Artificial Super Intelligence**
    [[📝 Paper](https://arxiv.org/abs/2507.21046)]

-->
<!--
  - [Eval] (*arXiv'25_05*) **Nature's Insight: A Novel Framework and Comprehensive Analysis of Agentic Reasoning Through the Lens of Neuroscience**
    [[📝 Paper](https://arxiv.org/abs/2505.05515)] [[💻 Code](https://github.com/BioRAILab/Awesome-Neuroscience-Agent-Reasoning)]

-->
- [Eval] (*Comput Methods Programs Biomed'23*) **A Survey on Agents Applications in Healthcare: Opportunities, Challenges and Trends**
  [[📝 Paper](https://www.sciencedirect.com/science/article/pii/S0169260723001906)]

- [Eval] (*J. Med. Syst.'16*) **A Systematic Literature Review of Agents Applied in Healthcare**
  [[📝 Paper](https://doi.org/10.1007/s10916-015-0376-2)] [[Scopus](https://www.scopus.com/pages/publications/84947560681)]

- [Eval] (*Int. J. Med. Inf.'10*) **Agents applied in health care: A review**
  [[📝 Paper](https://www.sciencedirect.com/science/article/pii/S138650561000016X)] [[PubMed](https://pubmed.ncbi.nlm.nih.gov/20129820/)]

### Classic agent-based health care (2002–2008)

> Historical sections are kept as `[Archive]` background.

> Representative **software-agent / multi-agent** work targeting **clinical information systems, telecare, hospital workflows, guideline enactment, or surveillance**, with **first publication in 2002–2008** (aligned with the literature window in Isern & Sánchez & Moreno, *Int. J. Med. Inf.*, 2010).  
> **Not listed here (typical reasons):** general agent theory or MAS textbooks without a medical deployment (#1, #6–7, #38–40, #50); AI-in-medicine position pieces or surveys **dated 2009** (#5); agent papers **dated 2009** (#24 HealthAgents journal article, #54 interoperability survey); non-agent-centric bioinformatics reviews (#17); classic **ICMAS 1998** hospital scheduling (#9); incomplete / venue-unclear lines in the source list (#16).

- [Archive] (*Birkhäuser'03*) **Applications of Software Agent Technology in the Health Care Domain**
  [[📝 Book](https://link.springer.com/book/10.1007/978-3-0348-7976-7)]

- [Archive] (*PDCAT'04*) **Architecture of Agent-Based Healthcare Intelligent Assistant on Grid Environment**
  [[📝 Paper](https://doi.org/10.1007/978-3-540-30501-9_15)]

- [Archive] (*TELECARE'04*) **Aingeru: an Innovating System for Tele Assistance of Elderly People**
  [[📝 Paper](https://doi.org/10.5220/0002681100270036)]

- [Archive] (*Appl. Intell.'04*) **UCTx: A Multi-Agent System to Assist a Transplant Coordination Unit**
  [[📝 Paper](https://doi.org/10.1023/B:APIN.0000011142.91514.57)]

- [Archive] (*ISMIS'05*) **An Intelligent System for Assisting Elderly People**
  [[📝 Paper](https://doi.org/10.1007/11425274_48)]

- [Archive] (*AI Commun.'05*) **Integration of hospital data using agent technologies: A case study**
  [[📝 Paper](https://content.iospress.com/articles/ai-communications/aic342)]

- [Archive] (*AI Commun.'05*) **Agent-based ambient intelligence for healthcare**
  [[📝 Paper](https://content.iospress.com/articles/ai-communications/aic344)]

- [Archive] (*SGAI'05*) **Web-based Medical Teaching using a Multi-Agent System**
  [[📝 Paper](https://doi.org/10.1007/1-84628-224-1_14)]

- [Archive] (*IEEE Trans. IT Biomed.'05*) **A multiagent system enhancing home-care health services for chronic disease management**
  [[📝 Paper](https://doi.org/10.1109/TITB.2005.847511)]

- [Archive] (*IEEE Intell. Syst.'06*) **Secure integration of distributed medical data using mobile agents**
  [[📝 Paper](https://doi.org/10.1109/MIS.2006.120)]

- [Archive] (*IEEE Intell. Syst.'06*) **Privacy-aware autonomous agents for pervasive healthcare**
  [[📝 Paper](https://doi.org/10.1109/MIS.2006.118)]

- [Archive] (*IEEE Intell. Syst.'06*) **Increasing Human-Organ Transplant Availability: Argumentation-Based Agent Deliberation**
  [[📝 Paper](https://doi.org/10.1109/MIS.2006.116)]

- [Archive] (*Stud. Comput. Intell.'07*) **Assistive Wheelchair Navigation: A Cognitive View**
  [[📝 Paper](https://doi.org/10.1007/978-3-540-47527-9_7)]

- [Archive] (*CEEMAS'07*) **HeCaSe2: A Multi-agent Ontology-Driven Guideline Enactment Engine**
  [[📝 Paper](https://doi.org/10.1007/978-3-540-75254-7_38)]

- [Archive] (*KES-AMSTA'07*) **Mobile Agents Using Data Mining for Diagnosis Support in Ubiquitous Healthcare**
  [[📝 Paper](https://doi.org/10.1007/978-3-540-72830-6_83)]

- [Archive] (*AIME'07*) **Adaptive Optimization of Hospital Resource Calendars**
  [[📝 Paper](https://doi.org/10.1007/978-3-540-73599-1_41)]

- [Archive] (*Int. J. Med. Inf.'07*) **Towards patient-related information needs**
  [[📝 Paper](https://doi.org/10.1016/j.ijmedinf.2006.11.006)]

- [Archive] (*Artificial Intelligence in Medicine'08*) **A cognitive architecture for robot self-consciousness**
  [[📝 Paper](https://doi.org/10.1016/j.artmed.2008.07.004)]

- [Archive] (*Int. J. Med. Inf.'08*) **Computer-based execution of clinical guidelines: A review**
  [[📝 Paper](https://doi.org/10.1016/j.ijmedinf.2008.05.010)]

- [Archive] (*IEEE Intell. Syst.'08*) **GerAmI: Improving Healthcare Delivery in Geriatric Residences**
  [[📝 Paper](https://doi.org/10.1109/MIS.2008.27)]

- [Archive] (*Birkhäuser'08*) **Agent Technology and e-Health**
  [[📝 Book](https://link.springer.com/book/10.1007/978-3-7643-8547-7)]

- [Archive] (*AAMAS Industry'08*) **Agent-based patient admission scheduling in hospitals**
  [[📝 Paper](https://dl.acm.org/citation.cfm?id=1402804)]

### Agent-based healthcare systems (2009–2014)

> **Software-agent / multi-agent systems** for care delivery, health IT integration, telehealth, AAL, or clinical decision support, with **first publication in 2009–2014**.  
> **Excluded** from this block (per repository curation): epidemic/biological ABM and borderline platform-only papers; see **Curation scope** under [Contributing](#-contributing).

#### 2014

- [Archive] (*IJAIT'14*) **A multi-agent care system to support independent living**
  [[📝 Paper](https://doi.org/10.1142/S0218213014400016)]

- [Archive] (*J. Intell. Inf. Syst.'14*) **OBCAS: an agent-based system and ontology for mobile context aware interactions**
  [[📝 Paper](https://doi.org/10.1007/s10844-014-0305-8)]

- [Archive] (*IJAIT'14*) **Abductive agents for human activity monitoring**
  [[📝 Paper](https://doi.org/10.1142/S0218213014400028)]

- [Archive] (*IJAIT'14*) **Agent-based reasoning in medical planning and diagnosis combining multiple strategies**
  [[📝 Paper](https://doi.org/10.1142/S0218213014400041)]

- [Archive] (*IJAIT'14*) **Towards a simulator of integrated long-term care systems for elderly people**
  [[📝 Paper](https://doi.org/10.1142/S0218213014400053)]

- [Archive] (*J. Med. Syst.'14*) **Designing an architectural style for dynamic medical cross-organizational workflow management system: an approach based on agents and web services**
  [[📝 Paper](https://doi.org/10.1007/s10916-014-0032-2)]

- [Archive] (*ISCON'14*) **Architectural design of a multi agent enterprise knowledge management system (MAEKMS) for e-health**
  [[📝 Paper](https://doi.org/10.1109/iciscon.2014.6965225)]

- [Archive] (*Int. J. Environ. Res. Public Health'14*) **The next generation of interoperability agents in healthcare**
  [[📝 Paper](https://doi.org/10.3390/ijerph110505349)]

- [Archive] (*Procedia Technol.'14*) **Healthcare interoperability through intelligent agent technology**
  [[📝 Paper](https://doi.org/10.1016/j.protcy.2014.10.150)]

- [Archive] (*PAAMS'14*) **Assessment of agent architectures for telehealth**
  [[📝 Paper](https://doi.org/10.1007/978-3-319-07767-3_8)]

- [Archive] (*IJMLC'14*) **Multi-agent decision-making support model for the management of pre-hospital emergency services**
  [[📝 Paper](https://doi.org/10.7763/ijmlc.2014.v4.412)]

- [Archive] (*Stud. Comput. Intell.'14*) **Negotiation-based patient scheduling in hospitals — reengineering message-based interactions with services**
  [[📝 Paper](https://doi.org/10.1007/978-3-319-00467-9_10)]

- [Archive] (*Int. J. Simul. Process Model.'14*) **Evaluating policies using agent-based simulations: investigating policies for continuity of care**
  [[📝 Paper](https://doi.org/10.1504/ijspm.2014.066364)]

- [Archive] (*IJAIT'14*) **Secure P2P cross-community health record exchange in IHE compatible systems**
  [[📝 Paper](https://doi.org/10.1142/S0218213014400065)]

- [Archive] (*IJAIT'14*) **Editorial: special issue on new perspectives on the use of agents in health care**
  [[📝 Paper](https://doi.org/10.1142/S0218213014020011)]

- [Archive] (*Int. J. Environ. Res. Public Health'14*) **A mobile multi-agent information system for ubiquitous fetal monitoring**
  [[📝 Paper](https://doi.org/10.3390/ijerph110100600)]

- [Archive] (*IJAIT'14*) **A push-based agent communication model empowering assistive technologies**
  [[📝 Paper](https://doi.org/10.1142/S021821301440003x)]

#### 2013

- [Archive] (*JAISE'13*) **COMMODITY12: a smart e-health environment for diabetes management**
  [[📝 Paper](https://doi.org/10.3233/ais-130220)]

- [Archive] (*Comput. Biol. Med.'13*) **The self-aware diabetic patient software agent model**
  [[📝 Paper](https://doi.org/10.1016/j.compbiomed.2013.09.007)]

- [Archive] (*Inf. Sci.'13*) **Integrating hardware agents into an enhanced multi-agent architecture for ambient intelligence systems**
  [[📝 Paper](https://doi.org/10.1016/j.ins.2011.05.002)]

- [Archive] (*Procedia Comput. Sci.'13*) **Agent based health monitoring of elderly people in indoor environments using wireless sensor networks**
  [[📝 Paper](https://doi.org/10.1016/j.procs.2013.06.014)]

- [Archive] (*ACM Trans. Manag. Inf. Syst.'13*) **I can help you change! An empathic virtual agent delivers behavior change health interventions**
  [[📝 Paper](https://doi.org/10.1145/2544103)]

- [Archive] (*Procedia Comput. Sci.'13*) **Using an agent-based simulation for predicting the effects of patients derivation policies in emergency departments**
  [[📝 Paper](https://doi.org/10.1016/j.procs.2013.05.228)]

- [Archive] (*Comput. Biol. Med.'13*) **Formal specification and analysis of intelligent agents for model-based medicine usage management**
  [[📝 Paper](https://doi.org/10.1016/j.compbiomed.2013.01.021)]

- [Archive] (*Inf. Sci.'13*) **Context-aware multi-agent planning in intelligent environments**
  [[📝 Paper](https://doi.org/10.1016/j.ins.2012.11.021)]

- [Archive] (*Pers. Ubiquitous Comput.'13*) **Self-configuring agents for ambient assisted living applications**
  [[📝 Paper](https://doi.org/10.1007/s00779-012-0555-9)]

- [Archive] (*Int. J. Intell. Syst. Technol. Appl.'13*) **Agent-based communication systems for elders using a reminiscence therapy**
  [[📝 Paper](https://doi.org/10.1504/ijista.2013.056533)]

- [Archive] (*J. Med. Syst.'13*) **Secure mobile agent for telemedicine based on P2P networks**
  [[📝 Paper](https://doi.org/10.1007/s10916-013-9947-2)]

- [Archive] (*IJSEIA'13*) **An efficient multi-agent system for e-health functionalities**

#### 2012

- [Archive] (*J. Med. Syst.'12*) **A mobile agent approach for secure integrated medical information systems**
  [[📝 Paper](https://doi.org/10.1007/s10916-011-9749-3)]

- [Archive] (*J. Med. Syst.'12*) **Implementing an integrative multi-agent clinical decision support system with open source software**
  [[📝 Paper](https://doi.org/10.1007/s10916-010-9452-9)]

- [Archive] (*J. Med. Syst.'12*) **A study on agent-based secure scheme for electronic medical record system**
  [[📝 Paper](https://doi.org/10.1007/s10916-010-9595-8)]

- [Archive] (*J. Med. Syst.'12*) **Secure communication of medical information using mobile agents**
  [[📝 Paper](https://doi.org/10.1007/s10916-012-9857-8)]

- [Archive] (*J. Med. Syst.'12*) **Mobile agent application and integration in electronic anamnesis system**
  [[📝 Paper](https://doi.org/10.1007/s10916-010-9563-3)]

- [Archive] (*J. Med. Syst.'12*) **Deployment of secure mobile agents for medical information systems**
  [[📝 Paper](https://doi.org/10.1007/s10916-011-9716-z)]

- [Archive] (*Artif. Intell. Med.'12*) **Inconsistency as a diagnostic tool in a society of intelligent agents**
  [[📝 Paper](https://doi.org/10.1016/j.artmed.2012.04.005)]

- [Archive] (*IEEE Trans. Inf. Technol. Biomed.'12*) **Optimizing medical data quality based on multiagent web service framework**
  [[📝 Paper](https://doi.org/10.1109/titb.2012.2195498)]

- [Archive] (*Adv. Sci. Lett.'12*) **Construction of real-time weight control intelligent recommendation system using multi-agent mechanism**
  [[📝 Paper](https://doi.org/10.1166/asl.2012.2515)]

- [Archive] (*Expert Syst. Appl.'12*) **Multi-agent ontology-based Web 2.0 platform for medical rehabilitation**
  [[📝 Paper](https://doi.org/10.1016/j.eswa.2011.09.089)]

- [Archive] (*CISTI'12*) **Improving expressiveness of agents using openEHR to retrieve multi-institutional health data: feeding local repositories through HL7 based providers**

#### 2011

- [Archive] (*IEEE Trans. Knowl. Data Eng.'11*) **Integration of the HL7 standard in a multiagent system to support personalized access to e-health services**
  [[📝 Paper](https://doi.org/10.1109/tkde.2010.174)]

- [Archive] (*Procedia Comput. Sci.'11*) **An agent-based decision support system for hospitals emergency departments**
  [[📝 Paper](https://doi.org/10.1016/j.procs.2011.04.203)]

- [Archive] (*SUComS'11*) **Agent based approach in accessing distributed health care services**
  [[📝 Paper](https://doi.org/10.1007/978-3-642-23948-9_24)]

- [Archive] (*EIDWT'11*) **Designing and implementing intelligent agents for e-health**
  [[📝 Paper](https://doi.org/10.1109/eidwt.2011.19)]

- [Archive] (*J. Med. Syst.'11*) **Distributed agent based interoperable virtual EMR system for healthcare system integration**
  [[📝 Paper](https://doi.org/10.1007/s10916-009-9367-5)]

- [Archive] (*Appl. Soft Comput.'11*) **JADE implemented mobile multi-agent based, distributed information platform for pervasive health care monitoring**
  [[📝 Paper](https://doi.org/10.1016/j.asoc.2009.11.022)]

- [Archive] (*Int. J. Eng. Bus. Manag.'11*) **Building distributed E-healthcare for elderly using RFID and multi-agent**
  [[📝 Paper](https://doi.org/10.5772/45677)]

#### 2010

- [Archive] (*Int. J. E-Health Med. Commun.'10*) **Developing smart emergency applications with multi-agent systems**
  [[📝 Paper](https://doi.org/10.4018/jehmc.2010100101)]

- [Archive] (*J. Ambient Intell. Humaniz. Comput.'10*) **Ontology-based multi-agents for intelligent healthcare applications**
  [[📝 Paper](https://doi.org/10.1007/s12652-010-0011-5)]

- [Archive] (*IEEE Trans. Inf. Technol. Biomed.'10*) **A distributed, collaborative intelligent agent system approach for proactive postmarketing drug safety surveillance**
  [[📝 Paper](https://doi.org/10.1109/titb.2009.2037007)]

- [Archive] (*IEEE Intell. Syst.'10*) **An artificial urban healthcare system and applications**
  [[📝 Paper](https://doi.org/10.1109/mis.2010.76)]

- [Archive] (*Elektronika ir Elektrotechnika'10*) **Multi-agent-based human computer interaction of E-health care system for people with movement disabilities**
  [[📝 Paper](https://eejournal.ktu.lt/index.php/elt/article/view/9280)]

- [Archive] (*JAISE'10*) **An integrative ambient agent model for unipolar depression relapse prevention**
  [[📝 Paper](https://doi.org/10.3233/ais-2010-0054)]

- [Archive] (*J. Univers. Comput. Sci.'10*) **An agent-based architecture for developing activity-aware systems for assisting elderly**
  [[📝 Paper](http://www.jucs.org/jucs_16_12/an_agent_based_architecture.html)]

- [Archive] (*IGI Global book chapter'10*) **A multi-agent simulation of kidney function for medical education**
  [[📝 Paper](https://doi.org/10.4018/978-1-60566-772-0.ch010)]

- [Archive] (*IGI Global book chapter'10*) **Operating room simulation and agent-based optimization**
  [[📝 Paper](https://doi.org/10.4018/978-1-60566-772-0.ch005)]

- [Archive] (*IEEE Trans. Med. Imaging'09*) **User-agent cooperation in multiagent IVUS image segmentation**
  [[📝 Paper](https://doi.org/10.1109/tmi.2008.927351)]

#### 2009

- [Archive] (*Int. J. Telemed. Appl.'09*) **Enhancing E-health information systems with agent technology**
  [[📝 Paper](https://doi.org/10.1155/2009/279091)]

- [Archive] (*Int. J. Comput. Integr. Manuf.'09*) **Agent-services and mobile agents for an integrated HCIS**
  [[📝 Paper](https://doi.org/10.1080/09511920802537979)]

- [Archive] (*FUZZ-IEEE'09*) **Intelligent ontological multi-agent for healthy diet planning**
  [[📝 Paper](https://doi.org/10.1109/fuzzy.2009.5277049)]

- [Archive] (*Appl. Intell.'09*) **HealthAgents: distributed multi-agent brain tumor diagnosis and prognosis**
  [[📝 Paper](https://doi.org/10.1007/s10489-007-0085-8)]

- [Archive] (*Expert Syst. Appl.'09*) **Modeling and implementing an agent-based environmental health impact decision support system**
  [[📝 Paper](https://doi.org/10.1016/j.eswa.2008.01.041)]

#### Dissertation (2014; in-scope)

- [Archive] (*UAB PhD Thesis'14*) **Agent based virtual electronic patient record: from intra to inter-institution data integration**

### Agent-based healthcare systems (2015-2022)

> **Software-agent / multi-agent systems** for care delivery, clinical decision support, telehealth, or ambient assisted living, with **first publication in 2015-2022** — this block **adds Crossref DOI–verified agent-for-healthcare applications** complementing the year windows above.  
> **Excluded** (same curation policy): epidemic/biological ABM and platform-only papers without care-oriented agent behavior; see **Curation scope** under [Contributing](#-contributing).

#### 2021

- [Archive] (*J. Med. Syst.'21*) **Cohort and Trajectory Analysis in Multi-Agent Support Systems for Cancer Survivors**
  [[📝 Paper](https://doi.org/10.1007/s10916-021-01770-3)]

- [Archive] (*IEEE Access'21*) **A Multi-Agent Approach for Personalized Hypertension Risk Prediction**
  [[📝 Paper](https://doi.org/10.1109/access.2021.3074791)]

#### 2020

- [Archive] (*J. Med. Syst.'20*) **On the Integration of Agents and Digital Twins in Healthcare**
  [[📝 Paper](https://doi.org/10.1007/s10916-020-01623-5)]

- [Archive] (*J. Med. Syst.'20*) **Agent-oriented Decision Support System for Business Processes Management with Genetic Algorithm Optimization: an Application in Healthcare**
  [[📝 Paper](https://doi.org/10.1007/s10916-020-01608-4)]

#### 2019

- [Archive] (*Simul. Model. Pract. Theory'19*) **Agent-based dynamic optimization for managing the workflow of the patient's pathway**
  [[📝 Paper](https://doi.org/10.1016/j.simpat.2019.101935)]

- [Archive] (*Artif. Intell. Med.'19*) **Personalized conciliation of clinical guidelines for comorbid patients through multi-agent planning**
  [[📝 Paper](https://doi.org/10.1016/j.artmed.2018.11.003)]

#### 2018

- [Archive] (*Telemat. Inform.'18*) **Developing a multi-agent platform supporting patient hospital stays following a socio-technical approach: Management and governance benefits**
  [[📝 Paper](https://doi.org/10.1016/j.tele.2017.12.013)]

#### 2017

- [Archive] (*J. Med. Syst.'17*) **A Therapy System for Post-Traumatic Stress Disorder Using a Virtual Agent and Virtual Storytelling to Reconstruct Traumatic Memories**
  [[📝 Paper](https://doi.org/10.1007/s10916-017-0771-y)]

- [Archive] (*Simul. Model. Pract. Theory'17*) **A multi-agent system based on reactive decision rules for solving the caregiver routing problem in home health care**
  [[📝 Paper](https://doi.org/10.1016/j.simpat.2017.03.006)]

#### 2016

- [Archive] (*J. Biomed. Inform.'16*) **Agents endowed with uncertainty management behaviors to solve a multiskill healthcare task scheduling**
  [[📝 Paper](https://doi.org/10.1016/j.jbi.2016.08.011)]

- [Archive] (*Decis. Support Syst.'16*) **A multi-agent system to support evidence based medicine and clinical decision making via data sharing and data privacy**
  [[📝 Paper](https://doi.org/10.1016/j.dss.2016.05.008)]

- [Archive] (*J. Syst. Softw.'16*) **A model-driven approach for constructing ambient assisted-living multi-agent systems customized for Parkinson patients**
  [[📝 Paper](https://doi.org/10.1016/j.jss.2015.09.014)]

#### 2015

- [Archive] (*IEEE Intell. Syst.'15*) **Engineering ambient intelligence systems using agent technology**
  [[📝 Paper](https://doi.org/10.1109/mis.2015.3)]

- [Archive] (*Inf. Syst. Front.'15*) **OptiPres: a distributed mobile agent decision support system for optimal patient drug prescription**
  [[📝 Paper](https://doi.org/10.1007/s10796-015-9595-9)]

- [Archive] (*J. Med. Syst.'15*) **Using Semantic Components to Represent Dynamics of an Interdisciplinary Healthcare Team in a Multi-Agent Decision Support System**
  [[📝 Paper](https://doi.org/10.1007/s10916-015-0375-3)]

- [Archive] (*J. Med. Syst.'15*) **Development of a Multi-Agent m-Health Application Based on Various Protocols for Chronic Disease Self-Management**
  [[📝 Paper](https://doi.org/10.1007/s10916-015-0401-5)]

#### 2008

- [Archive] (*Birkhäuser WSST book ch.'08*) **SAPHIRE: A Multi-Agent System for Remote Healthcare Monitoring through Computerized Clinical Guidelines**
  [[📝 Paper](https://doi.org/10.1007/978-3-7643-8547-7_3)]

---

## 🧭 By Topic

> A complementary topic-wise view.
> Some papers appear in multiple categories.
> Each entry should carry the same scope and capability tags as in the time-ordered list (see [Tags](#-tags)).

### Medical Diagnosis and Consultation

- [Core] (*arXiv'26_03*) **MediHive: A Decentralized Agent Collective for Medical Question Answering**
  [[📝 Paper](https://arxiv.org/abs/2603.27150)]

- [Core] (*arXiv'26_03*) **SkinGPT-X: A Self-Evolving Collaborative Multi-Agent System for Transparent and Trustworthy Dermatological Diagnosis**
  [[📝 Paper](https://arxiv.org/abs/2603.26122)]

- [Core] (*arXiv'24_01*) **Towards Conversational Diagnostic AI (AMIE)**
  [[📝 Paper](https://arxiv.org/abs/2401.05654)] [[Nature](https://www.nature.com/articles/s41586-025-08866-7)] [[🌐 Google Research](https://research.google/pubs/towards-conversational-diagnostic-ai/)]

- [Core] (*arXiv'24_12*) **KG4Diagnosis: A Hierarchical Multi-Agent LLM Framework with Knowledge Graph Enhancement for Medical Diagnosis**
  [[📝 Paper](https://arxiv.org/abs/2412.16833)]

- [Core] (*arXiv'24_10*) **Adaptive Reasoning and Acting in Medical Language Agents**
  [[📝 Paper](https://arxiv.org/abs/2410.10020)]

- [Core] (*arXiv'24_05*) **Agent Hospital: A Simulacrum of Hospital with Evolvable Medical Agents**
  [[📝 Paper](https://arxiv.org/abs/2405.02957)]

- [Core] (*arXiv'24_05*) **AgentClinic: A Multimodal Agent Benchmark to Evaluate AI in Simulated Clinical Environments**
  [[📝 Paper](https://arxiv.org/abs/2405.07960)] [[🌐 Project](https://agentclinic.github.io)] [[💻 Code](https://github.com/samuelschmidgall/agentclinic)]

- [Core][Eval] (*arXiv'26_05*) **AgentRx: A Benchmark Study of LLM Agents for Multimodal Clinical Prediction Tasks**
  [[📝 Paper](https://arxiv.org/abs/2605.10286)] [[💻 Code](https://github.com/nyuad-cai/AgentRX)]

- [Core][Eval] (*arXiv'26_05*) **Measuring What Matters: Benchmarking Generative, Multimodal, and Agentic AI in Healthcare**
  [[📝 Paper](https://arxiv.org/abs/2605.08445)]

- [Core] (*arXiv'26_05*) **PhysicianBench: Evaluating LLM Agents in Real-World EHR Environments**
  [[📝 Paper](https://arxiv.org/abs/2605.02240)]

- [Core] (*arXiv'26_05*) **Healthcare AI GYM for Medical Agents**
  [[📝 Paper](https://arxiv.org/abs/2605.02943)] [[💻 Code](https://github.com/minstar/Healthcare_GYM)]

- [Core] (*arXiv'26_03*) **CarePilot: A Multi-Agent Framework for Long-Horizon Computer Task Automation in Healthcare**
  [[📝 Paper](https://arxiv.org/abs/2603.24157)] [[🌐 Project](https://akashghosh.github.io/Care-Pilot/)] [[💻 Code](https://github.com/AkashGhosh/CarePilot)]

- [Core] (*arXiv'26_05*) **A Versatile AI Agent for Rare Disease Diagnosis and Risk Gene Prioritization**
  [[📝 Paper](https://arxiv.org/abs/2605.06226)]

- [Core] (*arXiv'26_02*) **Closing Reasoning Gaps in Clinical Agents with Differential Reasoning Learning**
  [[📝 Paper](https://arxiv.org/abs/2602.09945)]

- [Core] (*arXiv'26_05*) **CuraView: A Multi-Agent Framework for Medical Hallucination Detection with GraphRAG-Enhanced Knowledge Verification**
  [[📝 Paper](https://arxiv.org/abs/2605.03476)]

- [Core] (*arXiv'26_04*) **One Panel Does Not Fit All: Case-Adaptive Multi-Agent Deliberation for Clinical Prediction (CAMP)**
  [[📝 Paper](https://arxiv.org/abs/2604.00085)]

- [Core] (*arXiv'26_04*) **Joint Optimization of Reasoning and Dual-Memory for Self-Learning Diagnostic Agent**
  [[📝 Paper](https://arxiv.org/pdf/2604.07269)]

- [Core] (*arXiv'26_04*) **LungCURE: Benchmarking Multimodal Real-World Clinical Reasoning for Precision Lung Cancer Diagnosis and Treatment**
  [[📝 Paper](https://arxiv.org/pdf/2604.06925)]

- [Core] (*arXiv'26_04*) **Agentic Clinical Reasoning over Longitudinal Myeloma Records: A Retrospective Evaluation Against Expert Consensus**
  [[📝 Paper](https://arxiv.org/abs/2604.24473)]

- [Foundation] (*arXiv'26_04*) **SymptomWise: A Deterministic Reasoning Layer for Reliable and Efficient AI Systems**
  [[📝 Paper](https://arxiv.org/pdf/2604.06375)]

- [Core] (*arXiv'26_03*) **Doctorina MedBench: End-to-End Evaluation of Agent-Based Medical AI**
  [[📝 Paper](https://arxiv.org/pdf/2603.25821)]

<!--
  - [Foundation] (*arXiv'26_04*) **SEA-Eval: A Benchmark for Evaluating Self-Evolving Agents Beyond Episodic Assessment**
    [[📝 Paper](https://arxiv.org/abs/2604.08988)]

-->
- [Core] (*arXiv'26_04*) **QuarkMedSearch: A Long-Horizon Deep Search Agent for Exploring Medical Intelligence**
  [[📝 Paper](https://arxiv.org/pdf/2604.12867)]

- [Eval] (*arXiv'26_04*) **Can LLMs Score Medical Diagnoses and Clinical Reasoning as well as Expert Panels?**
  [[📝 Paper](https://arxiv.org/abs/2604.14892)]

- [Core] (*arXiv'26_04*) **Can Large Language Models Self-Correct in Medical Question Answering? An Exploratory Study**
  [[📝 Paper](https://arxiv.org/abs/2604.00261)]

- [Core] (*arXiv'26_04*) **From Exposure to Internalization: Dual-Stream Calibration for In-context Clinical Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2604.06262)]

- [Core] (*arXiv'26_03*) **GSEM: Graph-based Self-Evolving Memory for Experience Augmented Clinical Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2603.22096)]

- [Core] (*arXiv'26_03*) **Improving Clinical Diagnosis with Counterfactual Multi-Agent Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2603.27820)]

- [Core] (*ACL'26_04*) **Dialectic-Med: Mitigating Diagnostic Hallucinations via Counterfactual Adversarial Multi-Agent Debate**
  [[📝 Paper](https://arxiv.org/abs/2604.11258)]

- [Eval] (*Health Inf Sci Syst'26*) **Enhancing LLM-based medical decision-making by test-time knowledge acquisition**
  [[📝 Paper](https://doi.org/10.1007/s13755-026-00449-8)]

- [Core] (*arXiv'26_04*) **PsychAgent: An Experience-Driven Lifelong Learning Agent for Self-Evolving Psychological Counselor**
  [[📝 Paper](https://arxiv.org/abs/2604.00931)]

- [Core] (*arXiv'26_01*) **EvoClinician: A Self-Evolving Agent for Multi-Turn Medical Diagnosis via Test-Time Evolutionary Learning**
  [[📝 Paper](https://arxiv.org/abs/2601.22964)] [[💻 Code](https://github.com/yf-he/EvoClinician)]

- [Core] (*arXiv'26_03*) **Med-Evo: Test-time Self-evolution for Medical Multimodal Large Language Models**
  [[📝 Paper](https://arxiv.org/abs/2603.07443)]

- [Core] (*npj Digital Medicine'26*) **EvoMDT: A Self-Evolving Multi-Agent System for Structured Clinical Decision-Making in Multi-Cancer**
  [[📝 Paper](https://www.nature.com/articles/s41746-025-02304-8)] [[💻 Code](https://github.com/KesselZ/EvoMDT)]

- [Core] (*arXiv'25_10*) **Evolving Diagnostic Agents in a Virtual Clinical Environment**
  [[📝 Paper](https://arxiv.org/abs/2510.24654)]

- [Core] (*IEEE ICASSP'25*) **SeM-Agents: A Self-Evolving Framework for Multi-Agent Medical Consultation Based on Large Language Models**
  [[📝 Paper](https://ieeexplore.ieee.org/abstract/document/10889517)]

- [Core] (*arXiv'25_09*) **MACD: Multi-Agent Clinical Diagnosis with Self-Learned Knowledge for LLM**
  [[📝 Paper](https://arxiv.org/abs/2509.20067)]

- [Core] (*ICLR'26_03*) **MedAgent-Pro: Towards Evidence-based Multi-modal Medical Diagnosis via Reasoning Agentic Workflow**
  [[📝 Paper](https://arxiv.org/abs/2503.18968)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10008810)] [[💻 Code](https://github.com/jinlab-imvr/MedAgent-Pro)]

- [Core] (*arXiv'25_03*) **MDTeamGPT: A Self-Evolving LLM-based Multi-Agent Framework for Multi-Disciplinary Team Medical Consultation**
  [[📝 Paper](https://arxiv.org/abs/2503.13856)] [[🌐 Project](https://kaichennj.github.io/MDTeamGPT-Main/)]

- [Core] (*arXiv'25_03*) **MAP: Evaluation and Multi-Agent Enhancement of Large Language Models for Inpatient Pathways**
  [[📝 Paper](https://arxiv.org/abs/2503.13205)]

- [Core] (*arXiv'25_02*) **PathFinder: A Multi-Modal Multi-Agent System for Medical Diagnostic Decision-Making Applied to Histopathology**
  [[📝 Paper](https://arxiv.org/pdf/2502.08916)]

### Medical Imaging and Theranostics

- [Core] (*arXiv'26_05*) **NeuroAgent: LLM Agents for Multimodal Neuroimaging Analysis and Research**
  [[📝 Paper](https://arxiv.org/abs/2605.06584)]

- [Core] (*arXiv'26_04*) **NeuroClaw Technical Report: Closed-Loop Agentic AI for Executable and Reproducible Neuroimaging Research**
  [[📝 Paper](https://arxiv.org/abs/2604.24696)] [[🌐 Project](https://cuhk-aim-group.github.io/NeuroClaw/index.html)] [[💻 Code](https://github.com/CUHK-AIM-Group/NeuroClaw)]

- [Background] (*arXiv'26_04*) **MedSynapse-V: Bridging Visual Perception and Clinical Intuition via Latent Memory Evolution**
  [[📝 Paper](https://arxiv.org/abs/2604.26283)]

<!--
  - [Background] (*arXiv'26_03*) **How Well Do Multimodal Models Reason on ECG Signals?**
    [[📝 Paper](https://arxiv.org/abs/2603.00312)]

-->
- [Core] (*arXiv'26_04*) **BAAI Cardiac Agent: An intelligent multimodal agent for automated reasoning and diagnosis of cardiovascular diseases from cardiac magnetic resonance imaging**
  [[📝 Paper](https://arxiv.org/abs/2604.04078)] [[💻 Code](https://github.com/plantain-herb/Cardiac-Agent)]

- [Core] (*arXiv'26_03*) **TheraAgent: Multi-Agent Framework with Self-Evolving Memory and Evidence-Calibrated Reasoning for PET Theranostics**
  [[📝 Paper](https://arxiv.org/abs/2603.13676)]

- [Core] (*arXiv'26_03*) **EviAgent: Evidence-Driven Agent for Radiology Report Generation**
  [[📝 Paper](https://arxiv.org/pdf/2603.13956)]

- [Core] (*arXiv'26_04*) **RadAgent: A Tool-Using AI Agent for Stepwise Interpretation of Chest Computed Tomography**
  [[📝 Paper](https://arxiv.org/abs/2604.15231)] [[🌐 Project](https://rad-agent.github.io/)]

<!--
  - [Background] (*arXiv'26_04*) **Seeing Through Experts' Eyes: A Foundational Vision Language Model Trained on Radiologists' Gaze and Reasoning**
    [[📝 Paper](https://arxiv.org/abs/2604.14316)]

-->
- [Background] (*arXiv'26_04*) **Enhancing Reinforcement Learning for Radiology Report Generation with Evidence-aware Rewards and Self-correcting Preference Learning**
  [[📝 Paper](https://arxiv.org/abs/2604.13598)]

- [Core] (*arXiv'26_04*) **XrayClaw: Cooperative-Competitive Multi-Agent Alignment for Trustworthy Chest X-ray Diagnosis**
  [[📝 Paper](https://arxiv.org/pdf/2604.02695)]

- [Core] (*arXiv'26_04*) **Evidence-Based Actor-Verifier Reasoning for Echocardiographic Agents**
  [[📝 Paper](https://arxiv.org/pdf/2604.06347)]

- [Core] (*arXiv'26_03*) **Med-Evo: Test-time Self-evolution for Medical Multimodal Large Language Models**
  [[📝 Paper](https://arxiv.org/abs/2603.07443)]

- [Core] (*arXiv'26_03*) **Evolving Medical Imaging Agents via Experience-driven Self-skill Discovery (MACRO)**
  [[📝 Paper](https://arxiv.org/abs/2603.05860)]

- [Core] (*arXiv'26_04*) **CAMYLA: Scaling Autonomous Research in Medical Image Segmentation**
  [[📝 Paper](https://arxiv.org/abs/2604.10696)] [[🌐 Project](https://yifangao112.github.io/camyla-page/)]

- [Core] (*arXiv'26_01*) **IBISAgent: Reinforcing Pixel-Level Visual Reasoning in MLLMs for Universal Biomedical Object Referring and Segmentation**
  [[📝 Paper](https://arxiv.org/abs/2601.03054)]

- [Core] (*arXiv'26_01*) **Route, Retrieve, Reflect, Repair (R⁴): Self-Improving Agentic Framework for Visual Detection and Linguistic Reasoning in Medical Imaging**
  [[📝 Paper](https://arxiv.org/abs/2601.08192)] [[💻 Code](https://github.com/faiyazabdullah/MultimodalMedAgent)]

- [Core] (*arXiv'25_09*) **A Co-evolving Agentic AI System for Medical Imaging Analysis (TissueLab)**
  [[📝 Paper](https://arxiv.org/abs/2509.20279)] [[🖥️ Platform](https://tissuelab.org)]

- [Core] (*ICLR'26_03*) **MedAgent-Pro: Towards Evidence-based Multi-modal Medical Diagnosis via Reasoning Agentic Workflow**
  [[📝 Paper](https://arxiv.org/abs/2503.18968)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10008810)] [[💻 Code](https://github.com/jinlab-imvr/MedAgent-Pro)]

- [Core] (*arXiv'25_02*) **PathFinder: A Multi-Modal Multi-Agent System for Medical Diagnostic Decision-Making Applied to Histopathology**
  [[📝 Paper](https://arxiv.org/pdf/2502.08916)]

### Clinical Simulation and Virtual Clinical Environments

- [Core] (*arXiv'26_03*) **OpenHospital: A Thing-in-itself Arena for Evolving and Benchmarking LLM-based Collective Intelligence**
  [[📝 Paper](https://arxiv.org/abs/2603.14771)] [[💻 Code](https://github.com/ZJU-LLMs/Agent-Kernel/tree/main/demo/OpenHospital)]

- [Core] (*arXiv'26_04*) **EMSDialog: Synthetic Multi-person Emergency Medical Service Dialogue Generation from Electronic Patient Care Reports via Multi-LLM Agents**
  [[📝 Paper](https://arxiv.org/abs/2604.07549)]

- [Core] (*CEEM'26*) **From Non-Agentic LLMs to Multi-Agent Systems in Emergency Medicine: A Scoping Review**
  [[📝 Paper](https://doi.org/10.15441/ceem.26.136)]

- [Core] (*arXiv'25_10*) **Evolving Diagnostic Agents in a Virtual Clinical Environment**
  [[📝 Paper](https://arxiv.org/abs/2510.24654)]

- [Core] (*MICCAI'25_03*) **MedAgentSim: Self-Evolving Multi-Agent Simulations for Realistic Clinical Interactions**
  [[📝 Paper](https://arxiv.org/pdf/2503.22678)] [[💻 Code](https://github.com/MAXNORM8650/MedAgentSim)]

- [Core] (*arXiv'24_05*) **Agent Hospital: A Simulacrum of Hospital with Evolvable Medical Agents**
  [[📝 Paper](https://arxiv.org/abs/2405.02957)]

- [Core] (*arXiv'24_05*) **AgentClinic: A Multimodal Agent Benchmark to Evaluate AI in Simulated Clinical Environments**
  [[📝 Paper](https://arxiv.org/abs/2405.07960)] [[🌐 Project](https://agentclinic.github.io)] [[💻 Code](https://github.com/samuelschmidgall/agentclinic)]

### Biomedical and Healthcare Research

- [Core] (*AACR Annual Meeting'26*) **Agentic AI as the Cancer Researcher: Autonomous Discovery in Oncology**
  [[🌐 Program](https://www.aacr.org/meeting/aacr-annual-meeting-2026/program/)]

- [Core] (*arXiv'25_06*) **Agentomics-ML: Autonomous Machine Learning Experimentation Agent for Genomic and Transcriptomic Data**
  [[📝 Paper](https://arxiv.org/abs/2506.05542)] [[💻 Code](https://github.com/BioGeMT/Agentomics-ML)]

- [Core] (*arXiv'26_05*) **A Versatile AI Agent for Rare Disease Diagnosis and Risk Gene Prioritization**
  [[📝 Paper](https://arxiv.org/abs/2605.06226)]

- [Core] (*bioRxiv'26_04*) **A Unified Agent-Enabled Platform for Drug Repurposing across Molecular, Phenotypic, and Clinical Scales**
  [[📝 Paper](https://www.biorxiv.org/content/10.64898/2026.04.19.719462v1)]

- [Core] (*arXiv'26_04*) **From Clinical Intent to Clinical Model: An Autonomous Coding-Agent Framework for Clinician-driven AI Development**
  [[📝 Paper](https://arxiv.org/abs/2604.17110)] [[💻 Code](https://github.com/zhaozh10/clinical-automata)]

- [Core] (*arXiv'26_03*) **Self-evolving AI agents for protein discovery and directed evolution**
  [[📝 Paper](https://arxiv.org/abs/2603.27303)] [[💻 Code](https://github.com/ai4protein/VenusFactory2)]

- [Core] (*Nature Biomedical Engineering'26*) **BioMedAgent: A Self-Evolving LLM Multi-Agent Framework for Autonomous, Tool-Aware Biomedical Data Analyses**
  [[📝 Paper](https://www.nature.com/articles/s41551-026-01634-6)] [[🌐 Project](http://biomed.drai.cn)] [[💻 Code](https://github.com/BOBQWERA/BioMedAgent)]

- [Core] (*arXiv'26_03*) **Emulating Clinician Cognition via Self-Evolving Deep Clinical Research**
  [[📝 Paper](https://arxiv.org/abs/2603.10677)]

- [Core] (*arXiv'26_04*) **QuarkMedSearch: A Long-Horizon Deep Search Agent for Exploring Medical Intelligence**
  [[📝 Paper](https://arxiv.org/pdf/2604.12867)]

- [Core] (*arXiv'26_04*) **CARIS: Coding-Free and Privacy-Preserving MCP Framework for Clinical Agentic Research Intelligence System**
  [[📝 Paper](https://arxiv.org/abs/2604.12258)]

- [Foundation] (*arXiv'26_04*) **FastOMOP: A Foundational Architecture for Reliable Agentic Real-World Evidence Generation on OMOP CDM Data**
  [[📝 Paper](https://arxiv.org/abs/2604.24572)] [[💻 Code](https://github.com/fastomop)]

- [Core] (*bioRxiv'26_02*) **PantheonOS: An Evolvable Multi-Agent Framework for Automatic Genomics Discovery**
  [[📝 Paper](https://www.biorxiv.org/content/10.64898/2026.02.26.707870v1)] [[🌐 Project](https://pantheonos.stanford.edu)] [[💻 Code](https://github.com/aristoteleo)]

- [Core] (*arXiv'26_04*) **MAT-Cell: A Multi-Agent Tree-Structured Reasoning Framework for Batch-Level Single-Cell Annotation**
  [[📝 Paper](https://arxiv.org/abs/2604.06269)] [[💻 Code](https://github.com/jiangliu91/MAT-Cell-A-Multi-Agent-Tree-Structured-Reasoning-Framework-for-Batch-Level-Single-Cell-Annotation)]

<!--
  - [Foundation] (*arXiv'26_04*) **MDAgent: A Multi-Agent Framework for End-to-End Molecular Dynamics Research**
    [[📝 Paper](https://arxiv.org/abs/2604.18622)]

-->
- [Core] (*arXiv'26_04*) **AblateCell: A Reproduce-then-Ablate Agent for Virtual Cell Repositories**
  [[📝 Paper](https://arxiv.org/abs/2604.19606)]

- [Core] (*bioRxiv'26_01*) **Agentomics: An Agentic System that Autonomously Develops Novel State-of-the-art Solutions for Biomedical Machine Learning Tasks**
  [[📝 Paper](https://www.biorxiv.org/content/10.64898/2026.01.27.702049v1)]

- [Core] (*arXiv'26_04*) **Agentic AI Platforms for Autonomous Training and Rule Induction of Human-Human and Virus-Human Protein-Protein Interactions**
  [[📝 Paper](https://arxiv.org/abs/2604.23924)]

- [Core] (*bioRxiv'26_06*) **OriGene: A Self-Evolving Virtual Disease Biologist Automating Therapeutic Target Discovery**
  [[📝 Paper](https://www.biorxiv.org/content/10.1101/2025.06.03.657658v2)]

- [Core] (*bioRxiv'26_07*) **STELLA: Towards a Biomedical World Model with Self-Evolving Multimodal Agents**
  [[📝 Paper](https://www.biorxiv.org/content/10.1101/2025.07.01.662467v2)]

- [Core] (*arXiv'25_08*) **HealthFlow: A Self-Evolving AI Agent with Meta Planning for Autonomous Healthcare Research**
  [[📝 Paper](https://arxiv.org/abs/2508.02621)] [[💻 Code](https://github.com/yhzhu99/HealthFlow)]

- [Core] (*arXiv'25_06*) **MedAgentGym: A Scalable Agentic Training Environment for Code-Centric Reasoning in Biomedical Data Science**
  [[📝 Paper](https://arxiv.org/abs/2506.04405)]

- [Core] (*bioRxiv'25_10*) **LabOS: The AI-XR Co-Scientist That Sees and Works With Humans**
  [[📝 Paper](https://www.biorxiv.org/content/10.1101/2025.10.16.679418v2)] [[💻 Code](https://github.com/zaixizhang/LabOS)] [[🌐 Project](https://ai4labos.com/)]

- [Core] (*arXiv'25_10*) **RareAgent: Self-Evolving Reasoning for Drug Repurposing in Rare Diseases**
  [[📝 Paper](https://arxiv.org/abs/2510.05764)]

- [Core] (*arXiv'26_04*) **Constraint-Aware Corrective Memory for Language-Based Drug Discovery Agents (CACM)**
  [[📝 Paper](https://arxiv.org/abs/2604.09308)]

- [Core] (*Advanced Science'25*) **Autonomous Self-Evolving Research on Biomedical Data: The DREAM Paradigm**
  [[📝 Paper](https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.202417066)]

- [Foundation] (*IJISAE'25*) **Self-Evolving LLM Ecosystems for Precision Medicine**
  [[📝 Paper](https://ijisae.org/index.php/IJISAE/article/view/7793)]

### Clinical Decision-Making and Trial Optimization

- [Core] (*arXiv'26_03*) **Symphony for Medical Coding: A Next-Generation Agentic System for Scalable and Explainable Medical Coding**
  [[📝 Paper](https://arxiv.org/abs/2603.29709)]

- [Core] (*Cambridge Open Engage'26*) **Artificial Epidemiology: How Self-Evolving Clinical AI Manufactures Disease Prevalence from Administrative Coding Artifacts**
  [[📝 Paper](https://doi.org/10.33774/coe-2026-ssm1q)]

- [Core] (*arXiv'26_04*) **Agentic AI for Clinical Urgency Mapping and Queue Optimization in High-Volume Outpatient Departments: A Simulation-Based Evaluation**
  [[📝 Paper](https://arxiv.org/abs/2604.00215)]

- [Core] (*arXiv'26_01*) **ClinicalReTrial: A Self-Evolving AI Agent for Clinical Trial Protocol Optimization**
  [[📝 Paper](https://arxiv.org/abs/2601.00290)]

- [Core] (*ACM-BCB'24_04*) **ClinicalAgent: Clinical Trial Multi-Agent System with LLM-based Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2404.14777)] [[💻 Code](https://github.com/LeoYML/clinical-agent)]

- [Core] (*npj Digital Medicine'26*) **EvoMDT: A Self-Evolving Multi-Agent System for Structured Clinical Decision-Making in Multi-Cancer**
  [[📝 Paper](https://www.nature.com/articles/s41746-025-02304-8)] [[💻 Code](https://github.com/KesselZ/EvoMDT)]

- [Core] (*arXiv'26_04*) **Development, Evaluation, and Deployment of a Multi-Agent System for Thoracic Tumor Board**
  [[📝 Paper](https://arxiv.org/abs/2604.12161)]

- [Core] (*arXiv'26_04*) **Evo-MedAgent: Beyond One-Shot Diagnosis with Agents That Remember, Reflect, and Improve**
  [[📝 Paper](https://arxiv.org/abs/2604.14475)]

- [Foundation] (*arXiv'26_05*) **TheraAgent: Self-Improving Therapeutic Agent for Precise and Comprehensive Treatment Planning**
  [[📝 Paper](https://arxiv.org/abs/2605.05963)]

<!--
  - [Foundation] (*arXiv'26_04*) **Multi-Agent Decision-Focused Learning via Value-Aware Sequential Communication (SeqComm-DFL)**
    [[📝 Paper](https://arxiv.org/abs/2604.08944)]

-->
- [Core] (*arXiv'25_06*) **Integrating Dynamical Systems Learning with Foundational Models: A Meta-Evolutionary AI Framework for Clinical Trials**
  [[📝 Paper](https://arxiv.org/abs/2506.14782)]

- [Core] (*arXiv'25_03*) **MDTeamGPT: A Self-Evolving LLM-based Multi-Agent Framework for Multi-Disciplinary Team Medical Consultation**
  [[📝 Paper](https://arxiv.org/abs/2503.13856)] [[🌐 Project](https://kaichennj.github.io/MDTeamGPT-Main/)]

- [Core] (*arXiv'25_03*) **MAP: Evaluation and Multi-Agent Enhancement of Large Language Models for Inpatient Pathways**
  [[📝 Paper](https://arxiv.org/abs/2503.13205)]

### Health Communication and Alignment

- [Eval] (*J. Med. Syst.'26*) **When Chatbots Become Agents: The Next Phase of Healthcare AI**
  [[📝 Paper](https://doi.org/10.1007/s10916-026-02402-4)]

- [Core] (*arXiv'26_04*) **A Safety-Aware Role-Orchestrated Multi-Agent LLM Framework for Behavioral Health Communication Simulation**
  [[📝 Paper](https://arxiv.org/abs/2604.00249)]

- [Core] (*arXiv'26_04*) **PsychAgent: An Experience-Driven Lifelong Learning Agent for Self-Evolving Psychological Counselor**
  [[📝 Paper](https://arxiv.org/abs/2604.00931)]

- [Core] (*NeurIPS'25 Workshop*) **HealthAlign-Agents: Self-Play Reflective Prompting for Culturally Aligned Health Communication in Low-Resource Languages**
  [[📝 Paper](https://neurips.cc/virtual/2025/135933)]

- [Core] (*arXiv'25_06*) **CounselBench: A Large-Scale Expert Evaluation and Adversarial Benchmarking of Large Language Models in Mental Health Question Answering**
  [[📝 Paper](https://arxiv.org/abs/2506.08584)]

- [Core] (*arXiv'24_09*) **Depression Diagnosis Dialogue Simulation: Self-improving Psychiatrist with Tertiary Memory**
  [[📝 Paper](https://arxiv.org/abs/2409.15084)]

- [Core] (*arXiv'26_03*) **Perfecting Human–AI Interaction at Clinical Scale: Turning Production Signals into Safer, More Human Conversations**
  [[📝 Paper](https://arxiv.org/abs/2603.29893)]

- [Background] (*arXiv'26_04*) **Rethinking Patient Education as Multi-turn Multi-modal Interaction**
  [[📝 Paper](https://arxiv.org/abs/2604.14656)]

- [Core] (*arXiv'26_05*) **Virtual Speech Therapist: A Clinician-in-the-Loop AI Speech Therapy Agent for Personalized and Supervised Therapy**
  [[📝 Paper](https://arxiv.org/abs/2605.01101)]

### Ethics, Safety, and Limits

- [Foundation][Evolution][Eval] (*arXiv'26_05*) **On-Policy Self-Evolution via Failure Trajectories for Agentic Safety Alignment (FATE)**
  [[📝 Paper](https://arxiv.org/abs/2605.11882)]

- [Foundation][Eval] (*arXiv'26_05*) **Agent-ValueBench: A Comprehensive Benchmark for Evaluating Agent Values**
  [[📝 Paper](https://arxiv.org/abs/2605.10365)]

- [Core][Eval] (*arXiv'26_05*) **Measuring What Matters: Benchmarking Generative, Multimodal, and Agentic AI in Healthcare**
  [[📝 Paper](https://arxiv.org/abs/2605.08445)]

- [Core] (*Cambridge Open Engage'26*) **Artificial Epidemiology: How Self-Evolving Clinical AI Manufactures Disease Prevalence from Administrative Coding Artifacts**
  [[📝 Paper](https://doi.org/10.33774/coe-2026-ssm1q)]

- [Core] (*arXiv'26_04*) **CARE: Privacy-Compliant Agentic Reasoning with Evidence Discordance**
  [[📝 Paper](https://arxiv.org/abs/2604.01113)]

- [Core] (*arXiv'25_05*) **MedSentry: Understanding and Mitigating Safety Risks in Medical LLM Multi-Agent Systems**
  [[📝 Paper](https://arxiv.org/abs/2505.20824)] [[💻 Code](https://github.com/KaiChenNJ/MedSentry)]

- [Core] (*arXiv'26_05*) **CuraView: A Multi-Agent Framework for Medical Hallucination Detection with GraphRAG-Enhanced Knowledge Verification**
  [[📝 Paper](https://arxiv.org/abs/2605.03476)]

- [Core] (*arXiv'26_04*) **A Safety-Aware Role-Orchestrated Multi-Agent LLM Framework for Behavioral Health Communication Simulation**
  [[📝 Paper](https://arxiv.org/abs/2604.00249)]

- [Eval] (*arXiv'26_02*) **The Doctor Will (Still) See You Now: On the Structural Limits of Agentic AI in Healthcare**
  [[📝 Paper](https://arxiv.org/abs/2602.18460)]

- [Eval] (*arXiv'26_02*) **Agentic AI, Medical Morality, and the Transformation of the Clinic**
  [[📝 Paper](https://arxiv.org/abs/2602.16553)]

- [Eval] (*arXiv'26_04*) **Grounding Clinical AI Competency in Human Cognition Through the Clinical World Model and Skill-Mix Framework**
  [[📝 Paper](https://arxiv.org/abs/2604.08226)]

- [Eval] (*medRxiv'26_04*) **Dissecting clinical reasoning failures in frontier artificial intelligence using 10,000 synthetic cases**
  [[📝 Paper](https://www.medrxiv.org/content/10.64898/2026.04.22.26351488v1)]

- [Eval] (*medRxiv'26_04*) **HAARF: Healthcare AI Agents Regulatory Framework**
  [[📝 Paper](https://www.medrxiv.org/content/10.64898/2026.04.09.26350519v1)] [[💻 Code](https://github.com/Task-force-for-AI-agents-in-Healthcare/haarf)]

- [Eval] (*medRxiv'25_08*) **Automation Bias in Large Language Model Assisted Diagnostic Reasoning Among AI-Trained Physicians**
  [[📝 Paper](https://www.medrxiv.org/content/10.1101/2025.08.23.25334280v2)]

### General Self-Evolving Frameworks and Methods

- [Foundation][Memory][Evolution] (*arXiv'26_05*) **SAGE: A Self-Evolving Agentic Graph-Memory Engine for Structure-Aware Associative Memory**
  [[📝 Paper](https://arxiv.org/abs/2605.12061)]

- [Foundation][Evolution][Eval] (*arXiv'26_05*) **On-Policy Self-Evolution via Failure Trajectories for Agentic Safety Alignment (FATE)**
  [[📝 Paper](https://arxiv.org/abs/2605.11882)]

- [Foundation] (*arXiv'26_05*) **MCP-Cosmos: World Model-Augmented Agents for Complex Task Execution in MCP Environments**
  [[📝 Paper](https://arxiv.org/abs/2605.09131)]

<!--
  - [Foundation] (*arXiv'26_03*) **Meta-Harness: End-to-End Optimization of Model Harnesses**
    [[📝 Paper](https://arxiv.org/pdf/2603.28052)]

-->
<!--
  - [Foundation] (*arXiv'26_05*) **ARA: Agentic Reproducibility Assessment for Scalable Support of Scientific Peer-Review**
    [[📝 Paper](https://arxiv.org/abs/2605.02651)] [[💻 Code](https://github.com/AndresLaverdeMarin/agentic_reproducibility_assessment)]

-->
<!--
  - [Foundation] (*arXiv'26_05*) **MemTier: Tiered Memory Architecture and Retrieval Bottleneck Analysis for Long-Running Autonomous AI Agents**
    [[📝 Paper](https://arxiv.org/abs/2605.03675)]

-->
<!--
  - [Foundation] (*arXiv'26_05*) **SkillOS: Learning Skill Curation for Self-Evolving Agents**
    [[📝 Paper](https://arxiv.org/abs/2605.06614)]

-->
<!--
  - [Foundation] (*arXiv'25_05*) **Nature's Insight: A Novel Framework and Comprehensive Analysis of Agentic Reasoning Through the Lens of Neuroscience**
    [[📝 Paper](https://arxiv.org/abs/2505.05515)] [[💻 Code](https://github.com/BioRAILab/Awesome-Neuroscience-Agent-Reasoning)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **Autogenesis: A Self-Evolving Agent Protocol**
    [[📝 Paper](https://arxiv.org/abs/2604.15034)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **A Self-Evolving Framework for Efficient Terminal Agents via Observational Context Compression**
    [[📝 Paper](https://arxiv.org/abs/2604.19572)]

-->
<!--
  - [Foundation] (*ACL'26_04*) **From Experience to Skill: Multi-Agent Generative Engine Optimization via Reusable Strategy Learning**
    [[📝 Paper](https://arxiv.org/abs/2604.19516)] [[💻 Code](https://github.com/Wu-beining/MAGEO)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **Co-Evolving LLM Decision and Skill Bank Agents for Long-Horizon Tasks**
    [[📝 Paper](https://arxiv.org/abs/2604.20987)] [[🌐 Project](https://wuxiyang1996.github.io/COSPLAY_page/)] [[💻 Code](https://github.com/wuxiyang1996/cos-play)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **AEL: Agent Evolving Learning for Open-Ended Environments**
    [[📝 Paper](https://arxiv.org/abs/2604.21725)] [[💻 Code](https://github.com/WujiangXu/AEL)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **GenericAgent: A Token-Efficient Self-Evolving LLM Agent via Contextual Information Density Maximization**
    [[📝 Paper](https://arxiv.org/abs/2604.17091)] [[💻 Code](https://github.com/lsdefine/GenericAgent)]

-->
<!--
  - [Foundation] (*arXiv'26*) **MAGE: Multi-Agent Self-Evolution with Co-Evolutionary Knowledge Graphs**
    [[🌐 arXiv](https://arxiv.org/search/?searchtype=all&query=MAGE%3A%20Multi-Agent%20Self-Evolution%20with%20Co-Evolutionary%20Knowledge%20Graphs&abstracts=show&order=-announced_date_first&size=25)]

-->
<!--
  - [Foundation] (*arXiv'25_09*) **Evolving-RL: End-to-End Optimization of Experience-Driven Self-Evolving Capability**
    [[📝 Paper](https://arxiv.org/abs/2509.15194)] [[💻 Code](https://github.com/YujunZhou/EVOL-RL)]

-->
<!--
  - [Foundation] (*GitHub'26*) **NanoResearch: Co-Evolving Skills, Memory, and Policy for Personalized Research Automation**
    [[💻 Code](https://github.com/OpenRaiser/NanoResearch)]

-->
<!--
  - [Foundation] (*arXiv'26_03*) **SkillEvolver: Dynamic Skill Lifecycle Management for Agentic RL**
    [[📝 Paper](https://arxiv.org/abs/2603.17187)] [[💻 Code](https://github.com/aiming-lab/MetaClaw)]

-->
<!--
  - [Foundation] (*arXiv'26_03*) **AgentFactory: A Self-Evolving Framework Through Executable Subagent Accumulation and Reuse**
    [[📝 Paper](https://arxiv.org/abs/2603.18000)] [[💻 Code](https://github.com/zzatpku/AgentFactory)]

-->
<!--
  - [Foundation] (*arXiv'26_02*) **S1-NexusAgent: a Self-Evolving Agent Framework for Multidisciplinary Scientific Research**
    [[📝 Paper](https://arxiv.org/abs/2602.01550)]

-->
- [Core] (*arXiv'26_03*) **OpenHospital: A Thing-in-itself Arena for Evolving and Benchmarking LLM-based Collective Intelligence**
  [[📝 Paper](https://arxiv.org/abs/2603.14771)] [[💻 Code](https://github.com/ZJU-LLMs/Agent-Kernel/tree/main/demo/OpenHospital)]

<!--
  - [Foundation] (*arXiv'26_04*) **Mem^2Evolve: Towards Self-Evolving Agents via Co-Evolutionary Capability Expansion and Experience Distillation**
    [[📝 Paper](https://arxiv.org/abs/2604.10923)] [[💻 Code](https://buaa-irip-llm.github.io/Mem2Evolve)]

-->
- [Core] (*arXiv'24_05*) **Agent Hospital: A Simulacrum of Hospital with Evolvable Medical Agents**
  [[📝 Paper](https://arxiv.org/abs/2405.02957)]

- [Core] (*arXiv'24_05*) **AgentClinic: A Multimodal Agent Benchmark to Evaluate AI in Simulated Clinical Environments**
  [[📝 Paper](https://arxiv.org/abs/2405.07960)] [[🌐 Project](https://agentclinic.github.io)] [[💻 Code](https://github.com/samuelschmidgall/agentclinic)]

<!--
  - [Foundation] (*arXiv'26_04*) **SEA-Eval: A Benchmark for Evaluating Self-Evolving Agents Beyond Episodic Assessment**
    [[📝 Paper](https://arxiv.org/abs/2604.08988)]

-->
- [Core] (*bioRxiv'26_02*) **PantheonOS: An Evolvable Multi-Agent Framework for Automatic Genomics Discovery**
  [[📝 Paper](https://www.biorxiv.org/content/10.64898/2026.02.26.707870v1)] [[🌐 Project](https://pantheonos.stanford.edu)] [[💻 Code](https://github.com/aristoteleo)]

- [Core] (*Nature Biomedical Engineering'26*) **BioMedAgent: A Self-Evolving LLM Multi-Agent Framework for Autonomous, Tool-Aware Biomedical Data Analyses**
  [[📝 Paper](https://www.nature.com/articles/s41551-026-01634-6)] [[🌐 Project](http://biomed.drai.cn)] [[💻 Code](https://github.com/BOBQWERA/BioMedAgent)]

- [Core] (*arXiv'26_03*) **GSEM: Graph-based Self-Evolving Memory for Experience Augmented Clinical Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2603.22096)]

<!--
  - [Foundation] (*GitHub'26*) **EverOS: Build, evaluate, and integrate long-term memory for self-evolving agents**
    [[💻 Code](https://github.com/EverMind-AI/EverOS)]

-->
<!--
  - [Foundation] (*arXiv'26_03*) **MemMA: Coordinating the Memory Cycle through Multi-Agent Reasoning and In-Situ Self-Evolution**
    [[📝 Paper](https://arxiv.org/abs/2603.18718)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **Multi-Agent Decision-Focused Learning via Value-Aware Sequential Communication (SeqComm-DFL)**
    [[📝 Paper](https://arxiv.org/abs/2604.08944)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **SKILLFOUNDRY: Building Self-Evolving Agent Skill Libraries from Heterogeneous Scientific Resources**
    [[📝 Paper](https://arxiv.org/abs/2604.03964)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **Skill Retrieval Augmentation for Agentic AI**
    [[📝 Paper](https://arxiv.org/abs/2604.24594)] [[💻 Code](https://github.com/oneal2000/SR-Agents)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **ClawTrace: Cost-Aware Tracing for LLM Agent Skill Distillation**
    [[📝 Paper](https://arxiv.org/abs/2604.23853)] [[💻 Code](https://github.com/epsilla-cloud/clawtrace)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **CORAL: Towards Autonomous Multi-Agent Evolution for Open-Ended Discovery**
    [[📝 Paper](https://arxiv.org/abs/2604.01658)] [[💻 Code](https://github.com/Human-Agent-Society/CORAL)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **CoEvoSkills: Self-Evolving Agent Skills via Co-Evolutionary Verification**
    [[📝 Paper](https://arxiv.org/abs/2604.01687)]

-->
<!--
  - [Foundation] (*arXiv'26_04*) **SEARL: Joint Optimization of Policy and Tool Graph Memory for Self-Evolving Agents**
    [[📝 Paper](https://arxiv.org/abs/2604.07791)]

-->
<!--
  - [Foundation] (*arXiv'26_03*) **Cognitive Friction: A Decision-Theoretic Framework for Bounded Deliberation in Tool-Using Agents**
    [[📝 Paper](https://arxiv.org/abs/2603.30031)]

-->
<!--
  - [Foundation] (*ICLR'26_10*) **CoT-Evo: Evolutionary Distillation of CoT for Scientific Reasoning**
    [[📝 Paper](https://arxiv.org/abs/2510.13166)] [[💻 Code](https://github.com/Irving-Feng/CoT-Evo)]

-->
- [Foundation] (*ICLR'26_10*) **EvoTest: Evolutionary Test-Time Learning for Self-Improving Agentic Systems**
  [[📝 Paper](https://arxiv.org/abs/2510.13220)] [[💻 Code](https://github.com/yf-he/EvoTest)]

- [Core] (*ICLR'26_10*) **Doctor-R1: Mastering Clinical Inquiry with Experiential Agentic Reinforcement Learning**
  [[📝 Paper](https://arxiv.org/abs/2510.04284)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10006814)] [[💻 Code](https://github.com/thu-unicorn/Doctor-R1)]

- [Core] (*ICLR'26_06*) **MMedAgent-RL: Optimizing Multi-Agent Collaboration for Multimodal Medical Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2506.00555)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10011724)]

- [Core] (*ICLR'26_06*) **Language Agents for Hypothesis-driven Clinical Decision Making with Reinforcement Learning**
  [[📝 Paper](https://arxiv.org/abs/2506.13474)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10011252)] [[💻 Code](https://github.com/dharouni/LA-CDM)]

- [Core] (*ICLR'26_09*) **KnowGuard: Knowledge-Driven Abstention for Multi-Round Clinical Reasoning**
  [[📝 Paper](https://arxiv.org/abs/2509.24816)] [[🌐 ICLR](https://iclr.cc/virtual/2026/poster/10008150)] [[💻 Code](https://github.com/IcecreamArtist/KnowGuard)]

<!--
  - [Foundation] (*ICLR'26 Rejected*) **SkillEvo: An Experience Learning Framework with Reinforcement Learning for Skill Evolution**
    [[📝 Paper](https://openreview.net/forum?id=S1cIE9pe3k)]

-->
<!--
  - [Foundation] (*EMNLP'25 Demo*) **EvoAgentX: An Automated Framework for Evolving Agentic Workflows**
    [[📝 Paper](https://aclanthology.org/2025.emnlp-demos.47/)] [[💻 Code](https://github.com/EvoAgentX/EvoAgentX)]

-->
<!--
  - [Foundation] (*arXiv'25_02*) **EvoAgent: Self-evolving Agent with Continual World Model for Long-Horizon Tasks**
    [[📝 Paper](https://arxiv.org/abs/2502.05907)] [[💻 Code](https://github.com/siyuyuan/evoagent)]

-->
<!--
  - [Foundation] (*arXiv'23_12*) **ReST meets ReAct: Self-Improvement for Multi-Step Reasoning LLM Agent**
    [[📝 Paper](https://arxiv.org/abs/2312.10003)]

-->
<!--
  - [Foundation] (*arXiv'23_06*) **SELFEVOLVE: A Code Evolution Framework via Large Language Models**
    [[📝 Paper](https://arxiv.org/abs/2306.02907)]

  ---

-->
## 🔗 Related Repositories

- **Awesome-Self-Evolving-AI-for-Agentic-Healthcare**
  A curated source list for self-evolving AI in agentic healthcare.
  [[💻 Repository](https://github.com/ZhihaoPENG-CityU/Awesome-Self-Evolving-AI-for-Agentic-Healthcare)]

- **Hermes Agent**
  An agent framework and product direction centered on agents that grow with users through memory and reusable skills.
  [[💻 Repository](https://github.com/nousresearch/hermes-agent)]

- **Awesome-Self-Evolving-Agents**
  A comprehensive collection of self-evolving AI agents across general domains.
  [[💻 Repository](https://github.com/EvoAgentX/Awesome-Self-Evolving-Agents)]

- **Awesome-World-Models-for-Healthcare**
  A curated collection of world models for healthcare.
  [[💻 Repository](https://github.com/chengwang96/Awesome-World-Models-for-Healthcare)]

---

## ⭐ Star History

<a href="https://www.star-history.com/?repos=ZhihaoPENG-CityU%2FAwesome-Hermes-Agent-in-Healthcare&type=date&legend=top-left">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/image?repos=ZhihaoPENG-CityU/Awesome-Hermes-Agent-in-Healthcare&type=date&theme=dark&legend=top-left" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/image?repos=ZhihaoPENG-CityU/Awesome-Hermes-Agent-in-Healthcare&type=date&legend=top-left" />
   <img alt="Star History Chart" src="https://api.star-history.com/image?repos=ZhihaoPENG-CityU/Awesome-Hermes-Agent-in-Healthcare&type=date&legend=top-left" />
 </picture>
</a>

---

## 🙏 Acknowledgements

This repository is distilled and adapted for **Awesome-Hermes-Agent-in-Healthcare** from the following inspirations and source projects:

- [Awesome-Self-Evolving-AI-for-Agentic-Healthcare](https://github.com/ZhihaoPENG-CityU/Awesome-Self-Evolving-AI-for-Agentic-Healthcare)
- [Hermes Agent](https://github.com/nousresearch/hermes-agent)

---

## 🤝 Contributing

[Back to Content](#contents)

Your contributions are always welcome! Please contact [Zhihao Peng](mailto:zhihaopeng@cuhk.edu.hk)<!-- or [Cheng Wang](mailto:chengwang@link.cuhk.edu.hk) -->.

If you find relevant papers, codebases, benchmarks, or project pages related to **healthcare agents**, **agent memory**, **agent skills**, **self-evolution**, or **clinical agent evaluation and governance**, feel free to:

- open an **Issue**
- submit a **Pull Request**

Suggested format:

```markdown
- [Core][Memory][Evolution] (*Venue'YY_MM*) **Paper Title** [[📝 Paper](link)] [[💻 Code](link)]
- [Foundation][Skill] (*Venue'YY*) **Paper Title** [[📝 Paper](link)]
```

Use `[Core]` when the paper fits the primary healthcare-agent scope; otherwise choose `[Foundation]` or `[Archive]` per [Tags](#-tags). Add `[Memory]`, `[Skill]`, `[Evolution]`, or `[Eval]` when they describe the paper's main contribution.

Use two-digit `YY` (e.g. `26` for 2026). Add `_MM` (month from arXiv id or preprint URL) only when it can be inferred; otherwise keep **`(*Venue'YY*)`** without `_MM`.

Please try to keep the formatting consistent with the existing entries. Prefer an `arxiv.org/abs/YYMM.NNNNN` (or `pdf/`) link when available so entries sort correctly by month.

### Curation scope (clinical agents vs. epidemic / biological ABM)

**In scope:** software agents, multi-agent systems, mobile agents, or LLM-based agents applied to **clinical workflows, hospitals, telehealth, EMR/EHR integration, ambient assisted living with an explicit agent architecture**, and similar **care-delivery or health-informatics** settings.

<!-- **Do not add** (even if “agent” appears in the title or venue):

- **Epidemiological or biological ABM** — population-level infection dynamics, within-host pathogen or immune simulations, trial-design ABMs, geographic or network disease spread, “super-spreader” ABMs, etc. (typical examples from screening lists: hepatitis / alveolar / cholera / TB / HIV-trial ABMs, influenza spread in communities or EDs framed as disease dynamics, immune-system processes in a virtual anatomy). These belong in computational epidemiology or systems biology, not this **agentic healthcare software** list.

- **Borderline platform papers** — exclude when the contribution is primarily: **Web services or cloud home-care** without a stated multi-agent design; **generic IoT / sensor monitoring or wellness dashboards** without agent-centric methods; **generic distributed MAS architecture** without healthcare-centric evaluation; **preventive-medicine or network influenza** models that are disease models rather than clinical information agents; **ubiquitous fitness / physical-activity** sensor platforms without agent methods; **biology-style immune** simulations described as decentralized processes rather than clinical AI agents.

These rules keep the repository aligned with **healthcare agents, memory, skills, self-evolution, and clinical agent evaluation**, not ABM-for-disease-modeling alone.
-->

---

## ✉️ Contact Us

If you have any questions or suggestions, please feel free to contact us via:

**Email:** zhihaopeng@cuhk.edu.hk<!-- , chengwang@link.cuhk.edu.hk -->
