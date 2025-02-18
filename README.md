# Multithreading-Based Vector Average Calculation in C

## Overview
This project demonstrates the use of multithreading in C to calculate the average of a predefined vector using POSIX threads (pthreads). By distributing the workload across multiple threads, the program optimizes performance, ensures efficient resource utilization, and provides hands-on experience with concurrency and synchronization concepts.

## Features
- Implements POSIX threads (pthreads) for parallel computation
- Uses mutex locks to ensure safe access to shared data
- Optimizes performance by leveraging multi-core processors
- Demonstrates thread synchronization with pthread_mutex_lock and pthread_mutex_unlock
- Handles dynamic thread allocation and workload distribution

## Implementation Details
- The vector is divided into equal parts, with each thread processing a subset of elements.
- Each thread calculates the partial sum of its assigned segment.
- A mutex lock ensures safe updates to the global sum variable.
- The final average is computed after all threads complete execution.
