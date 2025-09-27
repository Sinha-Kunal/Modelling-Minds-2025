# Modelling Minds - VITMAS
# Codex of Conundrums
# Track ID: CCC02A
**Dataset Link:** [Codex of Conundrums Dataset](https://kaggle.com/datasets/4a1e06fd4e57334d09cc5dada035ebab749a87175bdad385a76a4fb0fcfb5175)
## Objective
Multi-class classification of mathematical problems into 7 distinct categories covering various areas of mathematics from basic algebra to advanced number theory, based on structured problem data including problem statements, difficulty levels, types, and solutions.

## Dataset Description
This dataset contains mathematical problems organized into 7 mathematical subject classes. Each class in the train directory contains JSON files with structured problem data. The dataset follows a standard train/test split structure with labeled train directories for supervised learning.

**Classes (7 total):**
- algebra
- counting_and_probability
- geometry
- intermediate_algebra
- number_theory
- prealgebra
- precalculus

**Directory Structure:**
```
codex of conundrums/
├── train/
│   ├── algebra/
│   │   └── [JSON files with problem data]
│   ├── counting_and_probability/
│   │   └── [JSON files with problem data]
│   ├── geometry/
│   │   └── [JSON files with problem data]
│   ├── intermediate_algebra/
│   │   └── [JSON files with problem data]
│   ├── number_theory/
│   │   └── [JSON files with problem data]
│   ├── prealgebra/
│   │   └── [JSON files with problem data]
│   └── precalculus/
│       └── [JSON files with problem data]
└── test/
```

**JSON File Format:**
Each class directory contains JSON files structured as follows:
```json
{
    "problem": "Let $f(x)=7x+5$ and $g(x)=x-1$. If $h(x)=f(g(x))$, then what is the inverse of $h(x)$?",
    "level": "Level 4",
    "type": "Algebra",
    "solution": "\\[h(x)=f(g(x))=7(x-1)+5=7x-2.\\]Let's replace $h(x)$ with $y$ for simplicity, so \\[y=7x-2.\\]In order to invert $h(x)$ we may solve this equation for $x$. That gives \\[y+2=7x\\]or \\[x=\\frac{y+2}{7}.\\]Writing this in terms of $x$ gives the inverse function of $h$ as \\[h^{-1}(x)=\\boxed{\\frac{x+2}{7}}.\\]"
}
```

**JSON Fields:**
- **problem**: The mathematical problem statement
- **level**: Difficulty level (e.g., "Level 4")
- **type**: Mathematical subject category
- **solution**: Detailed solution with mathematical notation

## Evaluation Metrics

### 1. F1-Score (Primary)
**Formula:** F1 = 2 × (Precision × Recall) / (Precision + Recall)
### 2. Accuracy
**Formula:** Accuracy = (TP + TN) / (TP + TN + FP + FN)
### 3. Precision
**Formula:** Precision = TP / (TP + FP)
### 4. Recall
**Formula:** Recall = TP / (TP + FN)

**Legend:**
- TP: True Positives
- TN: True Negatives  
- FP: False Positives
- FN: False Negatives

## Submission Format
Submission has to be a CSV file. The file name must be **{team_ID}_{track_ID}.csv** 

The submitted file cannot be edited after 6:00 A.M. on 28th Sept. 2025.
