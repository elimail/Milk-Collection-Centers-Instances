# Milk-Collection-Centers-Instances
The file format is a CPLEX-like input format.
- First item (set Nodes: =) lists the whole set of nodes: The first one (Id = 1000) is the depot.
- Second item (set I: =) lists the set of farms. It excludes the depot.
- Third item (set C: =) lists the set of available places to locate collection centers. Places that are available to locate more than one collection center are repeated in this list.
- Fourth item (MC: =) lists the maximum number of collection centers to settle.
- Fifth item (set K: =) lists the available trucks.
- Sixth item (param Q: =) lists for each truck their capacity and type (large or small routes)
- Seventh item (MT: =) lists the maximum number of small trucks available in each collection center.
- Eighth item (param P: =) lists the milk of each type to collect (A, B, and C)
- Nineth item (param qu: =) lists the production and type of milk of each node (1 = milk A, 2 = milk B, and 3 = milk C). It lists the depot and farms.
- Tenth item (param cap: =) lists the capacity of each collection center. In some locations, there is possible to allocate collection centers of any type. In these cases, one line per milk type can be found in this list.
- Last item (param c [*, *]) shows the distance matrix between nodes. The first line shows the ids of nodes. In all the following lines, the first column shows the id of the corresponding node. Id = 1000 is reserved for the depot.
