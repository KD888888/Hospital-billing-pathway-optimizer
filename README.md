# Hospital-billing-pathway-optimizer
NLP-based optimization of hospital billing workflows using Word2Vec and Topic Modeling
# Hospital Billing Pathway Optimizer (Word2Vec + Topic Modeling)

## Project Overview

Billing workflows in hospitals are mission-critical but rarely optimized using modern machine learning.  
Manual billing processes are slow, inconsistent, and fragmented, leading to:

- Claim rejections
- Revenue leakage
- Delays in reimbursement
- Increased operational overhead

This project introduces a data-driven **Hospital Billing Pathway Optimizer** using **representation learning (Word2Vec)** and **topic modeling (LDA)** to learn hidden operational patterns from real hospital billing logs.

Rather than recommending products or users, this system models **process behaviour** — an underexplored but high-impact application of NLP-based machine learning.

---

## 💡 Impactful Use Case (Non-Generic, Real-World Driven)

### 🔍 Problem:  
Hospitals do not have visibility into:
- why some billing cases flow smoothly
- why others require corrections
- where inefficiencies are silently accumulating

### ✅ Solution:
We model *billing workflows as language*:

| Billing System | NLP Equivalent |
|----------------|----------------|
| Activity | Word |
| Case | Sentence |
| Billing Flow | Document |
| Process Pattern | Topic |

Using natural language techniques, the system:
- learns which billing activities usually go together
- recomposes "healthy" billing flows
- flags abnormal sequences
- recommends next best steps

---

## ✅ What This System Can Do

### 1️⃣ Learn Smart Billing Sequences  
Trains a **Word2Vec model** on real billing activity sequences to capture how billing steps influence one another.

### 2️⃣ Recommend Next Best Billing Step  
Given a live partial billing workflow, the system recommends:
- most probable next actions
- operationally similar activities
- alternatives when a flow deviates

### 3️⃣ Detect Hidden Billing Process Types  
Applies **LDA Topic Modeling** to discover:
- fast-track pathways
- error-heavy flows
- correction-dominant cases
- administrative bottlenecks

### 4️⃣ Visualize Process Behaviour  
- UMAP embedding plots
- Distribution of discovered workflow topics
- Frequency distributions of billing steps

---

## 🧠 Machine Learning & Algorithms Used

### Representation Learning:
- Word2Vec (Skip-Gram Architecture)

### Dimensionality Reduction:
- UMAP

### Topic Modeling:
- Latent Dirichlet Allocation (LDA)

### Vectorization:
- CountVectorizer (Bag of Activities)

### NLP Methodology:
- Distributional Semantics
- Context-driven embeddings
- Sequence learning

---

## ⚙️ Technology Stack

| Component | Used |
|------------|------|
| Language | Python 3 |
| Machine Learning | Gensim |
| Visualization | Matplotlib |
| Process Mining | PM4Py |
| Topic Modeling | Scikit-Learn |
| Dimensionality Reduction | UMAP |
| Platform | Google Colab |
| Data Format | XES Event Logs |

---

## 📂 Dataset

This project uses **public hospital billing event logs** in `.xes` format.

You can replace the event log with any process mining dataset:

