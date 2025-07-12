# Task: Assemble Benchmark Dataset Collection

## Objective
Create a curated collection of diverse benchmark datasets for validating the coherence metric across different data types and low-rank modeling approaches.

## Deliverables

### 1. Dataset Collection
Assemble at least 10 datasets covering:
- **Text data** (3+ datasets)
- **Image data** (2+ datasets)  
- **Numerical/tabular data** (3+ datasets)
- **Time series data** (1+ dataset)
- **Mixed-type data** (1+ dataset)

### 2. Dataset Documentation
For each dataset, provide:
- Dataset name and source
- Dimensions (samples × features)
- Key characteristics (sparsity, distribution, known structure)
- Why this dataset tests coherence effectively
- Any preprocessing applied

### 3. Baseline Measurements
For each dataset, compute and record:
- Explained variance (PCA with k=10 components)
- Reconstruction error
- Basic statistics (mean, std, sparsity)

## Acceptance Criteria

- [ ] All datasets are publicly available or shareable
- [ ] Each dataset can be loaded with provided code
- [ ] Dataset sizes range from small (< 1K samples) to large (> 100K samples)
- [ ] Feature dimensions vary from low (< 100) to high (> 10K)
- [ ] All code to load and preprocess datasets is included
- [ ] Documentation is complete for all datasets
- [ ] Datasets cover different challenges (noise, sparsity, multimodality)
- [ ] Total collection can run on a machine with 32GB RAM

## Format
Organize as:
```
benchmark_datasets/
├── catalog.csv (summary table of all datasets)
├── load_datasets.py (unified loading script)
└── datasets/
    ├── text/
    ├── image/
    ├── numerical/
    ├── timeseries/
    └── mixed/
```

## Timeline
Expected completion: 2 weeks