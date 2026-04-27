# Priority Dynamics in Centralized vs Decentralized Systems  
## Queueing, Latency, and Strategic Execution under Uncertainty

---

## Overview

This project studies **priority-based execution mechanisms** in two fundamentally different environments:

- **Centralized systems (CEX-like architectures)**  
- **Decentralized systems (DEX-like architectures)**  

The focus is on understanding how **latency, priority rules, and stochastic delays** shape the outcome of competing agents interacting in a shared system.

---

## Motivation

Modern large-scale systems frequently involve:

- multiple agents competing for execution  
- delayed and uncertain information  
- priority mechanisms (fees, timestamps, ordering rules)  

This project explores a key question:

> How do **priority rules and stochastic delays** impact system dynamics and agent outcomes?

---

## Key Concepts

### 1. Priority Mechanisms

Agents compete to have their actions executed first.

Two main paradigms:

- **Deterministic priority (centralized systems)**  
  → ordering based on arrival time or queue position  

- **Fee-based priority (decentralized systems)**  
  → ordering influenced by willingness to pay  

---

### 2. Stochastic Delays

Execution is not instantaneous.

Instead, actions are subject to:

- random latency  
- network propagation delays  
- asynchronous updates  

This introduces **uncertainty in ordering**, even when priorities are defined.

---

### 3. Queueing Dynamics

The system can be modeled as a **priority queue with randomness**, where:

- agents submit actions  
- actions compete under delay  
- execution order emerges from both **priority and randomness**

---

## Core Insights

### 1. Priority is not absolute under latency

Even with clear ordering rules, stochastic delays can:

- invert execution order  
- create race conditions  
- introduce probabilistic outcomes  

---

### 2. Trade-off between speed and priority

Agents face a structural trade-off:

- act early with uncertain priority  
- act later with stronger priority (e.g., higher fee)  

This leads to **strategic behavior under uncertainty**.

---

### 3. System design shapes equilibrium behavior

Different architectures induce different dynamics:

| System Type      | Dominant Mechanism        | Key Effect                     |
|-----------------|--------------------------|--------------------------------|
| Centralized     | Queue ordering           | Deterministic but latency-sensitive |
| Decentralized   | Fee-based priority       | Strategic bidding + randomness |

---

## Methodology

The project is based on:

- probabilistic modeling of delays  
- priority queue analysis  
- stochastic process reasoning  
- comparison of execution mechanisms  

The analysis highlights how **micro-level rules** translate into **macro-level system behavior**.

---

## Project Structure

- `CEX_DEX_report.pdf`  
  → Detailed theoretical analysis and modeling framework  

- `CEX_DEX_presentation.pdf`  
  → Concise summary of key mechanisms and insights  

---

## Interpretation

This project reveals a general principle:

> In systems with both **priority rules and randomness**, outcomes are inherently probabilistic—even when rules are deterministic.

---

## Broader Perspective

The framework applies beyond the specific context studied here.

It is relevant to any system involving:

- asynchronous decision-making  
- competing agents  
- resource allocation under latency  
- priority-based scheduling  

---

## Applications

- analysis of distributed systems  
- optimization of scheduling policies  
- design of robust priority mechanisms  
- understanding emergent behavior in competitive environments  

---

## Skills Demonstrated

- stochastic modeling  
- queueing theory intuition  
- system-level reasoning  
- analysis of asynchronous processes  
- translating theoretical models into practical insights  

---

## Author

**Théo BASSERAS**

Background in mathematics, machine learning, and complex system modeling.

---

## Key Takeaway

> When priority meets randomness, **deterministic rules no longer guarantee deterministic outcomes**.

Understanding this interaction is essential for designing and analyzing modern distributed systems.

---