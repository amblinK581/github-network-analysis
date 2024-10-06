# github-network-analysis
Open Source Ecosystems - Behavioral Insights from GitHub's Development Network: Conducted social network analysis of the GitHub developer community using R, applying ERGM to infer the underlying social mechanisms driving collaboration and diversity, providing insights to foster cross-disciplinary interactions and inform platform engagement strategies
This repository contains the project “Open Source Ecosystems - Behavioral Insights from GitHub’s Development Network.” The project focuses on analyzing collaboration patterns among developers on GitHub, using social network analysis (SNA) and Exponential Random Graph Models (ERGM) to uncover the social mechanisms driving collaboration and diversity.

Project Overview

This project aims to understand how individual behaviors and social dynamics shape the structure and evolution of the open-source software development community on GitHub. By analyzing the network of mutual follower relationships among developers, we provide insights into collaboration trends, community formation, and diversity within the GitHub ecosystem. These insights inform strategies to foster cross-disciplinary interactions and enhance platform engagement.

Table of Contents

	•	Introduction
	•	Data Source
	•	Methodology
	•	Results
	•	Conclusion
	•	How to Use This Repository
	•	Requirements
	•	License
	•	Authors

Introduction

The GitHub developer network is a dynamic space for collaboration, where individual behaviors and group dynamics play a key role in shaping the ecosystem. This project seeks to uncover these patterns by applying social network analysis and ERGM to explore how developers form connections, collaborate, and drive innovation across different fields.

Data Source

	•	GitHub API: The data was collected from GitHub’s API (June 2019) and includes 37,700 nodes (developers) and 289,003 edges (follower relationships).
	•	Node Features: Developer type (web developer or machine learning developer).
	•	Network Metrics: Network density (0.001) and transitivity (0.013), which indicate the overall structure and connectedness of the network.

Methodology

	1.	Exploratory Data Analysis:
	•	Analyzed various centrality measures (degree, closeness, eigenvector, and betweenness centrality) to understand the roles of developers in the network.
	•	Detected communities using graph-based approaches to identify clusters of developers based on collaboration patterns.
	2.	Community Analysis:
	•	Examined the distribution of web developers and machine learning developers across the network.
	•	Analyzed homophily (the tendency for similar nodes to connect) to understand the diversity of collaborations.
	3.	ERGM Analysis:
	•	Applied Exponential Random Graph Models (ERGM) to infer the underlying social mechanisms shaping the network.
	•	Tested for factors like density, node type, and homophily to understand the likelihood of different types of developers connecting.

Results

	•	Community Insights: Web developers formed more cohesive and tightly connected groups, while machine learning developers were more distributed, providing opportunities for cross-disciplinary collaboration.
	•	Homophily Findings: Strong homophily was observed, with web developers primarily connecting with other web developers, while machine learning developers showed more cross-disciplinary interactions.
	•	ERGM Findings: Statistically significant results showed that developer type (web vs. machine learning) strongly influenced connection patterns, with a slight preference for machine learning developers to form connections.

Conclusion

Our analysis provides key insights into the collaboration dynamics within GitHub’s open-source ecosystem. By understanding the social and behavioral factors that drive connections, platform developers can enhance recommendation algorithms and create initiatives that foster more diverse collaborations.

How to Use This Repository

	1.	Data: The data/ folder contains the preprocessed network dataset of GitHub developers.
	2.	Scripts: The scripts/ folder includes R code for performing social network analysis and ERGM modeling.
	3.	Results: The results/ folder contains visualizations and analysis results from the network analysis.
	4.	Report: The final project report is available in the docs/ folder.

Requirements

	•	R 4.x or higher
	•	Required libraries: igraph, ergm, ggplot2, dplyr

Install the required libraries by running:

install.packages(c("igraph", "ergm", "ggplot2", "dplyr"))


Authors

	•	Shruti Gupta
	•	Tzu-Hsuan Lin
	•	Stacy Shang
	•	Cathy Zhang
