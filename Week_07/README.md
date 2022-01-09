The goals of this week of exercises was to construct a large network in an easy way and to know where the complex network analysis fits in the context of other subjects and disciplines.

The Wikipedia was used to create the network. We start with a chosen wikipedia page—the seed page. To build a network out of the seed page and other relevant pages, we treat the pages (and the respective Wikipedia subjects) as the network nodes and the links between the pages as the network edges. We use snowball sampling (a breadth-first search or BFS algorithm) to discover all the nodes and edges of interest.


The steps followed were:

- Get the Data, Build the Network

- Eliminate Duplicates

- Truncate the network

- Explore the network

To analize the data, we used Gephi, wich is a graphic visualization software. Gephi implemets the Modularity Class, that automatically split the dataset into groups using the modularity value. The different groups were painted in different colors and the nodes were resized, based on their In Degree.

Acess the network: https://matheusriv.github.io/network_analysis_2021_exercises/Week_07/network/
