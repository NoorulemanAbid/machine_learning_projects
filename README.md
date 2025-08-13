
# 🚀 Computational Drug Discovery: Bioactivity Data Collection & Preprocessing

[![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Colab](https://img.shields.io/badge/Open%20in-Colab-red?logo=googlecolab&logoColor=white)](https://colab.research.google.com/drive/16LULDqTYip9gcXiwzVpGRx6m6alBV10f)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

---

## 🔬 Project Overview

This project collects, processes, and visualizes **bioactivity data** from [ChEMBL](https://www.ebi.ac.uk/chembl/) for **SARS coronavirus 3C-like proteinase**, a key target in drug discovery.  

It automates **data retrieval, cleaning, preprocessing, and visualization** to generate ready-to-use datasets for **machine learning or cheminformatics tasks**.

---

## 🧩 Features

- ✅ Search ChEMBL for coronavirus-related protein targets  
- ✅ Retrieve IC50 bioactivity values for selected targets  
- ✅ Clean and preprocess data: remove missing values, classify compounds (active/intermediate/inactive)  
- ✅ Visualize distribution of compound activity  
- ✅ Save raw and processed datasets for ML applications  

---

## 🗂️ Files Generated

| File Name                           | Description                                      |
|-------------------------------------|--------------------------------------------------|
| `bioactivity_data.csv`              | Raw bioactivity data extracted from ChEMBL      |
| `bioactivity_preprocessed_data.csv` | Cleaned and classified bioactivity dataset      |
| `biological_data/`                  | Folder containing additional bioactivity info   |

---

## 🛠️ Technologies Used

- **Python** (`pandas`, `matplotlib`, `seaborn`)  
- **ChEMBL Web Resource Client** for bioactivity retrieval  
- **Google Colab** for cloud execution  
- **Google Drive** for file storage  

---

## 🧭 Workflow Diagram

```mermaid
graph TD
A[Start: Search ChEMBL Targets] --> B[Select Target: CHEMBL3927]
B --> C[Retrieve Bioactivity Data (IC50)]
C --> D[Clean & Preprocess Data]
D --> E[Classify Compounds: Active/Intermediate/Inactive]
E --> F[Visualize Data]
F --> G[Save CSV Files & Folder]
````

---

## 📊 Example Visualization

```python
from matplotlib import pyplot as plt
import seaborn as sns

df3.groupby('bioactivity_class').size().plot(kind='barh', color=sns.color_palette('Dark2'))
plt.gca().spines[['top', 'right']].set_visible(False)
plt.show()
```

*Shows the distribution of compounds by activity class.*

---

## 🔗 Notebook Access

[Open in Colab](https://colab.research.google.com/drive/16LULDqTYip9gcXiwzVpGRx6m6alBV10f)

---

## 💡 Key Insights

* Automatically generates curated bioactivity datasets
* Preprocessed datasets are ML-ready for activity prediction
* Supports reproducible drug discovery workflows

---

## 🚀 Future Work

* Extend search to other viral proteins
* Include additional bioactivity measures (Ki, EC50, etc.)
* Develop ML/DL models for compound activity prediction
* Combine chemical descriptors for QSAR modeling

---

*Created by Noor ul Eman – Bioinformatics & Computational Drug Discovery Enthusiast*

```

---

This version includes:

- Badges for **Python, Colab, License**
- Mermaid workflow diagram for **visual clarity**
- Emojis for better visual appeal  
- Organized sections for GitHub readers  

---

If you want, I can also **add a small “project banner” image** at the top so it looks even more professional when people open your repo.  

Do you want me to do that next?
```
