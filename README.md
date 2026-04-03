# Dimentionality_Reduction_StudentGradeAnalysis_TMP

## ​👤 Author
**Parama Dey**

---

## 📌 Project Overview & Problem Statement
In educational environments, raw grade data often hides complex relationships between subjects and student learning behaviors. This project applies **Principal Component Analysis (PCA)** and **t-SNE (t-distributed Stochastic Neighbor Embedding)** to a dataset of 100 students across 8 subjects:
* **STEM:** Math, Science, Computer Science (CS)
* **Humanities:** English, History, Spanish
* **Creative/Physical:** Band, Physical Education (PhysEd)

**The Objective:** To reduce the 8-dimensional grade space into a 2D visualization to identify "Academic Archetypes," understand subject difficulty correlations, and provide data-driven recommendations for curriculum improvement.

---

## ​🛠️ Technologies & Libraries
​Language: Python 3.x

​Data Manipulation: Pandas, NumPy

​Dimensionality Reduction: Scikit-Learn (PCA, TSNE, StandardScaler)

​Visualization: Matplotlib, Seaborn

## 📊 Summary of Findings

### 1. Subject Difficulty & Distribution
* **STEM Performance Gap:** Math, Science, and CS show significant positive skewness (1.06 to 1.12), identifying these as the most challenging subjects where the majority of students score below the mean.
* **The Humanities Variance:** History and Spanish exhibit the highest standard deviation (~17.5), suggesting a wide comprehension gap that necessitates differentiated teaching strategies.
* **The "Grading Ceiling":** Band and PhysEd show high averages (70+) with low variance, indicating high consistency but limited room for elite differentiation.
  
### 2. PCA: Global Trends & Interpretability
* **PC1 (Academic Core):** Heavily weighted toward traditional subjects like Math and English. It serves as a primary metric for identifying "at-risk" students.
* **PC2 (Specialized Proficiency):** Effectively separates students based on their performance in Band and Physical Education, distinguishing "academic-heavy" profiles from "all-rounder" profiles.

### 3. t-SNE: Local Groupings & Archetypes
* **Cluster Identification:** t-SNE successfully revealed hidden clusters of students with near-identical performance profiles—patterns that remained invisible in raw tabular data.
* **Specialist Outliers:** Identified small, isolated groups at the periphery, likely representing "Subject Specialists" (e.g., students excelling in CS but struggling in Humanities).
---

## 💡 Actionable Recommendations
* **STEM Bridge Programs:** Implement targeted quantitative reasoning modules to address the low performance floor in Math and CS.
* **Peer-Tutoring Systems:** Leverage high-achievers in high-variance subjects (History/Spanish) to mentor struggling peers.
* **Early Warning System:** Utilize PCA coordinates to flag students falling below specific thresholds for immediate academic counseling.

---

## 📂 Repository Structure
* `PCA_Implementation_.ipynb`: Detailed notebook covering feature scaling and linear dimensionality reduction.
* `T-SNE_Implementation_.ipynb`: Exploration of non-linear embeddings and hyperparameter tuning (perplexity).
* `Student_Grades.csv`: The original dataset containing 100 student records.
* `Dimensionality reduction on student grade dataset.pdf`: A summary presentation for stakeholders.
* `README.md`: Project documentation.

---

## 🛠️ How to Run
1. Clone the repository: `git clone https://github.com/Parama-Dey/Dimentionality_Reduction_StudentGradeAnalysis_TMP.git`
2. Install dependencies: `pip install pandas matplotlib seaborn scikit-learn`
3. Run the Jupyter Notebooks to reproduce the visualizations.
