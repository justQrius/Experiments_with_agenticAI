# Financial Research Crew

**Autonomous Financial Analysis System**

A CrewAI-powered research system for financial data analysis and market intelligence. Demonstrates web scraping, data synthesis, and autonomous report generation for investment research.

## Technical Stack

- **Framework**: CrewAI - Multi-agent orchestration
- **Python**: 3.10-3.13
- **Package Manager**: UV

## Architecture

Specialized financial research agents:
- **Data Collector**: Web scraping and information gathering
- **Analyst**: Financial data interpretation
- **Report Writer**: Research synthesis and documentation

Agent workflows configured for comprehensive market research.

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

Generates `output/report.md` with:
- Market analysis
- Company research
- Investment insights
- Data-driven recommendations

## Customization

- Research roles: `src/financial_researcher/config/agents.yaml`
- Analysis workflows: `src/financial_researcher/config/tasks.yaml`
- Research logic: `src/financial_researcher/crew.py`
- Query parameters: `src/financial_researcher/main.py`

## Resources

- [CrewAI Documentation](https://docs.crewai.com)
- [GitHub Repository](https://github.com/joaomdmoura/crewai)
