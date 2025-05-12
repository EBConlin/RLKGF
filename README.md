# HEG: Hierarchical Embedded Graphs for Scalable Path Queries

This system accelerates shortest-path queries over large-scale knowledge graphs using hierarchical summarization, community-aware embeddings, and distributed A*.

## 📊 Performance
- Sublinear query time
- Parallel A* outperforms NetworkX for long paths

## 🧱 Components
- Node2vec embeddings within Louvain/METIS communities
- Bitmask-based boundary node indexing
- Multi-level abstraction + descent-based path planning

## 🔬 Use Cases
- Knowledge graph search
- Scalable fact validation
- Dynamic graph exploration

## 🛠 Setup
```bash
pip install networkx faiss-cpu
```

## 📝 Example
```python
from heg_search import query_path
query_path("protein_kinase", "DNA_repair")
```

## 📄 Paper
See "Theoretical Justification for a Hierarchical Embedded Graph Approach to Shortest Path Abstraction and Knowledge Validation" (2024)
