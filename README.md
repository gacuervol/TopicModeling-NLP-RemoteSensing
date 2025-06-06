# 🔍 Remote Sensing Literature Analysis | NLP & Topic Modeling  
*Automated topic extraction from 200+ scientific papers using LDA and web scraping*  

![Python](https://img.shields.io/badge/Python-3.7+-blue?logo=python) ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3-red) ![PyLDAvis](https://img.shields.io/badge/PyLDAvis-2.1.2-lightblue) ![Selenium](https://img.shields.io/badge/Web_Scraping-Selenium-orange) ![NLTK](https://img.shields.io/badge/NLTK-3.6.7-blue?logo=nltk) ![spaCy](https://img.shields.io/badge/spaCy-3.2.0-brightgreen?logo=spacy)
## 📌 Project Overview  
**Objective**: Analyze remote sensing research trends by:  
- **Automated Data Collection**: Scraping 236 papers from ScienceDirect  
- **Topic Modeling**: Latent Dirichlet Allocation (LDA) implementation  
- **Visual Analytics**: Interactive topic exploration with PyLDAvis  

**Key Findings**:  
- Identified **10 dominant research themes** in remote sensing literature  
- Discovered **3 distinct research clusters** through t-SNE visualization  
- Achieved **optimal model performance** at 10 topics (perplexity analysis)  

## 🛠️ Technical Stack  
```python
from selenium import webdriver  # Automated scraping
from sklearn.decomposition import LatentDirichletAllocation  # Topic modeling  
import pyLDAvis.sklearn  # Interactive visualization
from wordcloud import WordCloud  # Text analytics
```

## 📊 Key Visualizations  
### 1. Research Topic Clusters  
![t-SNE Plot](https://github.com/gacuervol/TopicModeling-NLP-RemoteSensing/blob/main/figures/t-SNE_Plot.png) 
*3 distinct research clusters identified through dimensionality reduction*

### 2. Topic Modeling Results  
```python
# LDA implementation
lda = LatentDirichletAllocation(n_components=10, random_state=0)
lda.fit(document_term_matrix)
```
![LDA Visualization](https://github.com/gacuervol/TopicModeling-NLP-RemoteSensing/blob/main/figures/LDA_Visualization.png)  
*Interactive exploration of topic-term relationships*

### 3. Word Frequency Analysis  
![Word Cloud](https://github.com/gacuervol/TopicModeling-NLP-RemoteSensing/blob/main/figures/Word_Cloud.png)  
*Most frequent terms in remote sensing literature*

## 🔍 Statistical Insights  
| Metric | Value |  
|---------|-------|  
| Optimal Topics | 10 |  
| Key Terms | "coastal", "marine", "monitoring" |  
| Papers Analyzed | 236 |  

## 📂 Repository Structure  
```text
/Data
├── abstract_pln.csv 
├── abstract_pln_earth.csv 
/Notebooks
├── 1_business_data_load.ipynb       # Data collection
├── 4_modeling.ipynb     # Main analysis
├── Copia de Proyecto_final.ipynb   # Main analysis
├── Practica_4_pipeline.ipynb.txt  # Main analysis
├── Proyecto_Aplicado_PLN.ipynb  # Main analysis
├── Proyecto_Modulo_4.ipynb  # Main analysis
/figures
├── LDA_Visualization.png      # Interactive visualization
├── Word_Cloud.png         # Cluster analysis
└── t-SNE_Plot.png              # Term frequency
```

## 🚀 How to Use  
### 1. Clone repository:  
```bash
git clone https://github.com/gacuervo/remote-sensing-analysis.git
```  

### 2. Install dependencies:  
```bash
pip install -r requirements.txt
```  

### 3. Run analysis:  
```bash
jupyter notebook Notebooks/2_Topic_Modeling.ipynb
```  

## 📜 References  
```bibtex
@article{blei2003latent,
  title={Latent Dirichlet Allocation},
  author={Blei, David M and Ng, Andrew Y and Jordan, Michael I},
  journal={Journal of Machine Learning Research},
  volume={3},
  pages={993--1022},
  year={2003}
}
```  

## 🔗 Connect  
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Geospatial_Data_Scientist-0077B5?logo=linkedin)](https://www.linkedin.com/in/giovanny-alejandro-cuervo-londo%C3%B1o-b446ab23b/)
[![ResearchGate](https://img.shields.io/badge/ResearchGate-Publications-00CCBB?logo=researchgate)](https://www.researchgate.net/profile/Giovanny-Cuervo-Londono)  
[![Email](https://img.shields.io/badge/Email-giovanny.cuervo101%40alu.ulpgc.es-D14836?style=for-the-badge&logo=gmail)](mailto:giovanny.cuervo101@alu.ulpgc.es)  

> 🔬 **Research Applications**:  
> - Literature review automation  
> - Research trend analysis  
> - Academic paper recommendation systems  
