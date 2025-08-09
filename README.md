# Shark-Clustering-GNNs
Clustering of shark interaction network using Graph Neural Networks (GNNs), association rule mining, and the Affinity Propagation clustering algorithm.  
The project clusters learned node (shark) embeddings from Graph Convolutional Networks (GCN) and Graph Attention Networks (GAT) applied to a shark co-occurrence graph, combined with features derived from association rule mining, and visualizes relationships between individuals.

## Data Source
The primary dataset is hosted on **Zenodo** and can be accessed via [this link](https://zenodo.org/records/15250000).

---

## Repository Structure

### **Code/**
| File | Description |
|------|-------------|
| `Association_Rules.ipynb` | Implements association rule mining to discover frequent patterns in shark detection data. |
| `GCN_GAT_AP_NodeClustering.ipynb` | Applies GCN, GAT, and Affinity Propagation for node clustering. |
| `Graph_Construction.ipynb` | Builds the network graph from the detection dataset. |
| `Transaction.ipynb` | Prepares transaction-based datasets for association rule mining. |

### **Results/**
| File | Description |
|------|-------------|
| `full_shark_relations.csv` | Complete interaction network of sharks. |
| `shark_relations.csv` | Filtered subset of shark relationships. |
| `Graph.gml` | GraphML representation of the shark network. |
| `GAT4_200_best_partition_visualization.png` | Visualization of GAT4 clustering best partition. |
| `GCN_200_best_partition_visualization.png` | Visualization of GCN clustering best partition. |
| `GAT4_200_training_progress.png` | Training progress for GAT4 model. |
| `GCN_200_training_progress.png` | Training progress for GCN model. |
| `venn_with_labels.png` | Venn diagram showing overlap of detected communities. |

---

## How to Use

1. **Download the dataset** from the Zenodo link above.  
2. Place the dataset in the appropriate directory as required by the notebooks.  
3. Run the notebooks in the following order:
   - `Graph_Construction.ipynb` → Build the network graph.  
   - `Transaction.ipynb` → Prepare transactions.  
   - `Association_Rules.ipynb` → Extract frequent association rules.  
   - `GCN_GAT_AP_NodeClustering.ipynb` → Apply GNN-based clustering.  
4. Check the `Results/` directory for generated graphs, CSV files, and visualizations.


