# Network Analysis of Smart City Collaboration Structures

### Citizen Participation and Regional Governance Disparities

An empirical network analysis of South Korea's smart-city governance ecosystem, examining the structural positions of civic and local-government actors, regional collaboration patterns, and citizen-to-policy pathways.

**[View the Full Analysis →](./smart-city-network-analysis.html)**

---

## Overview

Smart-city governance involves interactions among central and local governments, public institutions, private firms, academic organizations, and civic actors. Despite an institutional emphasis on participatory and decentralized governance, these actors may occupy substantially different structural positions within the policy network.

This project examines these differences using organizational co-occurrence data extracted from **7,359 smart city-related news articles**.

A weighted network was constructed from organizations appearing in the same articles, and its structure was analyzed using **centrality measures, modularity-based community detection, and shortest-path analysis**.

The project addresses three research questions:

1. **Structural Position** — Where do citizen organizations and local governments sit within the smart-city governance network?
2. **Regional Structure** — How do regional communities differ in network structure and social-capital characteristics?
3. **Citizen-to-Policy Pathways** — Which organizations connect civic actors to policy-related nodes, and how do their structural roles differ across centrality measures?

---

## Data & Methodology

| Component | Description |
|---|---|
| **Data** | 7,359 smart city-related news articles |
| **Source** | BIG Kinds |
| **Network Unit** | Organizations appearing in news articles |
| **Edge Definition** | Co-occurrence of two organizations within the same article |
| **Edge Filtering** | Co-occurrence count ≥ 2 |
| **Stakeholder Classification** | Rule-based classification into seven stakeholder groups |
| **Centrality Measures** | Degree, Closeness, Betweenness, Eccentricity |
| **Community Detection** | Modularity-based clustering |
| **Pathway Analysis** | Citizen-to-policy shortest paths |
| **Tools** | Python, pandas, NetworkX, Gephi |

### Analysis Workflow

`News Articles` → `Organization Extraction` → `Weighted Co-occurrence Network` → `Stakeholder Classification` → `Centrality Analysis` → `Community Detection` → `Citizen-to-Policy Path Analysis`

---

## Key Findings

### 1. Structural Position of Citizen Organizations and Local Governments

Citizen organizations and local governments occupied comparatively peripheral positions in the observed network.

Their combined average **Degree Centrality was approximately 31.3% lower than the overall network average**, indicating comparatively fewer direct connections to other actors.

Citizen organizations also exhibited particularly low Betweenness Centrality, while local governments remained below central-government and private-sector actors across major centrality measures.

These results indicate a structural imbalance between central actors and civic/local-government actors within the observed smart-city governance network.

### 2. Regional Governance Structures

Modularity-based community detection identified **36 communities with a modularity score of 0.507**.

Seven policy-relevant communities were examined in greater detail. The analysis revealed distinct regional configurations, including:

- globally connected technology-oriented clusters,
- metropolitan policy and international-cooperation networks,
- local-government-led decentralized structures,
- regional smart-city testbed networks, and
- industry–academia–government collaboration structures.

These findings indicate that regional smart-city ecosystems differ in their internal connectivity, external linkages, and governance characteristics.

### 3. Citizen-to-Policy Pathways

Shortest-path analysis was used to examine how citizen-participation organizations connect to policy-related actors.

The analysis highlighted intermediary organizations such as **Living Labs, Urban Regeneration Support Centers, and Creative Economy Innovation Centers** in structurally important positions along citizen-to-policy pathways.

Their roles differed across centrality measures:

- **Degree Centrality** identified organizations with broad direct connectivity.
- **Closeness Centrality** highlighted actors positioned relatively close to other nodes in the network.
- **Betweenness Centrality** identified organizations occupying intermediary positions along network paths.

The results highlight intermediary organizations and structural intervention points that could strengthen connections between civic and policy-related actors.

---

## Analytical Framework

The project combines three levels of network analysis:

### Stakeholder-Level Analysis

Degree, Closeness, Betweenness, and Eccentricity were used to compare the structural positions of central government, local government, public institutions, private firms, academia, citizen organizations, and other actors.

### Regional-Level Analysis

Modularity-based community detection was used to identify regional collaboration structures and compare their social-capital characteristics and policy-diffusion patterns.

### Pathway-Level Analysis

Shortest paths between citizen-participation organizations and policy-related actors were examined to identify intermediary nodes and differences in their structural roles.

---

## Tools & Techniques

**Programming & Data Processing**

- Python
- pandas
- NetworkX

**Network Analysis**

- Weighted organizational co-occurrence networks
- Degree Centrality
- Closeness Centrality
- Betweenness Centrality
- Eccentricity
- Shortest-path analysis

**Network Visualization & Community Analysis**

- Gephi
- Modularity-based community detection

---

## Full Analysis

The full report contains the complete analytical process, including:

- network construction and preprocessing
- rule-based stakeholder classification
- centrality calculations and distributions
- stakeholder-level comparisons
- Gephi network visualizations
- modularity-based community detection
- regional community analysis
- social-capital structure comparison
- citizen-to-policy shortest-path analysis
- policy implications
- research limitations and future research directions

### [View the Full HTML Report →](./smart-city-network-analysis.html)

For the underlying Quarto source:

[View the QMD Source](./smart-city-network-analysis.qmd)

---

## Interpretation Note

The network is constructed from **organizational co-occurrence in news articles**. An edge therefore indicates that two organizations appeared in the same article and should not automatically be interpreted as evidence of a formal partnership or direct institutional collaboration.

Centrality measures describe structural positions within the observed network rather than legal authority, actual decision-making power, or the quality of collaboration.

---

## References

The full report contains the complete references for the theoretical and methodological foundations of the analysis, including social network analysis, brokerage and closure, modularity, smart-city governance, and Korean smart-city policy.

See the **[Full Analysis](./smart-city-network-analysis.html)** for the complete reference list.
