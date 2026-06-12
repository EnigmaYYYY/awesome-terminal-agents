# Awesome Terminal Agents

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Survey](https://img.shields.io/badge/Survey-PDF-blue)](terminal-agents-survey.pdf)

A curated list of papers, benchmarks, tools, and runtime systems for **terminal agents**: AI agents that make progress through command-line environments by issuing shell commands, reading textual observations, mutating workspaces, running tests, and recovering from execution feedback.

This repository accompanies the survey **Terminal Agents: A Survey of AI Agents in Command-Line Environments**.

- [Read the survey PDF](terminal-agents-survey.pdf)
- Scope: terminal-native agents, repository-grounded coding agents, executable benchmarks, CLI environments, harnesses, training pipelines, process evaluation, safety, and adjacent computer-use agents.
- Status: v1 release candidate. The repository is currently maintained privately while public release materials are prepared. README entries are restricted to works cited in the current survey PDF and remain a curated subset rather than an exhaustive index.

## Contents

- [Terminal-Native Tools](#terminal-native-tools)
- [Core Terminal-Agent Systems](#core-terminal-agent-systems)
- [Terminal Benchmarks and Environments](#terminal-benchmarks-and-environments)
- [Repository and Software Engineering Benchmarks](#repository-and-software-engineering-benchmarks)
- [Harnesses, Runtimes, and Agent-Computer Interfaces](#harnesses-runtimes-and-agent-computer-interfaces)
- [Training, Trajectories, and Competence Acquisition](#training-trajectories-and-competence-acquisition)
- [Process, Trace, and Long-Horizon Evaluation](#process-trace-and-long-horizon-evaluation)
- [Safety, Security, and Governance](#safety-security-and-governance)
- [Adjacent Computer-Use and Tool-Use Agents](#adjacent-computer-use-and-tool-use-agents)
- [Foundational Work](#foundational-work)
- [Survey Positioning](#survey-positioning)
- [Corpus Notes](#corpus-notes)
- [Contributing](#contributing)
- [Citation](#citation)

## Terminal-Native Tools

Deployment-facing tools that package terminal-mediated agency as a developer or operator workflow.

| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| Claude Code | 2025 | deployment tool | [Docs](https://code.claude.com/docs/en/overview) | Engineering-Practice-Tool |
| Codex CLI | 2025 | deployment tool | [GitHub](https://github.com/openai/codex) | Engineering-Practice-Tool |
| Aider: AI Pair Programming in Your Terminal | 2025 | deployment tool | [GitHub](https://github.com/Aider-AI/aider) | Engineering-Practice-Tool |
| Gemini CLI | 2025 | deployment tool | [GitHub](https://github.com/google-gemini/gemini-cli) | Engineering-Practice-Tool |
| ShellGPT | 2026 | boundary comparator | [GitHub](https://github.com/TheR1D/shell_gpt) | Engineering-Practice-Tool |

## Core Terminal-Agent Systems

Systems and studies where terminal-mediated execution is the dominant locus of progress.

| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| SWE-agent: Agent-Computer Interfaces Enable Automated Software Engineering | 2024 | architecture | [Paper](https://arxiv.org/abs/2405.15793) / [GitHub](https://github.com/SWE-agent/SWE-agent) | Core-Terminal-Primary |
| The OpenHands Software Agent SDK: A Composable and Extensible Foundation for Production Agents | 2025 | architecture | [Paper](https://arxiv.org/abs/2511.03690) / [GitHub](https://github.com/All-Hands-AI/OpenHands) | Core-Terminal-Primary |
| Building Effective AI Coding Agents for the Terminal: Scaffolding, Harness, Context Engineering, and Lessons Learned | 2026 | architecture | [Paper](https://arxiv.org/abs/2603.05344) | Core-Terminal-Primary |
| Terminal Is All You Need: Design Properties for Human-AI Agent Collaboration | 2026 | definition | [Paper](https://arxiv.org/abs/2603.10664) | Core-Terminal-Primary |
| Terminal Agents Suffice for Enterprise Automation | 2026 | empirical study | [Paper](https://arxiv.org/abs/2604.00073) | Core-Terminal-Primary |
| Curie: Toward Rigorous and Automated Scientific Experimentation with AI Agents | 2025 | architecture | [Paper](https://arxiv.org/abs/2502.16069) | Core-Terminal-Primary |
| Ircopilot: Automated Incident Response with Large Language Models | 2025 | architecture | [Paper](https://arxiv.org/abs/2505.20945) | Core-Terminal-Primary |
| KubeIntellect: A Modular LLM-Orchestrated Agent Framework for End-to-End Kubernetes Management | 2025 | architecture | [Paper](https://arxiv.org/abs/2509.02449) | Core-Terminal-Primary |
| Towards Agentic OS: An LLM Agent Framework for Linux Schedulers | 2025 | architecture | [Paper](https://arxiv.org/abs/2509.01245) | Core-Terminal-Primary |
| Beyond State Machines: Executing Network Procedures with Agentic Tool-Calling Sequences | 2026 | architecture | [Paper](https://arxiv.org/abs/2605.02584) | Core-Terminal-Primary |
| kRAIG: A Natural Language-Driven Agent for Automated DataOps Pipeline Generation | 2026 | architecture | [Paper](https://arxiv.org/abs/2603.20311) | Core-Terminal-Primary |
| FinOps Agent: A Use-Case for IT Infrastructure and Cost Optimization | 2025 | architecture | [Paper](https://arxiv.org/abs/2510.25914) | Core-Terminal-Primary |
| NetAgentBench: A State-Centric Benchmark for Evaluating Agentic Network Configuration | 2026 | benchmark | [Paper](https://arxiv.org/abs/2604.09678) | Core-Terminal-Primary |

## Terminal Benchmarks and Environments

Benchmarks and executable environments that directly measure command formulation, observation interpretation, setup, state tracking, recovery, or long-horizon terminal behavior.

| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| Terminal-Bench: Benchmarking Agents on Hard, Realistic Tasks in Command Line Interfaces | 2026 | benchmark | [Paper](https://arxiv.org/abs/2601.11868) | Core-Terminal-Primary |
| CLI-Gym: Scalable CLI Task Generation via Agentic Environment Inversion | 2026 | training / environment | [Paper](https://arxiv.org/abs/2602.10999) | Core-Terminal-Primary |
| TerminalWorld: Benchmarking Agents on Real-World Terminal Tasks | 2026 | benchmark | [Paper](https://arxiv.org/abs/2605.22535) | Core-Terminal-Primary |
| LongCLI-Bench: A Preliminary Benchmark and Study for Long-Horizon Agentic Programming in Command-Line Interfaces | 2026 | benchmark | [Paper](https://arxiv.org/abs/2602.14337) | Core-Terminal-Primary |
| ClawForge: Generating Executable Interactive Benchmarks for Command-Line Agents | 2026 | benchmark | [Paper](https://arxiv.org/abs/2605.14133) | Core-Terminal-Primary |
| WildClawBench: A Benchmark for Real-World, Long-Horizon Agent Evaluation | 2026 | benchmark | [Paper](https://arxiv.org/abs/2605.10912) | Core-Terminal-Primary |
| SetupBench: Assessing Software Engineering Agents' Ability to Bootstrap Development Environments | 2025 | benchmark | [Paper](https://arxiv.org/abs/2507.09063) | Core-Terminal-Primary |
| BashArena: A Control Setting for Highly Privileged AI Agents | 2025 | benchmark | [Paper](https://arxiv.org/abs/2512.15688) | Core-Terminal-Primary |
| CTFusion: A CTF-based Benchmark for LLM Agent Evaluation | 2026 | benchmark | [Paper](https://arxiv.org/abs/2605.11504) | Core-Terminal-Primary |
| PACEbench: A Framework for Evaluating Practical AI Cyber-Exploitation Capabilities | 2025 | benchmark | [Paper](https://arxiv.org/abs/2510.11688) | Core-Terminal-Primary |
| ITBench: Evaluating AI Agents across Diverse Real-World IT Automation Tasks | 2025 | benchmark | [Paper](https://arxiv.org/abs/2502.05352) | Core-Terminal-Primary |
| debug-gym: A Text-Based Environment for Interactive Debugging | 2025 | benchmark | [Paper](https://arxiv.org/abs/2503.21557) | Core-Terminal-Primary |
| Exp-Bench: Can AI Conduct AI Research Experiments? | 2025 | benchmark | [Paper](https://arxiv.org/abs/2505.24785) | Core-Terminal-Primary |
| Evaluating LLM-Based 0-to-1 Software Generation in End-to-End CLI Tool Scenarios | 2026 | benchmark | [Paper](https://arxiv.org/abs/2604.06742) | Core-Terminal-Primary |
| Do Agents Dream of Root Shells? Partial-Credit Evaluation of LLM Agents in Capture The Flag Challenges | 2026 | benchmark | [Paper](https://arxiv.org/abs/2604.19354) | Core-Terminal-Primary |
| Quantifying Frontier LLM Capabilities for Container Sandbox Escape | 2026 | benchmark | [Paper](https://arxiv.org/abs/2603.02277) | Core-Terminal-Primary |

## Repository and Software Engineering Benchmarks

Repository-centered benchmarks are not always terminal-native, but they are central to executable evaluation of coding agents and often rely on terminal-mediated setup, testing, patching, and recovery.

| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| SWE-bench: Can Language Models Resolve Real-World GitHub Issues? | 2024 | benchmark | [Paper](https://arxiv.org/abs/2310.06770) / [Website](https://www.swebench.com/) / [GitHub](https://github.com/SWE-bench/SWE-bench) | Core-Terminal-Primary |
| SWE-PolyBench: A Multi-Language Benchmark for Repository Level Evaluation of Coding Agents | 2025 | benchmark | [Paper](https://arxiv.org/abs/2504.08703) | Core-Hybrid-Terminal |
| SWE-bench Pro: Can AI Agents Solve Long-Horizon Software Engineering Tasks? | 2025 | benchmark | [Paper](https://arxiv.org/abs/2509.16941) | Core-Terminal-Primary |
| SWE-EVO: Benchmarking Coding Agents in Long-Horizon Software Evolution Scenarios | 2025 | benchmark | [Paper](https://arxiv.org/abs/2512.18470) | Core-Hybrid-Terminal |
| NL2Repo-Bench: Towards Long-Horizon Repository Generation Evaluation of Coding Agents | 2025 | benchmark | [Paper](https://arxiv.org/abs/2512.12730) | Core-Hybrid-Terminal |
| AgencyBench: Benchmarking the Frontiers of Autonomous Agents in 1M-Token Real-World Contexts | 2026 | benchmark | [Paper](https://arxiv.org/abs/2601.11044) | Core-Hybrid-Terminal |
| A Scalable Benchmark for Repository-Oriented Long-Horizon Conversational Context Management | 2026 | benchmark | [Paper](https://arxiv.org/abs/2603.06358) | Core-Hybrid-Terminal |
| SlopCodeBench: Benchmarking How Coding Agents Degrade Over Long-Horizon Iterative Tasks | 2026 | benchmark | [Paper](https://arxiv.org/abs/2603.24755) | Core-Hybrid-Terminal |
| When the Specification Emerges: Benchmarking Faithfulness Loss in Long-Horizon Coding Agents | 2026 | benchmark | [Paper](https://arxiv.org/abs/2603.17104) | Core-Hybrid-Terminal |
| SWE-MERA: A Dynamic Benchmark for Agenticly Evaluating Large Language Models on Software Engineering Tasks | 2025 | benchmark | [Paper](https://arxiv.org/abs/2507.11059) | Core-Hybrid-Terminal |
| ProjDevBench: Benchmarking AI Coding Agents on End-to-End Project Development | 2026 | benchmark | [Paper](https://arxiv.org/abs/2602.01655) | Core-Hybrid-Terminal |
| RepoMod-Bench: A Benchmark for Code Repository Modernization via Implementation-Agnostic Testing | 2026 | benchmark | [Paper](https://arxiv.org/abs/2602.22518) | Core-Hybrid-Terminal |
| SWE-Hub: A Unified Production System for Scalable, Executable Software Engineering Tasks | 2026 | benchmark | [Paper](https://arxiv.org/abs/2603.00575) | Core-Terminal-Primary |
| SWE-rebench v2: Language-Agnostic SWE Task Collection at Scale | 2026 | benchmark | [Paper](https://arxiv.org/abs/2602.23866) | Core-Terminal-Primary |
| ATime-Consistent Benchmark for Repository-Level Software Engineering Evaluation | 2026 | benchmark | [Paper](https://arxiv.org/abs/2603.26137) | Core-Hybrid-Terminal |
| Saving SWE-Bench: A Benchmark Mutation Approach for Realistic Agent Evaluation | 2025 | benchmark | [Paper](https://arxiv.org/abs/2510.08996) | Core-Hybrid-Terminal |
| SWE-Next: Scalable Real-World Software Engineering Tasks for Agents | 2026 | benchmark | [Paper](https://arxiv.org/abs/2603.20691) | Core-Terminal-Primary |

## Harnesses, Runtimes, and Agent-Computer Interfaces

Outer-loop systems that shape action spaces, observation formats, context delivery, workspace persistence, recovery, orchestration, and evaluation protocols.

| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| AutoHarness: Improving LLM Agents by Automatically Synthesizing a Code Harness | 2026 | architecture | [Paper](https://arxiv.org/abs/2603.03329) | Core-Hybrid-Terminal |
| Meta-Harness: End-to-End Optimization of Model Harnesses | 2026 | architecture | [Paper](https://arxiv.org/abs/2603.28052) | Core-Hybrid-Terminal |
| Agentic Harness Engineering: Observability-Driven Automatic Evolution of Coding-Agent Harnesses | 2026 | architecture | [Paper](https://arxiv.org/abs/2604.25850) | Core-Hybrid-Terminal |
| Copilot Evaluation Harness: Evaluating LLM-Guided Software Programming | 2024 | architecture | [Paper](https://arxiv.org/abs/2402.14261) | Core-Hybrid-Terminal |
| HyperAgent: Generalist Software Engineering Agents to Solve Coding Tasks at Scale | 2024 | architecture | [Paper](https://arxiv.org/abs/2409.16299) | Core-Hybrid-Terminal |
| AgentStepper: Interactive Debugging of Software Development Agents | 2026 | architecture | [Paper](https://arxiv.org/abs/2602.06593) | Core-Hybrid-Terminal |
| Debugging the Debuggers: Failure-Anchored Structured Recovery for Software Engineering Agents | 2026 | architecture | [Paper](https://arxiv.org/abs/2605.08717) | Core-Hybrid-Terminal |
| Scaling Long-Horizon LLM Agent via Context-Folding | 2025 | architecture | [Paper](https://arxiv.org/abs/2510.11967) | Core-Hybrid-Terminal |
| Agyn: A Multi-Agent System for Team-Based Autonomous Software Engineering | 2026 | architecture | [Paper](https://arxiv.org/abs/2602.01465) | Core-Hybrid-Terminal |
| Camels Can Use Computers Too: System-Level Security for Computer Use Agents | 2026 | architecture | [Paper](https://arxiv.org/abs/2601.09923) | Core-Hybrid-Terminal |
| DockSmith: Scaling Reliable Coding Environments via an Agentic Docker Builder | 2026 | architecture | [Paper](https://arxiv.org/abs/2602.00592) | Core-Hybrid-Terminal |
| Effective Strategies for Asynchronous Software Engineering Agents | 2026 | architecture | [Paper](https://arxiv.org/abs/2603.21489) | Core-Hybrid-Terminal |
| Externalization in LLM Agents: A Unified Review of Memory, Skills, Protocols and Harness Engineering | 2026 | architecture | [Paper](https://arxiv.org/abs/2604.08224) | Core-Hybrid-Terminal |
| AgentRM: An OS-Inspired Resource Manager for LLM Agent Systems | 2026 | architecture | [Paper](https://arxiv.org/abs/2603.13110) | Adjacent-Comparator |
| AIOS: LLM Agent Operating System | 2024 | architecture | [Paper](https://arxiv.org/abs/2403.16971) | Adjacent-Comparator |

## Training, Trajectories, and Competence Acquisition

Work on executable environments, trajectory generation, reinforcement learning, relabeling, filtering, context management, and skill acquisition for terminal or terminal-adjacent agents.

| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| Endless Terminals: Scaling RL Environments for Terminal Agents | 2026 | training | [Paper](https://arxiv.org/abs/2601.16443) | Core-Terminal-Primary |
| TermiGen: High-Fidelity Environment and Robust Trajectory Synthesis for Terminal Agents | 2026 | training | [Paper](https://arxiv.org/abs/2602.07274) | Core-Terminal-Primary |
| Large-Scale Terminal Agentic Trajectory Generation from Dockerized Environments | 2026 | training | [Paper](https://arxiv.org/abs/2602.01244) | Core-Terminal-Primary |
| On Data Engineering for Scaling LLM Terminal Capabilities | 2026 | training | [Paper](https://arxiv.org/abs/2602.21193) | Core-Terminal-Primary |
| Training Software Engineering Agents and Verifiers with SWE-Gym | 2024 | training | [Paper](https://arxiv.org/abs/2412.21139) | Core-Terminal-Primary |
| SWE-dev: Evaluating and Training Autonomous Feature-Driven Software Development | 2025 | training | [Paper](https://arxiv.org/abs/2505.16975) | Core-Terminal-Primary |
| Agent-RLVR: Training Software Engineering Agents via Guidance and Environment Rewards | 2025 | training | [Paper](https://arxiv.org/abs/2506.11425) | Core-Terminal-Primary |
| Training Long-Context, Multi-Turn Software Engineering Agents with Reinforcement Learning | 2025 | training | [Paper](https://arxiv.org/abs/2508.03501) | Core-Terminal-Primary |
| SWE-Master: Unleashing the Potential of Software Engineering Agents via Post-Training | 2026 | training | [Paper](https://arxiv.org/abs/2602.03411) | Core-Terminal-Primary |
| AgentFly: Extensible and Scalable Reinforcement Learning for LM Agents | 2025 | training | [Paper](https://arxiv.org/abs/2507.14897) | Core-Hybrid-Terminal |
| Hybrid-Gym: Training Coding Agents to Generalize Across Tasks | 2026 | training | [Paper](https://arxiv.org/abs/2602.16819) | Core-Hybrid-Terminal |
| TRACE: Capability-Targeted Agentic Training | 2026 | training / acquisition | [Paper](https://arxiv.org/abs/2604.05336) | Core-Hybrid-Terminal |
| AgentHER: Hindsight Experience Replay for LLM Agent Trajectory Relabeling | 2026 | training | [Paper](https://arxiv.org/abs/2603.21357) | Core-Terminal-Primary |
| CLEANER: Self-Purified Trajectories Boost Agentic Reinforcement Learning | 2026 | training | [Paper](https://arxiv.org/abs/2601.15141) | Core-Hybrid-Terminal |
| davinci-dev: Agent-Native Mid-Training for Software Engineering | 2026 | training | [Paper](https://arxiv.org/abs/2601.18418) | Core-Hybrid-Terminal |
| R2E-Gym: Procedural Environments and Hybrid Verifiers for Scaling Open-Weights SWE Agents | 2025 | training | [Paper](https://arxiv.org/abs/2504.07164) | Core-Terminal-Primary |

## Process, Trace, and Long-Horizon Evaluation

Evaluation work that moves beyond binary success toward process defects, trajectories, scaffold compliance, behavioral drivers, production usage, contamination, and long-horizon degradation.

| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| ProcBench: Evaluating Process-Level Defects and Control Preservation in LLM Coding Agents | 2026 | benchmark | [Paper](https://arxiv.org/abs/2605.20251) | Core-Hybrid-Terminal |
| OctoBench: Benchmarking Scaffold-Aware Instruction Following in Repository-Grounded Agentic Coding | 2026 | benchmark | [Paper](https://arxiv.org/abs/2601.10343) | Core-Hybrid-Terminal |
| Process-Level Trajectory Evaluation for Environment Configuration in Software Engineering Agents | 2025 | benchmark | [Paper](https://arxiv.org/abs/2510.25694) | Core-Hybrid-Terminal |
| AgentEval: DAG-Structured Step-Level Evaluation for Agentic Workflows with Error Propagation Tracking | 2026 | benchmark | [Paper](https://arxiv.org/abs/2604.23581) | Core-Hybrid-Terminal |
| AgentPulse: A Continuous Multi-Signal Framework for Evaluating AI Agents in Deployment | 2026 | benchmark | [Paper](https://arxiv.org/abs/2604.24038) | Core-Hybrid-Terminal |
| Agent Psychometrics: Task-Level Performance Prediction in Agentic Coding Benchmarks | 2026 | benchmark | [Paper](https://arxiv.org/abs/2604.00594) | SWE-Executable-Adjacent |
| Understanding Software Engineering Agents Through the Lens of Traceability: An Empirical Study | 2025 | empirical study | [Paper](https://arxiv.org/abs/2506.08311) | SWE-Executable-Adjacent |
| Understanding Software Engineering Agents: A Study of Thought-Action-Result Trajectories | 2025 | empirical study | [Paper](https://arxiv.org/abs/2506.18824) | SWE-Executable-Adjacent |
| Where Do AI Coding Agents Fail? An Empirical Study of Failed Agentic Pull Requests in GitHub | 2026 | empirical study | [Paper](https://arxiv.org/abs/2601.15195) | SWE-Executable-Adjacent |
| AIDev: Studying AI Coding Agents on GitHub | 2026 | benchmark / empirical study | [Paper](https://arxiv.org/abs/2602.09185) | Core-Hybrid-Terminal |
| Beyond Resolution Rates: Behavioral Drivers of Coding Agent Success and Failure | 2026 | benchmark | [Paper](https://arxiv.org/abs/2604.02547) | Core-Hybrid-Terminal |
| Beyond Binary Correctness: Scaling Evaluation of Long-Horizon Agents on Subjective Enterprise Tasks | 2026 | benchmark | [Paper](https://arxiv.org/abs/2603.22744) | Core-Hybrid-Terminal |

## Safety, Security, and Governance

Work on privileged execution, risky code, sandbox escape, harmful behavior, secure code generation, access control, oversight, and containment.

| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| ClawSafety: "Safe" LLMs, Unsafe Agents | 2026 | safety | [Paper](https://arxiv.org/abs/2604.01438) | Core-Hybrid-Terminal |
| The Blind Spot of Agent Safety: How Benign User Instructions Expose Critical Vulnerabilities in Computer-Use Agents | 2026 | safety | [Paper](https://arxiv.org/abs/2604.10577) | Core-Hybrid-Terminal |
| CLAWSBench: Evaluating Capability and Safety of LLM Productivity Agents in Simulated Workspaces | 2026 | safety | [Paper](https://arxiv.org/abs/2604.05172) | Core-Hybrid-Terminal |
| SecureVibeBench: Benchmarking Secure Vibe Coding of AI Agents via Reconstructing Vulnerability-Introducing Scenarios | 2026 | benchmark | [Paper](https://arxiv.org/abs/2509.22097) | Core-Hybrid-Terminal |
| SecureAgentBench: Benchmarking Secure Code Generation under Realistic Vulnerability Scenarios | 2025 | benchmark | [Paper](https://arxiv.org/abs/2509.22097) | SWE-Executable-Adjacent |
| CIBER: A Comprehensive Benchmark for Security Evaluation of Code Interpreter Agents | 2026 | safety | [Paper](https://arxiv.org/abs/2602.19547) | Adjacent-Comparator |
| LPS-Bench: Benchmarking Safety Awareness of Computer-Use Agents in Long-Horizon Planning under Benign and Adversarial Scenarios | 2026 | benchmark | [Paper](https://arxiv.org/abs/2602.03255) | Adjacent-Comparator |
| Secure and Efficient Access Control for Computer-Use Agents via Context Space | 2025 | architecture | [Paper](https://arxiv.org/abs/2509.22256) | Background-Theory |

## Adjacent Computer-Use and Tool-Use Agents

Boundary comparators for web, GUI, mobile, database, app-world, and general tool-use agents. These works clarify what is specific to terminal-mediated agency.

| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| AppWorld: A Controllable World of Apps and People for Benchmarking Interactive Coding Agents | 2024 | benchmark | [Paper](https://arxiv.org/abs/2407.18901) | Adjacent-Comparator |
| OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments | 2024 | benchmark | [Paper](https://arxiv.org/abs/2404.07972) | Adjacent-Comparator |
| WebArena: A Realistic Web Environment for Building Autonomous Agents | 2024 | benchmark | [Paper](https://arxiv.org/abs/2307.13854) | Adjacent-Comparator |
| AndroidWorld: A Dynamic Benchmarking Environment for Autonomous Agents | 2025 | benchmark | [Paper](https://arxiv.org/abs/2405.14573) | Adjacent-Comparator |
| ASTRA-Bench: Evaluating Tool-Use Agent Reasoning and Action Planning with Personal User Context | 2026 | benchmark | [Paper](https://arxiv.org/abs/2603.01357) | Adjacent-Comparator |
| LifelongAgentBench: Evaluating LLM Agents as Lifelong Learners | 2025 | benchmark | [Paper](https://arxiv.org/abs/2505.11942) | Adjacent-Comparator |
| ToolSandbox: A Stateful, Conversational, Interactive Evaluation Benchmark for LLM Tool Use Capabilities | 2025 | architecture / benchmark | [Paper](https://arxiv.org/abs/2408.04682) | Core-Hybrid-Terminal |
| CodeAct: Executable Code Actions Elicit Better LLM Agents | 2024 | architecture / training | [Paper](https://arxiv.org/abs/2402.01030) | SWE-Executable-Adjacent |
| Agentless: Demystifying LLM-Based Software Engineering Agents | 2024 | baseline | [Paper](https://arxiv.org/abs/2407.01489) | Adjacent-Comparator |

## Foundational Work

Background work on tool use, reasoning, code models, and executable action paradigms.

| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| ReAct: Synergizing Reasoning and Acting in Language Models | 2022 | definition | [Paper](https://arxiv.org/abs/2210.03629) | Background-Theory |
| Toolformer: Language Models Can Teach Themselves to Use Tools | 2023 | definition | [Paper](https://arxiv.org/abs/2302.04761) | Background-Theory |
| TALM: Tool Augmented Language Models | 2022 | definition | [Paper](https://arxiv.org/abs/2205.12255) | Background-Theory |
| Evaluating Large Language Models Trained on Code | 2021 | background | [Paper](https://arxiv.org/abs/2107.03374) | Background-Theory |
| Program-Aided Language Models | 2023 | background | [Paper](https://arxiv.org/abs/2211.10435) | Background-Theory |
| Competition-Level Code Generation with AlphaCode | 2022 | background | [Paper](https://www.science.org/doi/10.1126/science.abq1158) | Background-Theory |

## Survey Positioning

The survey treats the terminal as an execution substrate rather than merely a surface interface. A system is in scope when command execution drives task progress, textual feedback informs subsequent actions, and stateful environment interaction is central to the workload.

The current synthesis emphasizes three claims:

- Terminal-agent behavior should be analyzed through a substrate-centered command-observation loop.
- Terminal competence is multi-dimensional: action formulation, feedback interpretation, runtime management, state and context tracking, progress verification, failure recovery, and side-effect control are separable capability dimensions.
- Outer-loop design, including harnesses, context handling, observation shaping, permissions, and recovery policies, is a first-class variable that can materially change measured performance.

## Corpus Notes

The survey corpus uses evidence-calibrated inclusion tiers rather than quality rankings.

| Tier | Meaning |
|---|---|
| Core-Terminal-Primary | Terminal-mediated execution is the dominant locus of task progress. |
| Core-Hybrid-Terminal | Terminal execution is materially present alongside IDE, GUI, browser, API, or other modalities. |
| SWE-Executable-Adjacent | Execution is present, but terminal interaction is not the primary object of study. |
| Adjacent-Comparator | GUI/browser agents, agentless pipelines, and other boundary cases used for comparison. |
| Background-Theory | Conceptual or framing sources without direct terminal-agent evidence. |
| Engineering-Practice-Tool | Deployment-facing product or project reference, not treated as controlled empirical evidence. |

The latest survey PDF cites 192 bibliography entries, including 187 coded research entries and 5 engineering-practice tool references. In this README, entries are grouped by their primary role in the survey narrative, so a paper may reasonably fit more than one section.

## Contributing

PRs and issues are welcome. When adding an entry, please include:

- Name, year, and type.
- Link to paper, code, project page, dataset, or documentation.
- A short note explaining why the work belongs in the terminal-agent corpus.
- Suggested section and, if known, corpus tier.

Recommended entry format:

```markdown
| Name | Year | Type | Links | Corpus tier |
|---|---:|---|---|---|
| Example Agent | 2026 | benchmark | [Paper](https://arxiv.org/abs/0000.00000) / [GitHub](https://github.com/example/example) | Core-Terminal-Primary |
```

## Citation

If you use this list or the survey, please cite:

```bibtex
@misc{yuan2026terminalagents,
  title        = {Terminal Agents: A Survey of AI Agents in Command-Line Environments},
  author       = {Yuan, Xiaoyang and Zeng, Haoxi and Ye, Wencheng and Bin, Yi and Shao, Wenqi and Qian, Chen and Ye, Wei and Ding, Yujuan and Song, Jingkuan and Shen, Heng Tao},
  year         = {2026},
  howpublished = {\url{https://github.com/EnigmaYYYY/awesome-terminal-agents}},
  note         = {Survey and curated bibliography for terminal agents}
}
```
