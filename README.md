# AI Industry Conflict Graph & Game Analysis (V0.1)

This project uses **graph theory** and **game theory** to model the competitive relationships among major AI companies (OpenAI, DeepSeek, Anthropic, Google, xAI, Meta).

## What's inside

- `ai-conflict-analysis-v0.1.md` — The full article in Markdown (Chinese)
- `conflict-graph-sketch.jpg` — Hand-drawn conflict graph
- `adjacency-matrix.png` — Hand-written adjacency matrix
- `vertex-coloring.jpg` — Vertex coloring result (4 colors = 4 strategic positions)
- `edge-coloring.jpg` — Edge coloring result (5 colors = 5 conflict management types)
- `game-profit.png` — Game profit / Nash equilibrium analysis

## Key Findings (V0.1)

- The conflict graph is **connected** — local competition pressure transmits globally through the network
- **Chromatic number χ(G) = 4** — at least 4 different strategic positions are needed for the industry
- **Edge chromatic number χ'(G) = 5** — managing conflicts is more complex than finding positions
- A **K₄ subgraph** (OpenAI, DeepSeek, Google, Meta) forms a "zero-buffer conflict core" — any pairwise clash immediately involves the other two
- The 4-coloring strategy profile is a **pure Nash equilibrium** under simplified assumptions (uniform edge weights, zero intrinsic strategy payoffs)

## Limitations (V0.1)

All edge weights are uniform; all strategies are treated as equally valuable; the graph is static and undirected. These simplifications will be lifted in V0.3 with weighted edges and intrinsic strategy payoffs.

## Author

A math master's student exploring complex systems through graph theory and game theory.

## Read the full article (Chinese)

Published on Zhihu: [我用图论和博弈论，分析了AI行业的多边博弈 - 咖啡的文章 - 知乎
https://zhuanlan.zhihu.com/p/2034028512240215179]
