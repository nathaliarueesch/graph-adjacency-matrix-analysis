
# graph-adjacency-matrix-analysis

Analysis of a directed graph using its adjacency matrix representation and determinant.

This project presents an analytical study of a directed graph with 6 vertices. The work includes:

- Construction of the adjacency matrix  
- Determinant analysis  
- Identification of matrix singularity  
- Visualization of the graph using Python  
- Interpretation of results in the context of Linear Algebra and Data Science  

> This project was developed for academic learning purposes and serves as part of my Data Science portfolio.

---

## 1. Problem Description

Given a directed graph with 6 vertices, the tasks are:

1. Construct the adjacency matrix **A**.  
2. Compute **det(A)**.  
3. Explain whether the matrix is singular or not.  
4. Visualize the graph from the adjacency matrix.

---

## 2. Adjacency Matrix

The adjacency matrix **A** used in this project is defined as:

```text
A = [
    [0, 1, 1, 0, 0, 0],  # Vertex 1
    [0, 0, 1, 0, 1, 0],  # Vertex 2
    [0, 0, 0, 1, 0, 0],  # Vertex 3
    [0, 0, 0, 0, 1, 0],  # Vertex 4
    [0, 0, 0, 0, 0, 1],  # Vertex 5
    [0, 0, 0, 0, 0, 0]   # Vertex 6 (no outgoing edges)
]
```

---

## 3. Determinant Analysis

- The last row of matrix **A** contains only zeros.  
- A matrix with an all-zero row is **singular**.  
- Therefore: **det(A) = 0**.

This also indicates that the transformation represented by **A** is not invertible and that the graph is not strongly connected, since at least one vertex has no outgoing edges.

---

## 4. Technologies Used

- Python 3  
- NumPy  
- NetworkX  
- Matplotlib  

---

## 5. Project Files

- `notebooks/graph_analysis.ipynb` – main notebook with explanations, determinant calculation, and graph visualization.  
- `src/matrix_operations.py` – helper functions to work with adjacency matrices.  
- `requirements.txt` – Python dependencies.

---

## 6. How to Run

```bash
pip install -r requirements.txt
jupyter notebook
```

Then open the notebook in the `notebooks/` folder:

```text
notebooks/graph_analysis.ipynb
```

---

## 7. Repository Structure

```text
graph-adjacency-matrix-analysis/
│
├── notebooks/
│   └── graph_analysis.ipynb
│
├── src/
│   └── matrix_operations.py
│
├── data/
│   └── (optional files, e.g. saved graph images)
│
├── README.md
└── requirements.txt
```

---

## 8. Author

**Nathalia Rüesch Neiva**  
Data Science & Behavioral Analysis Student  
Based in Bern, Switzerland
