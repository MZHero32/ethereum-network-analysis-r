# Ethereum Network Analysis with R

A graph-analysis project exploring Ethereum exchange and stablecoin address data through directed-network visualization, centrality measures, and community detection.

**Tools shown:** R, tidyverse, readr, and igraph.

## Available materials

- [Project presentation](presentation/ethereum_network_analysis.pptx): 30-slide presentation with student identification numbers removed with code screenshots and analysis figures.
- [Methodology notes](docs/methodology.md): workflow and interpretation limits.
- Network visualization extracted from the supplied presentation.

![Network visualization from the presentation](images/network_visualization.png)

## Topics covered

| Area | Methods shown in the presentation |
| --- | --- |
| Data preparation | CSV import, structure inspection, summaries, missing values, duplicates |
| Graph construction | Directed graph with igraph |
| Centrality | In-degree, out-degree, betweenness, closeness |
| Communities | Walktrap and edge-betweenness clustering |
| Representation | Adjacency matrix and important-node inspection |

## Data reference

The presentation references the [Stanford SNAP AlphaCore Ethereum Exchanges dataset](https://snap.stanford.edu/data/ethereum-exchanges.html), specifically `alphacore_labels_stablecoin.csv`. The original CSV and executable R files are not included in the recovered materials.

## Implementation status

This repository currently presents the project through its original slides, code screenshots, and figures. It is not a runnable R package or a complete reproduction of the transaction-network analysis. See the methodology notes before interpreting graph results.

## Contributors

The original presentation credits Mohamed Zoher Mohamed and Abdelrahman Mohamed Abdelfattah. Student identification numbers have been removed for public sharing. It is preserved as a team project; individual task ownership is not specified in the surviving materials.
