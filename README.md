## Hi, I'm Harsh 👋

Backend engineer at **Irdeto**, where I build Java and Python services for OTT and PayTV platforms. On the side, I build **evals and guardrails for AI agents**. I care less about what an agent *says* it did and more about the state it actually left behind.

- 🎓 B.Tech CSE, NIT Srinagar (2024)
- ⚙️ Day job: I raised content ingestion throughput by 5× for non-media and 7× for media by removing redundant API calls and making execution asynchronous
- 🔬 Side work: test harnesses, safety hooks and head-to-head comparisons for coding and inbox agents

### Agent evals

| Project | What it answers | Result |
|---|---|---|
| [**said-vs-did**](https://github.com/harshkumawat5/said-vs-did) | When an inbox agent says "Done, I've declined the 3pm", did it? It uses a mock Gmail and Calendar with 25 tasks and grades from the final mailbox state, then checks every claim in the agent's final message against that state. | 225 runs across Haiku 4.5, Sonnet 5.5 and Opus 5.5. None of the 201 claims was false. The one mismatch went the other way: Haiku said "it failed" after a 504 on a write that had actually succeeded. |
| [**salus-shadow-hook**](https://github.com/harshkumawat5/salus-shadow-hook) | Would five simple safety policies have caught anything real? It's a Claude Code `PreToolUse` hook that runs in shadow mode, replayed over 51 public SWE-agent trajectories. | Out of 1,629 calls, it found an `rm -f *.py` that deleted matplotlib's `setup.py`, and SWE-bench still scored that task as resolved. It also showed that all 254 false positives came from one cause. |
| [**superset-race**](https://github.com/harshkumawat5/superset-race) | Which coding agent actually fixes the bug? It gives the same prompt to agents in parallel git worktrees, runs your tests in each one and prints a scoreboard. | Claude Code vs Codex on a real open bug in `python-humanize`: 770 passed vs 676 passed and 90 failed. |

### Other projects

- [**latency-topology-visualizer**](https://github.com/harshkumawat5/latency-topology-visualizer): a 3D globe of crypto exchange and cloud-region latency (Next.js, Three.js)
- [**Custom_Object_detection**](https://github.com/harshkumawat5/Custom_Object_detection): YOLOv4, v7 and v8 and the TF Object Detection API, from my research internship with the University of Essex on detecting symbols in architectural floor plans

### Stack

**Work:** Java · Spring Boot · gRPC · Python · Docker · AWS · OpenSearch · ActiveMQ · ArgoCD · BPMN
**Agents & evals:** Python · TypeScript · Claude Code hooks · Claude API · pytest

### Elsewhere

[LinkedIn](https://www.linkedin.com/in/harsh-kumawat-1678a8210/)
