# Benchmarking BERT-based Models for Sentence-level Topic Classification in Nepali Language

## Overview
This repository contains the implementation and experiments for benchmarking various BERT-based transformer models on **sentence-level topic classification in Nepali**, a low-resource language.

We evaluate multilingual, Indic, Hindi, and Nepali-specific models to understand their effectiveness in capturing linguistic nuances of Nepali text.

---

## Objectives
- Benchmark multiple BERT-based models on Nepali text classification
- Analyze performance differences across multilingual, Indic, and monolingual models
- Establish a strong baseline for future Nepali NLP tasks
- Provide insights into low-resource language modeling

---

## Dataset
The dataset consists of **25,006 Nepali sentences** categorized into five domains:

- 🌾 Agriculture  
- 🏥 Health  
- 🎓 Education & Technology  
- 🏔️ Culture & Tourism  
- 💬 General Communication  

The dataset is balanced across all categories.

🔗 **Dataset Link:** *(Add here)*

---

## Models Evaluated
We benchmarked the following transformer-based models:

### Multilingual Models
- mBERT  
- XLM-RoBERTa  
- mDeBERTa  

### Indic Models
- MuRIL (base & large)  
- IndicBERT  
- DevBERT  

### Language-Specific Models
- HindiBERT  
- NepBERTa  

### English Model
- RoBERTa  

🔗 **Model Links:** *(Add here)*

---

## Experimental Setup
- Training samples: 20,005  
- Validation samples: 2,500  
- Test samples: 2,501  
- Epochs: 10  
- Learning rate: 2e-5  
- Batch size: 8  
- Gradient accumulation: 2  
- Max sequence length: 256  

Framework: 🤗 Hugging Face Transformers  

---

## Evaluation Metrics
- Accuracy  
- Precision (Weighted)  
- Recall (Weighted)  
- F1-score (Weighted)  
- AUROC  

---

## Key Results
- **MuRIL-large** achieved the best performance:
  - F1-score: **90.60%**
- **NepBERTa** showed strong competitive performance:
  - F1-score: **88.26%**
- Indic models outperformed multilingual and general models overall

---

## Key Insights
- Region-specific (Indic) models perform better for Nepali
- Monolingual pretraining (NepBERTa) is highly effective
- General multilingual models are slightly less optimized for Nepali

---

## Limitations
- Limited to sentence-level classification
- Dataset covers only five domains
- No extensive error analysis performed
- Results may not generalize to other NLP tasks

---

## Future Work
- Extend to document-level classification
- Expand dataset with more domains
- Perform detailed error analysis
- Explore ensemble methods
- Improve Nepali-specific pretraining

---

## Citation

If you use this work, please cite:

```bibtex
@inproceedings{karki2026benchmarking,
  title={Benchmarking BERT-based Models for Sentence-level Topic Classification in Nepali Language},
  author={Karki, Nischal and Subedi, Bipesh and Poudyal, Prakash and Ghimire, Rupak Raj and Bal, Bal Krishna},
  booktitle={Proceedings of the Regional International Conference on Natural Language Processing (RegICON 2025)},
  year={2026},
  address={Guwahati, India},
  note={Gauhati University, November 27--29, 2025},
  url={https://arxiv.org/abs/2602.23940}
}
