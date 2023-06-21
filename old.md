
## Topic: Music Preferences and Social Connections in Three European Countries: A Social Network Analysis

# Abstract
In this project, we will analyze the relationship between music preferences and social connections in three European countries - Romania, Croatia, and Hungary. We will create friendship networks for each nation using information from music streaming provider Deezer, and we will look at the musical genres that are most popular among users in each network To explore the patterns and relationships in the data, with the goal of identifying groups of users with similar music preferences and social connections we will use social network analysis (SNA) methods.

# Introduction
Music plays an important role in people's lives and has the power to evoke emotions, memories, and social connections. In the digital age, music streaming services like Deezer have made it easier for people to access and discover music from all over the world. As a result, music has become a global phenomenon that transcends national and cultural boundaries.

This project aims to explore the relationship between music preferences and social connections in Romania, Croatia, and Hungary. By analyzing Deezer user friendship networks, the project seeks to uncover insights into how music can shape social connections and interactions. This project can provide insights in understanding the social dimensions of music consumption. By using social network analysis methods, the project hopes to contribute to our understanding of the ways in which music influences social connections and relationships in different cultural contexts. So, the goal of this project is to use social network analysis methods to analyze the friendship networks and genre preferences of users.

To achieve this goal, we will take the following steps:

+ Acquire and preprocess the data: We will obtain the data from [Stanford Large Network Dataset Collection](https://snap.stanford.edu/data/gemsec-Deezer.html) and preprocess it to prepare it for analysis.
+ Construct the friendship networks: We will construct the friendship networks for each country.
+ Analyze the genre preferences: We will examine the genre preferences of users in each country.
+ Perform social network analysis: We will use social network analysis methods to explore the patterns and relationships in the data, including measures of centrality, clustering, and similarity.
+ Visualize the results: We will use various visualization techniques to present the results of our analysis and identify groups of users with similar music preferences and social connections.

# Main Part
## Literature Review
Detecting the cross-cultural differences in music preferences across social connections is a challenging problem and various methods have been suggested to tackle it, but the quantity of information is pretty small. In this section, we will review some of the relevant research on this subject.

There are several popular community algorithms in network analysis, but they differ in their approach and complexity, for example, the Louvain method and the Girvan-Newman algorithm (Blondel et al., 2008; Girvan & Newman, 2002). The Louvain method uses iterative association of communities, while the Girvan-Newman algorithm uses sequential removal of edges to find communities in the network. The Louvain Method, was used to identify communities among music genres and to analyze the social networks of lastfm users in their work Dolgikh and Jelínek (2015). These authors, as well as other studies emphasize that this method is superior to others in terms of computation time.

For the genres preferences analysis and cross-cultural comparison we plan to use a matrix of pairwise Jaccard similarity coefficients for each country's users based on their genre preferences to understand the degree of similarity between users and compare network characteristics upper mentioned to to identify any similarities or differences. Regarding this part, we plan to use hypothesis testing such as t-tests or ANOVA to test for statistically significant differences in network and genre preference characteristics between the countries.

## Anticipated SNA Methods
Thus, the anticipated SNA methods for this project include measures of centrality (e.g., degree, betweenness, and closeness), community detection (Louvain Method) and similarity (e.g., Jaccard similarity coefficient). We will also use some statistical methods and visualization techniques, such as network graphs and heatmaps, to explore the data.

## Expected Results
We expect to identify groups of users with similar music preferences and social connections in each country. We also expect to find that music preferences are correlated with social connections, and that users with similar music preferences are more likely to be connected in the friendship network. By identifying these patterns and relationships, we hope to gain insights into the ways in which music can shape social connections and relationships in different cultural contexts.

# References

Blondel, V. D., Guillaume, J., Lambiotte, R., & Lefebvre, E. (2008). Fast unfolding of communities in large networks.Journal of Statistical Mechanics: Theory and Experiment, 2008(10), P10008. https://doi.org/10.1088/1742-5468/2008/10/p10008

Dolgikh, D. A., & Jelínek, I. (2015). Graph-based music recommendation approach using social network analysis and community detection method. https://doi.org/10.1145/2812428.2812453

Girvan, M., & Newman, M. (2002). Community structure in social and biological networks. Proceedings of the National Academy of Sciences of the United States of America, 99(12), 7821–7826. https://doi.org/10.1073/pnas.122653799

SNAP: Network datasets: Graph Embedding with Self Clustering: Facebook and Deezer. (n.d.). https://snap.stanford.edu/data/gemsec-Deezer.html
