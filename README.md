# Complex-Networks---Community-Detection

In this task, I was very ambitious and I thought it will be the opportunity to learn more about the
different algorithms that would help me to do community detection as best as possible. Some of the
algorithms are used in igraph and will be as well helping me to plot the different partitions. An
addition was to use algorithms using networkx to have a comparison table just as we did use igraph
algorithms. The overall objective behind what I did is just to compare the overall performance of the
algorithms and get to the conclusion ”What’s the best algorithm?”
- Fast Greedy : The communityfastgreedy algorithm bases its modularity optimization on a greedy
strategy. In order to generate clusters that maximize the modularity score, nodes or groups of nodes
are gradually merged. Although this method is quick, it might not always result in the modularity
function’s global maximum.
- Optimal Modularity : The communityoptimalmodularity algorithm is another that has been
tested. To identify the partition that has the maximum modularity score, this algorithm does a
thorough search. However, this computation may take a while for big networks.
- Label Propagation : The label propagation algorithm created by Raghavan, Albert, and Kumara
serves as the foundation for the communitylabelpropagation algorithm. By using a majority vote, this
technique first assigns a node an initial label before propagating that label to any nearby nodes. Up
until there are no more label modifications, this process is repeated. Depending on the initial labeling,
the algorithm’s nondeterministic output may differ.
- Leading Eigenvector : Using the eigenvectors of the modularity matrix, the community-leading
eigenvector method maximizes modularity. The pairwise connections between nodes in a network
are encoded in the modularity matrix, which is a matrix. This matrix’s eigenvectors can be used to
determine which nodes are most crucial for maximizing modularity. Although this approach might
take longer than the communityfastgreedy algorithm, it might yield superior outcomes.
- Louvain : A community recognition approach called the Louvain algorithm maximizes modularity,
a metric for the effectiveness of dividing a network into communities. It accomplishes this by repeatedly
merging communities that raise the modularity rating until no more advancements are possible. The
technique is a preferred option for extensive network research because of its speed and scalability.
For the added Networkx algorithms, we can explain them as follows :
- Greedy Modularity : The communityfastgreedy algorithm in igraph is comparable to the greedymodularitycommunities
algorithm.
- Label Propagation : The communitylabelpropagation algorithm in igraph is comparable to the
labelpropagationcommunities algorithm.
- Louvain : The louvain algorithm in igraph is comparable to the louvainnx algorithm.
- Kclique : The kcliquecommunities approach was also tested, and we had to change k in order to
get good comparison results. In fact, the algorithm searches for densely linked subgraphs of a network
known as k-cliques, where k is a parameter that establishes the minimum size of the subgraph. All
k-cliques in the network are first identified by the algorithm, which then combines them to create
larger communities. The resulting communities’ sizes are not specified, and they may overlap. The
network’s properties and the required level of granularity in the community structure must be taken
into consideration while selecting the k value.
