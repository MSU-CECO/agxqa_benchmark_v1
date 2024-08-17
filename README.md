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

The Python packages can be installed in a conda environment:
```
conda env create -f environment.yaml
```

## Data Preparation



## Model Training


## Acknowledgments

- AgXQA was inspired by Rajpurkar et al. (2016)'s work on [SQuAD](https://aclanthology.org/D16-1264).

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

