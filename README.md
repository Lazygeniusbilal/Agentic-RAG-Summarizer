# AI Researcher Paper Assistant

AI Researcher Paper Assistant is an intelligent research workflow tool that leverages the latest in LLMs and agentic graph orchestration to automate the process of finding, summarizing, and reporting on cutting-edge research papers from arXiv.

## Features

- **Automated Keyword Extraction:** Extracts relevant keywords from your research query using LLMs.
- **arXiv Integration:** Searches arXiv for the most relevant papers based on extracted keywords.
- **PDF Retrieval & Parsing:** Downloads and extracts text from research paper PDFs.
- **LLM-Powered Summarization:** Summarizes the content of papers and provides real-world application examples.
- **Beautiful PDF Report Generation:** Generates a well-formatted PDF summary report for easy sharing.
- **Agentic Workflow:** Modular, graph-based pipeline using [LangGraph](https://github.com/langchain-ai/langgraph) and [LangChain](https://github.com/langchain-ai/langchain).

## How It Works

1. **User Query:** Enter a research question (e.g., "How are Vision Transformers better than previous Vision models?").
2. **Keyword Extraction:** The system extracts a concise keyword for searching arXiv.
3. **Paper Retrieval:** The most relevant paper is fetched from arXiv and its PDF is downloaded.
4. **Summarization:** The paper is summarized and a real-world application is generated.
5. **PDF Report:** A polished PDF report is created and saved.

## Example Output

![PDF Example](notebooks/Summarized_Report.pdf)

## Quickstart

### 1. Clone the Repository

```sh
git clone https://github.com/yourusername/ai-researcher-paper-assistant.git
cd ai-researcher-paper-assistant
```

### 2. Install Dependencies

It is recommended to use a virtual environment.

```sh
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Set Up API Keys

Create a `.env` file in the root directory and add your OpenAI API key:

```
OPENAI_API_KEY=your-openai-api-key
```

### 4. Run the Notebook

Open [notebooks/Agentic_Rag.ipynb](notebooks/Agentic_Rag.ipynb) in VS Code or Jupyter and run all cells.

## Project Structure

```
.
├── .env
├── requirements.txt
├── notebooks/
│   ├── Agentic_Rag.ipynb
│   └── Summarized_Report.pdf
```

- **notebooks/Agentic_Rag.ipynb**: Main notebook containing the agentic workflow.
- **notebooks/Summarized_Report.pdf**: Example output report.

## Dependencies

- [LangChain](https://github.com/langchain-ai/langchain)
- [LangGraph](https://github.com/langchain-ai/langgraph)
- [OpenAI](https://platform.openai.com/)
- [pypdf](https://pypdf.readthedocs.io/)
- [fpdf](https://pyfpdf.github.io/fpdf2/)
- [python-dotenv](https://github.com/theskumar/python-dotenv)
- [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/)

Install all dependencies with:

```sh
pip install -r requirements.txt
```

## License

MIT License

---

_Crafted with ❤️ for AI-powered research._
