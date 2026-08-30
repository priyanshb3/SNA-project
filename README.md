Unsupervised Community Detection using Ensemble GNN

Course Project — CSET 347: Social Network Analysis (Phase 2)
Team: Priyansh Bansal, Jitesh Kumar, Daksh Baliyan
Supervised by Dr. Soumita Das

Overview

This project detects communities in graph-structured data without using any ground-truth labels. It ensembles three Graph Neural Network encoders — GCN, GraphSAGE, and GAT — to generate node embeddings, then applies K-Means clustering on the combined embeddings to discover communities.

Pipeline
Encode — Three GNN encoders (GCN, GraphSAGE, GAT) independently learn node embeddings purely from graph structure and features, no labels used.
Ensemble — Embeddings from all three encoders are averaged into one unified representation per node.
Cluster — K-Means groups the ensembled embeddings into communities.
Evaluate — Modularity, NMI, and Silhouette Score measure cluster quality.
Tech Stack

Python, PyTorch, PyTorch Geometric, scikit-learn, NetworkX, Google Colab (GPU)

Outputs

Quantitative results (Excel), t-SNE community visualization, comparative NMI chart
