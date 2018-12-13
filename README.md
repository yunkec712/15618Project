## Parallel Strassen’s Matrix Multiplication with OpenMPI
by Yunke Cao and Yuhao Lei

[Proposal](./proposal.html).

[Checkpoint](./checkpoint.html).

[Final Report](./15618 Final Report.pdf)

Current Schedule

| Work                                               | Participants         | Progress         |
|----------------------------------------------------|----------------------|------------------|
| (11/16) Design the structure for the BFS variation | Yuhao Lei, Yunke Cao | Done             |
| (11/30) Implement BFS variation of CAPS            |       Yuhao Lei      | Done (12.2)      |
| (12/05) BFS version verification and optimization  | Yuhao Lei, Yunke Cao | Done (12.2)      |
| (11/30) Design the structure for DFS variation     | Yunke Cao, Yuhao Lei | Done             |
| (12/05) Implement DFS variation of CAPS            |       Yunke Cao      | Done             |
| (12/10) DFS version verification and optimization  | Yunke Cao, Yuhao Lei | Done             |
| (12/14) Have our poster ready                      | Yuhao Lei, Yunke Cao | Done             |
| (12/15) Final report                               | Yuhao Lei, Yunke Cao | Done             |
| (Canceled) Extra goal: benchmark test              | Yuhao Lei, Yunke Cao | Canceled         |
| (12/16) Poster session                             | Yuhao Lei, Yunke Cao |                  |

We canceled the extra goal. The reason is that we tried to find some OpenMPI implementation of Strassen's algorithm. The ones we found on Github are either: cannot compile at all, or cannot accept input matrix with large enough size to compare performance.
