# AI Bias Mitigation Workshop for Black Women in Data

## Addressing Fairness in Machine Learning Models

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-orange.svg)](https://jupyter.org/)

This repository contains hands-on examples and workshops demonstrating how to identify, measure, and mitigate bias in machine learning models using two leading fairness libraries: **Fairlearn** and **AIF360**.

## Overview

Machine learning models can perpetuate and amplify existing biases present in training data, leading to unfair outcomes for protected groups. This workshop provides practical tools and techniques to build more equitable AI systems.

### What You'll Learn
- How to detect bias in ML models
- Pre-processing, in-processing, and post-processing bias mitigation techniques
- Fairness metrics and trade-offs
- Real-world implementation using industry-standard libraries

## Repository Structure

```
├── notebooks/
├── fairlearn_bias_mitigation.ipynb    # Fairlearn implementation examples
├── aif360_bias_mitigation.ipynb       # AIF360 implementation examples
│── data/                              # Sample datasets
├── requirements.txt                   # Python dependencies
├── README.md                          # This file
└── LICENSE                            # MIT License
```

## Getting Started

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- Basic knowledge of machine learning and pandas

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ai-bias-mitigation-workshop.git
   cd ai-bias-mitigation-workshop
   ```

2. **Create virtual environment** (recommended)
   ```bash
   python -m venv bias-workshop
   source bias-workshop/bin/activate  # On Windows: bias-workshop\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter**
   ```bash
   jupyter notebook
   ```

## Notebooks Overview

### 1. Fairlearn Bias Mitigation (`fairlearn_resume_example.ipynb`)

**Microsoft's Fairlearn Library Implementation**

- **Focus**: Hiring bias detection and mitigation
- **Techniques Covered**:
  - Demographic Parity
  - Equalized Odds
  - Post-processing with Threshold Optimization
- **Key Features**:
  - Interactive fairness-accuracy trade-off visualizations
  - Multiple constraint types
  - Easy integration with scikit-learn

**Fairness Methods Demonstrated**:
-  **Exponentiated Gradient** - In-processing constraint optimization
-  **Threshold Optimizer** - Post-processing threshold adjustment
-  **Reductions Approach** - Converting fairness problems to cost-sensitive learning

### 2. AIF360 Bias Mitigation (`aif_360_example.ipynb`)

**IBM's AI Fairness 360 Toolkit Implementation**

- **Focus**: Comprehensive bias detection and mitigation pipeline
- **Techniques Covered**:
  - Pre-processing: Disparate Impact Remover, Reweighing
  - In-processing: Adversarial Debiasing, Fair Representation Learning
  - Post-processing: Calibrated Equalized Odds
- **Key Features**:
  - 70+ fairness metrics
  - Bias detection algorithms
  - Explainability tools

**Fairness Methods Demonstrated**:
- **Pre-processing**: Data transformation before training
- **In-processing**: Fairness-aware learning algorithms
- **Post-processing**: Outcome adjustment after prediction

## Key Fairness Concepts Covered

| Fairness Criterion | Description | When to Use |
|-------------------|-------------|-------------|
| **Demographic Parity** | Equal positive prediction rates across groups | Legal compliance, equal representation goals |
| **Equalized Odds** | Equal TPR and FPR across groups | Merit-based decisions with fairness |
| **Equal Opportunity** | Equal TPR across groups | When false negatives are more costly |
| **Calibration** | Equal positive predictive value across groups | When prediction confidence matters |

## Libraries Used

- **[Fairlearn](https://fairlearn.org/)** - Microsoft's fairness toolkit
- **[AIF360](https://aif360.mybluemix.net/)** - IBM's comprehensive fairness library
- **scikit-learn** - Machine learning algorithms
- **pandas** - Data manipulation
- **matplotlib/seaborn** - Data visualization
- **numpy** - Numerical computing

## Workshop Flow

1. **Data Exploration** - Understanding bias in datasets
2. **Bias Detection** - Measuring unfairness using various metrics
3. **Baseline Model** - Training biased models to establish benchmarks
4. **Bias Mitigation** - Applying fairness constraints and algorithms
5. **Evaluation** - Comparing fairness-accuracy trade-offs
6. **Interpretation** - Understanding results and business implications

## Sample Datasets

- **Synthetic Hiring Dataset** - Demonstrates employment bias scenarios
- **Adult Income Dataset** - Census data for income prediction
- **Custom generated data** - Controlled bias scenarios for learning

## Acknowledgments

- **Microsoft Fairlearn Team** for the excellent fairness toolkit
- **IBM Research** for the comprehensive AIF360 library
- **Black Women in Data organizers** for promoting responsible AI practices


---

### Star this repository if you found it helpful!

**Together, we can build more fair and equitable AI systems.** 🚀

---

*Last updated: 09-08-25*

### Binder Link!
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dpaq-lab/bwd/HEAD)
