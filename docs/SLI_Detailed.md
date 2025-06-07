# 📈 Service Level Indicator (SLI) – Deep Dive

## What is an SLI?
A **Service Level Indicator (SLI)** is a carefully defined quantitative measure of some aspect of the level of service that is provided. SLIs are the foundation of SLOs and SLAs, and they help in assessing whether users are experiencing the desired reliability and performance.

SLI is a specific measurement that tells you how well a service is working from the user’s point of view.

## Characteristics of a Good SLI
- **User-Centric**: Reflects the user's experience with the service
- **Quantifiable**: Can be measured with real metrics
- **Relevant**: Maps to critical service behavior
- **Actionable**: Enables alerting, improvements, or incident response

## Common SLI Types
- **Availability** – How often is the service reachable?
- **Latency** – How fast is the service?
- **Error Rate** – How frequently does it fail?
- **Durability** – Is data safe and not corrupted?
- **Freshness** – Is data up-to-date?

## SLI Formula Example
```text
SLI = (Number of successful requests / Total requests) * 100
```

---
## 🗂️ Example SLIs by Service Type

| Service Type | Example SLIs |
|--------------|--------------|
| Web APIs / Backend Services | HTTP success rate, request latency, error rate |
| User-Facing Web Applications | Page load time, JS errors/session, navigation success rate |
| Mobile Apps | API latency, crash rate, sync latency |
| Authentication Services | Login success rate, authentication time, timeout rate |
| Data Pipelines / ETL Jobs | Data freshness, pipeline success rate, processing delay |
| CI/CD Services | Pipeline provision success, execution time, rollback rate |
| Messaging / Notification Systems | Message delivery rate, latency, duplication/drop rate |
| Database Services | Query success rate, latency, transaction failure rate |
| File/Storage Services | Retrieval success rate, download latency, data corruption rate |
| Streaming / Real-time Services | Stream start time, buffering ratio, dropped frames |
| Search Services | Search latency, result relevance, query failure rate |
| Email / Communication Services | Delivery time, bounce rate, spam/marked message rate |

---