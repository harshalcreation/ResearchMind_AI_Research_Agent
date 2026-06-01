# ResearchMind AI Research Agent

ResearchMind is a Multi-Agent AI Research System that automates the complete research workflow using specialized AI agents. The system searches the web, extracts relevant information, generates a detailed research report, and critiques the final output to ensure quality.

## Features

* Multi-Agent Architecture
* Real-time Web Search using Tavily
* Website Content Scraping using BeautifulSoup
* AI-Powered Research Report Generation
* Automated Report Critique & Scoring
* Interactive Streamlit User Interface
* LangGraph Agent Orchestration
* Mistral AI Integration

## System Workflow

### 1. Search Agent

* Searches the web for recent and reliable information.
* Collects relevant sources, URLs, and snippets.

### 2. Reader Agent

* Scrapes selected websites.
* Extracts meaningful textual content for deeper analysis.

### 3. Writer Chain

* Synthesizes gathered information.
* Produces a structured research report.

### 4. Critic Chain

* Reviews the generated report.
* Identifies strengths and weaknesses.
* Provides a quality score and improvement suggestions.

## Architecture

```text
User Query
    │
    ▼
Search Agent
    │
    ▼
Reader Agent
    │
    ▼
Writer Chain
    │
    ▼
Critic Chain
    │
    ▼
Final Research Report
```

## Tech Stack

### Frontend

* Streamlit

### AI & Agent Framework

* LangChain
* LangGraph
* Mistral AI

### Web Intelligence

* Tavily Search API
* Requests
* BeautifulSoup4

### Utilities

* Python
* Dotenv
* Rich

## Project Structure

```text
ResearchMind_AI_Research_Agent/
│
├── app.py
├── agents.py
├── tools.py
├── requirements.txt
├── .env
└── README.md
```

## Installation

### Clone Repository

```bash
git clone https://github.com/harshalcreation/ResearchMind_AI_Research_Agent.git

cd ResearchMind_AI_Research_Agent
```

### Create Virtual Environment

```bash
python -m venv venv
```

Activate Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

## Environment Variables

Create a `.env` file in the root directory.

```env
MISTRAL_API_KEY=your_mistral_api_key
TAVILY_API_KEY=your_tavily_api_key
GOOGLE_API_KEY=your_google_api_key
HF_TOKEN=your_huggingface_token
```

## Run Application

```bash
streamlit run app.py
```

## Example Output

The system generates:

* Search Results
* Scraped Website Content
* Detailed Research Report
* Critic Feedback & Score

### Sample Critic Output

```text
Score: 8/10

Strengths:
- Comprehensive coverage
- Well-structured report

Areas to Improve:
- Add quantitative evidence
- Improve citation consistency

Verdict:
Informative and well-organized research report.
```

## Future Improvements

* PDF Report Export
* Research Report Citation Generator
* Multi-LLM Support (Gemini, OpenAI, Claude)
* Research Memory & Knowledge Base
* RAG Integration
* Research Report Visualization
* Voice-based Research Queries
* Research Trend Analysis

## Deployment

### Streamlit Cloud

1. Push project to GitHub.
2. Connect repository to Streamlit Cloud.
3. Add secrets:

```toml
MISTRAL_API_KEY="your_key"
TAVILY_API_KEY="your_key"
GOOGLE_API_KEY="your_key"
HF_TOKEN="your_key"
```

4. Deploy.

## Author

Harshal Borkar

* Software Engineer
* Data Science Enthusiast
* AI & GenAI Developer

## License

This project is licensed under the MIT License.
