# Agentic AI Engineering - Implementations & Research

A comprehensive implementation portfolio exploring the cutting edge of autonomous AI agents and multi-agent systems. This repository demonstrates proficiency in building stateful, collaborative AI systems using modern frameworks including OpenAI, CrewAI, LangGraph, AutoGen, and the Model Context Protocol.

## Key Skills Demonstrated

- **Agent Architecture**: Custom ReAct loops, tool integration, autonomous reasoning systems
- **Multi-Agent Orchestration**: Team-based collaboration, hierarchical agents, distributed problem solving
- **Stateful Workflows**: Persistent memory, checkpointing, state management with LangGraph
- **Protocol Implementation**: Full Model Context Protocol servers, standardized tool interfaces
- **Production Patterns**: Human-in-the-loop workflows, error handling, real-world deployment strategies
- **Framework Expertise**: OpenAI Assistants API, CrewAI, LangGraph, AutoGen, MCP

## Implementation Overview

### [Module 1: Foundations](foundations/)
**Focus**: Core agent architecture and reasoning patterns

- **[01_ai_fundamentals.ipynb](foundations/01_ai_fundamentals.ipynb)**: LLM basics, API integration, prompt engineering fundamentals
- **[02_prompt_engineering_patterns.ipynb](foundations/02_prompt_engineering_patterns.ipynb)**: Chain-of-thought, few-shot learning, structured prompting
- **[03_function_calling_systems.ipynb](foundations/03_function_calling_systems.ipynb)**: Tool use patterns, function schemas, parameter extraction
- **[04_autonomous_agents_intro.ipynb](foundations/04_autonomous_agents_intro.ipynb)**: Building a ReAct agent from scratch, reasoning loops, autonomous decision-making

**Key Achievement**: Implemented a custom ReAct reasoning loop without frameworks, demonstrating deep understanding of agent fundamentals

**Tech Stack**: OpenAI API, Python, function calling patterns

---

### [Module 2: OpenAI Advanced Features](openai_experiments/)
**Focus**: Leveraging OpenAI's specialized APIs and capabilities

- **[01_api_integration.ipynb](openai_experiments/01_api_integration.ipynb)**: Advanced API patterns, streaming, error handling
- **[02_structured_outputs.ipynb](openai_experiments/02_structured_outputs.ipynb)**: JSON mode, Pydantic schemas, validated output generation
- **[03_assistants_api_deep_dive.ipynb](openai_experiments/03_assistants_api_deep_dive.ipynb)**: Threads, runs, file handling, code interpreter integration
- **[04_vision_and_audio.ipynb](openai_experiments/04_vision_and_audio.ipynb)**: Multi-modal analysis, image understanding, audio transcription

**Includes**: [deep_research](openai_experiments/deep_research/) - Extended research project exploring advanced OpenAI capabilities

**Key Achievement**: Built multi-modal analysis pipeline combining vision, audio, and text processing

**Tech Stack**: OpenAI API (GPT-4, Vision, Whisper), Assistants API, Pydantic

---

### [Module 3: CrewAI Multi-Agent Systems](crewai_agents/)
**Focus**: Role-based agent orchestration and team collaboration

#### **[Code Generation Crew](crewai_agents/coder/)**
Multi-agent system for autonomous software development. Demonstrates collaborative code generation, task delegation, and quality control.

#### **[Debate System](crewai_agents/debate/)**
Adversarial reasoning through structured debate. Agents propose arguments, generate counterarguments, and synthesize conclusions through deliberative collaboration.

**Outputs**: `propose.md`, `oppose.md`, `decide.md` - Complete debate workflow

#### **[Engineering Team](crewai_agents/engineering_team/)**
Simulates a complete software engineering team with specialized roles:
- Product Manager: Requirements analysis
- Software Architect: System design
- Developer: Implementation
- QA Engineer: Testing and validation

**Outputs**: Design documents, implementation plans, code reviews, test strategies

#### **[Financial Research](crewai_agents/financial_researcher/)**
Autonomous financial analysis system with web scraping, data synthesis, and comprehensive report generation for investment research.

**Outputs**: `output/report.md` - Market analysis and investment insights

#### **[Stock Selection System](crewai_agents/stock_picker/)**
AI-powered investment engine combining:
- Fundamental analysis (financial statements)
- Technical analysis (chart patterns, indicators)
- Sentiment analysis (news, social media)
- Portfolio management (risk assessment)

**Outputs**: `output/decision.md`, `report.md` - Data-driven stock recommendations

