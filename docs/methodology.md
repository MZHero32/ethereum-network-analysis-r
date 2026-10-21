# Methodology and interpretation

## Preserved workflow

The presentation shows importing the stablecoin address-label CSV with readr, inspecting its structure and summary, checking missing and duplicate entries, constructing a directed igraph graph, computing centrality, and visualizing communities and adjacency information.

## Graph meaning

The visible code calls `graph_from_data_frame(ethereum_data, directed = TRUE)` on the imported address-label table. With no explicit edge selection, igraph uses its first two columns as endpoints. The referenced label file describes `(label, address, name, asset)`, so that construction represents label-to-address associations rather than observed transfers between wallet addresses.

The SNAP dataset also contains weighted directed token transaction networks, but the original transaction edge files are not included here. The scope of this archived implementation should therefore not be confused with a verified analysis of the complete transaction network.

## Results in the slides

The presentation reports Uniswap as an important label and shows an out-degree value of 133. These are recorded claims from the original presentation, not recalculated results.

Zero betweenness alone does not establish that there are no graph bridges. Closeness values alone do not establish that every node is reachable from every other node. Connectivity and bridge claims require direct checks on the exact graph and its directionality.

The available materials do not establish whether community detection used a directed or undirected conversion. This choice should be made explicit in any future reproduction.

## Source

Stanford SNAP: https://snap.stanford.edu/data/ethereum-exchanges.html

F. Victor, C. G. Akcora, Y. R. Gel, and M. Kantarcioglu. Alphacore: Data Depth based Core Decomposition. ACM SIGKDD, 2021.
