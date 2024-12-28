# 🧬 Single-Cell Transcriptomics Analysis Project
#### Disease-Mechanisms-with-single-cell-transcriptomics
---

## 📖 **Project Overview**

Before we get started, please note that this project explores the systemic immunological modifications in type 2 diabetes mellitus (T2DM) patients with periodontitis using single-cell RNA sequencing (scRNA-seq) data. The dataset is sourced from [GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE244515). The dataset is companion to the report **"Uncovering systemic immunological modification by type 2 diabetes mellitus in periodontitis patients via single-cell RNA analysis"** by [Lee et al., 2024](https://pubmed.ncbi.nlm.nih.gov/38082425/).

This project served as my introduction to scRNA-seq analysis! 

---

## 🧪 Key scRNA-seq Analysis Features Demonstrated

### **1. Data Extraction and Loading**
- Extracted the raw `.tar` file into a directory.
- Loaded individual sample files using **Scanpy's** `read_10x_mtx` method.
- Annotated each cell with a unique sample identifier for traceability.

### **2. Data Integration**
- Concatenated all samples into a single `AnnData` object for unified analysis.

### **3. Quality Control**
- Filtered cells with fewer than 100 expressed genes.
- Removed genes detected in fewer than 3 cells.
- Calculated QC metrics, including percentages of mitochondrial, ribosomal, and other gene categories.

### **4. Exploratory Visualization**
- Generated violin plots and scatterplots to examine...
  - RNA diversity across cells.
  - Total counts of mitochondrial and ribosomal genes.
  - Other biologically relevant categories like microRNA and olfactory receptor genes.

### **5. Doublet Detection**
- Used the **Scrublet** algorithm to identify potential doublets, grouping results by sample ID.


---


## 💻 **Technical Skills Practiced**

- **Programming Languages**: Python
- **Libraries**: 
  - **Scanpy**: For scRNA-seq analysis and preprocessing.
  - **NumPy** & **Pandas**: For efficient data handling and manipulation.
  - **Matplotlib**: For creating visualizations.
