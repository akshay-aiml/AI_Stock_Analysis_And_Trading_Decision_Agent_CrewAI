📈 AI Stock Analysis & Trading Decision Agent (CrewAI)
Overview

This project is an Agentic AI system built using CrewAI that performs:

- Live stock analysis
- Market trend evaluation
- Trading decision suggestions
It uses multiple AI agents working together as a Crew to analyze real-time stock data and produce structured insights.

Features:-

- Fetches live stock data using Yahoo Finance
- Performs stock performance analysis
- Generates trading recommendations
- Multi-agent architecture (Analyst + Trader)
- Structured output with insights

Tech Stack:-

- Python
- CrewAI
- Groq LLM (Llama 3.3)
- yFinance API
- dotenv

  Project Structure:-

  stock_ai_project/
│
├── agents/
│   ├── analyst_agent.py
│   └── trader_agent.py
│
├── tasks/
│   ├── analyse_task.py
│   └── trade_task.py
│
├── tools/
│   └── stock_research_tool.py
│
├── crew.py
├── main.py
├── .env
└── README.md

Agents:-

Financial Analyst Agent:-

 - Retrieves live stock data
 - Performs market analysis
 - Generates performance insights
Uses tool:
 - Live Stock Information Tool

Trader Agent:-
- Uses analyst report
- Suggests BUY / HOLD / SELL decisions

Tool Used:-
 - Live Stock Information Tool
 - Fetches real-time stock data:
 - Current Price
 - Change %
 - Market Information

Output:
- Current price
- Market change
- Performance analysis
- Trading suggestion

Workflow:-
User enters stock name
Analyst Agent fetches live data
Analyst generates report
Trader Agent reviews report
Final decision generated

Learning Purpose:-

- This project demonstrates:
- Multi-Agent Collaboration
- Tool Calling
- Real-time data integration
- Agentic AI Architecture

Future Improvements:-

- Add historical analysis
- Add technical indicators
- Add portfolio optimization
- Build UI (Streamlit / FastAPI)
- Deploy on cloud
