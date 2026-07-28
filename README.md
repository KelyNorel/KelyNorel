# Raquel (Kely) Norel, PhD
### Principal Applied Scientist | AI/ML Research | NLP & LLM Systems | Healthcare AI

I build intelligent AI systems that reason over data, validate their decisions 
statistically, and operate reliably at scale. 15+ years at IBM Research, now 
applying that expertise to new challenges.

---

## Projects

### AI/ML Systems

| Project | Description | Stack |
|---|---|---|
| [legal-rlhf](https://github.com/KelyNorel/legal-rlhf) | End-to-end RLHF pipeline for legal document relevance — reward model (98.7% accuracy) + GRPO policy (64.5% selection acc) + LLM-as-a-Judge validation | PyTorch, HuggingFace, TRL, Claude API |
| [pain-llm-finetune](https://github.com/KelyNorel/pain-llm-finetune) | Local HIPAA-compliant LLM fine-tuning for chronic pain clinical scoring — RAG, LoRA, Ollama on Apple Silicon | MLX, Ollama, ChromaDB |
| [oncology-rwe-agent](https://github.com/KelyNorel/oncology-rwe-agent) | Agentic RWE pipeline for oncology — LangGraph, tool use, clinical reasoning | LangGraph, Claude API |
| [esm-variant-agent](https://github.com/KelyNorel/esm-variant-agent) | Zero-shot protein variant effect prediction — ESM2 embeddings + log-likelihood ratio scoring (Spearman ρ=0.364 on ProteinGym), LangGraph agent with UniProt annotation and real-time clinical evidence search (ClinVar, PubMed) | PyTorch, HuggingFace, LangGraph, Claude API, Streamlit |
| [tp53-captum-esm2](https://github.com/KelyNorel/tp53-captum-esm2) | Linear probe on frozen ESM2 embeddings predicts TP53 variant pathogenicity (ClinVar, AUC 0.806) — Captum's attribution locked onto a never-mutated residue in 99.7% of variants until the artifact was diagnosed and independently confirmed with SHAP | PyTorch, HuggingFace, Captum, SHAP, scikit-learn, Streamlit |

### Causal Data Science

| Project | Description | Stack |
|---|---|---|
| [data-confessions](https://github.com/KelyNorel/data-confessions) | Multi-agent causal analysis system — 5 LangGraph agents investigate whether rain reduces crime in Chicago using 1.4M records. Finds temperature is the real driver; rain effect only visible after controlling for confounders. Inspired by *The Book of Why* and *Everybody Lies* | LangGraph, Claude API, statsmodels, Streamlit |

### Women's Health / Time-Series

| Project | Description | Stack |
|---|---|---|
| [cycle-signal](https://github.com/KelyNorel/cycle-signal) | End-to-end time-series analysis of menstrual cycle dynamics — ovulation timing prediction across 1,665 cycles from 159 subjects (MAE=1.79 days); data leakage detection; linear model outperforms Random Forest and XGBoost | pandas, scikit-learn, matplotlib |

### Oncology / Real-World Evidence

| Project | Description | Stack |
|---|---|---|
| [cfdna-methylation-atlas](https://github.com/KelyNorel/cfdna-methylation-atlas) | Reproduced a published cfDNA methylation deconvolution method (Moss et al. 2018) from public GEO/TCGA data — traced a systematic tissue-of-origin misclassification to a single undersampled reference cell type (n=2), confirmed across 4 independent methods: real cancer patients, CpG hyperparameter sweep, synthetic TCGA admixture cohort, and bootstrap confidence intervals | Python, pandas, scipy (NNLS), GEOparse, GDC API |
| [tcga-luad-rwe](https://github.com/KelyNorel/tcga-luad-rwe) | Multi-modal survival analysis of lung adenocarcinoma — KM, Cox PH, KRAS subtypes, RNA-seq integration | lifelines, scikit-learn, pandas |
| [metabric-survival](https://github.com/KelyNorel/metabric-survival) | Breast cancer survival analysis — NPI validation, competing risks, causal inference | lifelines, scikit-survival |

### Speech Processing / Audio ML

| Project | Description | Stack |
|---|---|---|
| [fluency-from-alignment](https://github.com/KelyNorel/fluency-from-alignment) | Predicted spoken fluency from pause structure — forced alignment + energy-based VAD on 2,500 utterances. Found forced alignment fails systematically on disfluent speech (the population that matters most); switched to VAD-based pause detection. Speech rate alone captures 98% of the full 9-feature model's signal (test ρ=0.621 vs 0.630) | Qwen3-ForcedAligner, HuggingFace Transformers, PyTorch, scikit-learn, SHAP |

### Behavioral Data Science / A/B Testing

| Project | Description | Stack |
|---|---|---|
| [beats-and-focus](https://github.com/KelyNorel/beats-and-focus) | Does high-BPM music drive focus? A/B test on 2,016 Spotify tracks — sequential design, pilot study, frequentist + Bayesian analysis. The data agreed with the hypothesis — until SHAP revealed instrumentalness, not tempo, drives the effect. | scipy, scikit-learn, SHAP |
| [clinical-trial-nudges](https://github.com/KelyNorel/clinical-trial-nudges) | Do behavioral nudges increase trial enrollment? A/B test on 18,644 ClinicalTrials.gov trials — nudges show 2x enrollment advantage, until SHAP reveals it's largely mediated by trial design confounders. | scipy, statsmodels, scikit-learn, SHAP |

### Healthcare Data & SQL

| Project | Description | Stack |
|---|---|---|
| [provider-quality-sql](https://github.com/KelyNorel/provider-quality-sql) | SQL-first analysis of 5,400+ U.S. hospitals using real CMS data — weighted composite mortality scoring across 5 conditions (heart attack, stroke, pneumonia, heart failure, COPD), state and ownership type rankings, volume-quality relationship, and a provider recommendation engine returning top-5 hospitals by state and condition. VA hospitals outperform all ownership types nationally; Mississippi worst-performing state; NYU Langone #1 overall.  | DuckDB, Python, pandas, matplotlib |

### Healthcare AI

| Project | Description | Stack |
|---|---|---|
| [ncci-policy-assistant](https://github.com/KelyNorel/ncci-policy-assistant) | RAG-powered Medicare NCCI policy assistant — 85% accuracy, zero hallucinations, CPT conflict detection | ChromaDB, Claude API, Streamlit |
| [fhir-retrieval-system](https://github.com/KelyNorel/fhir-retrieval-system) | FHIR clinical data retrieval system matching paper SOTA — BM25, vector, hybrid retrieval strategies | SQLite, FHIR, sentence-transformers |

---

## Expertise
```
Large Language Models • Agentic AI • LLM-as-a-Judge • Reinforcement Learning • Reward Modeling • GRPO
NLP • Transformer Models • Deep Learning • Machine Learning • Explainable AI (SHAP, Captum) • Synthetic Data Generation
Real-World Evidence • Clinical AI • Digital Biomarkers • Survival Analysis
cfDNA / Liquid Biopsy • DNA Methylation • Reference-Atlas Deconvolution (NNLS) • Bootstrap / Uncertainty Quantification
Python • PyTorch • HuggingFace • scikit-learn • Pandas • SQL • DuckDB
Experimental Design • Statistical Modeling • Benchmarking & Evaluation • Cross-Functional Collaboration
Causal Inference • Confounder Analysis • Multi-Agent Systems • LangGraph
Protein Language Models • Variant Effect Prediction • Computational Biology

```
---

## Research Impact
- 80+ peer-reviewed publications, h-index 36, 7,100+ citations
- 13 U.S. patents
- IEEE ICDH Best Paper Award (2023)
- IBM Outstanding Research Accomplishment Award (2021)

---

## Connect
[![LinkedIn](https://img.shields.io/badge/LinkedIn-raquel--norel-blue)](https://www.linkedin.com/in/raquel-norel)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-Raquel%20Norel-green)](https://scholar.google.com/citations?user=_7vMqI4AAAAJ&hl=en)
