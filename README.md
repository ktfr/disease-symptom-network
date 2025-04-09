# Disease-Symptom Networks: Visualizing Health and Diagnosis

Understanding the relationships between diseases and symptoms is crucial for improving diagnostic accuracy and recognizing gaps in public health studies. Disease-Symptom Networks is a disease-symptom dataset which applies social network analysis to identify patterns, clusters, and key connections between diseases. 

  
---
## **Group Members: Group 4**

- **Rahat Chowdhury**
- **Jiayi Teh**
- **Kai Ferrer**

---

## **Set Up**
### Prerequisites
**Required Tools/Imports**
To run this project, you must have the following installed:
- Python 3.13.0 and installations of the following libraries:
    - pandas
    - pickle
    - matplotlib
    - seaborn
    - community_louvain
    - collections
- Jupyter Notebook

### Import requirements
To install any imports, you may rorunm ```pip install <import>```
- For example, to install pandas, in terminal run ```pip install pandas```

### Setup
It is suggested to run this within VS Code.
1. Clone the repository: ```git clone https://github.com/ktfr/disease-symptom-network.git```
2. Navigate to the 'dataframes' directory: ```cd notebooks```
3. View and run the relevant notebooks.

---

### File Specifications and Locations: 
(This directory is incomplete.)
```
disease-symptom-network/
├── dataframes/                                     # Contains dataframes in pickle files 
│   ├── df_aggregated.pk1                                   # Our aggegated dataset
│   ├── disease_network_edges.txt                       # Text file of our network edges for viewing
│   ├── edges_df_sorted.pk1                             # Our network edges dataset sorted
│   ├── edges_df.pk1                                    # Our network edges dataset unsorted
├── notebooks/                                          # Contains our main analyses
│   ├── Centrality.ipynb                                # Centrality analysis notebook
│   ├── DataProcessing.ipynb                            # Dataset data cleaning notebook
│   ├── DiseaseCommunityAnalysis.ipynb                  # Community detection analysis notebook
│   ├── GephiImports.ipynb                              # Extracts .csv files of our network for gephi
│   ├── LinkPrediction.ipynb                            # Link prediction analysis notebook
│   ├── NetworkResilience.ipynb                         # Network resilience analysis notebook
│   ├── PreliminarNetworkAnalysis.ipynb                 # Initial and basic statistic analysis notebook
│   ├── ScaleFreeNetworks.ipynb                         # Scale free network analysis notebook
│   ├── SpecificDiseaseAnalyses.ipynb                   # Analysis of specific diseases in our network
│   ├── gephi-imports/                                  # Contains .csv files from GephiImports.ipynb
│   │    ├── betweenness_values.csv                     # Contains betweenness values of nodes
│   │    ├── disease_nodes_with_communities.csv         # Contains disease nodes with communities
│   │    ├── disease_similarity_edge_list.csv           # Contains edge list for disease similarities
│   │    ├── top_degree_nodes_per_community.csv         # Contains top nodes per community
│   ├── community-analysis-outputs/                     # .txt files of outputs for full data
│   │    ├── diseases_per_community.txt                 # Contains a list of all diseases per community
│   │    ├── misdiagnosis_risk_scores.csv               # Contains misdiagnosis risk scores
│   │    ├── top_degree_nodes_per_community.txt         # Contains top degree nodes per community
│   │    ├── top_misdiagnosis_pairs_per_community.csv   # Contains top misdiagnosis pairs per community
├── README.md                                           # Project documentation

```