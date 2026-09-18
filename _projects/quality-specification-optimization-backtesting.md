---
title: Quality Specification Optimization & Backtesting
context: Professional Project
category: decision-support
order: 1
featured: false
card_summary: A production workflow combines backtesting, optimization, and automated reporting to evaluate numerical quality specifications before implementation. It supported one specification change prior to production introduction.
takeaway: A production evaluation workflow combined backtesting and optimization to support a specification change before its production introduction.
challenge: Assess how numerical quality specifications affect reject and rework outcomes, identify which specifications have the strongest influence, and refactor the existing evaluation codebase.
approach:
  - Refactored the evaluation backend into modular, object-oriented components.
  - Added historical what-if backtesting to compare candidate specification sets before applying changes in production.
  - Analyzed individual specification effects and used Differential Evolution to explore parameter combinations for a defined reject-rate target.
  - Added automated PDF reporting and rework evaluation based on defect types and time limits.
outcomes:
  - Delivered a refactored evaluation process that ran in production with a more modular, object-oriented backend.
  - Added comparison, optimization, and automated reporting tools for repeatable specification analysis and data-based rework decisions.
  - The workflow evaluated and supported one specification change before its introduction into production.
focus:
  - Backtesting
  - Differential Evolution
  - Decision support
methods:
  - Backtesting
  - Differential Evolution
  - Object-oriented design
  - Decision support
technologies:
  - Python
  - SciPy
  - PyLaTeX
---
