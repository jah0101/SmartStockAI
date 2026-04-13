# SmartStockAI
Multi-agent inventory decision system built with n8n and AI logic

SmartStockAI is a multi-agent inventory decision system built using n8n and structured AI prompts to automate retail inventory workflows.

## 📌 Overview

This project simulates real-world inventory decision-making using rule-based logic combined with AI-assisted reasoning.

It is based on real retail operations experience and incorporates key inventory metrics such as:
- MASC (Minimum Acceptable Shelf Condition)
- Weekly movement
- Ad and promotional activity
- Shelf capacity and facings

## 🧠 System Architecture

SmartStockAI is built using three core agents:

### Agent 1: Count Exception Triage
- Validates discrepancies between system counts and physical counts
- Determines whether to CONTINUE or STOP for recount

### Agent 2: Restock Decision Engine
- Calculates adjusted demand using business rules
- Uses ad and endcap multipliers to simulate real demand spikes
- Outputs:
  - RESTOCK NOW
  - MONITOR
  - NO ACTION

### Agent 3: Manager Approval Routing
- Determines whether decisions should be auto-approved or escalated
- Flags inconsistent or high-risk scenarios for review

## ⚙️ Technologies Used

- n8n (workflow automation)
- OpenAI API (structured prompt logic)
- JSON (data inputs and workflow structure)

## 📊 Example Output

Decision: RESTOCK NOW  
Approval: AUTO-APPROVE  
Reason: High adjusted movement due to ad and endcap activity

## 📁 Project Structure

- `/workflows` → n8n workflow exports
- `/assets` → workflow screenshots
- `/sample-data` → test scenarios

## 🚀 Purpose

This project demonstrates how AI and rule-based systems can improve efficiency in retail inventory management by reducing manual decision-making and increasing consistency.

## 🔗 Author

Jacob H – Business Analytics Student (UAH)
