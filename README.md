# SciBERT Citation Function Classifier

This repository provides the code and instructions to train a SciBERT-based model for citation function classification, as used in the CiteSense framework. The model is designed to categorize citation contexts according to citation functions such as background, contrast, motivation, extension uses, and future, facilitating both citation analysis and citation-aware recommendation tasks.

## Overview

The training pipeline leverages the [SciBERT](https://huggingface.co/allenai/scibert_scivocab_uncased) language model to classify citation contexts using labeled datasets. This component is used in the CiteSense framework, which integrates citation function modeling with local citation recommendation.

Both notebooks contains the same trainning, but using different metrics. Addtionally, the notebook named "... context-micro" also include the analysis about the recall and precision of the best model

Checkpoints used on the research are available on hugging face hub: juansanguino/SciBERT-citation-score

## Features

- Fine-tunes SciBERT on a custom citation function classification dataset.
- Supports multi-class classification based on citation motivation taxonomies.


Install dependencies with:

#### Note: Check before the cuda version of your GPU and setting the respective version before to install dependecies

```bash
pip install -r requirements.txt
