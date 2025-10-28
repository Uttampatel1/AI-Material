https://youtu.be/-mldKsBR0UM?si=_zB1QSdGK_VjM7IW 
---

## 🎯 **Main Idea**

The video explains **multi-method agentic AI**, a way of building intelligent systems that combine **large language models (LLMs)** with **other proven automation technologies** (like workflows, decision engines, and data systems).

This combination helps create **more reliable, transparent, and regulatory-compliant AI systems** than using LLMs alone.

---

## 🧩 **1. What is Agentic AI?**

* **Agentic AI** means AI systems made up of *agents*—autonomous components that can:

  * Perceive input (like a customer request)
  * Decide what to do next
  * Interact with other agents or systems to take action

* **LLMs** (like GPT-type models) are powerful tools for understanding and generating language, but:

  * They can be unreliable
  * They’re not good at managing state (remembering progress)
  * They can’t easily explain decisions

So, agentic AI systems should use **multiple methods** — not just LLMs — to be effective and trustworthy.

---

## 🏦 **2. Example Problem: A Bank Loan Application**

To illustrate, the speaker builds an example:

> “How does a bank decide whether to lend someone money?”

The goal is to show how a **multi-agent system** would handle this from start to finish.

---

## 💬 **3. Step-by-Step Breakdown**

### **Step 1 — Chat Agent (LLM)**

* The customer chats with the bank (“Can I get a loan for a boat?”).
* A **chat agent** (based on an LLM) interprets the customer’s intent (ask a question or request an action).
* It converts the messy input into a structured request for the bank’s AI system.

---

### **Step 2 — Orchestration Agent (LLM)**

* The **orchestration agent** acts as a coordinator.
* It looks up which specialized agent can handle this request (like a “loan policy agent” or “loan application agent”).
* It uses a **registry** (a directory of agents and what they do).

---

### **Step 3 — Loan Policy Agent (LLM + RAG)**

* This agent explains **loan policies** (what the bank will or won’t lend money for).
* Uses **Retrieval-Augmented Generation (RAG)**:

  * Pulls info from internal documents (loan policies, risk rules, etc.)
  * Summarizes the relevant content into a natural language answer.
* The orchestration agent routes the customer’s question here.

---

### **Step 4 — Workflow Agent (for Loan Application)**

* When the customer wants to **apply for a loan**, the system moves from chat to **action**.
* A **workflow agent** (built on workflow software like BPMN) manages the process:

  * Tracks progress (start → documents → approval)
  * Handles interruptions (if customer leaves and returns)
  * Ensures consistency
* This agent doesn’t need an LLM — it uses **workflow automation**.

---

### **Step 5 — Decision Agent (Eligibility Check)**

* Determines if the customer is **eligible** for a loan.
* Uses a **business rules engine / decision platform** (not an LLM).
* Ensures consistent, explainable, auditable logic for regulators.
* Example: “Given income, credit score, and loan amount — is this person eligible?”

---

### **Step 6 — Data Agents**

* Provide customer or external data to other agents.
* Example: Get **credit bureau data**, customer records, or other financial details.
* These are exposed as “data agents” using **Model Context Protocol (MCP)** so they integrate seamlessly.

---

### **Step 7 — Document Ingestion Agent (LLM)**

* If the customer provides a **document** (like a boat brochure), the **document ingestion agent** uses an LLM to:

  * Read the image/text
  * Extract structured data (price, model, weight, dealer info)
* This makes unstructured input usable for automation.

---

### **Step 8 — Decision + Workflow Continue**

* The workflow gathers:

  * Customer data
  * Credit data
  * Asset data (from the brochure)
* It submits all of that to the **loan origination decision agent**, which decides whether to approve, deny, or flag the loan.

---

### **Step 9 — Handling a “Maybe”**

* If the loan decision is **“maybe”**, the workflow asks the customer to speak with a human rep (call center).
* The system saves state, so the customer can come back later and continue from the same point.

---

### **Step 10 — Human Support with LLM Agents**

When a call center rep joins:

* A **companion agent (LLM)** helps the rep understand the customer’s context and data quickly.
* An **explainer agent (LLM)** translates the decision log (why the system said “maybe”) into plain language so the rep can explain it clearly to the customer.

---

## ⚙️ **4. Key Technologies Used**

| Agent Type          | Function                                     | Technology Used                    |
| ------------------- | -------------------------------------------- | ---------------------------------- |
| Chat Agent          | Understands and responds to customer input   | LLM                                |
| Orchestration Agent | Routes requests between agents               | LLM                                |
| Policy Agent        | Retrieves policy info from documents         | LLM + RAG                          |
| Workflow Agent      | Manages state, tracks process                | Workflow engine (BPMN)             |
| Decision Agent      | Applies consistent rules                     | Decision platform / business rules |
| Data Agent          | Retrieves customer and credit data           | Data platform via MCP              |
| Ingestion Agent     | Extracts data from documents                 | LLM (OCR + NLP)                    |
| Companion Agent     | Assists call center staff                    | LLM                                |
| Explainer Agent     | Translates system logs into natural language | LLM                                |

---

## 🔍 **5. Why Multi-Method Agentic AI Matters**

* **LLMs are great** for language understanding and flexible data handling.
* **But** they lack:

  * Reliability
  * State tracking
  * Auditability
  * Transparency

By combining LLMs with structured systems (workflows, rules engines, data agents), you get:
✅ **Consistency**
✅ **Explainability**
✅ **Compliance with regulations**
✅ **Better customer experience**

---

## 🧠 **In Summary**

> Multi-method agentic AI = LLMs + automation + decision logic + data integration.

It’s the **future architecture** for enterprise AI — adaptable, explainable, and capable of *doing real work*, not just chatting.
<img width="1536" height="1024" alt="ChatGPT Image Oct 28, 2025, 07_41_45 PM" src="https://github.com/user-attachments/assets/b942c2da-552b-401f-9db0-8edc090d0958" />

---
