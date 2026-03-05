# Awesome Agent Orchestration

[English](./README.md) | [中文](./README_zh.md)

A curated collection of open-source frameworks, tools, research papers, tutorials, and resources for **Agent Orchestration**, **Multi-Agent Systems**, and **Swarm Intelligence**. This repository focuses on the core concepts of coordinating, managing, and scaling multiple AI agents to work together collaboratively.

## Table of Contents

- [Why Agent Orchestration?](#why-agent-orchestration)
- [Core Frameworks](#core-frameworks)
  - [Multi-Agent Orchestration Frameworks](#multi-agent-orchestration-frameworks)
  - [Swarm Intelligence Frameworks](#swarm-intelligence-frameworks)
  - [Graph-Based Workflow Frameworks](#graph-based-workflow-frameworks)
  - [Type-Safe & Modern Frameworks](#type-safe--modern-frameworks)
  - [TypeScript & Node.js Frameworks](#typescript--nodejs-frameworks)
  - [Go Frameworks](#go-frameworks)
  - [Swift, Ruby & Elixir Frameworks](#swift-ruby--elixir-frameworks)
  - [PHP & Java Frameworks](#php--java-frameworks)
- [Agent Communication Protocols](#agent-communication-protocols)
  - [Agent-to-Agent (A2A)](#agent-to-agent-a2a)
  - [Model Context Protocol (MCP)](#model-context-protocol-mcp)
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
| [agency-swarm](https://github.com/VRSEN/agency-swarm) | Reliable multi-agent orchestration framework | ![Stars](https://img.shields.io/github/stars/VRSEN/agency-swarm) |
| [OpenAI Swarm](https://github.com/openai/swarm) | Educational lightweight multi-agent orchestration framework | ![Stars](https://img.shields.io/github/stars/openai/swarm) |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) | Framework for building, orchestrating and deploying AI agents | ![Stars](https://img.shields.io/github/stars/microsoft/agent-framework) |
| [OpenAI Agents Python](https://github.com/openai/openai-agents-python) | Lightweight powerful framework for multi-agent workflows | ![Stars](https://img.shields.io/github/stars/openai/openai-agents-python) |
| [Haystack](https://github.com/deepset-ai/haystack) | Open-source AI orchestration for context-engineered LLM applications | ![Stars](https://img.shields.io/github/stars/deepset-ai/haystack) |
| [LLMStack](https://github.com/trypromptly/LLMStack) | No-code multi-agent framework for LLM agents and workflows | ![Stars](https://img.shields.io/github/stars/trypromptly/LLMStack) |
| [LazyLLM](https://github.com/LazyAGI/LazyLLM) | Easiest way for building multi-agent LLM applications | ![Stars](https://img.shields.io/github/stars/LazyAGI/LazyLLM) |
| [MindSearch](https://github.com/InternLM/MindSearch) | LLM-based multi-agent framework for web search engine | ![Stars](https://img.shields.io/github/stars/InternLM/MindSearch) |
| [TradingAgents](https://github.com/TauricResearch/TradingAgents) | Multi-agent LLM financial trading framework | ![Stars](https://img.shields.io/github/stars/TauricResearch/TradingAgents) |
| [Shannon](https://github.com/Kocoro-lab/Shannon) | Production-oriented multi-agent orchestration framework | ![Stars](https://img.shields.io/github/stars/Kocoro-lab/Shannon) |
| [Solace Agent Mesh](https://github.com/SolaceLabs/solace-agent-mesh) | Event-driven framework for multi-agent AI systems | ![Stars](https://img.shields.io/github/stars/SolaceLabs/solace-agent-mesh) |
| [Pipelex](https://github.com/Pipelex/pipelex) | Declarative language for composable AI workflows | ![Stars](https://img.shields.io/github/stars/Pipelex/pipelex) |
| [CodeFuse-muAgent](https://github.com/codefuse-ai/CodeFuse-muAgent) | Innovative agent framework driven by KG Engine | ![Stars](https://img.shields.io/github/stars/codefuse-ai/CodeFuse-muAgent) |
| [L2MAC](https://github.com/samholt/L2MAC) | LLM Automatic Computer Framework | ![Stars](https://img.shields.io/github/stars/samholt/L2MAC) |
| [Patchwork](https://github.com/patched-codes/patchwork) | Agentic AI framework for enterprise workflow automation | ![Stars](https://img.shields.io/github/stars/patched-codes/patchwork) |

### Swarm Intelligence Frameworks

| Project | Description | Stars |
|---------|-------------|-------|
| [Swarms](https://github.com/kyegomez/swarms) | Production-grade multi-agent infrastructure platform | ![Stars](https://img.shields.io/github/stars/kyegomez/swarms) |
| [Swarm](https://github.com/autoreason/swarm) | Lightweight multi-agent orchestration framework | ![Stars](https://img.shields.io/github/stars/autoreason/swarm) |
| [Swarm-Tools](https://github.com/FelipeDaza7/swarm-tools) | Tool for coordinating AI agents with learning capabilities | ![Stars](https://img.shields.io/github/stars/FelipeDaza7/swarm-tools) |
| [Ruflo](https://github.com/ruvnet/ruflo) | Leading agent orchestration platform for Claude | ![Stars](https://img.shields.io/github/stars/ruvnet/ruflo) |
| [swarms-rs](https://github.com/The-Swarm-Corporation/swarms-rs) | Enterprise-grade multi-agent orchestration in Rust | ![Stars](https://img.shields.io/github/stars/The-Swarm-Corporation/swarms-rs) |
| [Lux](https://github.com/Spectral-Finance/lux) | Open-source framework for multi-agent swarmed intelligence | ![Stars](https://img.shields.io/github/stars/Spectral-Finance/lux) |
| [AutoRT](https://github.com/kyegomez/AutoRT) | Embodied foundation models for robotic agents | ![Stars](https://img.shields.io/github/stars/kyegomez/AutoRT) |

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

### Type-Safe & Modern Frameworks

| Project | Description | Stars |
|---------|-------------|-------|
| [PydanticAI](https://github.com/pydantic/pydantic-ai) | Type-safe agent framework using Pydantic models | ![Stars](https://img.shields.io/github/stars/pydantic/pydantic-ai) |
| [DeepAgents](https://github.com/vstorm-co/pydantic-deepagents) | Production-grade autonomous agents on PydanticAI | ![Stars](https://img.shields.io/github/stars/vstorm-co/pydantic-deepagents) |
| [Subagents](https://github.com/vstorm-co/subagents-pydantic-ai) | Subagent delegation framework for PydanticAI | ![Stars](https://img.shields.io/github/stars/vstorm-co/subagents-pydantic-ai) |
| [Flux0](https://github.com/flux0-ai/flux0) | Multi-agent deployment framework with session management | ![Stars](https://img.shields.io/github/stars/flux0-ai/flux0) |
| [Mamba Agents](https://github.com/sequenzia/mamba-agents) | Simple extensible AI Agent framework | ![Stars](https://img.shields.io/github/stars/sequenzia/mamba-agents) |

### TypeScript & Node.js Frameworks

| Project | Description | Stars |
|---------|-------------|-------|
| [openai-swarm-node](https://github.com/youseai/openai-swarm-node) | Node.js implementation of OpenAI's Swarm framework | ![Stars](https://img.shields.io/github/stars/youseai/openai-swarm-node) |
| [Network-AI](https://github.com/jovanSAPFIONEER/Network-AI) | TypeScript/Node multi-agent orchestrator with shared state | ![Stars](https://img.shields.io/github/stars/jovanSAPFIONEER/Network-AI) |
| [megazord](https://github.com/Sh3rd3n/megazord) | Claude Code framework for multi-agent coordination | ![Stars](https://img.shields.io/github/stars/Sh3rd3n/megazord) |
| [Voltmachines](https://github.com/ssdeanx/Voltmachines) | Multi-agent framework built on VoltAgent | ![Stars](https://img.shields.io/github/stars/ssdeanx/Voltmachines) |
| [agent-swarm-kit](https://github.com/tripolskypetr/agent-swarm-kit) | TypeScript library for framework-agnostic multi-agent systems | ![Stars](https://img.shields.io/github/stars/tripolskypetr/agent-swarm-kit) |
| [ai-orchestra](https://github.com/langtail/ai-orchestra) | Lightweight orchestration for AI Agents around Vercel's streamText | ![Stars](https://img.shields.io/github/stars/langtail/ai-orchestra) |

### Go Frameworks

| Project | Description | Stars |
|---------|-------------|-------|
| [openai-agents-go](https://github.com/nlpodyssey/openai-agents-go) | Lightweight powerful framework for multi-agent workflows in Go | ![Stars](https://img.shields.io/github/stars/nlpodyssey/openai-agents-go) |
| [swarm-go](https://github.com/feiskyer/swarm-go) | Ergonomic lightweight multi-agent orchestration in Go | ![Stars](https://img.shields.io/github/stars/feiskyer/swarm-go) |
| [rs-graph-llm](https://github.com/a-agmon/rs-graph-llm) | High-performance framework for interactive multi-agent workflows in Rust | ![Stars](https://img.shields.io/github/stars/a-agmon/rs-graph-llm) |

### Swift, Ruby & Elixir Frameworks

| Project | Description | Stars |
|---------|-------------|-------|
| [SwiftSwarm](https://github.com/jamesrochabrun/SwiftSwarm) | Swift framework for lightweight multi-agent orchestration | ![Stars](https://img.shields.io/github/stars/jamesrochabrun/SwiftSwarm) |
| [Swarm](https://github.com/christopherkarani/Swarm) | Lightweight agent orchestration framework in Swift | ![Stars](https://img.shields.io/github/stars/christopherkarani/Swarm) |
| [ruby-openai-swarm](https://github.com/graysonchen/ruby-openai-swarm) | Ruby-based framework for multi-agent orchestration | ![Stars](https://img.shields.io/github/stars/graysonchen/ruby-openai-swarm) |
| [swarm_ex](https://github.com/nrrso/swarm_ex) | Elixir library for lightweight AI agent orchestration | ![Stars](https://img.shields.io/github/stars/nrrso/swarm_ex) |
| [shifts](https://github.com/aaronrussell/shifts) | Elixir framework for composing autonomous AI agent workflows | ![Stars](https://img.shields.io/github/stars/aaronrussell/shifts) |

### PHP & Java Frameworks

| Project | Description | Stars |
|---------|-------------|-------|
| [neuron-ai](https://github.com/neuron-core/neuron-ai) | PHP agentic framework for production-ready AI applications | ![Stars](https://img.shields.io/github/stars/neuron-core/neuron-ai) |
| [swarm-ai](https://github.com/intelliswarm-ai/swarm-ai) | Java multi-agent orchestration with Spring AI | ![Stars](https://img.shields.io/github/stars/intelliswarm-ai/swarm-ai) |

### Workflow & Pipeline Frameworks

| Project | Description | Stars |
|---------|-------------|-------|
| [circuit](https://github.com/smogili1/circuit) | Drag-and-drop agent workflow builder | ![Stars](https://img.shields.io/github/stars/smogili1/circuit) |
| [routilux](https://github.com/lzjever/routilux) | Event-driven workflow orchestration for Python | ![Stars](https://img.shields.io/github/stars/lzjever/routilux) |
| [CraftFlow](https://github.com/scholarlords/CraftFlow) | Workflow orchestration for RAG and multi-agent collaborations | ![Stars](https://img.shields.io/github/stars/scholarlords/CraftFlow) |
| [sentinels](https://github.com/garyblankenship/sentinels) | Laravel package for agent-based task orchestration | ![Stars](https://img.shields.io/github/stars/garyblankenship/sentinels) |
| [titan-orchestrator](https://github.com/ramn51/titan-orchestrator) | Distributed orchestrator bridging DevOps and Agentic AI | ![Stars](https://img.shields.io/github/stars/ramn51/titan-orchestrator) |

---

## Agent Communication Protocols

### Agent-to-Agent (A2A)

Google's A2A protocol enables secure, interoperable communication between autonomous agents across frameworks and vendors.

| Project | Description | Stars |
|---------|-------------|-------|
| [awesome-a2a-agents](https://github.com/isekOS/awesome-a2a-agents) | Curated list of A2A tools and frameworks | ![Stars](https://img.shields.io/github/stars/isekOS/awesome-a2a-agents) |
| [python-a2a](https://github.com/themanojdesai/python-a2a) | Python implementation of A2A protocol | ![Stars](https://img.shields.io/github/stars/themanojdesai/python-a2a) |
| [a2a-net](https://github.com/neuroglia-io/a2a-net) | .NET implementation of A2A protocol | ![Stars](https://img.shields.io/github/stars/neuroglia-io/a2a-net) |
| [a2a-langgraph](https://github.com/ruska-ai/a2a-langgraph) | A2A protocol built on LangGraph | ![Stars](https://img.shields.io/github/stars/ruska-ai/a2a-langgraph) |
| [nestjs-a2a](https://github.com/thestupd/nestjs-a2a) | NestJS library for A2A protocol | ![Stars](https://img.shields.io/github/stars/thestupd/nestjs-a2a) |
| [a2a4j](https://github.com/PheonixHkbxoic/a2a4j) | Java implementation of A2A protocol | ![Stars](https://img.shields.io/github/stars/PheonixHkbxoic/a2a4j) |
| [A2A-MCP-Server](https://github.com/GongRzhe/A2A-MCP-Server) | Bridge between MCP and A2A protocols | ![Stars](https://img.shields.io/github/stars/GongRzhe/A2A-MCP-Server) |
| [a2a-x402](https://github.com/google-agentic-commerce/a2a-x402) | A2A protocol with cryptocurrency payments | ![Stars](https://img.shields.io/github/stars/google-agentic-commerce/a2a-x402) |
| [Routa](https://github.com/phodal/routa) | Multi-agent coordination platform via MCP/A2A | ![Stars](https://img.shields.io/github/stars/phodal/routa) |
| [mangaba_ai](https://github.com/Mangaba-ai/mangaba_ai) | Minimalist AI agents with A2A and MCP | ![Stars](https://img.shields.io/github/stars/Mangaba-ai/mangaba_ai) |

### Model Context Protocol (MCP)

An open protocol that enables seamless connection between AI models and external tools/data sources. MCP is becoming the standard for tool-augmented LLM applications.

#### Official Resources

| Project | Description | Stars |
|---------|-------------|-------|
| [awesome-mcp-servers](https://github.com/wong2/awesome-mcp-servers) | Most popular curated list of MCP servers | ![Stars](https://img.shields.io/github/stars/wong2/awesome-mcp-servers) |
| [modelcontextprotocol/registry](https://github.com/modelcontextprotocol/registry) | Community-driven MCP server registry | ![Stars](https://img.shields.io/github/stars/modelcontextprotocol/registry) |
| [microsoft/mcp](https://github.com/microsoft/mcp) | Official Microsoft MCP servers catalog | ![Stars](https://img.shields.io/github/stars/microsoft/mcp) |
| [modelcontextprotocol/swift-sdk](https://github.com/modelcontextprotocol/swift-sdk) | Official Swift SDK for MCP | ![Stars](https://img.shields.io/github/stars/modelcontextprotocol/swift-sdk) |

#### Database & Vector Stores

| Project | Description | Stars |
|---------|-------------|-------|
| [mcp-server-qdrant](https://github.com/qdrant/mcp-server-qdrant) | Official Qdrant vector database server | ![Stars](https://img.shields.io/github/stars/qdrant/mcp-server-qdrant) |
| [mcp-server-milvus](https://github.com/zilliztech/mcp-server-milvus) | Milvus vector database server | ![Stars](https://img.shields.io/github/stars/zilliztech/mcp-server-milvus) |
| [mcp-neo4j](https://github.com/neo4j-contrib/mcp-neo4j) | Neo4j graph database server | ![Stars](https://img.shields.io/github/stars/neo4j-contrib/mcp-neo4j) |
| [mongodb-mcp-server](https://github.com/mongodb-js/mcp-mcp-server) | MongoDB database server | ![Stars](https://img.shields.io/github/stars/mongodb-js/mongodb-mcp-server) |
| [mysql_mcp_server](https://github.com/designcomputer/mysql_mcp_server) | MySQL database server | ![Stars](https://img.shields.io/github/stars/designcomputer/mysql_mcp_server) |
| [MariaDB/mcp](https://github.com/MariaDB/mcp) | MariaDB database server | ![Stars](https://img.shields.io/github/stars/MariaDB/mcp) |

#### Browser & Automation

| Project | Description | Stars |
|---------|-------------|-------|
| [mcp-playwright](https://github.com/executeautomation/mcp-playwright) | Playwright browser automation | ![Stars](https://img.shields.io/github/stars/executeautomation/mcp-playwright) |
| [mcp-chrome](https://github.com/hangwin/mcp-chrome) | Chrome extension for browser control | ![Stars](https://img.shields.io/github/stars/hangwin/mcp-chrome) |
| [mobile-mcp](https://github.com/mobile-next/mobile-mcp) | iOS/Android automation | ![Stars](https://img.shields.io/github/stars/mobile-next/mobile-mcp) |

#### Development & Tools

| Project | Description | Stars |
|---------|-------------|-------|
| [mcp-filesystem-server](https://github.com/mark3labs/mcp-filesystem-server) | Filesystem operations | ![Stars](https://img.shields.io/github/stars/mark3labs/mcp-filesystem-server) |
| [jupyter-mcp-server](https://github.com/datalayer/jupyter-mcp-server) | Jupyter notebook integration | ![Stars](https://img.shields.io/github/stars/datalayer/jupyter-mcp-server) |
| [fetch-mcp](https://github.com/zcaceres/fetch-mcp) | HTTP fetching | ![Stars](https://img.shields.io/github/stars/zcaceres/fetch-mcp) |
| [mcp-graphql](https://github.com/blurrah/mcp-graphql) | GraphQL API integration | ![Stars](https://img.shields.io/github/stars/blurrah/mcp-graphql) |
| [mcpadapt](https://github.com/grll/mcpadapt) | Connect 650+ MCP servers to any framework | ![Stars](https://img.shields.io/github/stars/grll/mcpadapt) |

#### Specialized Servers

| Project | Description | Stars |
|---------|-------------|-------|
| [arxiv-mcp-server](https://github.com/blazickjp/arxiv-mcp-server) | arXiv paper search | ![Stars](https://img.shields.io/github/stars/blazickjp/arxiv-mcp-server) |
| [mcp-youtube](https://github.com/anaisbetts/mcp-youtube) | YouTube video analysis | ![Stars](https://img.shields.io/github/stars/anaisbetts/mcp-youtube) |
| [excel-mcp-server](https://github.com/haris-musa/excel-mcp-server) | Excel file manipulation | ![Stars](https://img.shields.io/github/stars/haris-musa/excel-mcp-server) |
| [drawio-mcp-server](https://github.com/lgazo/drawio-mcp-server) | Diagram creation | ![Stars](https://img.shields.io/github/stars/lgazo/drawio-mcp-server) |
| [freecad-mcp](https://github.com/neka-nat/freecad-mcp) | FreeCAD 3D modeling | ![Stars](https://img.shields.io/github/stars/neka-nat/freecad-mcp) |
| [ida-mcp-server](https://github.com/MxIris-Reverse-Engineering/ida-mcp-server) | IDA reverse engineering | ![Stars](https://img.shields.io/github/stars/MxIris-Reverse-Engineering/ida-mcp-server) |
| [kubernetes-mcp-server](https://github.com/containers/kubernetes-mcp-server) | Kubernetes management | ![Stars](https://img.shields.io/github/stars/containers/kubernetes-mcp-server) |

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
| [Chain-of-Thought Prompting](https://arxiv.org/abs/2201.11903) | Step-by-step reasoning in LLM prompts | 2022 |
| [Tree-of-Thoughts](https://arxiv.org/abs/2305.10601) | Multiple reasoning branches for complex problems | 2023 |
| [Reflexion](https://arxiv.org/abs/2309.00668) | Self-critique loop for long-horizon tasks | 2023 |
| [HuggingGPT](https://arxiv.org/abs/2303.17580) | LLM controller orchestrating expert models | 2023 |
| [Toolformer](https://arxiv.org/abs/2302.04761) | Self-supervised fine-tuning for API calling | 2023 |

### Memory & Long-Term Autonomy

| Paper | Description | Year |
|-------|-------------|------|
| [Generative Agents](https://arxiv.org/abs/2304.03442) | Interactive agents simulating humans in virtual worlds | 2023 |
| [Survey on Memory Mechanisms of LLM Agents](https://arxiv.org/abs/2402.13736) | Overview of memory architectures and retrieval | 2024 |

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
| [Logfire](https://github.com/pydantic/logfire) | Pydantic's open-source observability tool |
| [Langtrace](https://github.com/Scale3-Labs/langtrace) | Open-source observability for AI agents |
| [Okahu Monocle](https://github.com/OkahuAI/monocle) | Tracing framework by Linux Foundation |

### Memory & Knowledge

| Tool | Description |
|------|-------------|
| [Memori](https://github.com/MemoriLabs/Memori) | SQL Native Memory Layer for LLMs & Agents |
| [Letta](https://github.com/letta/letta) | Memory layer for AI agents |

### Deployment & Infrastructure

| Tool | Description |
|------|-------------|
| [OpenAgents](https://github.com/OpenAgentsInc/openagents) | Platform for deploying language agents |
| [FastAPI Agents](https://github.com/blairhudson/fastapi-agents) | FastAPI extension for AI agent frameworks |
| [AgentAPIProduction](https://github.com/The-Swarm-Corporation/AgentAPIProduction) | Production-ready agent API system |
| [AgentOS](https://github.com/The-Swarm-Corporation/AgentOS) | Operating system for AI agents |

### Evaluation & Benchmarking

| Tool | Description |
|------|-------------|
| [AgentBench](https://github.com/AgentBench/AgentBench) | Evaluates agents across diverse environments |
| [swarms-evals](https://github.com/The-Swarm-Corporation/swarms-evals) | Evaluation framework for swarm systems |
| [RAGAS](https://github.com/explodinggradients/ragas) | Evaluation framework for RAG systems |

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
- [awesome-a2a-agents](https://github.com/isekOS/awesome-a2a-agents) - A2A protocol ecosystem
- [awesome-agent-protocols](https://github.com/shanjai-raj/awesome-agent-protocols) - Agent communication protocols
- [awesome-agents](https://github.com/l-aime/awesome-agents) - Cutting-edge AI agent projects
- [awesome-agentic-ai](https://github.com/mlnjsh/awesome-agentic-ai) - Agentic AI frameworks and papers

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