**Key Achievement**: Deployed production-ready multi-agent systems for complex domain-specific tasks (finance, software engineering, research)

**Tech Stack**: CrewAI, OpenAI API, UV package management, YAML configuration

---

### [Module 4: LangGraph Stateful Workflows](langgraph_workflows/)
**Focus**: Building cyclic, stateful agent systems with persistence

- **[01_state_graph_basics.ipynb](langgraph_workflows/01_state_graph_basics.ipynb)**: Graph construction, nodes, edges, state management
- **[02_persistence_and_memory.ipynb](langgraph_workflows/02_persistence_and_memory.ipynb)**: Checkpointing, state recovery, conversation memory
- **[03_human_in_the_loop.ipynb](langgraph_workflows/03_human_in_the_loop.ipynb)**: Approval workflows, interrupts, user interaction patterns
- **[04_multi_agent_collaboration.ipynb](langgraph_workflows/04_multi_agent_collaboration.ipynb)**: Agent coordination, message passing, collaborative problem-solving

**Includes**:
- [Sidekick Application](langgraph_workflows/sidekick.py) - Production assistant with persistent memory
- [sandbox](langgraph_workflows/sandbox/) - Experimental workflow implementations

**Key Achievement**: Implemented production-ready human-in-the-loop approval system for sensitive operations (deployments, financial transactions)

**Tech Stack**: LangGraph, LangChain, SQLite checkpointing, state graphs

---

### [Module 5: AutoGen Conversable Agents](autogen_systems/)
**Focus**: Distributed agent communication and group collaboration

- **[01_conversable_agents.ipynb](autogen_systems/01_conversable_agents.ipynb)**: Agent communication patterns, message protocols
- **[02_group_chat_manager.ipynb](autogen_systems/02_group_chat_manager.ipynb)**: Multi-agent conversations, turn-taking, orchestration
- **[03_coding_agents.ipynb](autogen_systems/03_coding_agents.ipynb)**: Code generation with execution, testing, debugging workflows
- **[04_distributed_systems.ipynb](autogen_systems/04_distributed_systems.ipynb)**: Scalable agent architectures, distributed problem solving

**Supporting Implementation**:
- [agent.py](autogen_systems/agent.py) - Custom agent implementations
- [messages.py](autogen_systems/messages.py) - Message handling and protocols
- [world.py](autogen_systems/world.py) - Shared environment management
- [sandbox](autogen_systems/sandbox/) - Testing environments

**Key Achievement**: Built distributed coding system where agents autonomously generate, test, and debug code through group collaboration

**Tech Stack**: AutoGen, OpenAI API, distributed systems patterns

---

### [Module 6: Model Context Protocol](mcp_protocol/)
**Focus**: Standardized tool interfaces and resource management

- **[01_mcp_server_basics.ipynb](mcp_protocol/01_mcp_server_basics.ipynb)**: MCP architecture, server implementation, protocol fundamentals
- **[02_mcp_client_implementation.ipynb](mcp_protocol/02_mcp_client_implementation.ipynb)**: Client-server communication, connection management
- **[03_resource_management.ipynb](mcp_protocol/03_resource_management.ipynb)**: Exposing resources, access control, data sharing
- **[04_prompt_templates.ipynb](mcp_protocol/04_prompt_templates.ipynb)**: Dynamic prompt generation, template systems
- **[05_tool_integration.ipynb](mcp_protocol/05_tool_integration.ipynb)**: Tool registration, invocation, result handling

**Production Implementations**:

#### **[Accounts Server](mcp_protocol/accounts_server.py)**
Full MCP server exposing database operations for account management. Demonstrates secure resource access and CRUD operations.

**Components**: `accounts.py`, `accounts_client.py`, `database.py`

#### **[Market Data Server](mcp_protocol/market_server.py)**
Real-time market data access via MCP. Integrates with financial APIs and exposes standardized market information endpoints.

**Components**: `market.py`, `traders.py`, `trading_floor.py`

#### **[Push Notification Server](mcp_protocol/push_server.py)**
Event-driven notification system demonstrating asynchronous MCP patterns.

**Supporting Infrastructure**:
- [templates.py](mcp_protocol/templates.py) - Prompt template management
- [tracers.py](mcp_protocol/tracers.py) - Request tracing and debugging
- [util.py](mcp_protocol/util.py) - Shared utilities
- [sandbox](mcp_protocol/sandbox/) - Testing and experimentation

**Key Achievement**: Designed and deployed custom MCP servers exposing databases, APIs, and file systems through standardized interfaces - positioning for the future of AI-tool interoperability

