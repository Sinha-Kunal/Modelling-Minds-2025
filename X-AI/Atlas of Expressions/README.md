# Modelling Minds - VITMAS
# Atlas of Expressions
# Track ID: XAE001F
**Dataset Link:** . 
## Objective
Analyze gene expression data to identify the most highly expressed genes (ENSIG No. and Gene Name) in specific cell types using Explainable AI (XAI) techniques. The analysis must utilize SHAP, LIME, or MRMR scores for feature importance and interpretability.

## Dataset Description
This dataset contains single-cell gene expression data structured across three CSV files that together form a complete expression matrix with cell metadata and gene annotations. The task involves analyzing expression patterns and identifying key genes for different cell types using explainable AI methods.

**Data Format:** Three interconnected CSV files

**File Structure:**
```
Atlas of Expressions/
├── Barcodes.csv
├── Matrix.csv
└── Genes.csv
```

**File Descriptions:**

### 1. Barcodes.csv
Contains cell metadata and type information
**Columns:**
- **Sample**: Sample identifier
- **Cell Barcode**: Unique cell identifier
- **Type**: Cell type classification

### 2. Matrix.csv
Contains the gene expression matrix in sparse format
**Columns:**
- **row**: Row index (corresponds to genes)
- **col**: Column index (corresponds to cells)
- **value**: Expression value

### 3. Genes.csv
Contains gene annotation information
**Columns:**
- **ENSIG No.**: Ensemble gene identifier
- **Gene Name**: Human-readable gene name

**Task Requirements:**
- Perform gene expression analysis for different cell types
- Identify most highly expressed genes per cell type
- Use only approved XAI methods: SHAP, LIME, or MRMR
- Report both ENSIG No. and Gene Name for top expressed genes
- Provide explainability scores for gene importance

## Evaluation Metrics

### Explainable AI Methods (Required)

#### 1. SHAP (SHapley Additive exPlanations)
#### 2. LIME (Local Interpretable Model-agnostic Explanations)
#### 3. MRMR (Minimum Redundancy Maximum Relevance)

**Analysis Requirements:**
- Feature importance scores must be generated using one of the approved methods
- Results must include statistical significance.
- Inculding the biological significance will lead to bonus points.
- Gene rankings should be provided with corresponding XAI scores

## Submission Format
Submission has to be a CSV file. The file name must be **{team_ID}_{track_ID}.csv** 
The submitted file cannot be edited after 6:00 A.M. on 28th Sept. 2025.

**Expected Output Format:**
Results should include cell type, ENSIG No., Gene Name, and XAI importance scores for the most expressed genes per cell type.