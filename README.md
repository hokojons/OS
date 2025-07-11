# Dining Philosophers Problem (Concurrency in C)

This project is an implementation of the classic **Dining Philosophers Problem** using **POSIX Threads (`pthread`)**, **mutexes**, and a **semaphore** in C. The program demonstrates concurrency control and deadlock prevention by allowing up to 3 philosophers to eat at the same time.

## 🔧 How It Works

- There are 5 philosophers sitting around a table.
- Each philosopher alternates between **thinking** and **eating**.
- To eat, a philosopher needs two **chopsticks** (mutexes): one on their left and one on their right.
- A **semaphore (waiter)** is used to limit the number of philosophers who can try to pick up chopsticks simultaneously (set to 3 in this case) to prevent deadlock.

## 📁 Files

- `main.c`: The source code containing the implementation.
- `README.md`: This file.

## ▶️ How to Compile and Run

Requirements
- GCC compiler
- POSIX Threads library (commonly available on Linux/macOS)

### Compile:
```bash
gcc -o namafile.c -lpthread
