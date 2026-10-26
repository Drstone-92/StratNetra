# StratNetra

**StratNetra** is a Python-based research workflow for
sedimentary-structure image classification, quantitative lamina
analysis, and sedimentological interpretation in siliciclastic rocks.

This repository contains notebooks intended to develop, evaluate,
compare, and apply the StratNetra workflow.

## System requirements

-   **Programming language:** Python 3.10
-   **Operating system:** Windows 11
-   **Hardware:** Intel Core i5 CPU and 32 GB RAM
-   **Additional standalone software:** None specified

Python packages listed in `requirements.txt` must be installed in the
Python environment. The notebooks may be run in a compatible Jupyter
environment if they use Jupyter notebooks. The exact environment should
be checked against the notebook imports and tested workflow before
claiming reproducibility.

## Repository contents

The filenames below are suggested names based on the notebooks described
for this project. Update them to match the final repository, or keep
your existing filenames.

  -------------------------------------------------------------------------
  Notebook                              Purpose
  ------------------------------------- -----------------------------------
  `01_CNN_Model_Training.ipynb`         Training CNN-based
                                        sedimentary-structure classifiers.

  `02_CNN_Evaluation.ipynb`             CNN evaluation, prediction
                                        analysis, and benchmarking.

  `03_ViT_Training_Evaluation.ipynb`    Vision Transformer (ViT) training
                                        and evaluation.

  `04_CNN_vs_ViT_Benchmark.ipynb`       Comparative analysis of CNN and ViT
                                        model performance.

  `05_StratNetra_User_Workflow.ipynb`   Main user workflow: structure
                                        identification, structure-specific
                                        analysis, lamina detection and
                                        geometric characterization where
                                        applicable, and final
                                        sedimentological interpretation.
  -------------------------------------------------------------------------

The main user workflow is the recommended starting point for applying
the pipeline. The training and benchmarking notebooks document model
development and evaluation.

## Workflow overview

1.  **Input image:** Provide an image in the format accepted by the
    selected notebook.
2.  **Structure identification:** Run the trained classifier to predict
    a supported sedimentary-structure class.
3.  **Structure-specific analysis:** Route the classified image to the
    relevant analysis procedure, where implemented.
4.  **Lamina analysis:** For applicable structures, detect laminae and
    calculate geometric measurements supported by the code, such as
    apparent dip, thickness, or spacing.
5.  **Outputs and interpretation:** Review generated visualizations and
    data tables, then use the quantitative results to support
    sedimentological interpretation.

The exact supported classes, measurements, output files, and
interpretation rules must be confirmed from the notebook implementation.
Automated outputs should be checked against geological context and,
where possible, independent/manual observations.

## Installation

1.  Install Python 3.10.

2.  Download or clone this repository.

3.  Open a terminal in the repository folder.

4.  Install the Python dependencies:

    ``` bash
    python -m pip install --upgrade pip
    pip install -r requirements.txt
    ```

5.  Launch a Jupyter environment if needed to run the notebooks:

    ``` bash
    jupyter notebook
    ```

6.  Open the desired notebook and execute its cells in order.

If a notebook expects trained model weights, an image dataset,
calibration CSV files, or other external files, make sure those files
are available and update the relevant paths/configuration cells as
needed.

## Data and trained models

Do not assume that the image dataset or trained model weights are
included in this repository. If they are not, provide instructions for
obtaining them, subject to relevant licences and permissions. Do not
upload private, restricted, or third-party material unless you have
permission to redistribute it.

Before sharing the repository, check for: - absolute paths tied to a
particular computer; - missing data, model weights, calibration files,
or configuration files; - large files that should be hosted
separately; - notebook outputs containing private information or
unnecessarily large embedded images.

## Recommended citation

If you use StratNetra in research, please cite the associated
manuscript:

> Bailwal, R. et al. *StratNetra: Integrated deep learning and image
> analysis framework for automated sedimentary structure
> characterization in siliciclastic rocks.* \[Add journal, year, DOI,
> and the final author list after publication.\]

Replace the placeholder with the final bibliographic information when
available.

## Code status

This repository accompanies a research workflow. Unless explicitly
documented otherwise, notebooks should be treated as research code, and
outputs should be independently checked before being used to support
scientific conclusions.

## Contact

For questions about the workflow, contact the corresponding author
listed in the associated manuscript.
