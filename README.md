HR Analytics: Employee Attrition Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-orange?logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.0%2B-green?logo=scikit-learn&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## 📊 Project Overview

This project analyzes employee attrition data to identify key factors contributing to employee turnover and builds predictive models to help HR departments proactively address retention challenges. The analysis provides actionable insights that can help organizations reduce attrition rates and improve employee satisfaction.

### 🎯 Business Problem

Employee attrition is a significant challenge for organizations, leading to:
- Increased recruitment and training costs
- Loss of institutional knowledge
- Decreased team morale and productivity
- Disruption to ongoing projects

This project aims to answer critical questions:
- What factors influence employee attrition?
- Can we predict which employees are likely to leave?
- What actionable strategies can reduce attrition?

---

## 📁 Dataset Information

**Source:** IBM HR Analytics Attrition Dataset (Kaggle)

| Metric | Value |
|--------|-------|
| Total Records | 1,470 employees |
| Features | 35 attributes |
| Target Variable | Attrition (Yes/No) |
| Data Balance | 84% Stayed, 16% Left |

###Key Features:
- **Demographics:** Age, Gender, Marital Status, Education
- **Job-related:** Department, Job Role, Job Level, Monthly Income
- **Work Environment:** Distance From Home, Environment Satisfaction, Work-Life Balance
- **Career:** Years At Company, Years In Current Role, Training Times Last Year
- **Compensation:** Daily Rate, Hourly Rate, Monthly Rate, Percent Salary Hike, Stock Option Level
- **Performance:** Job Involvement, Performance Rating, Job Satisfaction

---

## 🔍 Analysis Workflow

```
1. Data Exploration & Understanding
         ↓
2. Data Cleaning & Preprocessing
         ↓
3. Exploratory Data Analysis (EDA)
         ↓
4. Feature Engineering & Selection
         ↓
5. Statistical Analysis
         ↓
6. Predictive Modeling
         ↓
7. Model Evaluation & Interpretation
         ↓
8. Business Recommendations
```

---
#### 4. Work-Life Balance Impact
| Work-Life Balance Rating | Attrition Rate |
|-------------------------|---------------|
| Bad | 31.25% |
| Good | 16.83% |
| Better | 14.52% |
| Best | 11.11% |

---

## 🤖 Predictive Models

### Model Performance Comparison

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-------|----------|-----------|--------|----------|---------|
| Random Forest | 86.2% | 0.72 | 0.58 | 0.64 | 0.82 |
| XGBoost | 87.5% | 0.75 | 0.61 | 0.67 | 0.85 |
| Logistic Regression | 85.1% | 0.68 | 0.55 | 0.61 | 0.79 |
| Decision Tree | 81.3% | 0.58 | 0.62 | 0.60 | 0.73 |

### Best Model: XGBoost Classifier
- **ROC-AUC Score:** 0.85
- **Cross-validation Score:** 86.8%

### Top 10 Predictive Features
1. OverTime
2. Monthly Income
3. Age
4. Total Working Years
5. Years At Company
6. Years In Current Role
7. Job Satisfaction
8. Environment Satisfaction
9. Job Involvement
10. Distance From Home

  --
  ##🛠️ Tech Stack & Tools

| Category | Tools Used |
|----------|-----------|
| Programming Language | Python 3.8+ |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn, Plotly |
| Machine Learning | Scikit-Learn, XGBoost |
| Statistical Analysis | SciPy, Statsmodels |
| IDE | Jupyter Notebook |

---
##📂 Project Structure

```
HR-ANALYTICS-/
│
├── 📁 data/
│   ├── WA_Fn_UseC_HR_Employee_Attrition.csv    # Raw dataset
│   └── processed_data.csv                       # Cleaned data
│
├── 📁 notebooks/
│   ├── 01_EDA_and_Data_Cleaning.ipynb           # Exploratory analysis
│   ├── 02_Feature_Engineering.ipynb             # Feature creation
│   ├── 03_Statistical_Analysis.ipynb            # Statistical tests
│   └── 04_Model_Building.ipynb                  # ML models
│
├── 📁 visualizations/
│   ├── attrition_by_department.png
│   ├── correlation_heatmap.png
│   ├── feature_importance.png
│   └── salary_distribution.png
│
├── 📁 models/
│   ├── xgboost_model.pkl                        # Saved model
│   └── model_metrics.json                       # Performance metrics
│
├── 📁 reports/
│   └── HR_Analytics_Report.pdf                  # Final report
│
├── 📄 README.md
├── 📄 requirements.txt
└── 📄 .gitignore
```

---
.🚀 Getting Started
### Prerequisites
- Python 3.8 or higher
- pip package manager

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/ibadkadri924-design/HR-ANALYTICS-.git
cd HR-ANALYTICS-
```

2. **Create virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Run Jupyter Notebook**
```bash
jupyter notebook
```

5. **Open notebooks in order:**
   - Start with `01_EDA_and_Data_Cleaning.ipynb`
   - Follow with subsequent notebooks

---
##📋 Requirements

```txt
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
plotly>=5.3.0
scikit-learn>=1.0.0
xgboost>=1.5.0
scipy>=1.7.0
statsmodels>=0.13.0
jupyter>=1.0.0
```

---

## 📊 Visualizations

### Correlation Heatmap
Shows relationships between numerical features and identifies multicollinearity.

### Attrition Distribution by Key Factors
Visual breakdown of attrition across different employee segments.

### Feature Importance Plot
Ranks features by their predictive power in the attrition model.

### Salary vs Attrition Analysis
Examines the relationship between compensation and employee retention.

---

## 💡 Business Recommendations

Based on the analysis, here are actionable strategies for HR:

---
###Immediate Actions
| Priority | Recommendation | Expected Impact |
|----------|---------------|-----------------|
| 🔴 High | Implement overtime monitoring and fair compensation policies | Reduce attrition by 15-20% |
| 🔴 High | Review salary structures for competitive positioning | Improve retention of key talent |
| 🟡 Medium | Develop### Immediate Actions career progression programs | Reduce early-career attrition |

### Long-term Strategies
| Strategy | Target Group | Timeline |
|----------|-------------|----------|
| Flexible work arrangements | Employees with long commutes | 3-6 months |
| Mentorship programs | New hires (< 2 years) | 6 months |
| Job rotation opportunities | Employees in same role > 4 years | 1 year |
| Performance-based incentives | Sales team | Immediate |

### Department-Specific Actions
- **Sales:** Review commission structures, reduce unrealistic targets
- **HR:** Focus on employee engagement initiatives
- **R&D:** Provide growth opportunities and skill development

---

## 📈 Future Scope

- [ ] Build an interactive dashboard using Streamlit/Dash
- [ ] Implement employee risk scoring system
- [ ] Add real-time prediction API
- [ ] Include employee survey data integration
- [ ] Develop automated reporting system
- [ ] Create Power BI/Tableau visualization

 ---
 ##📝 Key Learnings

1. **Data Quality Matters:** Clean, well-documented datasets are crucial for reliable insights
2. **Domain Knowledge:** Understanding HR processes enhances analysis quality
3. **Model Interpretability:** Business stakeholders need understandable models, not just accurate ones
4. **Actionable Insights:** Analysis must lead to concrete recommendations
5. **Communication:** Visual storytelling is essential for stakeholder buy-in

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📬 Contact

**Ibad Kadri**
- GitHub: [@ibadkadri924-design](https://github.com/ibadkadri924-design)
- LinkedIn: [Connect with me](https://www.linkedin.com/)

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
