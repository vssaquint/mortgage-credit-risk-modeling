# Mortgage Credit Risk Modeling with Temporal Calibration

**Master's in Economics**  
Universidad de Granada | March 2025 | Vanessa Quintero

## Project Overview

This project develops an advanced mortgage credit risk model using synthetic data designed to replicate temporal model drift challenges in financial applications. The core innovation addresses a 9x increase in default rates across economic regimes through a novel calibration adjustment system.

## Problem Statement

Traditional credit risk models suffer performance degradation during economic transitions. Using synthetic data that replicates real-world economic scenarios, this project demonstrates how models trained during stable periods (0.55% default rates) lose predictive power when economic conditions change dramatically (4.76% default rates post-pandemic).

## Key Technical Achievement

**Temporal Calibration Adjuster**: An economic regime-aware system that maintains model discrimination while adapting probability outputs to current economic conditions.

### Performance Results
- **Pandemic Crisis Period**: 87.8% prediction accuracy
- **Post-Pandemic Period**: 87.2% prediction accuracy  
- **Error Reduction**: 70% improvement over base model in current environments

## Methodology

### Data & Features
- Synthetic mortgage dataset spanning 2010-2024
- Economic regime classification: Recovery/Expansion, Pandemic Crisis, Post-Pandemic
- Features include credit scores, loan-to-value ratios, borrower demographics, temporal indicators

### Model Development
- **Algorithm Selection**: Gradient Boosting Classifier chosen through systematic comparison against Random Forest, Logistic Regression, and SVM
- **Machine Learning Pipeline**: Feature selection using F-statistics and mutual information, hyperparameter optimization via grid search and randomized search
- **Common ML Challenges Addressed**: Multicollinearity detection using Variance Inflation Factor (VIF), class imbalance handling for low default rates, overfitting prevention through cross-validation
- **Advanced Techniques**: Scikit-learn ensemble methods, cross-validation with temporal awareness, calibration curve analysis, missing value imputation strategies
- **Innovation**: Economic regime classification system with empirically-derived adjustment factors

### Regulatory Compliance
- Federal Reserve SR 11-7 requirements: Fully satisfied
- Basel III standards: Exceeded through comprehensive validation
- Population Stability Index (PSI) and Kolmogorov-Smirnov testing implemented

## Repository Structure

```
notebooks/
├── 01_project_overview_and_setup.ipynb
├── 02_data_understanding_and_exploration.ipynb  
├── 03_data_cleaning_and_preprocessing.ipynb
├── 04_exploratory_data_analysis.ipynb
├── 05_model_development.ipynb
├── 06_model_validation_and_testing.ipynb
└── 07_temporal_calibration_solution.ipynb
```

## Key Insights

1. **Economic Regime Impact**: Default rates increased 9x from recovery to post-pandemic periods
2. **Model Adaptation**: Successful calibration without loss of discriminatory power
3. **Regulatory Achievement**: Maintained compliance while enhancing performance
4. **Production Readiness**: Enterprise-grade deployment framework implemented

## Business Impact

The calibration system provides financial institutions with:
- Enhanced prediction accuracy during economic transitions
- Maintained regulatory compliance across economic cycles
- Transparent, auditable methodology for model risk management
- Framework applicable to multiple asset classes

## Technical Innovation

- **Object-oriented regime classification** with data-driven parameters
- **Multiplicative calibration adjustment** preserving model rankings
- **Production API** with comprehensive error handling and audit trails
- **Automated monitoring** for ongoing performance assessment

## Academic Contribution

This project demonstrates advanced application of:
- Machine learning for financial risk assessment
- Temporal model validation techniques
- Regulatory compliance implementation
- Production software development practices

The temporal calibration framework addresses a significant challenge in quantitative finance while maintaining academic rigor and regulatory standards.

## Future Applications

- Extension to other credit products and asset classes
- Integration with real-time economic indicators
- Automated regime detection using machine learning
- Enhanced regulatory reporting automation

---

**Universidad de Granada - Master's in Economics**  
*Advanced application of econometric and data science techniques for financial risk management*
