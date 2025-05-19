# AI Engineering Team

**Collaborative Software Engineering Agents**

A CrewAI system simulating a complete software engineering team with specialized roles: Product Manager, Architect, Developer, and QA Engineer. Demonstrates end-to-end software development workflows through agent collaboration.

## Technical Stack

- **Framework**: CrewAI - Multi-agent orchestration
- **Python**: 3.10-3.13
- **Package Manager**: UV

## Architecture

Multi-role agent team for software development:
- **Product Manager**: Requirements analysis
- **Software Architect**: System design
- **Developer**: Implementation
- **QA Engineer**: Testing and validation

Configuration files define agent behaviors and task workflows.

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

Generates software engineering artifacts:
- Design documents (e.g., `accounts.py_design.md`)
- Implementation plans
- Code reviews
- Test strategies

Outputs stored in `output/` or `example_output_*/` directories.

## Customization

- Agent roles: `src/engineering_team/config/agents.yaml`
- Development workflows: `src/engineering_team/config/tasks.yaml`
- Team logic: `src/engineering_team/crew.py`
- Project parameters: `src/engineering_team/main.py`

## Resources

- [CrewAI Documentation](https://docs.crewai.com)
- [GitHub Repository](https://github.com/joaomdmoura/crewai)
