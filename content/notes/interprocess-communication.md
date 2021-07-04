---
title: "Interprocess Communication"
date: 2021-07-04T16:17:24+10:00
draft: true
---

# How can processes communicate with one another?
- Shared memory (overlapping context)
- Synchronization instructions (hardware support)
- Supervisor calls (Message passing)

# Practical examples
## Producer Consumer
We can't consume data before its been produced
### Solutions
#### FIFO Buffering
Producer should wait if the buffer is full, consumer should wait until the buffer is not empty.

Can have a circular buffer - with a read index and a write index.

Bounded buffer problem - shared memory, with producer and consumer 

- Semaphores 
Supervisor call - using atomicity of kernel handlers. works in timeshared processor using single uninterrupted kernel

- Simultaneous transactions (Atomicity)


## UNIX Pipelines

# Interprocess communication in Java
https://www.java67.com/2020/05/how-to-do-inter-process-communication-in-java.html

## ActiveMQ
There are a variety of transports available for ActiveMQ which is a popular message broker. There is NIO, VM, TCP. Netty?


# Notes
- https://www.youtube.com/watch?v=Y_PNOmL_yqY
https://www.udemy.com/course/hands-on-systems-programming-with-rust/
https://www.udemy.com/course/advance-programming-concepts/
https://www.udemy.com/course/linuxipc/
https://www.udemy.com/course/linux-system-programming/
https://www.geeksforgeeks.org/methods-in-interprocess-communication/