**Tech Stack**: Model Context Protocol, FastAPI/Starlette, SQLite, async Python

---

## Technologies & Frameworks

**AI Platforms**: OpenAI (GPT-4, GPT-4 Vision, Whisper), Anthropic (Claude)

**Agent Frameworks**: CrewAI, LangGraph, LangChain, AutoGen, OpenAI Swarm

**Protocols**: Model Context Protocol (MCP), OpenAI Assistants API

**Infrastructure**: FastAPI, Starlette, SQLite, async Python, Docker

**Tools**: UV (package management), Jupyter, Python 3.12+

---

## Key Projects Summary

| Project | Module | Technologies | Achievement |
|---------|--------|--------------|-------------|
| **Custom ReAct Agent** | Foundations | OpenAI, Python | Built agent reasoning loop from scratch |
| **Multi-Modal Analysis** | OpenAI | Vision, Whisper, GPT-4 | Integrated vision, audio, and text processing |
| **Engineering Team Crew** | CrewAI | CrewAI, YAML configs | 4-agent software development team |
| **Stock Selection Engine** | CrewAI | CrewAI, Financial APIs | Multi-dimensional investment analysis |
| **Human-in-the-Loop Workflow** | LangGraph | LangGraph, Checkpointing | Production approval system for sensitive operations |
| **Sidekick Assistant** | LangGraph | LangGraph, SQLite | Persistent memory conversation agent |
| **Distributed Coding System** | AutoGen | AutoGen, Group Chat | Autonomous code generation and debugging |
| **Accounts MCP Server** | MCP Protocol | MCP, FastAPI, SQLite | Standardized database access interface |
| **Market Data Server** | MCP Protocol | MCP, Financial APIs | Real-time market data via MCP |

---

## Skills Progression

**Module 1-2**: Core concepts, API mastery, prompt engineering, function calling
**Module 3**: Multi-agent orchestration, role-based collaboration, domain expertise
**Module 4**: Stateful workflows, persistence, production patterns
**Module 5**: Distributed systems, group collaboration, autonomous coding
**Module 6**: Protocol implementation, standardization, future-ready architecture

---

## Repository Structure

Each module contains:
- **Jupyter notebooks**: Detailed implementations with documentation
- **Supporting Python modules**: Production-ready code and utilities
- **Project folders**: Complete applications with READMEs and outputs
- **Sandbox directories**: Experimental implementations and testing

---

## Getting Started

**Prerequisites**:
- Python 3.12 or higher
- OpenAI API key
- (Optional) UV package manager for faster dependency resolution

**Installation**:
```bash
# Clone the repository
git clone https://github.com/yourusername/experiments_with_agenticAI.git
cd experiments_with_agenticAI

# Install dependencies
pip install -r requirements.txt

# Or using UV for faster installation
pip install uv
uv pip install -r requirements.txt
```

**Configuration**:
Create a `.env` file in the root directory:
```
OPENAI_API_KEY=your_openai_key_here
ANTHROPIC_API_KEY=your_anthropic_key_here
```

**Running Projects**:

*Jupyter Notebooks:*
```bash
jupyter notebook
# Navigate to any module and open notebooks
```

*CrewAI Projects:*
```bash
cd crewai_agents/stock_picker
crewai install
crewai run
```

*LangGraph Applications:*
```bash
cd langgraph_workflows
python sidekick.py
```

*MCP Servers:*
```bash
cd mcp_protocol
python accounts_server.py
```

---

## Notable Implementations

### Human-in-the-Loop Approval System
Production-ready workflow pattern for enterprise AI deployment. Pauses execution before sensitive operations (deployments, payments, data deletions) for human review and approval. Demonstrates critical safety patterns for autonomous systems.

**Location**: `langgraph_workflows/03_human_in_the_loop.ipynb`

### Multi-Agent Debate System
Deliberative reasoning through structured adversarial collaboration. Agents propose arguments, generate counterarguments, and synthesize balanced conclusions. Demonstrates how multiple perspectives improve decision quality.

**Location**: `crewai_agents/debate/`

### Custom MCP Protocol Servers
Future-ready standardized interfaces for AI-tool interoperability. Multiple production servers exposing databases, APIs, and resources through the emerging Model Context Protocol standard.

**Location**: `mcp_protocol/`

---

**Note**: This repository represents a comprehensive exploration of modern agentic AI systems, progressing from fundamental concepts to production-ready, protocol-standardized implementations. Each module builds upon previous work, demonstrating both theoretical understanding and practical engineering capability.
