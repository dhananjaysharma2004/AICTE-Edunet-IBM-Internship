# Intelligent Classification of Rural Infrastructure Projects 

### AICTE-Edunet-IBM Internship Capstone Project  
**Intern:** Dhananjay Kumar Sharma  
**Institution:** School of Management Sciences, Lucknow  
**Stream:** B.Tech CSE  
**Internship Platform:** IBM SkillsBuild via Edunet Foundation  
**Duration:** Summer 2025  

---

## 📌 Problem Statement

Manual classification of rural infrastructure projects under PMGSY (Pradhan Mantri Gram Sadak Yojana) schemes is inefficient, error-prone, and unscalable. This project aims to **automatically classify projects** into their respective PMGSY phases (PMGSY-I, PMGSY-II, RCPLWEA, etc.) based on **physical and financial attributes**, using machine learning.

---

## ✅ Objectives

- Automate the classification of road/bridge projects into correct PMGSY schemes
- Enhance project monitoring and transparency
- Enable scalable classification for thousands of records

---

## 🔧 Tech Stack

- **Cloud Platform:** IBM Cloud  
- **Development Environment:** IBM Watson Studio  
- **Programming Language:** Python (scikit-learn, pandas, matplotlib)  
- **Storage:** IBM Cloud Object Storage  
- **Deployment:** IBM Watson Machine Learning API (JSON-based input/output)

---

## 🧠 ML Model

- **Algorithm Used:** Random Forest Classifier  
- **Alternatives Tested:** SVM  
- **Data Split:** 80:20 (Train:Test)  
- **Tuning:** GridSearchCV with 5-fold Cross-Validation  
- **Performance Metrics:** Accuracy, Precision, Recall, F1-score

---

## 🗂️ Dataset

- **Source:** [AI Kosh PMGSY Dataset](https://aikosh.indiaai.gov.in/web/datasets/details/pradhan_mantri_gram_sadak_yojna_pmgsy.html)  
- **Features:**  
  - Project Type (Road/Bridge)  
  - Length, Estimated & Actual Cost  
  - Time Duration (Planned vs Actual)  
  - Derived Metrics: Cost/meter, Delay %, Overrun Ratio  

---

## 🚀 Deployment

- Model is deployed as an API using **IBM Watson Machine Learning**
- Accepts input as JSON and returns the predicted PMGSY scheme
- Can be integrated into dashboards for real-time project classification

---

## 📊 Output

Sample predictions from the deployed model classify project records into:
- PMGSY-I  
- PMGSY-II  
- RCPLWEA  

---

## 🔍 Future Scope

- Add advanced features: contractor profiles, location terrain, satellite data
- Upgrade to deep learning/ensemble models (e.g., XGBoost, TabNet)
- Deploy at the edge for offline predictions
- Integrate with government portals for automatic intake and monitoring

---

## 📚 References

- [AI Kosh Dataset](https://aikosh.indiaai.gov.in/web/datasets/details/pradhan_mantri_gram_sadak_yojna_pmgsy.html)  
- [IBM Watson Studio Docs](https://dataplatform.cloud.ibm.com/docs)  
- IBM Cloud Lite & Object Storage  
- Research papers on ML-based project classification

---

## 🏅 Certifications

This project was completed as part of the **AICTE-Edunet-IBM SkillsBuild Internship** and certified by IBM.

---

## 🙌 Acknowledgements

Thanks to **Edunet Foundation**, **AICTE**, and **IBM SkillsBuild** for the opportunity to work on a real-world, impact-driven project with cutting-edge technologies.

---
