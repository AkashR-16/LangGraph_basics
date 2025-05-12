# 🤖 Multi-Personality Chatbot with LangGraph & Ollama

This project demonstrates how to build modular LLM applications using [LangGraph](https://github.com/langchain-ai/langgraph) with support for personality-based routing between logical and emotional chatbot agents.

## 📁 Project Structure

* `basic.py` — A minimal chatbot demo that showcases basic LLM integration using `ollama:llama3.2`. Great for sanity checking setup.
* `main.py` — A more advanced chatbot that:

  * Classifies user input into `emotional` or `logical`
  * Routes the message to the appropriate agent
  * Responds accordingly with empathy or logic

## ✨ Installation

Install the required dependencies using [uv](https://github.com/astral-sh/uv):

```bash
uv init .
```

Then we need to add the dependencies:

```bash
uv add langgraph ipykernel langchain-community langchain-ollama  
```

> **Note:** This project uses `uv` instead of `pip` for faster and deterministic dependency management.


## 🧠 LLM Configuration

This project uses:

* **LLM**: `ollama:llama3.2` (make sure Ollama is running locally)
* **Framework**: LangGraph + LangChain

## ▶️ Running the Bots

### 🧪 Basic Bot

```bash
python basic.py
```

This is a simple echo-style bot for validating LLM and LangGraph setup.

### 🗑️ Main Bot

```bash
python main.py
```

The bot will:

1. Classify your message as `emotional` or `logical`
2. Route it to the correct agent
3. Print a personalized assistant response

Type `exit` to quit the loop.

## 💠 Features

* Personality-based response logic
* LLM-based classification using structured output
* Modular architecture powered by LangGraph nodes

## 📌 TODO

* Add memory persistence
* Add streaming support
* Add unit tests

---

Created with ❤️ using LLMs + LangGraph
