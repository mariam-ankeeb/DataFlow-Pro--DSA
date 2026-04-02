# 🚀 DataFlow Pro — ETL & Analytics Processing Engine
### ITI PortSaid | PowerBI46R2 | DSA Project

---

## 📋 Project Overview

This project was built as part of the **Data Structures & Algorithms** course at **ITI Port Said**.

The scenario: I'm a junior data engineer at **NileMart Inc.**, an Egyptian retail chain. The BI analysts at Smart Village HQ are struggling because their Power BI dashboards take **hours** to refresh — the raw data is messy, unsorted, and unstructured.

My job was to build **DataFlow Pro**, a Python ETL (Extract, Transform, Load) engine that cleans, sorts, and structures the data *before* it ever reaches Power BI — using the DSA concepts I learned in this course.

---

## 🛠️ Project Phases

### Phase 1 — The Query Optimizer (Sorting & Searching)
- Implemented **Bubble Sort**, **Insertion Sort**, and **Selection Sort** on 500 records to demonstrate their O(n²) limitations
- Implemented **Merge Sort** and **Quick Sort** on 10,000 records to show O(n log n) performance
- Benchmarked all custom sorts against Python's built-in **Timsort** (`.sort()`)
- Built a **Linear Search** vs **Binary Search** lookup engine to find fraudulent transaction IDs
- Used Python's `bisect` module to slice Q3 time-series sales data in O(log n)

### Phase 2 — The "Applied Steps" Tracker (Linked Lists)
- Built a **Singly Linked List** to record Power Query transformation steps
- Upgraded to a **Doubly Linked List** with full **Undo/Redo** support in O(1) time

### Phase 3 — The DAX Formula Parser (Stacks)
- Implemented a **Stack using a Python List** (Array-based)
- Implemented a **Stack using a Linked List**
- Built a **DAX Postfix Expression Evaluator** to compute KPI formulas like `(Revenue - Cost) * Tax_Rate`
- Added a **Parentheses Validator** to catch unbalanced formulas before they crash

### Phase 4 — The Live Data Buffer (Queues)
- Demonstrated the **O(n) performance trap** of using a plain Python list as a queue (`pop(0)`)
- Built an **O(1) Queue using a Linked List** to fix the problem
- Upgraded to a production-grade buffer using **`collections.deque`** for White Friday traffic handling

### Phase 5 — The Hierarchical Matrix Builder (Trees)
- Built a **Binary Search Tree (BST)** to store and look up Customer National IDs in O(log n)
- Built an **N-ary Organizational Chart** using the `anytree` library (CEO → VPs → Sales Reps)
- Implemented a **recursive Roll-Up function** to aggregate sales from leaf nodes up to the CEO

---

## 📊 Key Findings (Big-O Summary)

| Data Structure | Operation | Complexity |
|---|---|---|
| Bubble / Insertion / Selection Sort | Sort | O(n²)  |
| Merge Sort / Quick Sort | Sort | O(n log n)  |
| Timsort (built-in) | Sort | O(n log n)  |
| Linear Search | Search | O(n) |
| Binary Search | Search | O(log n)  |
| Singly Linked List | Undo | O(n) |
| Doubly Linked List | Undo/Redo | O(1)  |
| Stack (Array or LL) | Push/Pop | O(1)  |
| List Queue | Dequeue | O(n)  |
| Deque / LL Queue | Dequeue | O(1)  |
| BST | Insert/Search | O(log n) avg  |
| Tree Roll-Up | Traversal | O(n) |

---

## ⚙️ How to Run

1. Clone the repository:
```bash
git clone https://github.com/mariam-ankeeb/DataFlow-Pro-DSA.git
cd DataFlow-Pro-DSA
```

2. Install the required library:
```bash
pip install anytree
```

3. Open the notebook:
```bash
jupyter notebook DataFlow_ProDSA_Project.ipynb
```

4. Run all cells from top to bottom (**Kernel → Restart & Run All**)

---

## 🧰 Requirements

- Python 3.8+
- `anytree` (for Phase 5 org chart)
- `jupyter` (to run the notebook)

---

## 👩‍💻 Author

**Mariam Ankeeb**  
ITI Port Said — Power BI Track 
GitHub: [@mariam-ankeeb](https://github.com/mariam-ankeeb)
