**PROBLEM**(Expanded node indexing):
A. Each node needs to be referenceable by any other node.
B. There are at least as many node as Natural numbers (probably more than Real numbers).
C. It is impossible to enumerate all of those with any set of finite numbers.
Therefore:
D. It is impossible to have all nodes present in memory at the same time.
E. It is impossible to have static reference to them by a natural number or hash.

**SOLUTION**:
Create Indexing Scheme that can specify simple and complex indexes depending on needs.
Each indexing scheme can be referenced by a small hash, and be stored in a dictionary.
Then every reference to a node, would contain the hash of the scheme and the contents of the actual index.
Example indexing schemes could be as follows:
- creation Hash - for in-memory nodes that could change their value
- type&value hash - for static in-memory nodes
- type enum & value string / blob - for static nodes
- type enum & value hash - for nodes with values stored in dictionary
- type enum & static connections - for nodes uniquely identifiable by their connections
- type enum & value string / blob & static connections - for nodes uniquely identifiable by their connections and values

This however may increase the size of memory footprint and execution time. To mitigate this, reoccurring indexes could be hashed and stored in a dictionary. Meaning that during run time, all used nodes (including virtual and static) would be in-memory.

This method could be expanded to include referencing sub graphs and general indexes.