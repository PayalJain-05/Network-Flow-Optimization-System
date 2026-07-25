# Network-Flow-Optimization-System
Modeled a logistics network as a directed graph, then used Ford-Fulkerson and minimum-cut analysis to find its true bottleneck. One route limits everything — no matter how large the rest of the network is. Fix that route, and throughput opens up for the whole system.

# Network Flow Optimization System

### Where does a logistics network actually break?

---

## What is this project about?

A graph model that finds the exact bottleneck in a logistics network.

**"Which single route is limiting how much this network can move?"**

Warehouses and hubs become nodes. Delivery routes become edges, weighted by capacity.

---

## Why does this matter?

Networks rarely fail everywhere. Usually, one route quietly limits everything.

Fixing that one route beats expanding the whole network — cheaper, faster, and it actually works.

---

## Methodology

- **Graph construction** — nodes = hubs, edges = routes weighted by capacity
- **Ford-Fulkerson** — repeatedly pushes flow along available paths
- **BFS / DFS** — finds each path used inside Ford-Fulkerson
- **Minimum-cut analysis** — finds the exact edges limiting total flow
- **Visualization** — NetworkX + Matplotlib, flow values labeled on each route

---

## Key Insight

Max-flow min-cut theorem: a network's maximum flow always equals the capacity of its minimum cut.

In short — the network can only move as much as its tightest bottleneck allows, no matter how big the rest is.

Fix that one bottleneck, and the whole network's throughput increases.

---

## Tools Used

| Tool | What it was used for |
|------|----------------------|
| **Python** | Core language |
| **NetworkX** | Building and analyzing the graph |
| **Matplotlib** | Visualizing flow across the network |
| **Ford-Fulkerson** | Computing maximum flow |
| **BFS / DFS** | Path-finding inside each iteration |
| **Min-Cut** | Identifying the true bottleneck |

---

## Original Files
<img width="840" height="555" alt="Screenshot 2026-04-27 at 4 36 59 PM" src="https://github.com/user-attachments/assets/559b4dee-4ff7-4e12-96cd-fab2cf75eadc" />



<img width="1239" height="760" alt="Screenshot 2026-04-27 at 4 37 17 PM" src="https://github.com/user-attachments/assets/9faadb77-e703-438e-b0c9-60d51c869807" />

---

## In One Line

**Models a logistics network as a graph and pinpoints the exact route limiting the entire system's throughput.**
