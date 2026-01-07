# 📝 Medium Article Generator using Agno

## 📌 About the Project
This project is an **AI-powered Medium article generation system** built using **Agno** and **LLM-based agents**.  
It automates **research and content creation** by coordinating multiple specialized agents that gather information from various platforms and generate **Medium-style articles**.

The system conducts research from multiple sources, synthesizes the information, and produces well-structured articles that can be saved as Markdown files.

---

## 🔍 What This Project Does
- Gathers research from **ArXiv, web search, HackerNews, Wikipedia, news articles, X (Twitter), YouTube**, and more
- Summarizes research content from multiple sources
- Generates **Medium-style articles** based on the collected research
- Allows user confirmation before saving the final article
- Saves articles as **Markdown (.md) files**
- Supports email drafting using Gmail tools (on user confirmation)

---

## 🤖 Agents Used
The system uses a **team of AI agents**, including:
- ArXiv Research Agent  
- Web Search Agent (DuckDuckGo)  
- HackerNews Research Agent  
- News Article Research Agent  
- Wikipedia Research Agent  
- X (Twitter) Research Agent  
- YouTube Research Agent  
- Gmail Agent  
- Team Leader Agent for orchestration and article creation  

---

## ⚙️ Requirements
- **Python 3.13**
- **uv** (Python package manager)

Install `uv` if not already installed :
```bash
pip install uv

```
---

## 📦 Installation & Dependencies :
Initialize the environment:
- uv init --python 3.13
Install required dependencies:
- uv add agno openai python-dotenv
- uv add pypdf arxiv
- uv add ddgs
- uv add newspaper4k lxml_html_clean
- uv add wikipedia
- uv add tweepy
- uv add youtube_transcript_api
- uv add praw
- uv add google-api-python-client google-auth-httplib2 google-auth-oauthlib
- uv add fastapi["standard"] uvicorn

---

## 🔑 Environment Setup :
Create a .env file in the project root and add:
- OPENAI_API_KEY=your_openai_api_key

---
## ▶️ Run the Project:
uv run app.py
