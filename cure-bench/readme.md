# CURE-Bench 🧠💊  
**Benchmarking AI for Clinical Drug Decision-Making and Precision Therapeutics**
 
## Overview 
**CURE-Bench** (Clinical Utility in REasoning for Benchmarking) is a competition and benchmark suite designed to evaluate AI models on their ability to support therapeutic decision-making. Unlike traditional QA datasets, CURE-Bench focuses on real-world, high-stakes clinical tasks such as:

- Recommending personalized treatments
- Assessing drug safety and efficacy
- Designing step-by-step treatment plans
- Identifying repurposing opportunities for rare or under-treated conditions

This benchmark is intended for evaluating **Large Language Models (LLMs)** and **Large Reasoning Models (LRMs)**, especially those using external tools and multi-agent coordination strategies.

## Why CURE-Bench?
Precision medicine requires structured, multi-step reasoning over heterogeneous data involving patients, drugs, and diseases. CURE-Bench provides a clinically relevant, task-diverse environment to assess the real-world utility of AI models in healthcare.

## Tasks
CURE-Bench includes the following task categories:

- **Treatment Recommendation**: Suggest appropriate therapies given patient/disease context
- **Safety & Efficacy Assessment**: Judge the viability of drug choices based on medical history or contraindications
- **Treatment Planning**: Sequence multi-drug regimens over time, considering dependencies and interactions
- **Drug Repurposing**: Identify alternative uses for existing drugs for rare or neglected diseases

Each task is grounded in real-world clinical data and expert-reviewed protocols.

## Format
- JSON-based input/output formats
- Prompt templates for popular LLM APIs (OpenAI, Anthropic, etc.)
- Supports few-shot and chain-of-thought prompting
- Tool-calling compatible for agents using retrieval, calculators, and medical knowledge bases

