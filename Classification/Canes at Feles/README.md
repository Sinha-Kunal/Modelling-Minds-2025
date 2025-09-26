# Modelling Minds - VITMAS
# Canes et Feles

**Dataset Link:** . 
## Objective
Multi-class image classification of animals into 17 distinct categories, including various wild cats, dogs, and other mammals.

## Dataset Description
This dataset contains images organized into 17 animal classes. The dataset follows a standard train/test split structure with labeled train directories for supervised learning.

**Classes (17 total):**
- cheetahs
- jaguars
- snow leopards
- panthers
- mountain lions
- leopards
- japanese spaniel
- borzoi
- bull terrier
- cocker
- coyote
- afghan
- blenheim
- yorkshire terrier
- mex hairless
- rhodesian
- staffordshire bull terrier

**Directory Structure:**
```
canes et feles/
├── train/
│   ├── cheetahs/
│   ├── jaguars/
│   ├── snow_leopards/
│   ├──panthers/
│   ├──mountain lions/
│   ├──leopards/
│   ├──japanese spaniel/
│   ├──borzoi/
│   ├──bull terrier/
│   ├──cocker/
│   ├──coyote/
│   ├──afghan/
│   ├──blenheim/
│   ├──yorkshire terrier/
│   ├──mex hairless/
│   ├──rhodesian/
│   └──staffordshire bull terrier/
├── test/
└── is this supposed to be here/
```

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
Submission has to be a CSV file. The file name must be **{team_ID}_{track_name}.csv** 
The submitted file cannot be edited after 6:00 A.M. on 28th Sept. 2025.
