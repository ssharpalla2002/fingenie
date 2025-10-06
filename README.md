# 🧠 FinGenie — RAG AI Financial Assistant

FinGenie is an AI-powered financial assistant that leverages **Retrieval-Augmented Generation (RAG)** to answer finance-related queries and generate structured documents.  
It integrates **LangGraph** for workflow orchestration and **LangChain** for retrieval, embeddings, and agent reasoning.  

---

## Features

- Intelligent financial query answering with RAG  
- Automated document generation from retrieved data  
- Modular LangGraph-based agent workflows  
- Vector search via ChromaDB for efficient information retrieval   

---

## Tech Stack

- **Python 3.12+**  
- [LangGraph](https://github.com/langchain-ai/langgraph) – graph-based workflow engine  
- [LangChain](https://www.langchain.com/) – LLM orchestration framework  
- **ChromaDB** – vector database for embeddings  
- **OpenAI API** – LLM integration  
- **python-dotenv** – environment configuration  
- **JupyterLab** – interactive development & demos  

---

## Getting Started

Using pyenv and uv

```zsh
brew update
brew install pyenv
```

Add the following to your `~/.zshrc` if it's not already there:

```zsh
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init --path)"
eval "$(pyenv init -)"
```
Restart your terminal or source your `~/.zshrc`:

```zsh
source ~/.zshrc
```

#### Install Python Version

```zsh
pyenv install 3.12.6
pyenv local 3.12.6
```

#### Install uv

```zsh
pipx install uv     
pip install --user uv
```

If you don't have pipx, install it with:

```zsh
brew install pipx
pipx ensurepath
```

#### Set Up Virtual Environment with uv

```zsh
uv venv .venv
source .venv/bin/activate
```

#### Install Dependencies

```zsh
uv pip install -r requirements.txt
```

#### Set up Environment Variables

If you need API keys (such as for OpenAI), create a `.env` file in the root directory:

```zsh
echo "OPENAI_API_KEY=your_openai_key" > .env
```

#### Start JupyterLab

```zsh
uv pip install jupyterlab  
jupyter lab
```

---

## Requirements

Core dependencies (see `requirements.txt` for full list):

- langgraph
- langchain
- ipython
- langchain_openai
- langchain_community
- dotenv
- typing
- chromadb
- langchain_chroma

Install all dependencies with:

```zsh
uv pip install -r requirements.txt
```

---
