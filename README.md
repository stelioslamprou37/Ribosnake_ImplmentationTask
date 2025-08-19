# 16S rRNA Mock Pipeline Evaluation Task

This submission contains a reproducible workflow and evaluation questions based on a 16S rRNA mock dataset.

## Overview

The dataset used is derived from the QIIME 2 tutorial: CASAVA 1.8 paired-end demultiplexed FASTQ files. Only forward (R1) reads are processed.

The pipeline performs the following steps:

1. Quality Control (Phred ≥ 20)
2. Adapter Trimming (Illumina universal adapter: AGATCGGAAGAGC)
3. Unique sequence detection (ASVs)
4. Summary statistics on per-sample read retention

## Files

- `questions.yaml`: Five objective questions based on the pipeline.
- `answers.yaml`: Ground-truth answers.
- `workflow/run_pipeline.py`: Script to execute the pipeline.
- `data/casava-18-paired-end-demultiplexed.zip`: Dataset (forward reads only).

## Source

- Dataset: [QIIME 2 Tutorial](https://data.qiime2.org/2022.2/tutorials/importing/casava-18-paired-end-demultiplexed.zip)
- Paper reference: Mock task inspired by QIIME 2 usage.
- Tools: Python, Cutadapt, custom script (no third-party dependencies).

## Instructions

1. Unzip the dataset.
2. Run `run_pipeline.py` on the unzipped directory.
3. Answer the questions in `questions.yaml`.
