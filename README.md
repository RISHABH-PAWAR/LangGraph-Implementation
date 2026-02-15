LangGraph Implementation — Agentic Workflow Systems

This repository explores LangGraph for building structured, stateful, and production-grade LLM workflows.

Instead of building simple chatbots, this project focuses on:

Graph-based execution flows

Stateful agents

Human-in-the-loop systems

RAG pipelines

Tool integration

Subgraph modular architecture

Persistence handling

This is a hands-on implementation repo designed to deeply understand how agent systems actually work under the hood.

📌 Why LangGraph?

Traditional LLM chains break when:

You need state

You need loops

You need branching logic

You need human validation

You need tool calls

You need persistence

LangGraph solves this by modeling workflows as directed state graphs.

This repo demonstrates how.
```
📂 Project Structure
LangGraph-Implementation/
│
├── 0_test_installation.ipynb
├── 1_bmi_workflow.ipynb
├── 2_simple_llm_workflow.ipynb
├── 3_prompt_chaining.ipynb
│
├── 4_batsman_workflow.ipynb
├── 5_UPSC_essay_workflow.ipynb
├── 6_quadratic_equation_workflow.ipynb
├── 7_review_reply_workflow.ipynb
├── 8_X_post_generator.ipynb
├── 9_basic_chatbot.ipynb
│
├── 10_persistence.ipynb
├── 11_tools.ipynb
├── 12_mcp.py
│
├── 13_rag.ipynb
├── 14_hitl.ipynb
├── 15_subgraphs.ipynb
├── 15_subgraph_shared.ipynb
│
├── chatbot_without_hitl.py
├── chatbot_with_hitl.py
```

🧠 Concepts Implemented
1️⃣ Basic Graph Workflows

BMI calculator flow

Prompt chaining

Multi-step LLM pipelines

Decision-based graph routing

Focus: Understanding state transitions.

2️⃣ Applied Workflows

Essay generation (UPSC style)

Review reply automation

X (Twitter) post generator

Mathematical equation solver

Domain-specific LLM flows

Focus: Real-world automation pipelines.

3️⃣ Stateful Chatbots

Basic chatbot

Persistent memory chatbot

HITL-enabled chatbot

Tool-augmented chatbot

Focus: Managing conversational state inside graph systems.

4️⃣ Persistence

Demonstrates how to:

Store graph state

Resume execution

Maintain memory across sessions

Critical for production agents.

5️⃣ Tool Integration

Shows:

Tool calling within graph nodes

Structured execution

External function invocation

6️⃣ RAG with LangGraph

Implements:

Retrieval pipeline inside graph structure

Query → Retrieve → Augment → Generate flow

Modular node architecture

This bridges traditional RAG and agent workflows.

7️⃣ Human-in-the-Loop (HITL)

Implements:

Interrupt nodes

Human approval steps

Feedback loops

Controlled execution

Essential for compliance-heavy AI systems.

8️⃣ Subgraphs

Demonstrates:

Reusable subgraph components

Modular workflow design

Composable agent systems

Shared state management

This is where LangGraph becomes production-grade.

⚙️ Installation
pip install langchain langgraph openai


Set API key:

export OPENAI_API_KEY="your_key_here"

🚀 Running Examples

For notebooks:

jupyter notebook


For Python scripts:

python chatbot_with_hitl.py

🎯 Who This Is For

AI engineers building agent systems

Developers moving beyond simple chains

Engineers designing RAG + Agents

Builders preparing for GenAI engineering roles

SaaS founders building AI automation systems

🏗 Architecture Philosophy

This repository demonstrates:

Graph-based orchestration > linear chaining

State-driven execution

Explicit control over decision flow

Modular subgraph composition

Human oversight integration

Persistence-first design
