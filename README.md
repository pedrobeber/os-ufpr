# os-ufpr
Projects for the Operating Systems course at UFPR (Prof. Carlos Maziero), following the [PingPongOS](https://wiki.inf.ufpr.br/maziero/doku.php?id=ppos-v2:start) roadmap: a small teaching kernel written in C that runs as a user-space library, with tasks built on `ucontext`. Each folder `p0` … `p13` is one step and builds on the previous one.

| Dir | What was implemented |
|---|---|
| p0 | Generic doubly linked queue (`queue.c`) used by the whole kernel |
| p1 | Context-switch experiments with `getcontext` / `makecontext` / `swapcontext` |
| p2 | Cooperative tasks: `task_create`, `task_switch`, `task_exit`, `task_yield` |
| p3 | Task dispatcher with a ready queue |
| p4 | Priority scheduler with dynamic priorities (aging) |
| p5 | Time-slice preemption driven by a timer signal (quantum) |
| p6 | Clock and per-task accounting (execution time, CPU usage, activations) |
| p7 | The `main` task made a normal, schedulable task |
| p8 | Tasks that wait for another task (`task_wait`) |
| p9 | Tasks that sleep (`task_sleep`) |
| p10 | Counting semaphores |
| p11 | Producer/consumer problem solved with semaphores |
| p12 | Message queues (`mqueue_*`) |
| p13 | Disk manager: block read/write requests handled by a disk task (`ppos_disk.c`) on a simulated disk (`disk.c`) |

The numbering follows the course delivery order, which differs slightly from the numbering on the current wiki. Build a step from its folder, e.g. `gcc -o pp *.c`.
