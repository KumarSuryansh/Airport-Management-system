# ✈️ Airport Takeoff Queue Management System

A Win32 GUI–based Queue Implementation using C++

---

## 🚀 Overview

The **Airport Takeoff Queue Management System** is a Windows GUI application built using the **Win32 API** and **C++ Queue Data Structure**.
It simulates a real airport’s runway queue, where airplanes wait for takeoff in a **First-In-First-Out (FIFO)** order.

This project demonstrates a practical implementation of:

* Queue Data Structure
* File Handling
* Win32 GUI Programming
* Event-driven architecture
* Real-world simulation of airport takeoff operations

It is developed as part of:

* **Course:** CSE 201 – Coding Skills
* **Institution:** SRM University – AP
* **Academic Year:** 2025–26

---

## ✨ Key Features

### 1. Realistic Airport Takeoff Simulation

Imitates real runway operations where planes wait in a queue before takeoff.

### 2. GUI-Based Queue Operations

Built using **pure Win32 API** — no external libraries.

### 3. Full Queue Functionality

* Add Plane (Enqueue)
* Allow Takeoff (Dequeue)
* View Front Plane (Peek)
* Check Queue Status (Empty / Full / Size)
* Refresh Queue
* Exit System

### 4. Persistent Storage

The queue is saved in `runway.txt`, ensuring data remains available even after closing the program.

### 5. Takeoff Logging

Every aircraft takeoff is recorded in `takeoff_log.txt` for future audits.

### 6. Bounded Queue

Queue capacity is fixed at **5 planes** to resemble real runway limits.

---

## 🛠️ Tech Stack

* **Language:** C++
* **Interface:** Win32 API (Windows.h)
* **Data Structure:** `std::queue<Plane>`
* **Storage:** File handling (runway.txt, takeoff_log.txt)
* **Libraries Used:**

  * `<windows.h>`
  * `<queue>`
  * `<fstream>`
  * `<sstream>`
  * `<string>`
  * `<vector>`

---

## ⚙️ System Workflow

1. **Load Queue**
   Reads `runway.txt` and reconstructs the queue at startup.

2. **User Interacts with GUI Buttons**
   Each button triggers corresponding queue operations.

3. **Queue Operations Include:**

   * `enqueue` → add plane
   * `dequeue` → allow takeoff
   * `peek` → view next plane
   * `size` → count planes
   * `isEmpty` / `isFull` → queue status

4. **File Updates**
   After every operation, the queue is re-saved to maintain real-time accuracy.

---

## 📂 File Structure

```
Airport-Management-System/
│
├── main.cpp
├── runway.txt              # Stores active queue
├── takeoff_log.txt         # Stores takeoff history
└── README.md
```

*Note: Your repository may use different filenames based on implementation.*

---

## 📦 Installation & Usage

### 🧩 Clone the Repository

```bash
git clone https://github.com/KumarSuryansh/Airport-Management-system.git
cd Airport-Management-system
```

### ⚙️ Compile the Program

Compile using any Windows C++ compiler (MSVC recommended).

Example for MinGW:

```bash
g++ main.cpp -o airport_queue -lgdi32 -luser32
```

### ▶️ Run the Application

Double-click the generated `.exe` file or run:

```bash
airport_queue.exe
```

---

## 📊 Sample Output (GUI Behavior)

### 1️⃣ Add Plane

Adds a new plane to the end of the queue.

```
Plane Added:
Flight No: AI101
Airline: Air India
```

Queue Display:

```
Flight: AI101 | Airline: Air India
```

---

### 2️⃣ Allow Take-off

Removes the front plane from the queue.

Message:

```
Plane Taking Off:
Flight: AI101
Airline: Air India
```

Log entry added to `takeoff_log.txt`.

---

### 3️⃣ View Front Plane

Shows next plane in queue without removing it.

```
Front Plane:
Flight: AI204
Airline: Indigo
```

---

### 4️⃣ Is Queue Empty?

```
Queue is EMPTY
```

or

```
Queue is NOT EMPTY
```

---

### 5️⃣ Is Queue Full?

```
Queue is FULL (Max: 5)
```

---

### 6️⃣ Queue Size

```
Queue Size: 3 / 5
```

---

### 7️⃣ Refresh Queue

Reloads the display from runway.txt.

---

## 📘 Concepts Demonstrated

### 🧱 Data Structures

* Queue (FIFO)
* Bounded queue
* Enqueue/Dequeue operations

### 🪟 GUI Programming

* Windows API
* Controls: Buttons, Textbox, ListBox
* Event-driven callbacks

### 📂 File Handling

* Persistent queue storage
* Takeoff event logging

### 🔐 Input Validation

* Prevent adding when full
* Prevent taking off when empty

---

## 👥 Team Members (SRM University AP)

| Name               | Registration No.  | 
| ------------------ | ----------------- | 
| Om Mittal          | AP24110010404     | 
| **Suryansh Kumar** | **AP24110010446** | 
| G. Sri Sujan       | AP24110010413     | 
| Piyush Raj         | AP24110010439     | 
| I. Terish Charan   | AP24110010412     | 
| S. Pranav Saket    | AP24110010407     | 

---

## 📝 Conclusion

The Airport Takeoff Queue System successfully demonstrates:

* Implementation of Queue ADT
* Real-time event handling
* File-backed data persistence
* GUI-based control of a real-world simulation

Future enhancements may include:

* Multi-runway system
* Priority queues (emergency takeoff)
* Full airport dashboard
* Advanced analytics and filtering
* Database integration (SQLite/MySQL)

This project serves as a strong foundation for aviation management simulations and real-time system design.

---
