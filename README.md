# FinGenie: RAG AI Agent

## Overview

LangGraph is a Python framework for designing and managing the flow of tasks in your application using graph structures. This course demonstrates LangGraph concepts through step-by-step exercises, agent implementations, and Jupyter notebooks.

---

**Notable Directories:**
- **Agents/**: Python scripts for agents such as Retrieval-Augmented Generation (RAG) and document drafting.
- **Exercises/**: Jupyter notebooks for each exercise
- **Graphs/**: Notebooks demonstrating LangGraph patterns

---

## Getting Started

### Using pyenv and uv

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

## Usage

- Open and run Jupyter notebooks in `Graphs/` and `Exercises/` for hands-on practice and exploration.
- Run agent scripts in `Agents/` for more advanced experiments.
- All code is designed to work in a local, isolated Python environment managed by pyenv and uv.

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

