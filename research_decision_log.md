# Research Decision Log

## Dataset audit

- **Dataset:** PlantVillage, sourced through the `mohanty/PlantVillage` Hugging Face repository.
- **Selected representation:** Color (RGB).
- **Selected classes:** 10 tomato leaf categories.
- **Images audited:** 18,160.
- **Readable images:** 18,160.
- **Unreadable images:** 0.
- **Exact duplicate groups:** 14.
- **Redundant copies excluded:** 14.
- **Unique images retained:** 18,146.
- **Cross-class exact duplicates:** None detected.

## Dataset provenance

- **Download date:** To be confirmed from the download record.
- **Dataset revision/version:** To be recorded.
- **License:** Verify the source repository's license and conditions before redistribution.
- **Class mapping:** Folder names inspected; source metadata verification pending.

## Data quality and limitations

- Class counts are imbalanced, ranging from 373 to 5,357 images.
- Exact duplicates have been identified and excluded from the experiment manifest.
- Visual label verification and near-duplicate analysis remain pending.
- Controlled dataset conditions may limit generalization to real-world field images.

## Experimental protocol

- **Data split:** Pending source split and leaf-grouping metadata inspection.
- **Leakage prevention:** Images associated with the same physical leaf must not cross dataset splits.
- **Baseline model:** Not yet trained.
- **Evaluation metrics:** Accuracy, macro F1-score, and per-class precision and recall are planned.
- **Reproducibility:** Record split assignments, random seeds, model configuration, and software versions.

## Current decision

The initial file-integrity audit is complete. Model training will begin after source metadata and the data-splitting protocol have been reviewed.

## Next actions

1. Verify the source metadata and licensing.
2. Finalize the leakage-aware train/validation/test split.
3. Create the real-image baseline notebook.
4. Record baseline results before experimenting with improvements.
