# 🚖 Taxi Fraud Detection Analysis

**A comprehensive machine learning project for detecting and analyzing fraud in ride-based transactions using the STAR framework approach.**

---

## 📋 Project Overview (STAR Framework)

### 🎯 **Situation**
Ride-sharing and taxi companies face significant financial losses due to fraudulent transactions, particularly failed payments from first-time users and suspicious behavioral patterns. The challenge was to analyze a real-world taxi company dataset containing over 200,000 ride transactions to identify fraud indicators and develop predictive capabilities.

**Key Challenges:**
- High rate of payment failures among first-time users
- Geographic variations in fraud patterns across different countries
- Need to balance fraud detection with user experience
- Lack of systematic approach to identify high-risk user segments

### 📝 **Task**
Develop a comprehensive fraud detection system that could:
1. **Identify patterns** leading to first-time failed payments
2. **Segment users** by behavior to improve fraud detection accuracy
3. **Build predictive models** to classify failed vs. successful payments
4. **Provide actionable insights** for product and business decisions
5. **Create visualizations** to communicate findings effectively

### ⚡ **Action**
Implemented a structured data science pipeline with multiple analytical approaches:

#### **Data Analysis & Preparation**
- **Data Import & Cleaning**: Processed 200K+ transaction records with comprehensive data validation
- **Exploratory Data Analysis**: Conducted statistical analysis and correlation studies
- **Feature Engineering**: Created behavioral indicators, price ratios, and geographic features

#### **Advanced Analytics**
- **Geographic Visualization**: Country-level risk pattern analysis and transaction breakdowns
- **Regression Analysis**: Price-based behavior modeling and prediction signals
- **Clustering Analysis**: User behavior segmentation to isolate fraud-prone patterns
- **Machine Learning**: Built classification models with feature importance analysis

#### **Model Development**
- Implemented multiple ML algorithms for payment success prediction
- Performed comprehensive model evaluation using classification metrics
- Conducted feature importance analysis to identify key fraud indicators
- Validated model performance using ROC AUC and accuracy metrics

### 🏆 **Results**
Achieved exceptional model performance and actionable business insights:

#### **Model Performance**
- ✅ **Model Accuracy**: 97%
- 🧠 **ROC AUC Score**: 0.94
- 🔑 **Top Predictors**: `log_price_per_km`, `price`, `failed_before_success`, `is_first_attempt`
- 🌍 **Geographic Insights**: Identified high failure rates in specific country-device clusters

#### **Business Impact**
- **Risk Segmentation**: Successfully identified high-risk user patterns
- **Predictive Capability**: Enabled proactive fraud prevention
- **Geographic Intelligence**: Country-specific risk assessment
- **Behavioral Insights**: Clear patterns in first-time user failures

---

## 📁 Project Structure

```
Taxi/
├── 01 Product Management/          # Project requirements and specifications
│   └── Brief.pdf
├── 02 Data/                        # Raw and processed datasets
│   ├── Original data/              # Source data files
│   └── Prepared data/              # Cleaned and feature-engineered data
├── 03 Scripts/                     # Analysis notebooks and code
│   ├── 0.1 — Data import and descriptive analysis.ipynb
│   ├── 02_Correlation_cleaned.ipynb
│   ├── 0.3 Geographic Visualization.ipynb
│   ├── 0.4 — Regression.ipynb
│   ├── 0.5 — Clustering.ipynb
│   ├── 0.6 — Modeling.ipynb
│   └── structured_fraud_analysis_notebook.ipynb
├── 04 Analysis/                    # Generated visualizations and results
│   └── Visualisations/
└── 05 Sent to client/             # Final deliverables
```

## 📊 Analysis Pipeline

| Notebook | Description | Key Outputs |
|----------|-------------|-------------|
| **0.1 — Data import and descriptive analysis** | Data loading, cleaning, and initial statistics | Clean dataset, summary statistics |
| **02_Correlation_cleaned** | Correlation analysis between variables | Feature relationships, correlation matrix |
| **0.3 Geographic Visualization** | Country-level risk patterns and breakdowns | Geographic risk maps, country insights |
| **0.4 — Regression** | Price-based behavior and prediction signals | Regression models, price impact analysis |
| **0.5 — Clustering** | User behavior clustering for fraud patterns | User segments, behavioral clusters |
| **0.6 — Modeling** | ML model building and evaluation | Trained models, performance metrics |
| **structured_fraud_analysis_notebook** | Combined insights and final analysis | Complete analysis, recommendations |

## 🎯 Key Findings

### **Fraud Indicators**
- **Price Sensitivity**: Higher prices correlate with increased failure rates
- **First-Time Users**: Significantly higher failure rates among new users
- **Geographic Patterns**: Specific country-device combinations show elevated risk
- **Behavioral Signals**: Users with previous failures show predictable patterns

### **Risk Segments**
- **High-Risk**: First-time users with high-price rides in specific countries
- **Medium-Risk**: Repeat users with previous payment failures
- **Low-Risk**: Established users with consistent payment history

## 🚀 Product Recommendations

Based on the analysis results, implemented the following fraud prevention strategies:

### **Immediate Actions**
1. **Pre-ride Verification**: Require card verification for high-risk segments
2. **Soft Blocks**: Implement email/phone verification for suspicious first-time users
3. **Price Caps**: Limit ride prices for unverified or high-risk users

### **Long-term Strategies**
1. **Dynamic Risk Scoring**: Real-time risk assessment based on model predictions
2. **Geographic Controls**: Country-specific fraud prevention measures
3. **Behavioral Monitoring**: Continuous tracking of user payment patterns

## 📈 Interactive Dashboard

**🔗 [View Full Tableau Storyboard](https://public.tableau.com/views/TaxiFraudAnalysis/Story)** 

Explore the complete visual analysis including:
- Geographic risk heatmaps
- User behavior clustering
- Model performance metrics
- Business impact projections

## 🛠️ Technical Stack

- **Python**: Data analysis and machine learning
- **Pandas**: Data manipulation and cleaning
- **Scikit-learn**: Machine learning models
- **Matplotlib/Seaborn**: Data visualization
- **Jupyter Notebooks**: Interactive analysis
- **Tableau**: Business intelligence dashboards

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/HlibHav/Taxi.git
   cd Taxi
   ```

2. **Set up environment**
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn jupyter
   ```

3. **Run the analysis**
   - Start with `0.1 — Data import and descriptive analysis.ipynb`
   - Follow the numbered sequence through the analysis pipeline
   - Review final insights in `structured_fraud_analysis_notebook.ipynb`

4. **Explore results**
   - Check visualizations in `04 Analysis/Visualisations/`
   - Review the interactive Tableau dashboard

## 📊 Model Performance Details

| Metric | Value | Interpretation |
|--------|-------|----------------|
| **Accuracy** | 97% | Correctly classified 97% of transactions |
| **ROC AUC** | 0.94 | Excellent discrimination between fraud/legitimate |
| **Precision** | High | Low false positive rate |
| **Recall** | High | Successfully identifies most fraud cases |

## 🤝 Contributing

This project demonstrates a complete fraud detection pipeline. Feel free to:
- Explore the analysis notebooks
- Suggest improvements to the modeling approach
- Contribute additional visualization techniques
- Propose new feature engineering ideas

## 📄 License

This project is for educational and demonstration purposes. The dataset used is proprietary and not publicly available.

---

**Built with ❤️ for data-driven fraud prevention**
