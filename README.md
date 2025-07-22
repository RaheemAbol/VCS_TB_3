
### 🎟️ Ticket #004 – **"Wildcard Warriors: Organize the Data Ops Mess"**

#### 🔧 Focus: Wildcards, File Movement, and Directory Awareness (from parent dirs)

---

### 🧠 Scenario:

The analytics team left a mess of backup files scattered throughout different folders. It’s your job to **organize everything cleanly** using wildcards — all from their respective **parent directories**.

---

### 📂 Current Structure (Before):

```
sales-insights/
├── data/
│   ├── raw/
│   │   ├── april.csv
│   │   ├── may.csv
│   │   ├── june.csv
│   │   ├── april_backup.csv
│   │   ├── may_backup.csv
│   │   └── june_backup.csv
│   └── archive/
│
├── reports/
│   ├── summary_draft.md
│   ├── summary_final.md
│   ├── summary_backup.md
│   ├── notes.txt
│   └── notes_backup.txt
│
└── scripts/
    ├── clean_data.py
    ├── analyze_data.py
    ├── analyze_data_backup.py
```

---

### 📝 Tasks:

---

#### ✅ **1. Move Data Backups (from `data/`)**

From inside `sales-insights/data/`:

* Ensure `archive/` exists (create it if needed)
* Move all files ending in `_backup.csv` from `raw/` to `archive/`

---

#### ✅ **2. Clean the Reports Folder**

From inside `sales-insights/reports/`:

* Create a new folder called `backups/`
* Move:

  * `summary_backup.md`
  * `notes_backup.txt`
    into the `backups/` folder using a wildcard

*(Hint: What pattern matches both `.md` and `.txt` that end with `_backup`?)*

---

#### ✅ **3. Organize Script Archives**

From inside `sales-insights/scripts/`:

* Create a folder named `archive/`
* Move any script ending in `_backup.py` into the `archive/` folder
  *(Should be just one file for now)*

---

#### 🔍 **4. Final Check (From Root)**

* From `sales-insights/`, list contents of the following:

  * `data/raw/` → should only have `.csv` (no backups)
  * `data/archive/` → should now have the 3 backup `.csv` files
  * `reports/backups/` → should have 2 backup text/markdown files
  * `scripts/archive/` → should have 1 script file

---

### ✅ Completion Checklist:

* [ ] You used wildcards to match backup files in each section
* [ ] You created `archive/` or `backups/` folders where needed
* [ ] You listed and confirmed contents after moving
* [ ] You can explain what a wildcard is and when you'd use it

---

