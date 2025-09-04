# 📘 Data Analysis of Primary School Cumulative Networks

## 📌 Introduction
This project analyzes two empirical graphs from the **"Primary School – Cumulative Networks" dataset**, which captures **face-to-face interactions** between students and teachers over two days.  

- **Nodes** → Individuals (students/teachers), annotated with class, grade, and gender.  
- **Edges** → Interactions weighted by **cumulative duration** and **frequency**.  

The goal is to explore structural patterns, community dynamics, and epidemiological implications of these interaction networks.

---

## 🎯 Objectives
1. **Basic Properties** → Degree distribution, centralities, clustering coefficients, and other metrics.  
2. **Community Detection** → Compare number and size of communities across days.  
3. **Epidemiological Modeling** → Simulate virus spread and analyze propagation.  
4. **Storytelling & Interpretation** → Translate technical results into actionable insights.  

---

## 🛠 Data Loading & Preparation
- **Metadata Integration** → Each node annotated with class and gender; teachers categorized under a distinct "Teachers" class.  
- **Graph Construction** →  
  - Day 1 Graph (`day1.gexf`) – interactions recorded on first day  
  - Day 2 Graph (`day2.gexf`) – interactions recorded on second day  

This integration creates a rich context for analyzing patterns of interactions.

---

## 📊 Analysis

### 1. Basic Properties
**Graph Info**  
- **Day 1:** 236 nodes, 5899 edges  
- **Day 2:** 238 nodes, 5539 edges  

➡️ More participants on Day 2, but fewer interactions.  

**Degree Distribution**  
- Day 1: Higher number of edges → greater overall connectivity  
- Day 2: Fewer interactions → lower connectivity  

**Centralities**  
- Degree Centrality:  
  - Day 1: **0.213** avg  
  - Day 2: **0.196** avg  
- Closeness Centrality:  
  - Day 1: **0.541** avg  
  - Day 2: **0.521** avg  
- Betweenness Centrality:  
  - Day 1: **0.0037** avg  
  - Day 2: **0.00399** avg  

➡️ Teachers are likely hubs, bridging groups across the network.  

**Clustering Coefficient**  
- Day 1: **0.502**  
- Day 2: **0.560**  

➡️ Day 2 interactions are more localized and group-focused.  

---

### 2. Community Detection
- **Day 1:** 4 communities → strongly aligned with class divisions.  
- **Day 2:** 6 communities → more fragmented, suggesting evolving/mixed interactions.  

➡️ Day 1 shows structured, class-based groupings; Day 2 introduces overlaps.  

---

### 3. Epidemiological Modeling (SI Model)
- **Parameters:** Infection probability = 0.001, Steps = until all nodes infected  

**Results**  
- Day 1: 236 infected (100%) → rapid spread due to high connectivity  
- Day 2: 238 infected (100%) → slower spread due to clustering & fewer edges  

➡️ Teachers and central nodes accelerate propagation → targeted interventions could mitigate outbreaks.  

---

## 📝 Key Insights
1. **Interaction Patterns**  
   - Day 1: Higher edge count → rapid connectivity  
   - Day 2: Fewer interactions but stronger clustering  

2. **Community Dynamics**  
   - Day 1: Clearer class-based communities  
   - Day 2: More fragmented, overlapping groups  

3. **Epidemiological Implications**  
   - Teachers = super-spreaders (interaction hubs)  
   - Mitigation measures targeting these nodes would be most effective  

---

## 🌍 Broader Implications
- **Network Design** → Insights can guide safer school layouts.  
- **Epidemic Control** → Strategies focused on hubs reduce spread efficiently.  

---

## 📌 Conclusion
This study demonstrates how **graph-theoretical analysis** provides valuable insights into:  
- Student-teacher interaction patterns  
- Community dynamics over time  
- Epidemic spread modeling in real-world networks  

Findings are actionable for **education, public health, and network science**.  

---
