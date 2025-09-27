# Modelling Minds - VITMAS
# Resilient Minds
# Track ID: XRM002K
**Dataset Link:** [Resilient Minds Dataset](https://www.kaggle.com/datasets/6a32eafd9553a231912d75d97ab03b658f6fa691637dc88643cd1dd9a2ca29f1)
## Objective
Analyze student mental health data to identify patterns, risk factors, and relationships between academic performance, demographics, and mental health conditions. The analysis focuses on understanding factors that contribute to depression, anxiety, and panic attack diagnoses among students.

## Dataset Description
This dataset contains student mental health survey data with demographic information, academic performance metrics, and mental health diagnosis information. The task involves comprehensive analysis to understand mental health patterns in the student population.

**Data Format:** Single CSV file containing survey responses

**File Structure:**
```
Resilient Minds/
└── resilient_minds.csv
```

**Dataset Columns (10 total):**
- **Choose your gender**: Gender identity of the respondent
- **Age**: Age of the student
- **course**: Academic course/program of study
- **year of Study**: Current year of academic study
- **CGPA**: Cumulative Grade Point Average
- **Relationship status**: Current relationship status
- **Depression diagnosis**: Depression diagnosis status
- **Anxiety diagnosis**: Anxiety diagnosis status
- **Panic attack diagnosis**: Panic attack diagnosis status
- **any ongoing treatment?**: Current treatment status for mental health

**Task Requirements:**
- Perform comprehensive analysis of mental health patterns
- Identify correlations between academic performance and mental health
- Analyze demographic factors influencing mental health outcomes
- Examine relationships between different mental health conditions
- Provide insights into risk factors and protective factors

## Evaluation Metrics

### Explainable AI Methods (Required)

#### 1. SHAP (SHapley Additive exPlanations)
#### 2. LIME (Local Interpretable Model-agnostic Explanations)
#### 3. MRMR (Minimum Redundancy Maximum Relevance)

**Analysis Requirements:**
- Feature importance scores must be generated using one of the approved methods
- Results must include both statistical significance and interpretability
- Factor rankings should be provided with corresponding XAI scores

## Submission Format
Submission has to be a CSV file. The file name must be **{team_ID}_{track_ID}.csv** 
The submitted file cannot be edited after 6:00 A.M. on 28th Sept. 2025.

**Expected Output:**
Analysis results, statistical findings, identified patterns, and recommendations based on the mental health data analysis.



