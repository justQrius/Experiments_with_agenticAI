# AI Code Generation Crew

**Multi-Agent System for Autonomous Code Generation**

A CrewAI-powered system demonstrating collaborative AI agents for software development tasks. This project showcases agent orchestration, task delegation, and autonomous code generation workflows.

## Technical Stack

- **Framework**: [CrewAI](https://crewai.com) - Multi-agent orchestration
- **Python**: 3.10-3.13
- **Package Manager**: [UV](https://docs.astral.sh/uv/)

## Architecture

Multiple specialized AI agents collaborate on code generation tasks:
- Agent roles, goals, and capabilities defined in `config/agents.yaml`
- Task workflows specified in `config/tasks.yaml`
- Custom logic and tools implemented in `crew.py`

## Setup

```bash
# Install UV package manager
pip install uv

# Install dependencies
crewai install

# Configure environment
# Add OPENAI_API_KEY to .env file
```

## Usage

```bash
# Execute crew from project root
crewai run
```

## Output

Generates a `report.md` with research findings on LLMs and related topics.

## Customization

- Agent definitions: `src/coder/config/agents.yaml`
- Task configuration: `src/coder/config/tasks.yaml`
- Business logic: `src/coder/crew.py`
- Input parameters: `src/coder/main.py`

## Resources

- [CrewAI Documentation](https://docs.crewai.com)
- [GitHub Repository](https://github.com/joaomdmoura/crewai)
