---
title: SLA-Aware Ticket Assignment
context: Personal Project
category: additional
order: 1
featured: false
card_summary: A reproducible scheduling prototype compares dispatch rules with rolling constraint optimization under capacity, language, priority, and service-level constraints. It makes trade-offs between throughput, waiting time, and urgent-ticket protection visible.
takeaway: A reproducible scheduler exposes the trade-offs between simple dispatch rules and rolling constraint optimization for urgent tickets.
challenge: Assign queued tickets under capacity, language, priority, and SLA constraints without protecting urgent work at the expense of overall throughput.
approach:
  - Compared heuristic dispatch policies with an OR-Tools constraint-programming scheduler that replans as queue conditions change.
  - Evaluated throughput, waiting time, and protection of SLA-critical tickets.
outcomes:
  - Delivered a reproducible prototype comparing heuristic dispatch with rolling constraint optimization.
  - Made trade-offs between throughput, waiting time, and protection of SLA-critical tickets visible.
focus:
  - Constraint programming
  - Rolling-horizon scheduling
  - Heuristic dispatch
methods:
  - Constraint programming
  - Rolling-horizon scheduling
  - Heuristic dispatch
technologies:
  - Python
  - OR-Tools
  - CP-SAT
repository: https://github.com/feboe/sla-aware-ticket-assignment
repository_label: View repository
---
