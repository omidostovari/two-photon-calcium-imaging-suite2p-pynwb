# Two-Photon Calcium Imaging Pipeline (Suite2p + PyNWB)

This repository contains a **Jupyter notebook** implementing a full pipeline for two-photon calcium imaging analysis.  
The workflow uses **Suite2p** for preprocessing and signal extraction, and **PyNWB** for standardized data storage.  
It demonstrates reproducible analysis on a subset of the **DeepCAD-RT dataset**, specifically paired **LowSNR** and **HighSNR** imaging files.

---

## 📌 Project Overview
- **Dataset:** Subset of DeepCAD-RT (paired LowSNR/HighSNR recordings).  
- **Objective:** Build a reproducible pipeline for calcium imaging analysis and export results in NWB format.  
- **Tools:**  
  - [Suite2p](https://github.com/MouseLand/suite2p) → motion correction, ROI segmentation, trace extraction.  
  - [PyNWB](https://github.com/NeurodataWithoutBorders/pynwb) → NWB file creation for standardized sharing.  
- **Outputs:** Suite2p result files (`.npy`, `.bin`) and NWB file (`ZebrafishOT.nwb`).  

---

## ⚙️ Features
- End-to-end pipeline in a single Jupyter notebook.  
- Suite2p outputs stored in `kaggle/working_directory/suite2p/plane0/`.  
- NWB file generated at `kaggle/working_directory/ZebrafishOT.nwb`.  
- Demonstrates reproducibility across LowSNR and HighSNR paired recordings.  
- Ready-to-use workflow for computational neuroscience applications.  

---

## 📂 Repository Structure
```
├── notebooks/
│   └── Two_Photon_Calcium_Imaging_Suite2p_Pipeline.ipynb
├── suite2p_outputs/
│   ├── data.bin
│   ├── F.npy
│   ├── Fneu.npy
│   ├── iscell.npy
│   ├── ops.npy
│   ├── spks.npy
│   └── stat.npy
├── ZebrafishOT.nwb
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.9+
- Suite2p
- PyNWB
- NumPy, Matplotlib

Install dependencies:
```bash
pip install suite2p pynwb numpy matplotlib
```

### Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/calcium-imaging-suite2p-pynwb.git
   cd calcium-imaging-suite2p-pynwb
   ```
2. Open the notebook:
   ```bash
   jupyter notebook notebooks/Two_Photon_Calcium_Imaging_Suite2p_Pipeline.ipynb
   ```
3. Run the pipeline to reproduce Suite2p outputs and NWB export.  

---

## 📊 Outputs
- **Suite2p files** (`data.bin`, `F.npy`, `Fneu.npy`, `iscell.npy`, `ops.npy`, `spks.npy`, `stat.npy`) → located in `suite2p_outputs/`.  
- **NWB file** (`ZebrafishOT.nwb`) → standardized dataset for sharing and downstream analysis.  

---

## 🎯 Academic Impact
This project highlights:
- Expertise in **calcium imaging workflows**.  
- Ability to handle **LowSNR vs HighSNR paired datasets**.  
- Commitment to **open science and reproducibility**.  

It is featured in the **Notable Projects** section of my academic CV for PhD applications in computational neuroscience.

---

## 📜 License
Released under the MIT License.

---

## 📧 Contact
**Omid Ostovari**  
Aspiring PhD researcher in Computational Neuroscience & AI  
[LinkedIn](https://www.linkedin.com/in/omidostovari) | [Email](mailto:omidostovary@gmail.com)

