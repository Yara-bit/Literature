# Literature: A Public Collection of Papers on Airport Stand/Gate Assignment

## Aviation ground dispatch and gate allocation optimization

- [Optimal Schedule Recovery for the Aircraft Gate Assignment with Constrained Resources](https://www.sciencedirect.com/science/article/pii/S0360835221005866)  
  *Asadi, E., Schultz, M., & Fricke, H. (2021). Computers & Industrial Engineering.*

- [A Review on Airport Gate Assignment Problems: Single versus Multi Objective Approaches](https://www.sciencedirect.com/science/article/pii/S0305048319306000)  
  *Daş, G. S., Gzara, F., & Stützle, T. (2020). Omega.*

- [Flight Gate Scheduling: State-of-the-art and Recent Developments](https://www.sciencedirect.com/science/article/abs/pii/S0305048305000939)  
  *Omega (2007).*

- [An Airport Stand Assignment Problem Considering the Passenger Boarding Distance](https://onlinelibrary.wiley.com/doi/abs/10.1155/2023/3345138)  
  *Huyan, Z., Tang, T.-Q., Gao, Y., & Cao, F. (2023). Journal of Advanced Transportation.*

- [A Novel Deep Reinforcement Learning Approach for Real-Time Gate Assignment](https://papers.ssrn.com/abstract=4808146)  
  *Li, H., Wu, X., Ribeiro, M., Santos, B. F., & Zheng, P. (2024). SSRN.*

- [A Two-Stage Optimization Model for Airport Stand Allocation and Ground Support Vehicle Scheduling](https://www.mdpi.com/2076-3417/14/23/11407)  
  *Yao, M., Hu, M., Yin, J., Su, J., & Yin, M. (2024). Applied Sciences.*

---

## DRL for Airport Gate Assignment

### 1. Zhu et al. (2024)
**Title**: Gate Assignment Algorithm for Airport Peak Time Based on Reinforcement Learning  
- [Gate Assignment Algorithm for Airport Peak Time Based on Reinforcement Learning—Chenwei Zhu, Zhenchun Wei, Zengwei Lyu, Xiaohui Yuan, Dawei Hang, Lin Feng, 2024. (n.d.). Retrieved August 18, 2025, from](https://journals.sagepub.com/doi/abs/10.1177/03611981241242352)
**Approach**:  
- Proposes a two-stage PPO-based model (GABPPO) with pre-assignment and dynamic reassignment.
- Optimizes near-gate usage and passenger transfer efficiency.

**Results**:  
- Higher near-gate assignment rate (76.6%) and better gate matching than DQN/PG/APGA.

**Strengths**:  
- Joint optimization of airport and passenger objectives.
- Real-time reassignment included.

**Limitations**:  
- Small dataset (30 flights).
- No scalability or runtime analysis.
- Lacks comparison with stronger DRL baselines.

---

### 2. Li et al. (2025)
**Title**: Deep Reinforcement Learning for Real-Time Airport Gate Assignment  
- [Li, H., Wu, X., Ribeiro, M., Santos, B., & Zheng, P. (2025). Deep reinforcement learning approach for real-time airport gate assignment. Operations Research Perspectives, 14, 100338.](https://doi.org/10.1016/j.orp.2025.100338)
**Approach**:  
- Uses A3C for pre-assignment and a real-time reassignment agent (REGAPS).
- Action masking applied for feasibility filtering.

**Results**:  
- Reduces apron usage and passenger walking distance vs. rule-based baselines.
- Handles delayed flights adaptively.

**Strengths**:  
- Real-world dataset (124 flights).
- Handles dynamic delays and gate-sharing constraints.

**Limitations**:  
- Simplifies gate occupation logic (e.g., dep delay ignored).
- No evaluation against other DRL agents like PPO or DQN.

---

### 3. Jia et al. (2025)
**Title**: A Deep Reinforcement Learning Algorithm for AGAP  
- [Jia, A., Liu, H., Yang, H., Yang, W., Chen, H., & Yi, X. (2026). A Deep Reinforcement Learning Algorithm for Solving Airport Gate Allocation Problem. In M. Mahmud, M. Doborjeh, K. Wong, A. C. S. Leung, Z. Doborjeh, & M. Tanveer (Eds.), Neural Information Processing (pp. 75–88). Springer Nature.](https://doi.org/10.1007/978-981-96-6951-6_6)
**Approach**:  
- DQN-based assignment with hybrid rewards and conflict masking.
- Evaluated on both synthetic benchmarks and large real-world cases.

**Results**:  
- Solves 244-seat/102-gate cases in <2s.
- Outperforms FBS and RFH in quality and runtime.

**Strengths**:  
- High scalability.
- Considers transfer vs. non-transfer passenger walking distance.

**Limitations**:  
- Focused on static schedules.
- No dynamic reassignment or delay modeling.

---

###  Summary Table

| Paper             | DRL Model | Reassignment | Real Data | Delays | Large-scale |
|------------------|-----------|--------------|-----------|--------|-------------|
| Zhu et al. (2024)| PPO       | ✅           | ✅ (30)    | ⚠️     | ❌          |
| Li et al. (2025) | A3C       | ✅           | ✅ (124)   | ✅     | ❌          |
| Jia et al. (2025)| DQN       | ❌           | ✅ (244)   | ❌     | ✅          |

---


## Graph Neural Networks and Robot Learning

- [A Comprehensive Survey on Graph Neural Networks](https://ieeexplore.ieee.org/abstract/document/9046288)  
  *Wu, Z., Pan, S., Chen, F., Long, G., Zhang, C., & Yu, P. S. (2021). IEEE TNNLS.*

- [ROBOT LEARNING, Edited by Jonathan H. Connell and Sridhar Mahadevan](https://www.cambridge.org/core/journals/robotica/article/abs/robot-learning-edited-by-jonathan-h-connell-and-sridhar-mahadevan-kluwer-boston-19931997-xii240-pp-isbn-0792393651-hardback-21800-guilders-12000-8995/737FD21CA908246DF17779E9C20B6DF6#)  
  *Robotica (1999).*

---

## Data and open source platforms

- [OpenSky](https://opensky-network.org/)  
  *OpenSky Network – Real-time air traffic data platform.*
