# AgXQA: A benchmark for advanced Agricultural Extension question answering

Repository of code related to the [AgXQA v1](https://doi.org/10.1016/j.compag.2024.109349) paper 


## Table of Contents

- [Abstract](#abstract)
- [Dependencies](#dependencies)
- [Data Preparation](#data-preparation)
- [Model Training](#data-preparation)
- [Acknowledgments](#acknowledgments)
- [Citation](#citation)

## Abstract
This study addresses the limited application of large language models (LLMs) in the Agricultural Extension (AE) domain due to challenges with unstructured data and the limitations of general LLMs in handling domain-specific tasks. We introduced a new QA benchmark dataset, AgXQA, and further fine-tuned an encoder-LM, AgRoBERTa, which outperformed mainstream models in extractive QA tasks. AgRoBERTa achieved notable scores (EM: 55.15%, F1: 78.89%) and was validated with a custom human evaluation metric, showing a high agreement with expert assessments. The study underscores the potential of specialized LLMs to enhance agricultural practices through improved domain-specific NLP capabilities.

## Dependencies

The Python packages can be installed in a conda environment.
 * Instructions for Tranformers: [here](https://huggingface.co/docs/transformers/installation)
 * Instructions for Adapters-Tranformers:  [here](https://docs.adapterhub.ml/installation.html)

## Data Preparation

Please check out the README.md inside the `data` folder for further details. The HuggingFace repositories for the resulting datasets can be found here:
- [AEC v1](https://huggingface.co/datasets/msu-ceco/aec_v1)
- [AgXQA v1](https://huggingface.co/datasets/msu-ceco/agxqa_v1)

## Model Training

We used the standard and official scripts for the appropriate downstream tasks:
- [For MLM](https://github.com/huggingface/transformers/tree/main/examples/pytorch/language-modeling#robertabertdistilbert-and-masked-language-modeling)
- [For QA fine-tuning](https://github.com/huggingface/transformers/tree/main/examples/pytorch/question-answering)
- [For PEFT-based QA fine-tuning](https://github.com/adapter-hub/adapters/tree/main/examples/pytorch/question-answering)

The resulting models are hosted on our HuggingFace page:
- Base model (after MLM): [roberta-ft-on-agextcorpus](https://huggingface.co/msu-ceco/roberta-ft-on-agextcorpus-2023-12-10_v2)
- AgRoBERTa (post Pfeiffer pretrained adapter): [agroberta](https://huggingface.co/msu-ceco/agroberta_2024-01-11_21-02-21)

## Acknowledgments

- The format of AgXQA was inspired by Rajpurkar et al. (2016)'s work on [SQuAD](https://aclanthology.org/D16-1264).
- The modeleling code for MLM and QA tasks came from HF's [Transformers](https://github.com/huggingface/transformers) and the [Adapters](https://github.com/adapter-hub/adapters) libraries repositories.

## Citation

**BibTeX:**

```
@article{KPODO2024109349,
    title = {AgXQA: A benchmark for advanced Agricultural Extension question answering},
    journal = {Computers and Electronics in Agriculture},
    volume = {225},
    pages = {109349},
    year = {2024},
    issn = {0168-1699},
    doi = {https://doi.org/10.1016/j.compag.2024.109349},
    url = {https://www.sciencedirect.com/science/article/pii/S0168169924007403},
    author = {Josué Kpodo and Parisa Kordjamshidi and A. Pouyan Nejadhashemi},
    keywords = {Agricultural Extension, Question-Answering, Annotated Dataset, Large Language Models, Zero-Shot Learning},
}

```

**APA:**

```
Kpodo, J., Kordjamshidi, P., & Nejadhashemi, A. P. (2024). AgXQA: A benchmark for advanced Agricultural Extension question answering. Computers and Electronics in Agriculture, 225, 109349. https://doi.org/10.1016/J.COMPAG.2024.109349 
```

