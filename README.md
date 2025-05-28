# Crime-Data-Analysis
# Austin Crime Data Analysis

A Data Science and Machine Learning project predicting crime clearance times using historical crime data from the City of Austin, Texas.

## Project Summary

This project aims to classify crime clearance times into three categories—**Fast (0–7 days)**, **Medium (7–15 days)**, and **Slow (15+ days)**—using machine learning techniques. We processed a dataset of over 2.6 million crime records and trained multiple models to determine the most effective classifier. The **Random Forest** model achieved the best performance with \~46% accuracy and \~48% F1 score on unseen 2024 test data.

## Repository Structure

```bash
├── DAML_Final_code.ipynb      # Jupyter notebook with full implementation
├── Pavuluri_Bhattu_Bada_Project_updated.docx  # Full project report
├── README.md                  # Project overview (this file)
```

## Dataset

* **Source:** [City of Austin Open Data Portal](https://data.austintexas.gov/Public-Safety/Crime-Reports/fdj4-gpfu)
* **Time Span:** 2003 to early 2025
* **Filtered Data:** 2013–2024 (Holdout test year: 2024)
* **Final Training Set Size:** \~725,000 records
* **Final Holdout Set Size:** \~54,000 records

##  Machine Learning Models

1. **Naive Bayes**
2. **Random Forest Classifier** ✅ *Best Performer*
3. **K-Nearest Neighbors (KNN)**
4. **Neural Network (MLPClassifier)**

### Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* Learning Curves
* Training Time vs Performance

##  Preprocessing and Feature Engineering

* Handled missing and erroneous records
* Added features: report delay, time of day, season, weekend indicator
* Encoded high/low-cardinality categorical variables
* Used stratified sampling for model efficiency
* Avoided data leakage via proper preprocessing pipelines

##  Key Findings

* **Random Forest** achieved:

  * **Accuracy:** 46.08%
  * **F1 Score:** 48.21%
  * Best trade-off between training time and prediction performance
* **Neural Network** came close in performance but required more training time
* **Naive Bayes** performed the worst due to strong assumptions and imbalanced predictions

## Visualizations

* Yearly crime distribution
* Offense type frequency
* Clearance time histograms and boxplots
* Model confusion matrices
* Learning curves and feature importance graphs

##  Conclusion

Random Forest was the most reliable model for predicting crime clearance speed in Austin. The pipeline can be adapted to other cities or datasets with minor tuning.

## 📚 References

* City of Austin Crime Reports Dataset: [Link](https://data.austintexas.gov/Public-Safety/Crime-Reports/fdj4-gpfu)
* Austin Police Department: [Website](https://apdaustintx.govqa.us/)
