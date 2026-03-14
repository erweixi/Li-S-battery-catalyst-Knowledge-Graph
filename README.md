# Li-S Catalyst Global Knowledge Graph (Lithium-Sulfur Battery Catalyst Global Knowledge Graph) 
This is an interactive visualization tool built based on ECharts, aiming to visually present the complex network relationships in the fully automated and data-driven battery catalyst screening process. Through this graph, researchers can comprehensively explore the deep connections among candidate catalyst materials, underlying physical and chemical characteristics, textual evidence support, and high-dimensional evaluation logic. 
✨ Core Function 
* **Multidimensional Data Structure Visualization**: One-stop rendering of the global relationship network that includes candidate materials, evaluation dimensions, logical patterns, textual evidence, and indicator fields.
* **Dynamic Interaction and Filtering**:
* **Node Type Control**: Through the sidebar, specific types of nodes can be freely enabled or disabled (for example, hiding textual evidence and only viewing the correlations between core materials and dimension indicators).
* **Score Range Filtering**: Dragging the slider allows filtering out high-potential catalysts with `total_score` greater than a specific threshold, facilitating quick focus on top candidate materials.
* **Physics Engine Layout Adjustment**: Supports real-time manual adjustment of the "repulsive force" and "edge length" of the force-directed graph to meet the display requirements under different node filtering densities, avoiding visual stacking. 
## 📜 File Description 
`graph.html`: This single-file structure contains the complete DOM structure, CSS style control panel, ECharts rendering logic, and the embedded original data of the graph (`rawGraph`). 
## 🚀 How to Use 
1. **Local Execution**: No need to install any server environment or dependent libraries. Simply double-click the `graph.html` file and open it in any modern browser (such as Chrome, Edge, Safari) to interact with the graph.
2. **Online Deployment**: Since it is a purely static HTML file, it can be extremely conveniently uploaded to a common GitHub project repository and, by enabling the **GitHub Pages** service, it can serve as an affiliated demonstration page for personal academic homepage or project code repository for others to access online. 
## 🧠 Node Category Analysis 
The graph shows the five core nodes in the screening system by using different colors for distinction: 
* **🟩 Material (Material)**: Candidate battery catalyst phases that have undergone automated screening and evaluation (such as `Co2P`, `AgPdO2`, etc.), along with a comprehensive score (total_score).
* **🟦 Dimension (Evaluation Dimension)**: The core performance evaluation direction of the catalyst, including thermodynamic stability (Thermo Stability), electronic transport (Electronic Transport), catalytic activity (Catalytic Activity), and polysulfide affinity (Polysulfide Affinity).
* **🟫 TextEvidence (Text Evidence)**: Specific factual descriptions extracted from the original data or the screening process, used to provide positive, neutral, or negative evaluations for a particular dimension.
* **🟧 LogicPattern (Logical Pattern)**: The reasoning rules for mapping the underlying indicator fields to the high-dimensional evaluation dimensions (for example, "low band gap -> high electronic transport").
* **🩵 MetricField (Metric Field)**: Specific characteristic fields extracted or calculated from the material database (such as `band_gap_eV`, `energy_above_convex_hull_eV_per_atom`). 
---
This visual interface provides an intuitive and highly scalable interactive window for exploring the automatic screening mechanism of catalytic materials for transformational batteries. *