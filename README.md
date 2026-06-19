# 🛡️ Autonomous Financial Fraud Syndicate (Google ADK 2.0)
**Track:** Enterprise Agents | **Role:** Data Analyst / Backend Engineer

## 💡 The Pitch & Problem Statement
Modern financial institutions lose billions to fraudulent transactions that occur in the operational gap between a flagged alert and a human analyst's manual review. 

This project deploys a multi-agent "syndicate" using Google ADK 2.0 to eliminate that gap. It acts as an autonomous Tier-1 Fraud Analyst that calculates geographic velocity anomalies in real-time, cross-references historical risk scoring, and executes protective account freezes—reducing response time from minutes to milliseconds.

## 🤖 Why an Agent Architecture?
Traditional rule-based fraud detection suffers from massive false-positive rates because hardcoded logic cannot adapt to nuanced context. By utilizing an Agent Graph:
1. **Separation of Concerns:** The `TransactionSleuth` focuses purely on spatial-temporal data anomalies, while the `RiskManager` handles complex business-logic decision-making.
2. **Contextual Action:** The system doesn't just send an alert; it uses deterministic tool-calling to structurally isolate compromised accounts autonomously.

## 🛠️ Toolchain
* **Google ADK 2.0:** Graph-based sequential workflow orchestration.
* `analyze_geo_velocity`: Calculates physical distance vs. time deltas.
* `query_risk_profile`: Fetches historical account data (KYC status, account age).
* `execute_security_action`: Programmatically restricts outbound database transactions.
