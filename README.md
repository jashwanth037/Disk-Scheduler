# Disk Scheduling Simulator

This project is a Disk Scheduling Simulator built using Python.  
It implements and compares multiple disk scheduling algorithms with real-time visualization of disk head movement.

I built this to better understand how operating systems handle disk requests and how different algorithms affect seek time and performance.

---

## Features

- Implementation of 4 disk scheduling algorithms:
  - FCFS (First Come First Serve)
  - SSTF (Shortest Seek Time First)
  - SCAN
  - C-SCAN
- Accurate total seek time calculation
- Average seek time per request
- Interactive input handling
- Real-time disk head movement visualization
- Side-by-side performance comparison

---

## Tech Stack

- Python
- Streamlit (Web UI)
- Matplotlib (Visualization)

---

## Why I Built This

While studying Operating Systems, I realized disk scheduling algorithms are often explained theoretically but rarely visualized properly.

So I wanted to:

- See how the disk head actually moves
- Compare algorithms based on performance
- Understand why some algorithms perform better
- Simulate real request queues

This project helped me understand the trade-offs between fairness and efficiency in scheduling algorithms.

---

## Algorithms Implemented

### FCFS (First Come First Serve)
Processes requests in the order they arrive.  
Simple but can cause high seek time.

### SSTF (Shortest Seek Time First)
Selects the request closest to the current head position.  
Reduces seek time but may cause starvation.

### SCAN (Elevator Algorithm)
Moves in one direction servicing requests, then reverses.  
More balanced compared to SSTF.

### C-SCAN (Circular SCAN)
Moves in one direction only and jumps back to start.  
Provides more uniform wait time.

---


## 📂 Project Structure

Disk-Scheduler/
│
├── UI.py # Streamlit UI
├── scheduler.py # Algorithm implementations
└── README.md

