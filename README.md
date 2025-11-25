# Deep Research Clone

This project implements multi-agent AI teams using **AutoGen** and **Google Gemini** models. It features a "Deep Research Team" for conducting comprehensive web research and an "Email Optimizer Team" for refining communications.

## Features

- **Deep Research Team**: A squad of agents (Planner, Researcher, Analyst, Reviewer) that autonomously plans research, searches the web, and compiles detailed reports.
- **Email Optimizer Team**: A team of agents (Clarity, Tone, Persuasion, Critic) that collaborates to improve email drafts.
- **Google Gemini Integration**: Powered by `gemini-2.5-flash` for high-performance and cost-effective reasoning.
- **Web Search**: Integrated with **Firecrawl** for advanced web scraping and search capabilities.
- **Report Generation**: Automatically saves research findings to Markdown files.

## Prerequisites

- **Python**: >= 3.13
- **Package Manager**: [uv](https://github.com/astral-sh/uv) (recommended)
- **API Keys**:
  - [Google Gemini API Key](https://aistudio.google.com/)
  - [Firecrawl API Key](https://firecrawl.dev/)

## Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd deep-research-clone
   ```

2. **Install dependencies using `uv`:**
   ```bash
   uv sync
   ```
   Or using pip:
   ```bash
   pip install .
   ```

## Configuration

1. Create a `.env` file in the root directory:
   ```bash
   touch .env
   ```

2. Add your API keys to `.env`:
   ```env
   GEMINI_API_KEY=your_gemini_api_key_here
   FIRECRAWL_API_KEY=your_firecrawl_api_key_here
   ```

## Usage

### Deep Research Team
1. Open `deep-research-team.ipynb` in Jupyter Lab or VS Code.
2. Run the cells to initialize the agents.
3. The team will execute the research task defined in the last cell (default: "Research about the new development in Nuclear Energy").
4. The final report will be saved to `report.md`.

### Email Optimizer Team
1. Open `email-optimizer-team.ipynb`.
2. Run the cells to start the email optimization process.

## Project Structure

- `deep-research-team.ipynb`: Main notebook for the research agent team.
- `email-optimizer-team.ipynb`: Notebook for the email optimization team.
- `tools.py`: Custom tools for web search and file operations.
- `report.md`: Output file for research reports.
- `.project_rules.md`: Project-specific rules and conventions (e.g., commit messages).

## License

[Add License Here]
