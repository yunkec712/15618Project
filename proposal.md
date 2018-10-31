## Proposal

### Summary

Our project is to implement a parallel Strassen’s matrix multiplication algorithm with OpenMPI on the latedays cluster.

### Background
Strassen’s matrix multiplication algorithm is a famous divide-and-conquer algorithm. Compared to the classical matrix multiplication algorithm, it reduces the number of subblock multiplications in each iteration from 8 to 7. Parallelizing Strassen’s matrix multiplication is a challenging and well-studied problem. Various parallel algorithms are presented by researchers to improve the performance of the problem. In our project, we limit our interest in using Message Passing Model to parallel Strassen’s matrix multiplication algorithm.

### Challenges

Keep communication cost at a low level. In our previous experience, the communication cost across nodes are pretty high. In our implementation, we should reduce the unnecessary communication among cores and optimize the communication cost in the algorithm. That is, to increase the computation-communication ratio.

Make full use of the memory. In order to keep communication cost at a low level, our implementation should use as much local memory as possible. However, there’s limitation in local memory capacity. Thus, our implementation needs to figure out how to make a tradeoff between the communication cost and the memory usage.

### Resources

#### Computers
The latedays cluster at CMU.

#### Code
We are going to start from scratch with the OpenMPI as the message passing implementation.

#### Paper & Algorithm
We are going to implement and experiment on the Communication-Optimal Parallel Algorithm (CAPS) presented by Grey Ballard in 2012. The algorithm is based on the Strassen-Winograd algorithm, which is a faster slight variation of Strassen’s algorithm. 

Reference: Grey Ballard, James Demmel, Olga Holtz, Benjamin Lipshitz, and Oded Schwartz. 2012. Communication-optimal parallel algorithm for strassen's matrix multiplication. In Proceedings of the twenty-fourth annual ACM symposium on Parallelism in algorithms and architectures (SPAA '12). ACM, New York, NY, USA, 193-204. DOI: https://doi.org/10.1145/2312005.2312044

#### Goals and Deliverables

Grey Ballard presented two variations of CAPS as they traverse the recursive tree of the Strassen-Winograd algorithm in either BFS or DFS. Our first goal is to have the correct implementation of both of them.

Our second goal is to experiment these two variations on different problem size and environment settings (number of nodes, memory limits). In the poster session, we plan to show the speedup graphs.

#### Extra Goal:

When time permits, we are planning to compare our implementation with other matrix multiplication algorithms that adopt the message passing model. Design some benchmark tests and record the different metrics.

### Platform Choice

* Programming Language: C/C++
* Tools: OpenMPI

Since we want to explore the problem in the message passing model and run it on the latedays cluster. C/C++ and OpenMPI is a suitable choice.

### Schedule

* Week One (11/04): Read the paper, understand the algorithms
* Week Two (11/11): High-level design of the code, implement a serialized version of Strassen-Winograd.
* Checkpoint Report by (11/15)
* Week Three (11/18): Implement the BFS variation of CAPS
* Week Four (11/25): Implement the DFS variation of CAPS
* Week Five (12/02): Experiment and optimize the two versions
* Week Six (12/09): Extra Goal
* Week Seven (12/15): Wrap up and Final report
