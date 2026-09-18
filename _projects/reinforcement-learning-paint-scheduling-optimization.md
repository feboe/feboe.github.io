---
title: Reinforcement-Learning Paint Scheduling Optimization
context: Master Thesis & Professional Project
category: optimization
order: 2
featured: false
card_summary: A simulation environment compares reinforcement-learning scheduling with the existing heuristic for an industrial paint process. The modeled policy reduced solvent consumption by 2.92% with a 0.24% increase in simulated process duration.
takeaway: The modeled prototype reduced solvent consumption by 2.92% versus the heuristic while increasing simulated process duration by 0.24%.
challenge: Sequence color-assigned parts through an industrial paint process to reduce solvent-intensive color changes while also limiting idle time.
approach:
  - Modeled the process as a Gymnasium-compatible simulation environment and implemented single- and multi-agent DQN prototypes with Ray RLlib.
  - Applied action masking to enforce feasible decisions and reduce avoidable standstill periods.
  - Reimplemented the existing heuristic in Python and compared simulation outputs with reference production data.
outcomes:
  - The prototype reduced modeled solvent consumption by 2.92% relative to the heuristic reference.
  - The reinforcement-learning policy increased average process duration by 0.24% relative to the heuristic benchmark, measured in time steps within the simulation environment.
note: Reported improvements are simulation results. The discrete-time model shifted some state transitions relative to continuous process behavior, limiting direct transfer of the results to physical production.
focus:
  - Reinforcement learning
  - Simulation
  - Action masking
methods:
  - Reinforcement learning
  - DQN
  - Simulation
  - Action masking
technologies:
  - Python
  - Gymnasium
  - Ray RLlib
---
