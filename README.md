Product Recommendation Engine: Association Rules & Graph Analytics
📌 Project Overview
Developed during DataHack, a hackathon organized by CSE (Club Scientifique de l'ESI) at the National School of Computer Science (ESI Algiers). This project implements a hybrid recommendation system that combines Association Rule Mining with Graph Theory to predict the most likely next item a user will interact with based on their current "item set".

🚀 Research & Industry Relevance
This project demonstrates the practical application of structured knowledge systems. By representing product interactions as a graph and applying frequent itemset mining, we move beyond simple correlations to understand the structural "communities" and "influence" within a marketplace.  

🛠️ Technical Stack
Engine: PySpark (SparkSession & SparkContext) for scalable, parallelized data processing.

Algorithms: F-Growth (Frequent Pattern Growth) for association rule mining.

Graph Analysis: NetworkX (implied) for computing Betweenness Centrality and Community Detection.


Language: Python.  

📊 Methodology
1. Frequent Itemset Mining (F-Growth)
Used the F-Growth algorithm to identify patterns in transactions without the need for candidate generation.

Association Rules: Generated rules to define the strength of relationships between items (support, confidence).

2. Graph-Based Knowledge Extraction
Constructed a graph from co-purchase data where nodes represent products and edges represent frequent co-occurrences.

Community Detection: Applied label propagation to identify clusters of related products, helping the system understand product "categories" autonomously.

Betweenness Centrality: Calculated centrality scores to find "bridge" products that link different item communities, which are critical for diverse recommendations.

3. Predictive Logic
Developed a prediction pipeline that takes an existing item set and queries the hybrid model to identify the "most appropriate item" by combining the probabilistic strength of association rules with the structural position of the item in the graph.

📁 Repository Structure
store.ipynb: The primary notebook containing the Spark pipeline, graph analysis, and prediction logic.

data/: Directory for item_sets.txt and graph.txt (dataset descriptions).

💡 Key Features
Scalability: Built with Spark to handle large-scale transactional datasets.

Hybrid Approach: Merges statistical mining (F-Growth) with topological analysis (Graph Theory).

Automated Clustering: Uses community detection to organize complex product information into logical groups.

Author: Oussama Abderraouf ATTIA
