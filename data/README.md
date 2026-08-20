# Data Directory

This directory is structured to separate raw source data from processed datasets used in modeling and evaluation.

## Directory Structure

- `raw/`: Contains original, unmodified datasets. For this project, this will contain the Kaggle sample/subset of the **Google Cluster Trace 2019**.
- `processed/`: Contains intermediate and fully processed data (e.g., cleaned traces, aggregated usage tables, training/testing splits) that are ready for forecasting and optimization.

## Data Governance & Version Control Guideline

> [!IMPORTANT]
> **Do not commit raw or processed datasets to Git/GitHub.**
> Large dataset files must not be committed to avoid repository bloat and potential licensing violations. Ensure that files in these directories are ignored by git (e.g., via `.gitignore` rules like `data/raw/*` and `data/processed/*` except for `.gitkeep`).

## Dataset Provenance & Metadata

- **Source:** Google Cluster Trace 2019 sample/subset.
- **Acquisition:** Downloaded from Kaggle (provenance and exact URL will be documented here once the specific subset link is finalized).
- **Target Features:** Average CPU usage (`average_usage`) and related workload characteristics.
- **Licensing:** Refer to the official Google Cluster Data license terms.
