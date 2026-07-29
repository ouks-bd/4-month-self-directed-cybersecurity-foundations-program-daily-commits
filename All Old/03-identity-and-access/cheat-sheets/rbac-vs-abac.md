# RBAC vs ABAC — Quick Reference

| | RBAC | ABAC |
|---|------|------|
| Decision based on | Role assignment | Attributes (user, resource, action, environment) |
| Example | "Finance role can access invoices" | "User in Finance can access invoices from corp IP during business hours" |
| Simplicity | High | Lower (policies get complex) |
| Flexibility | Lower | Very high |
| Typical setting | On-prem AD, classic enterprise | Modern cloud (AWS IAM conditions) |
| Risk | Role explosion (hundreds of fine-grained roles) | Policy explosion (hard to audit) |

**Real systems combine both.** RBAC for the broad strokes, ABAC conditions for context.
