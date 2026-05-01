# Maintainability Dataset Repository

This repository contains datasets and artifacts used for analyzing structural maintainability and evolution in AI-assisted software development. The data is organized around three case systems:

- **MenuCal**
- **NutriCompass**
- **PartGuard**

Each system includes both **chat session records** and **code snapshot trees** collected across development stages.

---

## 📂 Repository Structure

.
├── MenuCal_ChatSessions/
│   ├── ChatGPT/
│   └── Gemini/
│
├── MenuCal_Snapshot_Trees/
│   ├── MenuCal_loc_backup_*.txt
│   └── ...
│
├── NutriCompass_ChatSessions/
│   ├── ChatGPT/
│   └── Gemini/
│
├── NutriCompass_Snapshot_Trees/
│   ├── NutriCompass_loc_backup_*.txt
│   └── ...
│
├── PartGuard_ChatSessions/
│   ├── ChatGPT/
│   └── Gemini/
│
├── PartGuard_Snapshot_Trees/
│   ├── partguard_loc_backup_*.txt
│   └── ...

---

## 🧠 Chat Session Data

Each system includes chat session logs generated using different LLMs.

### MenuCal
- `MenuCal_ChatSessions/ChatGPT/`
- `MenuCal_ChatSessions/Gemini/`

### NutriCompass
- `NutriCompass_ChatSessions/ChatGPT/`
- `NutriCompass_ChatSessions/Gemini/`

### PartGuard
- `PartGuard_ChatSessions/ChatGPT/`
- `PartGuard_ChatSessions/Gemini/`

Each directory contains sequentially numbered PDF files such as:

- `MenuCal-ChatGPT-Session1.pdf`
- `MenuCal-ChatGPT-Session2.pdf`
- ...

These files document:
- Prompt sequences  
- Model responses  
- Iterative development interactions  

---

## 🌳 Snapshot Trees

Snapshot trees represent the source code state at different development stages.

### Locations
- `MenuCal_Snapshot_Trees/`
- `NutriCompass_Snapshot_Trees/`
- `PartGuard_Snapshot_Trees/`

Each snapshot file:
- corresponds to a development stage (timestamped)
- contains a flattened Swift source representation
- serves as input for structural metric computation

---

## 📦 Large File Handling (External Data Access)

Some chat session files exceed GitHub’s file size limit (100MB), including files larger than 200MB and one exceeding 700MB.

To ensure both **reproducibility** and **compliance with GitHub storage constraints**, these large files are hosted externally.

### 🔗 External Dataset (Read-Only Access)

https://1drv.ms/f/c/082e08a9bc6a056f/IgDoSXiTPG05RLBeYnrOFFKCATcgyDYLY00HmMq8iwjani4?e=1IRmJO

### 📌 Data Distribution Policy

| Data Type | Location |
|----------|--------|
| Small / moderate-size chat sessions | Included in this repository |
| Snapshot trees (all systems) | Included in this repository |
| Large chat session files (>100MB) | External link |

### 🔒 Access Notes

- External files are provided in **read-only mode**
- No authentication is required beyond link access
- Files are preserved in original format to ensure reproducibility

---

## 📊 Purpose

This repository supports research on:

- Structural maintainability  
- Architectural evolution  
- AI-assisted software development workflows  
- Comparative analysis of LLM-driven development  
- Empirical evaluation of vibe architecting  

---

## 📌 Usage

Typical uses include:

- Computing structural metrics (e.g., CC, WMT, CBT, LCOT)  
- Evaluating structural evolution metrics (e.g., RI, GFR, FSS, SCR)  
- Reproducing experimental results  
- Analyzing LLM-driven development behavior  

---

## ⚠️ Notes

- `.DS_Store` files may appear due to macOS artifacts and can be ignored  
- Snapshot files are stored as `.txt` for portability and analysis  
- Chat session PDFs preserve original interaction context  
- External link is required for accessing large files exceeding GitHub limits  

---

## 📄 License

This repository is provided solely for academic and research purposes, specifically to support the reproducibility of the results reported in the associated study.

The contents of this repository are made available for:

- Reproducibility and verification of research findings  
- Non-commercial academic research and analysis  

The following restrictions apply:

- No commercial use  
- No redistribution without permission  
- No use for training or fine-tuning machine learning models without authorization  

By using this repository, you agree to use the data responsibly and solely for research reproducibility purposes.
