# Service Level Objective (SLO) – Explained

## Simple Definition

**SLO (Service Level Objective)** is a target or goal that tells you how good your service should be, based on a specific measurement (SLI).

> Example: "We want our website to load within 1 second at least **99.9% of the time**."

---

## What is an SLO?

An **SLO** is a reliability goal derived from an SLI. It defines:
- **What level of service** is acceptable
- **Over what time window** it should be measured

---

## SLI vs. SLO Example

| SLI (What You Measure) | SLO (What You Aim For) |
|------------------------|------------------------|
| 99.2% requests successful | 99.9% success over 30 days |
| 85% queries < 200ms | 95% in < 200ms over 7 days |
| 0.01% error rate | Max 0.1% errors over 30 days |

---

## 🧠 Why SLOs Matter
- Sets **realistic reliability goals**
- Helps with **alerting and error budgets**
- Supports **decision-making** on features vs reliability
- Prevents overengineering

---

## 🕓 SLO Time Windows

SLOs are always time-bound:
- Rolling window (e.g., last 30 days)
- Calendar-based (e.g., this month)

---

## 🛠️ Real-World Example

> "Login API should respond in under 300ms **99.95% of the time** over the past **30 days**."

This guides teams on whether the system is performing well enough or needs attention.

---

## 🧭 Summary

| Concept | Definition |
|--------|------------|
| **SLI** | What you measure (e.g., latency, error rate) |
| **SLO** | What you aim to achieve for that metric |

Overengineering means designing or building a solution that is more complex, costly, or powerful than necessary to solve the actual problem.
