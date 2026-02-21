# AI-Powered Automation Assistant

An AI-driven workflow orchestration system built using **n8n** that integrates multiple Google Workspace services and external APIs through a centralized webhook architecture.

This project enables dynamic execution of real-world actions (email, scheduling, document updates, search, expense tracking) based on structured natural language inputs.

---

## 🖼 Workflow Snapshot

![n8n Workflow](./n8n-workflow-screenshot.png)

---

## 💡 Why This Project

Most automation systems are static and tool-specific.  
This project introduces an AI-driven orchestration layer that dynamically selects and executes tools based on user intent.

Instead of predefined rules, the workflow interprets structured inputs and routes them to the correct service, enabling flexible and scalable automation.

Focus Areas:
- AI-based tool routing
- Multi-API integration
- Workflow reliability
- Structured output validation

---

## 🏗 Architecture Overview

The system follows a centralized orchestration model:

1. **Webhook Entry Point**  
   Receives user queries in structured format.

2. **AI Agent (LLM Node)**  
   Interprets user intent and generates structured JSON output.

3. **Intent-Based Routing Logic**  
   Dynamically selects appropriate API nodes based on parsed intent.

4. **Service Integrations**
   - Gmail API  
   - Google Calendar API  
   - Google Docs API  
   - Task Management API  
   - Search API  

5. **Response Formatter**
   Returns execution results or confirmation messages.

---

## 🚀 Key Capabilities

- Centralized webhook-based AI orchestration
- Dynamic tool execution from natural language inputs
- Integration of 5+ APIs
- Support for 10+ user-triggered actions
- Structured JSON parsing and validation
- Modular workflow design for scalability
- Basic rate-limit handling and execution safeguards

---

## 📌 Example Supported Actions

- Send and read emails
- Create, update, and fetch calendar events
- Create and modify Google Docs
- Add and retrieve tasks
- Perform search queries
- Log and track expenses

---

## 🛠 Tech Stack

- **n8n** (Workflow Orchestration)
- **REST APIs**
- **Google Workspace APIs**
- **Webhook Architecture**
- **Structured JSON Validation**

---

## 🔒 Reliability & Stability Measures

- Schema-based JSON parsing to prevent malformed tool execution
- Conditional routing to avoid incorrect API invocation
- Basic rate-limit handling
- Error-handling nodes for workflow continuity
- Tested across 50+ structured interactions

---

## ⚙ Setup Instructions

1. Clone this repository
2. Import the provided workflow JSON file into n8n
3. Configure Google API credentials
4. Set webhook endpoint
5. Execute workflow

> ⚠ API credentials are not included for security reasons.

---

## 📂 Repository Structure
