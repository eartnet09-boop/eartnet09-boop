# Expedito

### AI Orchestrator | DevSecOps | Software Engineer

I translate product vision into secure software by combining product thinking, sound architecture, and AI-assisted engineering. I build practical, privacy-conscious systems and orchestrate AI agents to accelerate delivery while keeping technical decisions and quality accountable.

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)](https://www.langchain.com/langgraph)
[![Ollama](https://img.shields.io/badge/Ollama-111111?style=flat-square)](https://ollama.com/)
[![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)](https://www.prisma.io/)

## Product Vision, Engineered

I shape product ideas into architectures, roadmaps, and clear engineering constraints. I then coordinate AI tools and agents through well-defined tasks, review their output, and integrate the results into cohesive software. This model combines the speed of AI-assisted development with human ownership of product direction, security, and quality.

```mermaid
graph TD
	subgraph ARCHITECT["PRODUCT ARCHITECTURE"]
		direction TB
		Vision["Product Vision & Architecture"]
		Review["Human-in-the-Loop<br/>Review & Approval"]
		Vision -. "defines scope & acceptance criteria" .-> Review
	end

	subgraph ORCHESTRATION["ORCHESTRATION LAYER"]
		direction TB
		Prompt["Prompt Engineering<br/>& Context"]
		LangGraph["LangGraph<br/>(State Machine)"]
		Prompt --> LangGraph
	end

	subgraph AGENTS["AI ENGINEERING TEAM"]
		direction TB
		LLM["Local LLMs<br/>(Ollama / Qwen)"]
		RAG["RAG<br/>(Knowledge Base)"]
		Execution["Code Generation<br/>& Task Execution"]
		LLM --> Execution
		RAG --> Execution
	end

	subgraph GUARDRAILS["SECURITY GUARDRAILS"]
		direction TB
		Security["DevSecOps<br/>(NIST / OWASP)"]
		Validation["Continuous Validation"]
		Security --> Validation
	end

	Vision --> Prompt
	LangGraph --> LLM
	LangGraph --> RAG
	Execution --> Security
	Validation --> Review
	Review -->|"approved"| Deploy["Approved Deployment"]
	Review -.->|"changes requested"| Prompt
	Security -.->|"security findings"| Prompt
	Validation -.->|"validation failures"| Prompt

	Deploy --> LexiQuest["LexiQuest"]
	Deploy --> NERO["NERO"]
	Deploy --> TeacherPro["TEACHER.PRO"]

	classDef architect fill:#2d3748,stroke:#718096,color:#f7fafc,stroke-width:1px;
	classDef human fill:#1d4ed8,stroke:#93c5fd,color:#eff6ff,stroke-width:2px;
	classDef orchestration fill:#0f766e,stroke:#5eead4,color:#f0fdfa,stroke-width:1px;
	classDef ai fill:#1c3c3c,stroke:#4fd1c5,color:#e6fffa,stroke-width:1px;
	classDef security fill:#7f1d1d,stroke:#ef4444,color:#fff7ed,stroke-width:2px;
	classDef output fill:#334155,stroke:#94a3b8,color:#f8fafc,stroke-width:1px;

	class Vision architect;
	class Review human;
	class Prompt,LangGraph orchestration;
	class LLM,RAG,Execution ai;
	class Security,Validation security;
	class Deploy,LexiQuest,NERO,TeacherPro output;
```

*Orchestration Model: Human-led architecture and approval, AI-driven execution, and layered DevSecOps guardrails from vision to deployment.*

## Core Skills & Orchestration Stack

| Capability | How it works | Orchestration value |
| --- | --- | --- |
| **Agentic Workflows (LangGraph)** | Represents agent workflows as stateful graphs: nodes perform work, edges define transitions, and shared state carries context. | Provides the control flow for tool use, branching, and multi-step execution, enabling bounded autonomy with explicit checkpoints. |
| **Local LLMs & Privacy (Ollama, Qwen)** | Runs models locally using tools such as Ollama, including Qwen model families. | Keeps data processing under local control, can reduce inference costs depending on hardware and workload, and limits dependence on a single hosted provider. |
| **RAG (Retrieval-Augmented Generation)** | Retrieves relevant material from a selected knowledge base and supplies it to the model at query time. | Grounds responses in domain sources, makes results easier to verify, and helps mitigate unsupported generations. |
| **Prompt Engineering & Context Management** | Defines agent roles, task instructions, constraints, tools, and the information available at each step. | Functions as the management layer for AI agents: clear scope and context improve consistency, output quality, and reviewability. |
| **Full-Stack Engineering (Next.js, FastAPI, Python)** | Connects interfaces, APIs, data, and model capabilities into complete applications. | Provides the robust product environment where agents can support real workflows and AI capabilities become maintainable user experiences. |
| **DevSecOps & Security (NIST, OWASP)** | Applies secure design, threat modeling, testing, and recognized security guidance across the development lifecycle. | Integrates security early and supports systems that are more resilient, auditable, and aligned with relevant standards and requirements. |

## Featured Projects

- **LexiQuest (E.IA)** — An EdTech SaaS for spaced-repetition learning (SRS), built around a Next.js and Prisma architecture. AI orchestration supports product planning and coordinated implementation.
- **NERO** — A local-first autonomous agent for tax automation, using LangGraph to structure workflows and Ollama to run local models.
- **TEACHER.PRO** — A local English tutor combining Whisper, WavLM, and Qwen for speech transcription, phonetic analysis, and personalized practice.
- **Security Guides** — Technical documentation and threat-intelligence mapping across NIST guidance, STIGs, CVEs, and security protocols.

## Connect

- **GitHub:** [@eartnet09-boop](https://github.com/eartnet09-boop)

<!-- Add verified LinkedIn and professional email links here when available. -->
