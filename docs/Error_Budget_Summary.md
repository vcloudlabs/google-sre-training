# Error Budget – Deep Dive

## Simple Definition

An **Error Budget** is the **allowed amount of failure** your system can have without violating its SLO (Service Level Objective).

> If your SLO is 99.9% availability, your **error budget is 0.1%**.

It’s the **margin for risk** you’re willing to tolerate while maintaining user trust.

---

## Why Error Budgets Matter

Error budgets help balance:
- **Stability** (keeping services reliable)
- **Innovation** (deploying new features)

If your service is too unreliable and exceeds the budget:
- You pause risky changes
- Focus on fixing issues

If you stay within the budget:
- You can push new updates
- Take calculated risks

---

## 🔢 How to Calculate an Error Budget

### Example:
- SLO = 99.9% over 30 days
- Total minutes in 30 days = 43,200 minutes
- Error Budget = 0.1% of 43,200 = **43.2 minutes of downtime allowed**

You can also calculate it for:
- Requests: 0.1% of 1 million = 1,000 allowed failures
- API errors, latency violations, etc.

---

## 📊 Example Breakdown

| Metric | Value |
|--------|-------|
| SLO | 99.9% availability |
| Total time in month | 43,200 minutes |
| Allowed downtime | 43.2 minutes |
| If system is down for 20 mins | ✅ Still within budget |
| If system is down for 60 mins | ❌ Exceeds budget (violation) |

---

## 🧠 Best Practices with Error Budgets

- **Monitor usage** regularly with dashboards
- Tie deployment policies to error budget health
- Use it as a trigger for **blameless postmortems**
- Avoid overengineering by not aiming for 100% if not required

---

## 🧭 Summary

| Term | Meaning |
|------|---------|
| **SLO** | The target level of service |
| **Error Budget** | How much you're allowed to fail before breaking the SLO |
| **Budget Burn** | How much of the error budget has already been used |

Error budgets bring **objectivity** to decisions around reliability vs speed.