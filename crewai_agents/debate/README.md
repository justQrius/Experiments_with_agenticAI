# AI Debate System

**Multi-Agent Deliberative Reasoning**

A CrewAI system demonstrating adversarial agent collaboration for decision-making through structured debate. Agents propose, oppose, and synthesize arguments to reach informed conclusions.

## Technical Stack

- **Framework**: CrewAI - Multi-agent orchestration
- **Python**: 3.10-3.13
- **Package Manager**: UV

## Architecture

Specialized agents engage in structured debate workflows:
- **Proposer**: Generates initial arguments
- **Opposer**: Provides counterarguments
- **Synthesizer**: Integrates perspectives
- Configuration: `config/agents.yaml`, `config/tasks.yaml`

## Setup

```bash
pip install uv
crewai install
# Configure OPENAI_API_KEY in .env
```

## Usage

```bash
crewai run
```

## Output

Generates debate outputs in `output/`:
- `propose.md`: Initial arguments
- `oppose.md`: Counterarguments
- `decide.md`: Final synthesis

## Customization

- Agent roles: `src/debate/config/agents.yaml`
- Debate structure: `src/debate/config/tasks.yaml`
- Logic: `src/debate/crew.py`
- Parameters: `src/debate/main.py`

## Resources

- [CrewAI Documentation](https://docs.crewai.com)
- [GitHub Repository](https://github.com/joaomdmoura/crewai)
