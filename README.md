# RecallLens: Unit-Level Product Recall Checker

## The Problem
Consumer product recalls are published as long, technical legal documents. Users struggle to determine if their *specific* unit (based on model number, date code, or lot number) is actually affected.

## The Solution
**RecallLens** is an AI-powered agentic application. Users describe their product in natural language. The system retrieves official recall notices using Hybrid Search, uses a stateful LangGraph agent to reason, asks for missing info, and outputs a verdict (Affected / Not Affected / Needs Info) with exact quotes from the official notice.

## Tech Stack
*   **Backend:** Python, FastAPI
*   **AI/Agent:** LangChain, LangGraph, Google Gemini API
*   **Retrieval:** ChromaDB, HuggingFace Embeddings
*   **MLOps:** Docker, GitHub Actions CI/CD