# multi_agent_tool

# 🧠 Multi-Agent AI Assistant with LangGraph

This project demonstrates how to build a multi-agent AI system using **LangGraph**, **FastAPI**, **Redis**, and **OpenAI**, inspired by ReAct and agentic workflows. It includes memory, streaming, tool use, and human-in-the-loop design patterns.

## 🚀 Features

- 🧩 Modular LangGraph agents with reasoning and action steps
- 🧠 Memory-enabled interaction using Redis
- 📦 Tool use (e.g., OpenAI, custom tools, Redis data fetchers)
- 📡 Real-time FastAPI backend
- 🧑‍💻 Human-in-the-loop feedback triggers
- 🎯 React frontend-ready architecture
- 🔍 Integrated with LangSmith for observability and traceability

## 📁 Structure

multi_ai_agent/<br>
├── multiaiagent.ipynb # Notebook demonstrating the architecture <br>
├── app/ # FastAPI app files (optional structure)<br>
├── static/ # Static frontend assets (JS/CSS)<br>
├── templates/ # Jinja2 HTML templates<br>
├── .env # Environment variables (OpenAI, Redis, etc.)<br>
└── README.md # You're here!


## 🛠️ Technologies Used

- [LangGraph](https://github.com/langchain-ai/langgraph)
- [LangChain](https://github.com/langchain-ai/langchain)

- [LangSmith](https://smith.langchain.com/) for agent monitoring

## 📦 Setup Instructions

```bash
# 1. Clone the repo
git clone https://github.com/your-username/multi_agent_tool.git
cd multi_agent_tool

# 2. Create virtual environment
python -m venv venv
source venv/bin/activate  # or venv\\Scripts\\activate on Windows

# 3. Install dependencies
pip install -r requirements.txt

# 4. Set environment variables
cp .env.example .env  # then edit with your keys

# 5. Run FastAPI app
uvicorn main:app --reload
📌 Sample Use Case
“Summarize the shopping cart for user123” →
Agent retrieves cart from Redis → Calls OpenAI for summary →
Returns friendly, personalized cart summary → Allows human override.

📈 Future Improvements
Add WebSocket or SSE streaming to frontend

Multi-agent task coordination (e.g., planner + executor)

Integration with product recommender or vector DB

LangGraph state visualization UI


