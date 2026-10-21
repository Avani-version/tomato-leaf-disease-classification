# Tomato Leaf Disease Classification

## Overview

This project investigates deep learning methods for classifying tomato leaf images into 10 health and disease categories. The goal is to build a reproducible experimental pipeline, establish a reliable baseline, and evaluate model performance using appropriate metrics.

## Research Objectives

- Audit and document the dataset.
- Establish a reproducible training, validation, and testing protocol.
- Train a real-image baseline model.
- Compare candidate deep learning architectures under consistent experimental conditions.
- Evaluate class-wise performance and investigate limitations in generalization.
- Explore further improvements only when supported by baseline results.

## Dataset

- **Source:** [PlantVillage dataset on Hugging Face](https://huggingface.co/datasets/mohanty/PlantVillage)
- **Image representation:** Color (RGB)
- **Selected categories:** 10 tomato leaf classes
- **Unique images after exact-duplicate removal:** 18,146

The dataset contains images collected under relatively controlled conditions. Results on this dataset may not fully represent performance on real-world field photographs.

Please consult the source dataset documentation and applicable license terms before redistributing data.

## Current Progress

- [x] Downloaded the color-image dataset.
- [x] Selected the 10 tomato leaf categories.
- [x] Audited image readability and dimensions.
- [x] Identified 14 groups of exact duplicate images.
- [x] Created a deduplicated image manifest.
- [ ] Verify source metadata and label mapping.
- [ ] Finalize a leakage-aware data-splitting protocol.
- [ ] Train and evaluate the baseline model.
- [ ] Compare model architectures.
- [ ] Document experimental results and limitations.

## Planned Project Structure

```text
tomato-leaf-disease-classification/
├── README.md
├── research_decision_log.md
├── notebooks/
│   ├── 01_data_audit.ipynb
│   └── 02_real_image_baseline.ipynb
├── src/
├── configs/
└── reports/
```

Additional files and directories will be introduced as the project develops.

## Reproducibility

Experiments will document dataset preparation, data splits, random seeds, model configurations, evaluation metrics, and software dependencies wherever applicable.

## Limitations

High performance on a controlled image dataset does not establish clinical or agricultural reliability in field conditions. Independent real-world evaluation is desirable before drawing broader conclusions.

## Project Status

**Current stage:** Dataset auditing and experimental design.

No baseline performance claims are made at this stage.

