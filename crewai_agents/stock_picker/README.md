# Stock Selection System

**AI-Powered Investment Decision Engine**

A CrewAI system for autonomous stock analysis and selection. Combines fundamental analysis, technical indicators, and market sentiment to generate data-driven investment recommendations.

## Technical Stack

- **Framework**: CrewAI - Multi-agent orchestration
- **Python**: 3.10-3.13
- **Package Manager**: UV

## Architecture

Investment analysis agent team:
- **Fundamental Analyst**: Financial statement analysis
- **Technical Analyst**: Chart patterns and indicators
- **Sentiment Analyst**: News and social media analysis
- **Portfolio Manager**: Risk assessment and final selection

Multi-dimensional analysis for informed decision-making.

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

Generates investment analysis documents:
- `output/decision.md`: Final stock selections with rationale
- `report.md`: Comprehensive analysis report
- Technical indicators, risk assessments, and recommendations

## Customization

- Analyst agents: `src/stock_picker/config/agents.yaml`
- Analysis workflows: `src/stock_picker/config/tasks.yaml`
- Decision logic: `src/stock_picker/crew.py`
- Input parameters: `src/stock_picker/main.py`

## Resources

- [CrewAI Documentation](https://docs.crewai.com)
- [GitHub Repository](https://github.com/joaomdmoura/crewai)
