
# 🚀 Computational Drug Discovery: Bioactivity Data Collection & Preprocessing

[![Python](https://img.shields.io/badge/Python-3.11-blue)](https://www.python.org/)
[![Colab](https://img.shields.io/badge/Colab-Notebook-orange)](https://colab.research.google.com/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

---

## 🔬 Project Overview
This project collects, processes, and visualizes bioactivity data from **ChEMBL** for SARS coronavirus 3C-like proteinase, a key target in drug discovery.

It automates:
- Data retrieval
- Cleaning and preprocessing
- Visualization
- Generation of ready-to-use datasets for ML or cheminformatics tasks

---

## 🧩 Features
- ✅ Search ChEMBL for coronavirus-related protein targets  
- ✅ Retrieve IC50 bioactivity values for selected targets  
- ✅ Clean and preprocess data: remove missing values, classify compounds as **active/intermediate/inactive**  
- ✅ Visualize compound activity distribution  
- ✅ Save **raw and processed datasets** for ML applications  

---

## 🗂️ Files Generated

| File Name | Description |
|-----------|-------------|
| bioactivity_data.csv | Raw bioactivity data extracted from ChEMBL |
| bioactivity_preprocessed_data.csv | Cleaned and classified bioactivity dataset |
| biological_data/ | Folder containing additional bioactivity info |

---

## 🛠️ Technologies Used
- **Python** (`pandas`, `matplotlib`, `seaborn`)  
- **ChEMBL Web Resource Client** for bioactivity retrieval  
- **Google Colab** for cloud execution  
- **Google Drive** for file storage  

---

## 🧭 Workflow Diagram

> **Tip:** GitHub README cannot render Mermaid diagrams directly. Export your workflow diagram as an image (PNG/SVG) and save it in your repo as `workflow.png`.

![Workflow Diagram](workflow.png)

**Workflow steps:**
1. Search ChEMBL Targets  
2. Select Target (e.g., CHEMBL3927)  
3. Retrieve Bioactivity Data (IC50)  
4. Clean & Preprocess Data  
5. Classify Compounds: Active/Intermediate/Inactive  
6. Visualize Data  
7. Save CSV Files & Folder  

---

## 📊 Example Visualization

```python
from matplotlib import pyplot as plt
import seaborn as sns

df3.groupby('bioactivity_class').size().plot(
    kind='barh', 
    color=sns.color_palette('Dark2')
)
plt.gca().spines[['top', 'right']].set_visible(False)
plt.show()
````

Shows the distribution of compounds by activity class.

---

## 🔗 Notebook Access

Open in [Colab](https://colab.research.google.com/drive/16LULDqTYip9gcXiwzVpGRx6m6alBV10f)

---

## 💡 Key Insights

* Automatically generates curated bioactivity datasets
* Preprocessed datasets are **ML-ready** for activity prediction
* Supports **reproducible drug discovery workflows**

---

## 🚀 Future Work

* Extend search to other viral proteins
* Include additional bioactivity measures (Ki, EC50, etc.)
* Develop ML/DL models for compound activity prediction
* Combine chemical descriptors for QSAR modeling

---

**Created by Noor ul Eman – Bioinformatics & Computational Drug Discovery Enthusiast**

````

