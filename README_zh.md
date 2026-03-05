# Awesome Agent Orchestration

[English](./README.md) | [中文](./README_zh.md)

精选的**智能体编排**、**多智能体系统**和**群体智能**相关的开源框架、工具、论文、教程和资源集合。本仓库专注于协调、管理和扩展多个 AI 智能体协同工作的核心概念。

## 目录

- [为什么需要智能体编排？](#为什么需要智能体编排)
- [核心框架](#核心框架)
  - [多智能体编排框架](#多智能体编排框架)
  - [群体智能框架](#群体智能框架)
  - [基于图的编排框架](#基于图的编排框架)
- [编排模式](#编排模式)
  - [层级式](#层级式)
  - [顺序式](#顺序式)
  - [并行/并发式](#并行并发式)
  - [混合专家模式 (MoA)](#混合专家模式-moa)
  - [智能体委员会](#智能体委员会)
- [通信与协调](#通信与协调)
- [研究论文](#研究论文)
- [工具与基础设施](#工具与基础设施)
- [学习资源](#学习资源)
- [相关 Awesome 列表](#相关-awesome-列表)

---

## 为什么需要智能体编排？

智能体编排是协调多个 AI 智能体共同完成复杂任务的实践，它能够实现：

- **可扩展性**：通过将任务分配给专业智能体来处理复杂工作流
- **专业化**：每个智能体可以专注于特定领域或任务
- **鲁棒性**：通过智能体冗余和恢复实现容错
- **涌现能力**：通过简单的智能体交互产生复杂行为
- **实际应用**：从软件开发到研究自动化

---

## 核心框架

### 多智能体编排框架

| 项目 | 描述 | Stars |
|------|------|-------|
| [AutoGen](https://github.com/microsoft/autogen) | 微软的多智能体会话系统框架 | ![Stars](https://img.shields.io/github/stars/microsoft/autogen) |
| [CrewAI](https://github.com/crewAIInc/crewAI) | 基于角色的多智能体框架，构建 AI 团队 | ![Stars](https://img.shields.io/github/stars/crewAIInc/crewAI) |
| [MetaGPT](https://github.com/geekan/MetaGPT) | 软件开发多智能体框架，支持角色分配 | ![Stars](https://img.shields.io/github/stars/geekan/MetaGPT) |
| [agentUniverse](https://github.com/agentuniverse-ai/agentUniverse) | 企业级多智能体框架 | ![Stars](https://img.shields.io/github/stars/agentuniverse-ai/agentUniverse) |
| [Langroid](https://github.com/langroid/langroid) | 基于消息传递的多智能体编程框架 | ![Stars](https://img.shields.io/github/stars/langroid/langroid) |
| [Phidata](https://github.com/agno-agi/phidata) | 多模态智能体框架，内置工具和 UI | ![Stars](https://img.shields.io/github/stars/agno-agi/phidata) |
| [OpenAgents](https://github.com/OpenAgentsInc/openagents) | 开放平台，用于部署语言智能体 | ![Stars](https://img.shields.io/github/stars/OpenAgentsInc/openagents) |
| [AgentVerse](https://github.com/OpenBML/AgentVerse) | 在模拟环境中运行多个 LLM 智能体的平台 | ![Stars](https://img.shields.io/github/stars/OpenBML/AgentVerse) |

### 群体智能框架

| 项目 | 描述 | Stars |
|------|------|-------|
| [Swarms](https://github.com/kyegomez/swarms) | 生产级多智能体基础设施平台 | ![Stars](https://img.shields.io/github/stars/kyegomez/swarms) |
| [Swarm](https://github.com/autoreason/swarm) | 轻量级多智能体编排框架 | ![Stars](https://img.shields.io/github/stars/autoreason/swarm) |
| [Swarm-Tools](https://github.com/FelipeDaza7/swarm-tools) | 协调具有学习能力的 AI 智能体的工具 | ![Stars](https://img.shields.io/github/stars/FelipeDaza7/swarm-tools) |

### 基于图的编排框架

| 项目 | 描述 | Stars |
|------|------|-------|
| [LangGraph](https://github.com/langchain-ai/langgraph) | 使用 LangChain 构建有状态的多智能体应用 | ![Stars](https://img.shields.io/github/stars/langchain-ai/langgraph) |
| [LangChain](https://github.com/langchain-ai/langchain) | 模块化 LLM 应用链接框架 | ![Stars](https://img.shields.io/github/stars/langchain-ai/langchain) |
| [LlamaIndex](https://github.com/jerryjliu/llama_index) | 以数据为中心的 RAG 智能体框架 | ![Stars](https://img.shields.io/github/stars/jerryjliu/llama_index) |
| [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | 微软面向 .NET/Python 的编排 SDK | ![Stars](https://img.shields.io/github/stars/microsoft/semantic-kernel) |

### 轻量级和专用智能体

| 项目 | 描述 | Stars |
|------|------|-------|
| [SmolAgents](https://github.com/smol-ai/smolagents) | 极简代码编写智能体库 | ![Stars](https://img.shields.io/github/stars/smol-ai/smolagents) |
| [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT) | 开创性的自主智能体 | ![Stars](https://img.shields.io/github/stars/Significant-Gravitas/Auto-GPT) |
| [BabyAGI](https://github.com/yoheinakajima/babyagi) | 简单的自主任务管理 | ![Stars](https://img.shields.io/github/stars/yoheinakajima/babyagi) |
| [GPT-Engineer](https://github.com/AntonOsika/gpt-engineer) | 根据规范生成完整项目的智能体 | ![Stars](https://img.shields.io/github/stars/AntonOsika/gpt-engineer) |
| [BMTools](https://github.com/OpenBMB/BMTools) | 智能体工具/API 注册表 | ![Stars](https://img.shields.io/github/stars/OpenBMB/BMTools) |

---

## 编排模式

### 层级式

在层级式编排中，主管智能体将任务委托给专业子智能体。这种模式适用于需要领域专业知识的复杂任务。

- **用例**：软件开发团队、研究自动化、企业工作流
- **框架**：AutoGen, CrewAI, LangGraph

### 顺序式

顺序工作流通过管道处理任务，每个智能体完成其步骤后再传递给下一个。

- **用例**：文档处理、数据转换管道
- **框架**：LangChain, LangGraph

### 并行/并发式

多个智能体同时处理独立子任务，之后汇总结果。

- **用例**：研究收集、并行代码生成
- **框架**：Swarms, AutoGen

### 混合专家模式 (MoA)

多个专家智能体贡献各自视角，通过迭代细化合并输出。

- **论文**：[混合专家模式论文](https://arxiv.org/abs/2406.04692)
- **实现**：Swarms MoA, LangGraph

### 智能体委员会

多个智能体讨论和辩论以达成共识。

- **用例**：决策、复杂分析、创意写作
- **框架**：AutoGen GroupChat

---

## 通信与协调

### 消息传递

- **Langroid**：基于消息传递的多智能体框架
- **AutoGen**：会话消息传递

### 共享状态/黑板系统

- **Swarm Matcher**：智能体匹配和选择
- **Message Pool**：共享通信系统

### 任务分配

- **Auto Swarm**：具有自动任务分配的自组织群体
- **Agent Delegation**：任务委托和管理

---

## 研究论文

### 多智能体协作

| 论文 | 描述 | 年份 |
|------|------|------|
| [CAMEL: 沟通智能体探索思维](https://arxiv.org/abs/2303.17760) | 通过对话进行角色扮演的智能体协作 | 2023 |
| [MetaGPT: 多智能体协作框架](https://arxiv.org/abs/2308.07370) | 软件开发中的智能体角色（产品经理、工程师、测试） | 2023 |
| [AgentVerse: 灵活的多智能体平台](https://arxiv.org/abs/2308.07429) | 模拟环境中的协作问题解决 | 2023 |
| [生成式智能体](https://arxiv.org/abs/2304.03442) | 虚拟世界中具有长期记忆的交互式智能体 | 2023 |
| [混合专家模式](https://arxiv.org/abs/2406.04692) | 并行处理与迭代细化 | 2024 |

### 编排与规划

| 论文 | 描述 | 年份 |
|------|------|------|
| [MALT: 多智能体 LLM 编排](https://arxiv.org/abs/2412.01928) | 创建者-验证者-优化器模式的结构化对话 | 2024 |
| [智能体即评判者](https://arxiv.org/abs/2410.10934) | 智能体评估其他智能体 | 2024 |
| [ReAct: 推理与行动的协同](https://arxiv.org/abs/2210.03629) | 交错思考和行动 | 2022 |

### 评估

| 基准 | 描述 |
|------|------|
| [AgentBench](https://arxiv.org/abs/2308.07258) | 在不同环境中评估智能体 |
| [多智能体评估](https://arxiv.org/abs/2312.04323) | 智能体评估指标综述 |

---

## 工具与基础设施

### 可观测性与追踪

| 工具 | 描述 |
|------|------|
| [Langfuse](https://github.com/langfuse/langfuse) | 开源 LLM 工程平台 |
| [Phoenix](https://github.com/Arize-ai/phoenix) | 开源 LLM 追踪 |
| [Opik](https://github.com/comet-ml/opik) | 开源 LLM 评估 |
| [Agenta](https://github.com/agenta-ai/agenta) | LLMOps 原型开发平台 |

### 记忆与知识

| 工具 | 描述 |
|------|------|
| [Memori](https://github.com/MemoriLabs/Memori) | LLM 和智能体的 SQL 原生记忆层 |
| [Letta](https://github.com/letta/letta) | AI 智能体的记忆层 |

---

## 学习资源

### 教程与指南

- [LLM 驱动的自主智能体](https://lilianweng.github.io/posts/2023-06-15-agent/) - Lilian Weng 的综合指南
- [提示工程指南：LLM 智能体](https://github.com/dair-ai/Prompt-Engineering-Guide#llm-agents) - 全面的智能体构建指南
- [使用 LangChain 构建自主智能体](https://www.youtube.com/watch?v=example) - 视频教程
- [企业级智能体课程](https://github.com/The-Swarm-Corporation/Enterprise-Grade-Agents-Course) - 综合课程

### 文档

- [AutoGen 文档](https://microsoft.github.io/autogen/) - 微软 AutoGen 文档
- [CrewAI 文档](https://docs.crewai.com/) - CrewAI 官方文档
- [LangGraph 文档](https://langchain-ai.github.io/langgraph/) - LangGraph 文档
- [Swarms 文档](https://docs.swarms.world/) - Swarms 框架文档

---

## 相关 Awesome 列表

- [awesome-ai-agents](https://github.com/heurema/awesome-ai-agents) - 综合 AI 智能体资源
- [awesome-LangGraph](https://github.com/von-development/awesome-LangGraph) - LangChain/LangGraph 生态系统
- [awesome-multi-agent-papers](https://github.com/kyegomez/awesome-multi-agent-papers) - 多智能体研究论文
- [awesome-Swarms-List](https://github.com/The-Swarm-Corporation/Awesome-Swarms-List) - Swarms 框架资源

---

## 贡献

欢迎贡献！请先阅读[贡献指南](CONTRIBUTING.md)。

1. Fork 本仓库
2. 在相应部分添加您的资源
3. 确保格式一致
4. 提交 Pull Request

---

## 许可证

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](LICENSE)

根据法律允许的范围，[您的名字](https://github.com/yourusername) 已放弃本作品的所有版权和相关权利。

---

*如果觉得有用，请给本仓库点个 Star！*
