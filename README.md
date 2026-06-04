# Awesome AI Agents [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated map of the tools, frameworks, and ideas for building LLM-powered agents.

Agents are moving fast and the landscape is noisy. This is the list I wish I'd had when I started: the frameworks I actually reach for, the building blocks that matter (memory, retrieval, eval, observability), and the papers worth reading more than once.

Curated by [Leo Tavares](https://github.com/leotavares26). Contributions welcome — see [Contributing](#contributing).

## Contents

- [Frameworks &amp; orchestration](#frameworks--orchestration)
- [Memory &amp; state](#memory--state)
- [Retrieval (RAG)](#retrieval-rag)
- [Evaluation &amp; testing](#evaluation--testing)
- [Observability &amp; tracing](#observability--tracing)
- [Tooling &amp; protocols](#tooling--protocols)
- [Must-read papers](#must-read-papers)
- [Contributing](#contributing)

## Frameworks &amp; orchestration

| Project | Language | Notes |
| --- | --- | --- |
| [LangGraph](https://github.com/langchain-ai/langgraph) | Python / JS | Graph-based orchestration with explicit state. My default for anything stateful or cyclic. |
| [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) | Python | Lightweight agents, handoffs, and guardrails from OpenAI. |
| [CrewAI](https://github.com/crewAIInc/crewAI) | Python | Role-based multi-agent "crews" with a gentle learning curve. |
| [AutoGen](https://github.com/microsoft/autogen) | Python | Multi-agent conversations and a research-friendly programming model. |
| [LlamaIndex](https://github.com/run-llama/llama_index) | Python / TS | Data framework with strong agent + workflow primitives. |
| [Pydantic AI](https://github.com/pydantic/pydantic-ai) | Python | Type-safe agents with structured outputs, from the Pydantic team. |
| [DSPy](https://github.com/stanfordnlp/dspy) | Python | Program — don't prompt. Optimizes prompts/weights against metrics. |
| [Semantic Kernel](https://github.com/microsoft/semantic-kernel) | C# / Python / Java | Microsoft's SDK for planners and skills. |
| [Mastra](https://github.com/mastra-ai/mastra) | TypeScript | TS-native framework: agents, workflows, RAG, evals. |

## Memory &amp; state

| Project | Notes |
| --- | --- |
| [Letta (MemGPT)](https://github.com/letta-ai/letta) | Stateful agents with long-term memory and a memory-management OS metaphor. |
| [Mem0](https://github.com/mem0ai/mem0) | A memory layer you can drop into existing agents. |
| [Zep](https://github.com/getzep/zep) | Long-term memory + retrieval for conversational agents. |

## Retrieval (RAG)

| Project | Notes |
| --- | --- |
| [pgvector](https://github.com/pgvector/pgvector) | Vector search inside Postgres. Boring, reliable, my default. |
| [Qdrant](https://github.com/qdrant/qdrant) | Fast vector DB with rich filtering. |
| [Chroma](https://github.com/chroma-core/chroma) | Easy local-first vector store for prototyping. |
| [RAGAS](https://github.com/explodinggradients/ragas) | Metrics specifically for evaluating RAG pipelines. |

## Evaluation &amp; testing

| Project | Notes |
| --- | --- |
| [DeepEval](https://github.com/confident-ai/deepeval) | Pytest-style assertions for LLM outputs. |
| [promptfoo](https://github.com/promptfoo/promptfoo) | Test, compare, and red-team prompts and models. |
| [TruLens](https://github.com/truera/trulens) | Feedback functions to score agent behavior. |

## Observability &amp; tracing

| Project | Notes |
| --- | --- |
| [Langfuse](https://github.com/langfuse/langfuse) | Open-source tracing, evals, and prompt management. |
| [Phoenix (Arize)](https://github.com/Arize-ai/phoenix) | OpenTelemetry-based tracing and eval for LLM apps. |
| [OpenLLMetry](https://github.com/traceloop/openllmetry) | OpenTelemetry instrumentation for LLM stacks. |

## Tooling &amp; protocols

| Project | Notes |
| --- | --- |
| [Model Context Protocol (MCP)](https://github.com/modelcontextprotocol) | Open protocol for connecting models to tools and data. |
| [Instructor](https://github.com/567-labs/instructor) | Structured outputs from LLMs via Pydantic. |
| [LiteLLM](https://github.com/BerriAI/litellm) | One API across 100+ model providers. |

## Must-read papers

- **ReAct: Synergizing Reasoning and Acting in Language Models** — Yao et al., 2022. The reason-act-observe loop that underpins most tool-using agents.
- **Reflexion: Language Agents with Verbal Reinforcement Learning** — Shinn et al., 2023. Self-reflection as a learning signal.
- **Toolformer: Language Models Can Teach Themselves to Use Tools** — Schick et al., 2023.
- **Generative Agents: Interactive Simulacra of Human Behavior** — Park et al., 2023. Memory, reflection, and planning in a simulated town.
- **MemGPT: Towards LLMs as Operating Systems** — Packer et al., 2023. Treating context as a managed memory hierarchy.
- **Voyager: An Open-Ended Embodied Agent with LLMs** — Wang et al., 2023. Skill libraries and lifelong learning.
- **Tree of Thoughts: Deliberate Problem Solving with LLMs** — Yao et al., 2023.

## Contributing

Found something great that's missing? Open a PR. Keep entries actively maintained and genuinely useful — quality over quantity. One line on *why* it earns a spot goes a long way.

## License

[CC0 1.0](LICENSE) — to the extent possible under law, the contributors have waived all copyright to this list.
