# CrewAI — Multi-Agent Crews

## Overview

- **Purpose:** Demonstrate modular multi-agent tooling for market research and content generation, suitable for interviews and technical portfolios.
- **Contents:** Two crew packages with tools, configs, and example entry points to run standalone crew workflows.

## Key Features

- Modular Python packages for crew orchestration
- Config-driven agents and tasks (YAML in each crew)
- Example tools and extensible utilities under `src/*/tools`
- Ready to extend for production or demo scenarios

## Tech Stack

- Python 3.10+
- Standard packaging via `pyproject.toml` in each crew folder
- YAML for configuration

## Quickstart (Windows)

1. Create and activate a virtual environment

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install --upgrade pip
```

2. Install the crew packages in editable mode

```powershell
pip install -e ./market_research_crew
pip install -e ./research_and_blog_crew
```

3. Run an example crew entry point

```powershell
python -m market_research_crew.main
python -m research_and_blog_crew.main
```

If a module import fails, check the package name under `src/` (there may be a minor folder/package name discrepancy to correct before running).

## Repository Structure

- `market_research_crew/` — market research crew package and config
- `research_and_blog_crew/` — research & blog crew package and config
- `resources/` — supporting assets (e.g., masterclass HTML)

Inside each crew package:

- `src/<package>/` — Python package sources
- `config/agents.yaml` — agent definitions
- `config/tasks.yaml` — task definitions
- `tools/` — custom utilities and helpers

## How to Use (for placement demos)

- Fork the repo and add a small demo script that shows an end-to-end flow (input → crew run → output). Keep the demo under `reports/` or `blogs/`.
- Record a short (2–3 minute) screencast walking through running the crew and explaining design decisions.

## Contributing

- Open an issue or submit a pull request. Keep changes focused and add tests or example runs when applicable.

## License

Specify your preferred license here (e.g., MIT). If none chosen, add a `LICENSE` file.

## Contact

Project owner: add your name and email or a link to your portfolio/GitHub profile.

