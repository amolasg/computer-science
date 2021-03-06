Analyze an algorithm :

1) Worst Case Analysis (Usually Done):In the worst case analysis, we calculate upper bound on running time of an algorithm by considering worst case  (a situation where algorithm takes maximum time)

2) Average Case Analysis (Sometimes done) :In average case analysis, we take all possible inputs and calculate computing time for all of the inputs.

3) Best Case Analysis (Bogus) :In the best case analysis, we calculate lower bound on running time of an algorithm.

Trees
     Trees: Unlike Arrays, Linked Lists, Stack and queues, which are linear data structures, trees are hierarchical data structures. Depth First Traversals: (a) Inorder (b) Preorder (c) Postorder

Binary Search Tree
                Binary Search Tree, is a node-based binary tree data structure which has the following properties:

                The left subtree of a node contains only nodes with keys less than the node’s key.
                The right subtree of a node contains only nodes with keys greater than the node’s key.
                The left and right subtree each must also be a binary search tree. There must be no duplicate nodes.

AVL Tree
        AVL tree is a self-balancing Binary Search Tree (BST) where the difference between heights of left and right subtrees cannot be more than one for all nodes.
B-Tree
        B-Tree is a self-balancing search tree. In most of the other self-balancing search trees (like AVL and Red Black Trees), it is assumed that everything is in main memory. To understand use of B-Trees, we must think of huge amount of data that cannot fit in main memory. When the number of keys is high, the data is read from disk in the form of blocks. Disk access time is very high compared to main memory access time. The main idea of using B-Trees is to reduce the number of disk accesses.

Graph
       Graph is a data structure that consists of following two components:
        1. A finite set of vertices also called as nodes.
        2. A finite set of ordered pair of the form (u, v) called as edge. The pair is ordered because (u, v) is not same as (v, u) in case of directed graph(di-graph). The pair of form (u, v) indicates that there is an edge from vertex u to vertex v. The edges may contain weight/value/cost. Following two are the most commonly used representations of graph.

        Adjacency Matrix: 
                        Adjacency Matrix is a 2D array of size V x V where V is the number of vertices in a graph.
        Adjacency List : 
                        An array of linked lists is used. Size of the array is equal to number of vertices. 

         Graph Algorithms 

            Breadth First Traversal for a Graph

                    Time Complexity : O(V+E) for adjacency list representation and O(V * V) for adjacency matrix representation.

            Depth First Traversal for a Graph 
                    Time Complexity :  
                    O(V+E) for adjacency list representation and O(V * V) for adjacency matrix representation. 

            Dijkstra’s shortest path algorithm 
                     Time Complexity : Adjacency matrix- O(V^2). Adjacency list- O(E log V) 

Minimum Spanning Tree
                    Minimum Spanning Tree (MST) problem: Given connected graph G with positive edge weights, find a min weight set of edges that connects all of the vertices. MST is fundamental problem with diverse applications.

                Network design– telephone, electrical, hydraulic, TV cable, computer, road
                Approximation algorithms for NP-hard problems –  traveling salesperson problem, Steiner tree
                Cluster analysis- k clustering problem can be viewed as finding an MST and deleting the k-1 most expensive edges.

                Example: Prim’s Minimum Spanning Tree Algorithm, Kruskal’s Minimum Spanning Tree Algorithm

Divide and Conquer  
                    Divide:Break the given problem into subproblems of same type.
                    Conquer: Recursively solve these subproblems
                    Combine: Appropriately combine the answers   

     Following are some standard algorithms that are Divide and Conquer algorithms.

        1) Binary Search is a searching algorithm. In each step, the algorithm compares the input element x with the value of the middle element in array. If the values match, return the index of middle. Otherwise, if x is less than the middle element, then the algorithm recurs for left side of middle element, else recurs for right side of middle element.

        2) Quicksort is a sorting algorithm. The algorithm picks a pivot element, rearranges the array elements in such a way that all elements smaller than the picked pivot element move to left side of pivot, and all greater elements move to right side. Finally, the algorithm recursively sorts the subarrays on left and right of pivot element.

        3) Merge Sort is also a sorting algorithm. The algorithm divides the array in two halves, recursively sorts them and finally merges the two sorted halves.

        4) Closest Pair of Points The problem is to find the closest pair of points in a set of points in x-y plane. The problem can be solved in O(n^2) time by calculating distances of every pair of points and comparing the distances to find the minimum. The Divide and Conquer algorithm solves the problem in O(nLogn) time.                           


Greedy Approach  
                Greedy is an algorithmic paradigm that builds up a solution piece by piece, always choosing the next piece that offers the most obvious and immediate benefit. Greedy algorithms are used for optimization problems. An optimization problem can be solved using Greedy if the problem has the following property: At every step, we can make a choice that looks best at the moment, and we get the optimal solution of the complete problem. 
                
    Following are some standard algorithms that are Greedy algorithms.

    1) Kruskal’s Minimum Spanning Tree (MST): In Kruskal’s algorithm, we create a MST by picking edges one by one. The Greedy Choice is to pick the smallest weight edge that doesn’t cause a cycle in the MST constructed so far.

    2) Prim’s Minimum Spanning Tree: In Prim’s algorithm also, we create a MST by picking edges one by one. We maintain two sets: set of the vertices already included in MST and the set of the vertices not yet included. The Greedy Choice is to pick the smallest weight edge that connects the two sets.

    3) Dijkstra’s Shortest Path: The Dijkstra’s algorithm is very similar to Prim’s algorithm. The shortest path tree is built up, edge by edge. We maintain two sets: set of the vertices already included in the tree and the set of the vertices not yet included. The Greedy Choice is to pick the edge that connects the two sets and is on the smallest weight path from source to the set that contains not yet included vertices.

    4) Huffman Coding: Huffman Coding is a loss-less compression technique. It assigns variable length bit codes to different characters. The Greedy Choice is to assign least bit length code to the most frequent character.

Dynamic Programming    
                    Dynamic Programming is an algorithmic paradigm that solves a given complex problem by breaking it into subproblems and stores the results of subproblems to avoid computing the same results again. Properties:

        1.Overlapping Subproblems: Dynamic Programming is mainly used when solutions of same subproblems are needed again and again. In dynamic programming, computed solutions to subproblems are stored in a table so that these don’t have to be recomputed.
    Uses: Fibonacci Numbers

        2.Optimal Substructure: A given problems has Optimal Substructure Property if optimal solution of the given problem can be obtained by using optimal solutions of its subproblems.

    Uses: Longest Increasing Subsequence, Shortest Path Two Approaches:

    1.Memoization (Top Down)
    2.Tabulation (Bottom Up)
    Examples: Floyd Warshall Algorithm, Bellman–Ford Algorithm for Shortest Paths

 BackTracking
             Backtracking is an algorithmic paradigm that tries different solutions until finds a solution that “works”. Backtracking works in an incremental way to attack problems. Typically, we start from an empty solution vector and one by one add items .Meaning of item varies from problem to problem. 
             Example: Hamiltonian Cycle
             





                


