# open-vocabulary-hallucination-reliability
Code for quantifying and mitigating hallucinations in open-vocabulary object detection.

# Quantifying and Mitigating Hallucinations in Open-Vocabulary Object Detection

This repository contains the experimental notebook for the study:

**Quantifying and Mitigating Hallucinations in Open-Vocabulary Object Detection: A Reliability Framework**

## Overview

The notebook evaluates hallucination behaviour in open-vocabulary object detection using OWL-ViT and Grounding DINO. The study analyses hallucination rates, typed hallucination decomposition, evidence-based verification, counter-evidence prompting, confidence calibration, prompt robustness, suppression--recall trade-offs, and bootstrap confidence intervals.

## Models

- OWL-ViT
- Grounding DINO

## Dataset

The main evaluation uses the MS-COCO 2017 validation split. The experiments use 1,000 qualifying validation images containing at least one of 17 held-out COCO categories.

The COCO and LVIS datasets are not redistributed in this repository. Users should download them from their official sources.

## Main analyses

- Baseline hallucination quantification
- Semantic / attribute / localisation decomposition
- Evidence-based verification
- Counter-evidence prompting
- Confidence calibration
- Prompt robustness
- Frequency-tier proxy analysis
- Suppression--recall trade-off
- Bootstrap confidence intervals

## Files

- `sinjini-banerjee-bthesis-2026.ipynb` — main experimental notebook
- `requirements.txt` — Python package requirements
- `dataset_links.txt` — dataset source links and notes

## Reproducibility

The notebook was executed in a Kaggle environment using a Tesla T4 GPU. The random seed is fixed at 42. Some analyses use subsets of the main evaluation set due to the computational cost of embedding-based scoring.

## Notes

Large datasets and model checkpoints are not included in this repository.
