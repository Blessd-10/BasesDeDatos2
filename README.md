# Workshop 3: Concurrency, Parallelism, and Performance Strategies
## Digital University Library System

**University:** Universidad Distrital Francisco José de Caldas  
**Course:** Bases de Datos II  
**Team:**
- David Stiven Muñoz Amaya
- Janeth Oliveros Ramírez
- Daniel Felipe Paez Mosquera

---

### 📄 Project Overview
This repository contains the deliverables for **Workshop 3**, focusing on the performance optimization and concurrency analysis of the Digital University Library Platform. The architecture evolves from a conceptual data model to a high-performance hybrid system using **Polyglot Persistence** (PostgreSQL + MongoDB + Redis).

### 🚀 Key Deliverables

#### 1. Final Technical Report (PDF)
The main document `Workshop3_Final_Report.pdf` integrates:
- **Refined Architecture:** Corrections from Workshop 2 (Scope, ER Model, Flowcharts).
- **Concurrency Analysis:** Identification of 5 critical scenarios (Lost Updates, Phantom Reads, Write Skews).
- **Performance Strategies:** Detailed implementation of Caching, Sharding, Geographic Replication, and Parallel Query Execution.

#### 2. Performance Strategy Highlights
To handle high concurrency and Big Data volume, we implemented:
* **Caching (Redis):** For sub-millisecond access to frequent metadata.
* **Sharding (MongoDB):** Horizontal partitioning of Activity Logs by `Faculty_ID`.
* **Geographic Replication:** Read-replicas to ensure availability across different campus locations.
* **Parallelism (PostgreSQL):** Multi-core query execution for BI analytics.

---

### 📂 Folder Structure

```text
/Workshop-3
│
├── /Latex_Source          # Source files for the report
│   ├── main.tex           # Main LaTeX file
│   ├── diagrams/          # PDFs and PNGs of architectures and flows
│   └── references.bib     # Bibliography (if applicable)
│
├── Workshop3_Final.pdf    # Compiled Final Report
│
└── README.md              # This documentation file