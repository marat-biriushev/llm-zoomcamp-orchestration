# LLM Zoomcamp 2026 – Orchestration Homework

This repository contains my solution for the **Orchestration** homework of **LLM Zoomcamp 2026**.

**Homework:** [LLM Zoomcamp 2026 – Orchestration Homework](https://github.com/DataTalksClub/llm-zoomcamp?utm_source=chatgpt.com)

## Repository Structure

* `1_chat_without_rag.yaml` – Basic chat flow without Retrieval-Augmented Generation (RAG).
* `2_chat_with_rag.yaml` – Chat flow enhanced with RAG using Kestra documentation.
* `4_simple_agent.yaml` – AI Agent example with a modified prompt that generates **exactly 3 English sentences** instead of 1.

## What I Learned

During this homework I explored several concepts related to AI orchestration with Kestra:

* Context Engineering and why providing relevant documentation improves LLM responses.
* The difference between a standard LLM workflow and a RAG-based workflow.
* Building AI-powered workflows using Kestra AI Agents.
* Monitoring input/output token usage and understanding how prompt changes affect cost.
* Choosing between deterministic task-based workflows and AI agents depending on the use case.

## Experiments

### RAG vs. No RAG

Compared responses generated with and without RAG.

**Result:** the RAG workflow produced more accurate and grounded answers by using Kestra documentation as context, while the non-RAG version relied only on the model's internal knowledge.

### Token Usage

Measured token consumption for different summary lengths.

* **Short summary:** lower output token count.
* **Long summary:** significantly higher output token count.
* Increasing the English summary from **1 sentence** to **3 sentences** approximately doubled the output token usage.

## Technologies

* Kestra
* Google Gemini 2.5 Flash
* YAML
* AI Agents
* Retrieval-Augmented Generation (RAG)

## Author

Marat Biryushev
