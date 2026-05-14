# AI Industry Conflict Graph & Game Analysis

This project uses **graph theory** and **game theory** to model the competitive relationships among major AI companies (OpenAI, DeepSeek, Anthropic, Google, xAI, Meta).

## What's inside

- `ai-conflict-analysis-v0.1.md` — V0.1: Static modeling with graph theory (Chinese)
- `ai-conflict-analysis-v0.2.md` — V0.2: Game theory analysis of equilibrium, convergence, and distributed coloring (Chinese)
- `conflict-graph.jpg` — Hand-drawn conflict graph
- `adjacency-matrix.jpg` — Hand-written adjacency matrix
- `vertex-coloring.jpg` — Vertex coloring (4 colors = 4 strategic positions)
- `edge-coloring.jpg` — Edge coloring (5 colors = 5 conflict management types)
- `v02-game-formalization.png` — Hand-drawn: Three elements of the game model
- `v02-equilibrium-check.png` — Hand-drawn: Nash equilibrium check for the 4-coloring scheme
- `v02-convergence-simulation.png` — Hand-drawn: Manual simulation of asynchronous convergence
- `v02-greedy-vs-frugal.png` — Hand-drawn: Derivation of available color sets for Greedy vs Frugal strategies

## Key Findings

### V0.1
- The graph is **connected** — local competition pressure transmits globally
- **Chromatic number χ(G) = 4** — at least 4 different strategic positions are needed
- **Edge chromatic number χ'(G) = 5** — managing conflicts is more complex than finding positions
- A **K₄ subgraph** (OpenAI, DeepSeek, Google, Meta) forms a "zero-buffer conflict core"

### V0.2
- The 4-coloring scheme is a **pure Nash equilibrium** — no company wants to deviate
- **PoA = 1** — decentralized decision-making is as efficient as central planning (under simplified assumptions)
- Asynchronous convergence completes in one round; synchronous requires stronger conditions
- The **Frugal strategy** reduces the distributed convergence requirement from Δ+2 to Δ+1 colors
- **Absorbing states** are the key mechanism — frozen nodes never unfreeze

## Limitations

All edge weights are uniform; all strategies have equal intrinsic payoffs; the graph is static and undirected. These will be upgraded in V0.3.

## Author

A math master's student using PDE tools by day, and building multi-agent game models by night.

## Read the full articles (Chinese)

- **V0.1 (Static Modeling)**：[我用图论和博弈论，分析了AI行业的多边博弈 - 咖啡的文章 - 知乎
https://zhuanlan.zhihu.com/p/2034028512240215179]
- **V0.2 (Dynamic Game)**：[当AI公司自主选择定位时，冲突网络会自我稳定吗？——用博弈论拆解多边博弈系列2 - 咖啡的文章 - 知乎
https://zhuanlan.zhihu.com/p/2037949266019217925]