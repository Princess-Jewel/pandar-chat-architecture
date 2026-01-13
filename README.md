# Pandar Chat – Internal Customer Support Platform (Architecture Case Study) Overview

## Overview

**Pandar Chat** is an internal, business‑critical customer support application built for **Pandar**. The platform enables Pandar’s customer service team to communicate directly with users, process gift card transactions, provide real‑time updates, and manage customer interactions efficiently.

This application is **used exclusively by Pandar insiders** and serves as the **primary communication channel** between the company and its customers.

This repository is a **public architecture and system design case study**. The production codebase is private.

---

## Problem Statement

Pandar required a reliable way for its internal team to:

* Communicate with customers in real time
* Process gift card submissions and conversions
* Provide status updates during transaction processing
* Maintain conversation history for accountability and support continuity

There was **no existing system** in place to handle these workflows. Relying on third‑party chat tools would limit integration with Pandar’s internal processes and create operational bottlenecks.

A **custom, tightly integrated internal chat system** was required.

---

## Solution

Pandar Chat was built as a **dedicated internal web application** that:

* Enables real‑time messaging between Pandar support staff and customers
* Integrates with internal workflows for gift card processing
* Provides visibility into transaction status and customer context
* Serves as the single source of truth for customer communications

The platform prioritizes **reliability, clarity, and operational efficiency**, as it directly supports live financial transactions.

---

## My Role

I **designed, built, and deployed the Pandar Chat application entirely on my own**, owning the system end‑to‑end.

My responsibilities included:

* Designing the system architecture and data flow
* Building the full frontend interface for support agents
* Implementing backend APIs and real‑time communication logic
* Integrating chat workflows with gift card processing operations
* Deploying and maintaining the application in production

This project demonstrates ownership of a **mission‑critical internal tool** used daily by a fintech operations team.

---

## System Architecture

### High‑Level Architecture

* **Frontend:** React.js (internal dashboard for support agents)
* **Backend:** Node.js (REST APIs + real‑time messaging)
* **Database:** Relational database for users, conversations, and message history
* **Real‑time Layer:** WebSockets or similar event‑driven communication
* **Deployment:** Cloud‑hosted with CI/CD pipelines

The architecture is designed for **low latency, consistency, and auditability**.

---

## Core Features

### Support Team Features

* Real‑time chat with customers
* Viewing customer profiles and transaction context
* Processing and updating gift card transactions
* Sending status updates and confirmations
* Conversation history tracking

---

## Key Engineering Decisions

### 1. Custom Internal Tooling

Rather than relying on third‑party chat services, the system was built in‑house to allow tight coupling with Pandar’s operational workflows.

### 2. Real‑Time Communication

Real‑time messaging was implemented to ensure immediate feedback during sensitive financial processes such as gift card verification and payout updates.

### 3. Reliability & Traceability

Conversation history and transaction context are persisted to ensure accountability, continuity, and dispute resolution.

---

## Challenges & Trade‑offs

* Ensuring message delivery reliability during peak support periods
* Balancing simplicity of the UI with operational needs
* Maintaining performance while handling concurrent conversations

---

## Impact

* Became the **core communication tool** for Pandar’s customer service operations
* Enabled efficient processing of gift card transactions
* Improved response times and customer experience
* Centralized all customer communications into a single internal system

---

## Tech Stack

* React.js
* Node.js
* REST APIs
* Real‑time messaging (WebSockets or similar)
* Relational database
* Git & CI/CD

---

## Notes

This repository intentionally excludes production source code. It exists to demonstrate **internal tooling design, real‑time systems, and ownership of mission‑critical fintech infrastructure**.

---

## Contact

**Princess Jewel Jel‑Edema**
Senior Full Stack Engineer (React & Node.js)
Portfolio: [https://princess-jewel.vercel.app](https://princess-jewel.vercel.app)
LinkedIn: [https://linkedin.com/in/princess-jewel-jel-edema](https://linkedin.com/in/princess-jewel-jel-edema)
