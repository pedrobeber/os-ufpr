# os-ufpr
Course projects for Operating Systems (UFPR), building **PingPongOS**, a small teaching OS kernel running as a user-space library in C. Each folder `p0` … `p13` is one incremental step:

| Dir | Topic |
|---|---|
| p0 | Generic queue (`queue.c`) used by the whole kernel |
| p1 | Context switching experiments (`makecontext` / `swapcontext`) |
| p2–p3 | Task management and the dispatcher |
| p4 | Priority-based scheduler (with aging) |
| p5 | Timer-driven preemption |
| p6 | Task accounting (execution time, CPU usage) |
| p7 | Main task handling |
| p8 | Task join/wait (`task_wait`) |
| p9 | Task sleep |
| p10 | Counting semaphores |
| p11 | Producer/consumer problem |
| p12 | Message queues |
| p13 | Disk driver simulation (`ppos_disk.c`, `disk.c`) |

Build each step with `gcc` from its directory (e.g. `gcc -o pp *.c`).
