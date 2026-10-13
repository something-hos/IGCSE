# Cambridge Multi-Subject Autonomous Revision Indexer (Extended & FLE)

This repository automatically indexes, categorizes, and serves past paper revision questions across **8 Cambridge IGCSE & O Level subjects** with **100% free hosting ($0.00 cost forever)** and **zero human intervention**.

---

## 📚 Supported Subjects & Target Tiers

| Code | Subject Name | Curriculum / Level | Target Papers Indexed |
| :--- | :--- | :--- | :--- |
| **0610** | Biology | Cambridge IGCSE | Extended: Paper 2 (MCQ), Paper 4 (Theory), Paper 6 (Alt. Practical) |
| **0620** | Chemistry | Cambridge IGCSE | Extended: Paper 2 (MCQ), Paper 4 (Theory), Paper 6 (Alt. Practical) |
| **0625** | Physics | Cambridge IGCSE | Extended: Paper 2 (MCQ), Paper 4 (Theory), Paper 6 (Alt. Practical) |
| **0500** | First Language English (FLE) | Cambridge IGCSE | Paper 1 (Reading), Paper 2 (Directed Writing & Composition) |
| **3226** | Tamil | Cambridge O Level | Paper 1 (Composition), Paper 2 (Translation & Comprehension) |
| **0417** | ICT | Cambridge IGCSE | Paper 1 (Theory), Paper 2 & 3 (Practical) |
| **0607** | International Mathematics | Cambridge IGCSE | Extended: Paper 2 (Non-calc), Paper 4 (Calc), Paper 6 (Investigation) |
| **0455** | Economics | Cambridge IGCSE | Paper 1 (MCQ), Paper 2 (Structured Questions) |

---

## ⚡ Zero-Cost Architecture

- **Database:** Stored as a flat, version-controlled JSON file (`data/papers.json`) directly in the repository.
- **Hosting:** 100% free via **GitHub Pages**.
- **Autopilot Pipeline:** A free **GitHub Actions** cron job runs weekly, checks for newly published sessions across all 8 subjects, updates `data/papers.json`, and commits back to the repo automatically.

---

## 🚀 One-Time Setup (2 Minutes)

1. Create a **New Repository** on [GitHub](https://github.com/) (choose **Public** for free unlimited GitHub Actions and Pages).
2. Upload the extracted files from `cambridge-multi-subject-indexer.zip`:
   - `index.html`
   - `pipeline_indexer.py`
   - `data/papers.json`
   - `.github/workflows/indexer_cron.yml`
3. Enable GitHub Pages:
   - Go to **Settings > Pages** &rarr; select `main` branch &rarr; click **Save**.
4. Enable Bot Write Permissions:
   - Go to **Settings > Actions > General** &rarr; under **Workflow permissions**, select **Read and write permissions** &rarr; click **Save**.

The multi-subject revision hub will be live immediately, updating itself autonomously as new Cambridge exam sessions are released.