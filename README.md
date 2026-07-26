# ncbi
A Python-based bioinformatics pipeline that fetches COL5A1 genomic sequences from NCBI Entrez, analyzes nucleotide distributions, and parses structured sequence metrics into a local SQLite database.
## Key Features
* **Automated NCBI Retrieval:** Interacts with NCBI Entrez APIs via Biopython to fetch *Homo sapiens* *COL5A1* RefSeq records.
* **Automated Data Directory Setup:** Dynamically verifies and manages local storage for raw FASTA files and database outputs.
* **Sequence Metrics Computation:** Parses FASTA files to compute base pair totals (A, T, C, G) and GC content percentages.
* **SQLite Database Integration:** Automatically creates a structured relational database schema and safely stores sequence metrics using parameter-bound SQL queries (`INSERT OR REPLACE`).

---

## Tech Stack
* **Language:** Python 3.x
* **Libraries:** `biopython`, `sqlite3`, `os`, `sys`
* **Database:** SQLite3
