🧠 Multi-Agent System using Phi Framework
This project sets up a multi-agent system using the Phi AI framework to handle real-time financial and web-based queries. It leverages advanced language models and tools to deliver enriched responses with sources and visual formatting.

📁 Project Overview
The code defines and orchestrates three agents:

Web Agent: Gathers real-time information from the internet using DuckDuckGo.

Finance Agent: Fetches financial data like stock prices, analyst recommendations, and company info using Yahoo Finance tools.

Agent Team: Combines the web and finance agents to answer complex multi-modal queries.

🔧 Features
🌐 Web scraping and summarization

📊 Real-time financial insights

🧑‍💻 Multi-agent collaboration

✅ Source-backed responses

📄 Markdown and table output support

🧩 Dependencies
Phi

groq for LLM (LLaMA 3-70B)

yfinance for financial tools

dotenv for environment variable loading

Install dependencies via:

bash
Copy
Edit
pip install phi
Ensure your .env file is configured properly (for any required keys).

🚀 Usage
To run the agent system:

bash
Copy
Edit
python agent.py
Example behavior:

python
Copy
Edit
agent_team.print_response("Summarize analyst recommendations and share the latest news for NVDA", stream=True)
This command instructs the agents to collaborate and return up-to-date financial recommendations and related news for NVIDIA.

📎 Notes
The Groq model llama-3.3-70b-versatile is used by default. You can switch to OpenAI’s GPT-4o by uncommenting the relevant lines.

Agents are instructed to show their tool usage and provide clean markdown-formatted outputs.

Modify or extend the agent team to suit custom use cases or domains (e.g., health, sports).

📜 License
MIT License (or replace with your preferred license)
