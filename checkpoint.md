## Checkpoint

### Progress reporting

|                                                                                                |         |
|------------------------------------------------------------------------------------------------|---------|
| (11/04) Read the paper and understand the algorithms                                           |   Done  |
| (11/11) High-level design of the code, implement a serialized version of the Strassen-Winograd |   Done  |
| (11/15) Checkpoint report                                                                      |   Done  |
| Implement the BFS variation of CAPS                                                            | Ongoing |

Our current progress, which almost keeps up with our initial schedule, is good. We’ve already read through the reference paper and learned how Strassen-Winograd algorithm works. Besides, we achieved the serialized version of the algorithm and it works. However, due to the final exam of this course and several other dues, our implementation of the BFS variation of CAPS has been delayed. Luckily, it’s still under our control and we believe we would deliver the things we’ve planned.

Currently, as we have a better understanding of our final project, we’ve planned to make some modifications on our schedule to better trace and process our project. The updated schedule is listed below.


| Work                                               | Participants         |
|----------------------------------------------------|----------------------|
| (11/16) Design the structure for the BFS variation | Yuhao Lei, Yunke Cao |
| (11/25) Implement BFS variation of CAPS            |       Yuhao Lei      |
| (11/30) BFS version verification and optimization  | Yuhao Lei, Yunke Cao |
| (11/21) Design the structure for DFS variation     | Yunke Cao, Yuhao Lei |
| (11/30) Implement DFS variation of CAPS            |       Yunke Cao      |
| (12/04) DFS version verification and optimization  | Yunke Cao, Yuhao Lei |
| (12/09) Extra goal: design and run benchmark test  | Yuhao Lei, Yunke Cao |
| (12/14) Have our poster ready                      | Yuhao Lei, Yunke Cao |
| (12/15) Final report                               | Yuhao Lei, Yunke Cao |
| (12/16) Poster session                             | Yuhao Lei, Yunke Cao |

### Poster session plan

For the poster session, our plan is to show a graph to compare our parallel version of Strassen’s Matrix Multiplication with the serialized version. If time permits, we may add our extra goal’s result to the poster, too.

### Preliminary results

Till now, we’ve achieved the serialized version of the Strassen-Winograd algorithm and it works. There’s one important thing to point out is that the Strassen-Winograd algorithm given in the Appendix of the paper Communication-Optimal Parallel Algorithm for Strassen’s Matrix Multiplication is wrong. We’ve checked its issue based on a very simple matrix multiplication and our implementation has fixed the problem using the correct algorithm.

The implementation of the parallel version is ongoing.

### Summary

In total, our current process is good and everything is under our control.

