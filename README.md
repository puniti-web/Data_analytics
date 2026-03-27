# 🧬 Gene Expression Analysis & Pathway Enrichment (GSE8671)

## 📌 Project Overview

This project performs **differential gene expression (DGE) analysis** on a microarray dataset and identifies biologically significant genes and pathways.

The workflow includes:

* Data preprocessing from GEO2R output
* Identification of Differentially Expressed Genes (DEGs)
* Visualization using Volcano Plot & Heatmap
* Functional enrichment using GO & KEGG

---

## 📂 Dataset

* **Source:** NCBI GEO
* **Dataset ID:** GSE8671
* **Type:** Microarray gene expression data

---

## ⚙️ Tools & Technologies

* **R Programming**
* Packages:

  * limma
  * GEOquery
  * clusterProfiler
  * org.Hs.eg.db
  * pheatmap
  * ggplot2

---

## 🔬 Workflow

### 1️⃣ Data Loading

* Imported GEO2R output file (.tsv)
* Cleaned and formatted column names
* Converted values to numeric

---

### 2️⃣ DEG Identification

* Criteria:

  * Adjusted p-value < 0.05
  * |logFC| ≥ 1
* Split into:

  * Upregulated genes
  * Downregulated genes

---

### 3️⃣ Visualization

#### 📊 Volcano Plot

* X-axis: log2 Fold Change
* Y-axis: -log10 P-value
* Highlights significant genes

#### 🔥 Heatmap

* Top 50 DEGs selected
* Row-wise scaling applied
* Shows clustering patterns

---

### 4️⃣ Functional Enrichment

#### 🧠 GO Biological Process

* Identifies biological functions
* Shows enriched processes like signaling & immune activity

#### 🧬 KEGG Pathway Analysis

* Identifies affected pathways
* Examples:

  * Cytokine signaling
  * Cell cycle
  * Calcium signaling

---

## 📈 Results

* Significant DEGs identified
* Clear separation in volcano plot
* Heatmap shows distinct clustering
* KEGG & GO reveal biologically relevant pathways

---

## 🌐 Web Deployment

All plots are exported as images and displayed on a simple frontend website.

### Website includes:

* Volcano Plot
* Heatmap
* KEGG Pathway Plot
* GO Enrichment Plot

---

## 🚀 How to Run

### 1. Clone repository

```bash
git clone https://github.com/puniti-web/Data_analytics.git
cd Data_analytics
```

### 2. Run R Script

* Open RStudio
* Run full script from top to bottom

### 3. Generate Plots

Plots will be saved as:

* volcano.png
* heatmap.png
* kegg.png
* go_bp.png

---

## 📁 Project Structure

```
bio_project/
│── index.html
│── style.css
│── volcano.png
│── heatmap.png
│── kegg.png
│── go_bp.png
│── analysis.R
│── README.md
```

---

## 📊 Key Learnings

* Microarray data analysis workflow
* DEG filtering and visualization
* Functional enrichment interpretation
* Integrating backend (R) with frontend (HTML)

---

## 📌 Future Improvements

* Add interactive plots (Plotly)
* Deploy using Flask/FastAPI backend
* Add user upload feature for new datasets

---

## 👨‍💻 Author

**Puniti Jodhwani**

---

## ⭐ Acknowledgements

* NCBI GEO Database
* Bioconductor packages
* clusterProfiler documentation

---
