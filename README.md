# Meetup Group Network Analytics
### CSE3021- Social and Information Networks Project 

---
### Dataset:

The dataset for this analysis is extracted from Kaggle. This dataset was primarily created for Networkx network analysis.For social analysis, we have two datasets that contain their network data and meta-data.

*  Member edges - A list of edges used to build a member-to-member graph. Weights indicate whether or not a person is a member of a shared group.It includes the following:Member1 is the first individual in the network, and Member2 is the second. Weight - Weights indicate whether or not a person is a member of a shared group. The total number of nodes is 11372. The total number of edges is 1176368.

* Group edges - A list of edges used to build a group-to-group graph. Members who are shared between groups are represented by weights. It includes the following: For the group to group graph, group1 and group2 create an edge list. The total number of nodes is 456. There are 6692 edges in total.

* meta-members - Information about each member, such as name and location. The index is member id.
It contains the following information: (member id, name, hometown, city, and state)
The following people are included in the dataset: 24591

* meta-groups - Information about each group, such as its name and classification. The index is group id.
It comprises the following information: (group id, group name, category name, group urlname, num-numbers).

* num-numbers: It shows how many people are in each group. 602 groups are included in the dataset.

---
### Proposed work:
* Meetup is a social media platform for people organizing and attending regular or semi-regular events ("meet-ups"). The relationships amongst users who are attending the meetup form a social network and is ideal for graph-based analysis. The Nashville Meetup Group relationship dataset is used to perform the analysis. The dataset consists of 1.17M members,spread over 456 meetup groups. First, we have calculated and set up the layout of the network from the relationship database. Mathematical analysis of the network (calculation of centralities), is done to identify different roles of individuals in the network ,for instance, the people who most influence the network, the people who influence the transfer of information and who are the best performers in information transfer.

* Further, we have performed visualization of the network to observe and analyze the network we are working with. Since the dataset is large, we have limited the visualization to a smaller subset.

* The next step is to calculate mathematical indicators from the theory of complex graphs such as centrality of proximity, betweenness centrality, eigenvector centrality in order to assign roles and make categories between individuals.We have utilized the member-to-member graph data to find out who are the people who has the highest "centrality" in the Nashville network.

* Next, we have analyzed the group-to-group graph of Nashville MeetUp data. For this graph, each node is considered an independent Nashville Meetup, and each edge is the number of shared members between each group. We import the data and create the graph. Next, we derive measures of the graph and add them to the dataframe. For plotting and visualizing the graphs, we have used seaborn and matplotlib. Finally, we analyzed the tech groups of the Nashville Meetup Network.

---
### Conclusion:

* Each meetup group is represented as a node in the Nashville meetup group data graph, and the edges show the weight of the link between pairs of meetups. There are 456 nodes and 6692 edges in the group dataset.

* In a network, the betweenness centrality measure finds key bridges. High centrality nodes are those that appear on many shortest pathways between other nodes in the network. The weighted distances between nodes are taken into account in the weighted form of betweenness.

* The group data analysis show the most central groups based on the centrality metrics. Betweenness centrality is measured by the ability of nodes in a network to connect divergent regions of that network.

* The Nashville meetup was further investigated by picking the largest group in the dataset, which was the tech group. It has the greatest degree with this community, with NashJS having 1975 members. The top five communities in the tech group with distinct groups in the network are shown above.

* The above analysis demonstrates the application of network analysis techniques to the datasets from meetup.com in Nashville. Based on centrality, the study of the Nashville meetups indicated the most important nodes. The names of the communities linked with the nodes were discovered using the meta data from the datasets. We discovered the communities in the network by using centrality measurements. Currently, only one city, Nashville, is being worked on. The findings of future research can be extended to other cities in order to identify the most strong communities. As a future project, we may create an application for providing meetup recommendations to individuals.


