# Product Recommendation Engine: Association Rules & Graph Analytics

---

## 📌 Project Overview
Developed during **DataHack**, a hackathon organized by **CSE (Club Scientifique de l'ESI)** at the **National School of Computer Science (ESI Algiers)**.  
This project implements a hybrid recommendation system that combines **Association Rule Mining** with **Graph Theory** to predict the most likely next item a user will interact with based on their current *"item set"*.

---

## 🚀 Research & Industry Relevance
This project demonstrates the practical application of **structured knowledge systems**.  
By representing product interactions as a graph and applying frequent itemset mining, we move beyond simple correlations to understand the structural *"communities"* and *"influence"* within a marketplace.

---

## 🛠️ Technical Stack

### ⚙️ Engine
- **PySpark** (SparkSession & SparkContext) for scalable, parallelized data processing

### 🧠 Algorithms
- **F-Growth (Frequent Pattern Growth)** for association rule mining

### 📊 Graph Analysis
- **NetworkX (implied)** for:
  - Betweenness Centrality
  - Community Detection

### 💻 Language
- **Python**

---

## 📊 Methodology

---

## 1. Frequent Itemset Mining (F-Growth)

Used the **F-Growth algorithm** to identify patterns in transactions without the need for candidate generation.

- **Association Rules:** Generated rules to define the strength of relationships between items  
  (support, confidence)

---

## 2. Graph-Based Knowledge Extraction

Constructed a graph from co-purchase data where:
- **Nodes = Products**
- **Edges = Frequent co-occurrences**

### 🔹 Community Detection
Applied **label propagation** to identify clusters of related products, helping the system understand product *categories* autonomously.

### 🔹 Betweenness Centrality
Calculated centrality scores to find **"bridge" products** that connect different item communities, which are critical for diverse recommendations.

---

## 3. Predictive Logic

Developed a prediction pipeline that:
- Takes an existing **item set**
- Queries the hybrid model
- Identifies the **most appropriate next item**

This is achieved by combining:
- Probabilistic strength from **association rules**
- Structural importance from the **graph**

---

## 📁 Repository Structure
