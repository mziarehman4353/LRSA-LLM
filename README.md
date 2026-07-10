
# Stress-Testing Large Language Models (LLMs) against Code-Mixing and Distributional Shifts in Low-Resource NLP

## Authors

Zia Ul Rehman Zafar  
Dedi Gunawan  
Endang Wahyu Pamungkas  
Widi Widayat  
Helmi Imaduddin  

Department of Informatics Engineering  
Universitas Muhammadiyah Surakarta, Indonesia

---

## Overview

This repository accompanies the research study:

**Stress-Testing Large Language Models (LLMs) against Code-Mixing and Distributional Shifts in Low-Resource NLP**

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

## Main Results

| Model | Accuracy | Macro F1 |
|---------|---------:|---------:|
| SVM | 0.8055 | 0.7796 |
| IndoBERT | 0.8731 | 0.8556 |
| XLM-R | 0.8610 | 0.8466 |

---

## Robustness Results

### Macro F1 under Noise

| Model | Clean | p=0.1 | p=0.2 | p=0.3 |
|---------|---------:|---------:|---------:|---------:|
| SVM | 0.7796 | 0.7275 | 0.7193 | 0.7061 |
| IndoBERT | 0.8556 | 0.8392 | 0.8150 | 0.7827 |
| XLM-R | 0.8466 | 0.8352 | 0.8175 | 0.7982 |

---

## Cross-Domain Generalization

| Model | Generalization Score |
|---------|---------:|
| SVM | 0.7071 |
| IndoBERT | 0.8394 |
| XLM-R | 0.8243 |

---

## Statistical Significance

McNemar tests confirmed statistically significant differences between all evaluated models.

| Comparison | p-value |
|------------|---------:|
| IndoBERT vs SVM | < 0.001 |
| XLM-R vs SVM | < 0.001 |
| IndoBERT vs XLM-R | < 0.001 |

---

## Repository Structure

models/  
results/  
figures/  
appendix_figures/  
data/  
notebooks/  
src/  
docs/

---

## Hugging Face Models

IndoBERT:  
https://huggingface.co/mziarehman4353

XLM-R:  
https://huggingface.co/mziarehman4353

---

## Citation

If you use this repository, please cite the associated publication.

---

## License

MIT License


## Pretrained Models

The transformer models are hosted separately on Hugging Face due to their size.

### IndoBERT
https://huggingface.co/mziarehman4353

### XLM-R
https://huggingface.co/mziarehman4353

