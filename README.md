# **IPL-Match-Prediction-System**

CricketIQ is a data-driven IPL match prediction system that analyzes past match statistics and learns patterns to forecast which team is more likely to win a match.
The system combines **Machine Learning models**, a **Flask backend**, and an **interactive HTML/CSS frontend** to provide real-time match predictions.

# **Key Features**

✔ Predict IPL match outcomes using historical data  
✔ Multi-model training and comparison  
✔ LightGBM-based final deployed model  
✔ Full-stack deployment with Flask  
✔ Interactive frontend UI (HTML + CSS)  
✔ Visual analysis: heatmaps, ROC curves, confusion matrices  
✔ Clean code, modular structure, and ready-to-deploy setup  

# **Machine Learning Models Used**

The project evaluates five different ML models:

| Model              | Purpose                 | Strength                             |
| ------------------ | ----------------------- | ------------------------------------ |
| **Random Forest**  | Ensemble decision trees | Balanced accuracy & interpretability |
| **XGBoost**        | Gradient boosting       | High performance on tabular data     |
| **LightGBM**       | Optimized boosting      | Fast, accurate, handles large data   |
| **SVM**            | Margin-based classifier | Works well in multiclass problems    |
| **MLP Classifier** | Neural network          | Learns non-linear patterns           |

After testing and evaluation, **LightGBM** was selected as the final model.

# **Model Evaluation**

The models were evaluated using:

* Accuracy
* Precision, Recall, F1-score
* Confusion Matrix
* ROC AUC Curve
* Train–Test Split (80% train, 20% test)

Visual insights such as **heatmaps** and **ROC curves** helped understand feature relationships and classification performance.

# **System Architecture**

```
Frontend (HTML/CSS) → Flask Backend → ML Model → Prediction Output
```

# **Flow**

1. User selects match input (teams, venue, etc.)
2. Data sent to Flask API
3. LightGBM model processes input
4. Predicted winning team is returned
5. Frontend displays result and insights

# **Tech Stack**

### Frontend

* HTML
* CSS

### Backend

* Python
* Flask

### Machine Learning & Data

* Pandas, NumPy
* Scikit-learn
* XGBoost
* LightGBM
* Matplotlib, Seaborn

# **Future Enhancements**

* Add live API integration for real-time IPL data
* Use deep learning (LSTM) for sequence-aware predictions
* Deploy on cloud (Render/Heroku/AWS)
* Create mobile-friendly UI
