# MCQ Generator

A learning project that generates multiple-choice quiz questions from a source
document (PDF or text) using an LLM. Built while following an applied LangChain
course to practice prompt chaining, structured-output parsing, and serving a
model behind a simple UI.

> **Note:** This is a follow-along learning project based on course material, not
> original product work. It's kept as a record of hands-on practice with the
> LangChain + OpenAI stack.

## Stack

- **LangChain** — prompt chaining and orchestration
- **OpenAI API** — question generation
- **Streamlit** — simple web UI
- **PyPDF2** — extract text from uploaded PDFs
- **python-dotenv** — manage the API key

## Setup

```bash
pip install -r requirements.txt
pip install -e .
```

Create a `.env` file with your OpenAI key:

```
OPENAI_API_KEY=your_key_here
```

## Run

```bash
streamlit run <app entrypoint>
```

Upload a PDF or paste text, choose the number of questions and difficulty, and
the app returns generated MCQs with answers.

## Repository layout

- `src/mcqgenerator/` — core generation logic
- `experiment/` — notebooks used while building and testing the approach
- `requirements.txt`, `setup.py` — dependencies and package config
