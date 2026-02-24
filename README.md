# Introduction to the Agentic AI Era
**Session Time:** 120 minutes  
**Format:** Instructor-Led  

---

## Prerequisites

- Basic familiarity with Artificial Intelligence concepts  
- Awareness of Large Language Models (LLMs)  
- Basic understanding of Python  

No prior experience with AI agents is required.

---

## Learning Objectives

By the end of this session, students will be able to:

1. **Define** the key concepts of Agentic AI and **distinguish** it from traditional Generative AI.
2. **Differentiate** between autonomous agents and simple automated tools, recognizing their architectural differences.
3. **Identify** real-world examples of Agentic AI applications across industries such as healthcare, finance, and customer service.

> In this course, Agentic AI is treated as a systems architecture discipline — focusing on autonomy, decision loops, tool integration, and production readiness.

---

## Session Breakdown

| # | Segment | Duration |
|---|---------|----------|
| 1 | From Generative AI to Agentic Systems | 15 min |
| 2 | Agents vs. Automated Tools | 20 min |
| 3 | Real-World Applications Across Industries | 10 min |
| 4 | Break | 10 min |
| 5 | Lab: Concept Mapping | 60 min |
| 6 | Wrap-Up & Reflection | 5 min |
|   | **Total** | **120 min** |

---

## 1. From Generative AI to Agentic Systems (15 min)

### The Linear Model of Generative AI

Traditional Generative AI follows a single-step, reactive interaction model:

```
User → Prompt → LLM → Response
```

This architecture is **stateless** and **single-turn**: the model produces text in response to an input, then stops. It has no goals, no persistence, and no ability to take actions in the world.

### The Shift to Agentic AI

Agentic AI introduces **autonomy and execution**:

> An AI agent is a system that perceives its environment, reasons about its goals, and takes actions to maximize objective fulfillment over time.

<img width="494" height="242" alt="image" src="https://git.generalassemb.ly/user-attachments/assets/297cfc38-4c49-47af-8193-074048cccbbf" />

```
User → Agent → Observe → Think → Plan → Act → Store Memory → Repeat
```

The agent doesn't just respond — it pursues goals across multiple steps, using tools and adapting based on results.

<img width="465" height="261" alt="image" src="https://git.generalassemb.ly/user-attachments/assets/f633adc8-5fc8-4982-b678-3fe123f1da9c" />


| Dimension | Generative AI | Agentic AI |
|-----------|---------------|------------|
| Output | Language | Outcomes |
| Interaction | Single-step | Multi-step loop |
| Memory | None | Short and long-term |
| Actions | None | Tool calls, API execution |
| Goal persistence | None | Active across sessions |

**The core shift:** Generative AI produces language. Agentic AI produces outcomes


### Discussion Prompt (2 min)

> Think of a task you do repeatedly at work. What would it look like if an AI could handle it end-to-end — not just answer a question about it, but actually do it?

---

## 2. Agents vs. Automated Tools (20 min)

### What Makes Something an "Agent"?

The term *agent* is overloaded in tech. It's important to draw a clear line between:

**Automated tools** follow deterministic, predefined scripts:
- If X → Do Y
- No reasoning, no adaptation, no decision-making

**AI Agents** reason, plan, and adapt:
- Observe the environment
- Decide what to do based on context and goals
- Use tools dynamically
- Update their approach based on results

### The Spectrum of Autonomy

| Level | System | Description |
|-------|--------|-------------|
| 0 | Prompt-based LLM | Text in, text out. No memory, no tools. |
| 1 | LLM + Memory | Maintains context across turns. |
| 2 | LLM + Memory + Tools | Can search, calculate, query APIs. |
| 3 | Planning + Multi-step execution | Decomposes complex goals into subtasks. |
| 4 | Multi-agent systems | Multiple specialized agents collaborate. |
| 5 | Enterprise orchestration | Human-in-the-loop, audit trails, governance. |

> This course progresses through these levels.

<img width="464" height="271" alt="image" src="https://git.generalassemb.ly/user-attachments/assets/8f72492b-d501-4bfc-b0d4-228b3e927a9a" />


### What an Agent Is NOT

- An agent is not a chatbot with extra steps.
- An agent is not a macro or an if/then script.
- An agent is not magic — it still needs clear goals, reliable tools, and proper memory.

An agent without tools and memory is just an advanced chatbot.

### Architectural Limitations of LLMs in Production

| Limitation | Impact in Production |
|------------|---------------------|
| Stateless responses | No continuity between interactions |
| No tool execution | Cannot take real-world actions |
| No environment awareness | Cannot validate outcomes |
| No goal persistence | Cannot pursue multi-step objectives |
| No execution verification | Cannot detect or recover from failure |

Enterprise systems require **action, verification, and persistence** — not just text generation.

### Quick Check (2 min)

> Is a customer-facing chatbot that follows a decision tree an agent? What would need to change for it to become one?

---

## 3. Real-World Applications Across Industries (10 min)

Agentic AI is already deployed across industries. Below are examples organized by how the agent components — reasoning, memory, tools, and actions — work together to deliver value.

### Healthcare

**Use Case:** Clinical documentation assistant  
An agent listens to patient-provider conversations, accesses EHR systems via API, drafts clinical notes, and flags potential drug interactions — all autonomously.

- **Tools:** EHR API, drug interaction database  
- **Memory:** Patient history across visits  
- **Action:** Drafts notes, sends alerts to providers  

### Finance

**Use Case:** Loan eligibility agent  
Instead of a simple chatbot, a full agent pulls real-time credit data, validates against current policy rules, escalates edge cases to human reviewers, and logs every decision for audit.

- **Tools:** Credit bureau API, policy rule engine  
- **Memory:** Application state across sessions  
- **Action:** Approves, denies, or escalates with documented reasoning  

### Customer Service

**Use Case:** Intelligent support agent  
Routes tickets to the correct team, retrieves purchase history, drafts resolution emails, and learns from past ticket outcomes to improve future routing.

- **Tools:** CRM, email API, ticketing system  
- **Memory:** Customer history, previous interactions  
- **Action:** Resolves, routes, escalates  

### Case Study: Why Chatbots Fail in Production

A financial institution deployed a chatbot for loan processing. Offline testing showed high accuracy.

In production, the system failed because:
- No real-time API access to credit data
- No eligibility validation against live policy
- No state persistence — customers had to restart every session
- No escalation path for edge cases

**The issue was architectural, not model quality.** It was a chatbot, not an agent.

After redesigning with API tool integration, session memory, a decision loop, and execution logging:

> **Resolution time dropped by 37%.**

---

## 4. Break (10 min)

---

## 5. Lab (60 min)

---

## 6. Wrap-Up & Reflection (5 min)


1. In one sentence, what is the defining difference between Generative AI and Agentic AI?
2. What is the minimum a system needs to qualify as a true AI agent, as opposed to an automated tool?
3. What industry not covered in this session do you think has the highest potential for Agentic AI? Why?

Next session: **Anatomy of an Agent**
---

## Resources

- [OpenAI Platform Documentation](https://platform.openai.com/docs)
- [Microsoft Copilot Architecture Overview](https://learn.microsoft.com/en-us/copilot/)
- [Google Research: Autonomous Agents](https://research.google/pubs/)
- Russell & Norvig — *Artificial Intelligence: A Modern Approach* (Chapter 2: Intelligent Agents)
- Sculley et al. — *Hidden Technical Debt in Machine Learning Systems*
- [LangChain Agent Docs](https://docs.langchain.com/docs/components/agents)
