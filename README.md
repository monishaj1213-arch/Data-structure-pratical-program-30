from collections import defaultdict

class Graph:
    def __init__(self):
        self.graph = defaultdict(list)

    def add_edge(self, u, v):
        self.graph[u].append(v)

    def print_graph(self):
        for node in self.graph:
            print(node, "->", self.graph[node])

# Example usage
g = Graph()
g.add_edge(0, 1)
g.add_edge(0, 2)
g.add_edge(1, 3)
g.add_edge(2, 4)

g.print_graph()
# Output:
# 0 -> [1, 2]
# 1 -> [3]
# 2 -> [4]# Data-structure-pratical-program-30
