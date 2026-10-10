
# Stress-Testing Indonesian Sentiment Classification under Weak Supervision, Domain Generalization, and Character-Level Perturbations

## Authors

Zia Ul Rehman Zafar  
Dedi Gunawan  
Muhammad Nouman  

Department of Informatics Engineering  
Universitas Muhammadiyah Surakarta, Indonesia

---

## Overview

This repository accompanies the research study:

**Stress-Testing Indonesian Sentiment Classification under Weak Supervision, Domain Generalization, and Character-Level Perturbations**

The study investigates the robustness, generalization capability, and statistical reliability of Large Language Models for Indonesian sentiment analysis under realistic low-resource conditions.

The framework evaluates:

- Linear SVM (TF-IDF baseline)
- IndoBERT
- XLM-RoBERTa (XLM-R)

across:

- Cross-domain distributional shifts
- Synthetic noise perturbations
- Informal social-media language
- Formal news language
- Code-mixing scenarios

---

## Dataset

The corpus contains approximately 75,000 Indonesian-language sentiment samples collected from:

- YouTube comments
- Online news articles and comments

Domains include:

- Politics
- Economics
- Social issues
- Public policy

Sentiment labels:

- Negative
- Neutral
- Positive

---

## Experimental Pipeline

1. Data Collection
2. Data Preprocessing
3. Sentiment Modeling
4. Robustness Stress Testing
5. Cross-Domain Evaluation
6. Statistical Significance Testing

---

## Repository Structure

models/  
results/  
figures/  
appendix_figures/  
data/  
src/  
docs/

---

## Citation

If you use this repository, please cite the associated publication.

---

## License

MIT License


## Suplimentary Materials

The transformer models and Dataset are hosted separately on Hugging Face due to their size.

### IndoBERT
https://huggingface.co/mziarehman4353/LRSA-IndoBERT-Sentiment-ID/
### XLM-R
https://huggingface.co/mziarehman4353/LRSA-XLMR-Sentiment-ID
### Dataset
https://huggingface.co/datasets/mziarehman4353/LRSA-LLM-Dataset
### DOI Archive:
https://doi.org/10.5281/zenodo.21297896
