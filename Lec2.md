# Lecture 2 

### I.what is search

#### 1.1.background

#####    PEAS

- Performance, Environment, Actuators, Sensors (artificial intelligence task environment)
-  define what is a good solution.

#####    Representation

- How to organize the search space **but not** to make it smaller



#####    Search space

- defined by the solution representation
- reduce the possibilities (sequence)
- combine with good algorithm



#### 1.2.The State-Space formulation

- **states**: All reachable states from the initial state
- **initial state**: the state at beginning
- **Action:**
- **Transition model**:
- **Goal test:**
- **Path cost:**

### II.Search tree

#### 2.1 representation of search tree

1. ***formulize the process of searching***
2. ***A branch (from the root to the leaf) is a path in the graph***

> - **states**: the current node
> - **initial state**: the node at beginning
> - **Action: **move from one node to another node
> - **Transition model**:  pick the order of node expansion
> - **Goal test:** How many movements it has to make to reach  the goa;
> - **Path cost:** 



#### 2.2 performance matrix

- **Completeness**:  Whether it always can find a solution **(*the cost of every step must be finite*)**

- **Optimality**:  Whether it always can find the best solution

- **Time complexity**:  nbcs    **(*should consider basic operation***)

  > **matrix inversion** and **bubble sort** are has the same time complexity (O(n^2)), but their action are different.

- **Space complexity**:    nbcs

  ​

**three domains of time complexity**

| b    | d    | m    |
| ---- | ---- | ---- |
| ??   |      |      |

### III.Formal search

#### 3.1 BFS

1. implement: Use queue  (FIFO)
2. ?????:

> - **Completeness**:  yes
> - **Optimality**:  yes
> - **Time complexity**:  好大好大  
> - **Space complexity**:   好大好大

#### 3.2 Uniform-cost search (UCS)

1. implement:
2. ?????:

> - **Completeness**:  yes
> - **Optimality**:  yes
> - **Time complexity**:  好大好大  
> - **Space complexity**:   好大好大 

#### 3.3 DFS

1. implement: stack (LIFO)
2. ?????:

> - **Completeness**:  no
> - **Optimality**:  no
> - **Time complexity**:  好大好大  
> - **Space complexity**:   好大好大 

#### 3.4 DLS (Depth limited search)

1. implement:
2. ?????:

> - **Completeness**:  no
> - **Optimality**:  no
> - **Time complexity**:  好大好大  
> - **Space complexity**:   好大好大 

#### 3.5 IDS (Iterative Deepening Search)

1. implement:
2. combine the advantages of BFS and DFS

> - **Completeness**:  no
> - **Optimality**:  no
> - **Time complexity**:  好大好大  
> - **Space complexity**:   好大好大 

### IV.Informal search

new solution: (optimal but slow) + ( not optimal but fast )

Bidirectional search : search from the start point and the goal , build two sub trees, it find the solution when these two sub trees meet 

- **Completeness**:  yes (sub tree implemented by BFS)
- **Optimality**:  yes (sub tree implemented by BFS)
- **Time complexity**:  
- **Space complexity**: 
- **Weakness**:  