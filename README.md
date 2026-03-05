# Awesome Agent Orchestration

[English](./README.md) | [中文](./README_zh.md)

A curated collection of open-source frameworks, tools, research papers, tutorials, and resources for **Agent Orchestration**, **Multi-Agent Systems**, and **Swarm Intelligence**. This repository focuses on the core concepts of coordinating, managing, and scaling multiple AI agents to work together collaboratively.

## Table of Contents

- [Why Agent Orchestration?](#why-agent-orchestration)
- [Core Frameworks](#core-frameworks)
  - [Multi-Agent Orchestration Frameworks](#multi-agent-orchestration-frameworks)
  - [Swarm Intelligence Frameworks](#swarm-intelligence-frameworks)
  - [Graph-Based Workflow Frameworks](#graph-based-workflow-frameworks)
- [Orchestration Patterns](#orchestration-patterns)
  - [Hierarchical](#hierarchical)
  - [Sequential](#sequential)
  - [Parallel/Concurrent](#parallelconcurrent)
  - [Mixture of Agents (MoA)](#mixture-of-agents-moa)
  - [Agent Council](#agent-council)
- [Communication & Coordination](#communication--coordination)
- [Research Papers](#research-papers)
- [Tools & Infrastructure](#tools--infrastructure)
- [Learning Resources](#learning-resources)
- [Related Awesome Lists](#related-awesome-lists)

---

## Why Agent Orchestration?

Agent orchestration is the practice of coordinating multiple AI agents to work together on complex tasks. It enables:

- **Scalability**: Handle complex workflows by distributing tasks across specialized agents
- **Specialization**: Each agent can focus on a specific domain or task
- **Robustness**: Fault tolerance through agent redundancy and recovery
- **Emergent Capabilities**: Complex behaviors arising from simple agent interactions
- **Real-World Applications**: From software development to research automation

---

## Core Frameworks

### Multi-Agent Orchestration Frameworks

| Project | Description | Stars |
|---------|-------------|-------|
| [AutoGen](https://github.com/microsoft/autogen) | Microsoft's framework for building multi-agent conversational systems | ![Stars](https://img.shields.io/github/stars/microsoft/autogen) |
| [CrewAI](https://github.com/crewAIInc/crewAI) | Role-based multi-agent framework for building AI teams | ![Stars](https://img.shields.io/github/stars/crewAIInc/crewAI) |
| [MetaGPT](https://github.com/geekan/MetaGPT) | Multi-agent framework for software development with role assignment | ![Stars](https://img.shields.io/github/stars/geekan/MetaGPT) |
| [agentUniverse](https://github.com/agentuniverse-ai/agentUniverse) | Enterprise-level multi-agent framework | ![Stars](https://img.shields.io/github/stars/agentuniverse-ai/agentUniverse) |
| [Langroid](https://github.com/langroid/langroid) | Multi-agent programming framework with message-passing | ![Stars](https://img.shields.io/github/stars/langroid/langroid) |
| [Phidata](https://github.com/agno-agi/phidata) | Multi-modal agent framework with built-in tools and UI | ![Stars](https://img.shields.io/github/stars/agno-agi/phidata) |
| [OpenAgents](https://github.com/OpenAgentsInc/openagents) | Open platform for deploying language agents | ![Stars](https://img.shields.io/github/stars/OpenAgentsInc/openagents) |
| [AgentVerse](https://github.com/OpenBML/AgentVerse) | Platform for running multiple LLM agents in simulated environments | ![Stars](https://img.shields.io/github/stars/OpenBML/AgentVerse) |

### Swarm Intelligence Frameworks

| Project | Description | Stars |
|---------|-------------|-------|
| [Swarms](https://github.com/kyegomez/swarms) | Production-grade multi-agent infrastructure platform | ![Stars](https://img.shields.io/github/stars/kyegomez/swarms) |
| [Swarm](https://github.com/autoreason/swarm) | Lightweight multi-agent orchestration framework | ![Stars](https://img.shields.io/github/stars/autoreason/swarm) |
| [Swarm-Tools](https://github.com/FelipeDaza7/swarm-tools) | Tool for coordinating AI agents with learning capabilities | ![Stars](https://img.shields.io/github/stars/FelipeDaza7/swarm-tools) |

### Graph-Based Workflow Frameworks

| Project | Description | Stars |
|---------|-------------|-------|
| [LangGraph](https://github.com/langchain-ai/langgraph) | Build stateful multi-agent applications with LangChain | ![Stars](https://img.shields.io/github/stars/langchain-ai/langgraph) |
| [LangChain](https://github.com/langchain-ai/langchain) | Modular framework for LLM application chaining | ![Stars](https://img.shields.io/github/stars/langchain-ai/langchain) |
| [LlamaIndex](https://github.com/jerryjliu/llama_index) | Data-centric agent framework for RAG | ![Stars](https://img.shields.io/github/stars/jerryjliu/llama_index) |
| [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | Microsoft orchestration SDK for .NET/Python | ![Stars](https://img.shields.io/github/stars/microsoft/semantic-kernel) |

### Lightweight & Specialized Agents

| Project | Description | Stars |
|---------|-------------|-------|
| [SmolAgents](https://github.com/smol-ai/smolagents) | Minimalist library for code-writing agents | ![Stars](https://img.shields.io/github/stars/smol-ai/smolagents) |
| [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT) | Pioneering autonomous agent with self-prompting | ![Stars](https://img.shields.io/github/stars/Significant-Gravitas/Auto-GPT) |
| [BabyAGI](https://github.com/yoheinakajima/babyagi) | Simple autonomous task management | ![Stars](https://img.shields.io/github/stars/yoheinakajima/babyagi) |
| [GPT-Engineer](https://github.com/AntonOsika/gpt-engineer) | Agent for generating full projects from specs | ![Stars](https://img.shields.io/github/stars/AntonOsika/gpt-engineer) |
| [BMTools](https://github.com/OpenBMB/BMTools) | Tool/API registry for agents | ![Stars](https://img.shields.io/github/stars/OpenBMB/BMTools) |

---

## Orchestration Patterns

### Hierarchical

In hierarchical orchestration, a supervisor agent delegates tasks to specialized sub-agents. This pattern is suitable for complex tasks requiring domain expertise.

- **Use Cases**: Software development teams, research automation, enterprise workflows
- **Frameworks**: AutoGen, CrewAI, LangGraph

### Sequential

Sequential workflows process tasks through a pipeline where each agent completes its step before passing to the next.

- **Use Cases**: Document processing, data transformation pipelines
- **Frameworks**: LangChain, LangGraph

### Parallel/Concurrent

Multiple agents work simultaneously on independent subtasks, with results aggregated afterward.

- **Use Cases**: Research gathering, parallel code generation
- **Frameworks**: Swarms, AutoGen

### Mixture of Agents (MoA)

Multiple expert agents contribute their perspectives, with outputs combined through iterative refinement.

- **Research**: [Mixture of Agents Paper](https://arxiv.org/abs/2406.04692)
- **Implementation**: Swarms MoA, LangGraph

### Agent Council

Multiple agents discuss and debate to reach consensus on decisions.

- **Use Cases**: Decision making, complex analysis, creative writing
- **Framework**: AutoGen GroupChat

---

## Communication & Coordination

### Message Passing

- **Langroid**: Message-passing based multi-agent framework
- **AutoGen**: Conversational message passing

### Shared State / BlackBoard Systems

- **Swarm Matcher**: Agent matching and selection
- **Message Pool**: Shared communication system

### Task Distribution

- **Auto Swarm**: Self-organizing swarm with automatic task distribution
- **Agent Delegation**: Task delegation and management

---

## Research Papers

### Multi-Agent Collaboration

| Paper | Description | Year |
|-------|-------------|------|
| [CAMEL: Communicative Agents for "Mind" Exploration](https://arxiv.org/abs/2303.17760) | Role-playing agent collaboration through dialogue | 2023 |
| [MetaGPT: Multi-Agent Collaboration Framework](https://arxiv.org/abs/2308.07370) | Software development with agent roles (PM, Engineer, QA) | 2023 |
| [AgentVerse: Flexible Multi-Agent Platform](https://arxiv.org/abs/2308.07429) | Collaborative problem-solving in simulated environments | 2023 |
| [Generative Agents](https://arxiv.org/abs/2304.03442) | Interactive agents with long-term memory in virtual worlds | 2023 |
| [Mixture of Agents](https://arxiv.org/abs/2406.04692) | Parallel processing with iterative refinement | 2024 |

### Orchestration & Planning

| Paper | Description | Year |
|-------|-------------|------|
| [MALT: Multi-Agent LLM Orchestration](https://arxiv.org/abs/2412.01928) | Structured conversations with Creator-Verifier-Refiner pattern | 2024 |
| [Agent-as-a-Judge](https://arxiv.org/abs/2410.10934) | Agents evaluate other agents | 2024 |
| [ReAct: Synergizing Reasoning and Acting](https://arxiv.org/abs/2210.03629) | Interleaving thoughts and actions | 2022 |

### Evaluation

| Benchmark | Description |
|-----------|-------------|
| [AgentBench](https://arxiv.org/abs/2308.07258) | Evaluates agents across diverse environments |
| [Multi-Agent Evaluation](https://arxiv.org/abs/2312.04323) | Survey of metrics for agent evaluation |

---

## Tools & Infrastructure

### Observability & Tracing

| Tool | Description |
|------|-------------|
| [Langfuse](https://github.com/langfuse/langfuse) | Open-source LLM engineering platform |
| [Phoenix](https://github.com/Arize-ai/phoenix) | Open-source LLM tracing |
| [Opik](https://github.com/comet-ml/opik) | Open-source LLM evaluation |
| [Agenta](https://github.com/agenta-ai/agenta) | LLMOps platform for prototyping |

### Memory & Knowledge

| Tool | Description |
|------|-------------|
| [Memori](https://github.com/MemoriLabs/Memori) | SQL Native Memory Layer for LLMs & Agents |
| [Letta](https://github.com/letta/letta) | Memory layer for AI agents |

---

## Learning Resources

### Tutorials & Guides

- [LLM Powered Autonomous Agents](https://lilianweng.github.io/posts/2023-06-15-agent/) - Lilian Weng's comprehensive guide
- [Prompt Engineering Guide: LLM Agents](https://github.com/dair-ai/Prompt-Engineering-Guide#llm-agents) - Comprehensive agent building guide
- [Building Autonomous Agents with LangChain](https://www.youtube.com/watch?v=example) - Video tutorial
- [Enterprise-Grade-Agents-Course](https://github.com/The-Swarm-Corporation/Enterprise-Grade-Agents-Course) - Comprehensive course

### Documentation

- [AutoGen Documentation](https://microsoft.github.io/autogen/) - Microsoft AutoGen docs
- [CrewAI Documentation](https://docs.crewai.com/) - CrewAI official docs
- [LangGraph Documentation](https://langchain-ai.github.io/langgraph/) - LangGraph docs
- [Swarms Documentation](https://docs.swarms.world/) - Swarms framework docs

---

## Related Awesome Lists

- [awesome-ai-agents](https://github.com/heurema/awesome-ai-agents) - Comprehensive AI agent resources
- [awesome-LangGraph](https://github.com/von-development/awesome-LangGraph) - LangChain/LangGraph ecosystem
- [awesome-multi-agent-papers](https://github.com/kyegomez/awesome-multi-agent-papers) - Multi-agent research papers
- [awesome-Swarms-List](https://github.com/The-Swarm-Corporation/Awesome-Swarms-List) - Swarms framework resources

---

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first.

1. Fork the repository
2. Add your resource in the appropriate section
3. Ensure consistent formatting
4. Submit a pull request

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)

To the extent possible under law, [Your Name](https://github.com/yourusername) has waived all copyright and related rights to this work.

---

*Star this repository if you find it useful!*
