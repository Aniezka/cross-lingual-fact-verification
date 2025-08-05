# Cross-Lingual Fact Verification: Analyzing LLMs Performance Patterns Across Languages
The link to the paper: TBA

## 📄 Overview

This repository contains the analysis results and supplementary materials for our RANLP 2025 paper investigating how well current LLMs handle fact verification across different languages and writing systems. Our research reveals significant performance disparities based on script systems and identifies systematic cross-lingual instruction following failures.

## 🔍 Key Findings

- **Script System Impact**: Latin script languages consistently outperform others across all models
- **Cross-lingual Transfer Patterns**: Norwegian achieves exceptional zero-shot performance (0.34 macro-F1), while South Asian languages struggle significantly
- **Official Language Support**: Languages officially supported by models (e.g., Indonesian and Polish for Qwen 2.5) often outperform traditionally high-resource languages like German and Spanish
- **Instruction Following Failures**: Systematic failures in producing requested English labels, particularly affecting non-Latin script languages

## 🎯 Results Summary

!

## 📁 Repository Contents

```
├── model_biases/           # Analysis of model prediction biases across labels
├── model_performance/      # Detailed performance results 
└── prompt/                 # Prompt
```

## 🔬 Experimental Setup

### Models Evaluated
- **Llama 3.1 (8B)**: Supports 8 languages including English, German, French, Italian, Portuguese, Hindi, Spanish, and Thai
- **Qwen 2.5 (7B)**: Broadest coverage with 29 languages, strong in Asian languages
- **Mistral Nemo (12B)**: Largest model supporting 11 languages including European and some Asian languages

### Dataset: X-Fact
- **Languages**: 25 languages across 11 language families
- **Claims**: 31,189 total claims
- **Categories**: 7 fine-grained veracity labels
  - `true`, `mostly_true`, `partly_true`, `mostly_false`, `false`, `complicated`, `other`
- **Evaluation splits**: In-domain, out-of-domain, zero-shot cross-lingual

### Approaches

- **Few-shot prompting**: 7 examples balanced across languages and veracity categories
- **Fine-tuning**: LoRA with rank 16, alpha 32, targeting attention and feed-forward components

## 📋 Language Categories

### By Script System
- **Latin**: German, Spanish, Indonesian, Italian, Polish, Portuguese, etc.
- **Arabic**: Arabic, Persian
- **Devanagari**: Hindi, Marathi
- **Other**: Georgian, Tamil, Bengali, Gujarati, Punjabi, Russian, Sinhala

### By Resource Level
- **Well-represented**: German, Spanish, French, Arabic
- **Moderately-represented**: Portuguese, Italian, Dutch, Polish, Turkish, Persian, Hindi, Russian, Serbian
- **Under-represented**: Indonesian, Romanian, Georgian, Tamil, Bengali, Punjabi, Marathi, Albanian, Azerbaijani, Gujarati, Norwegian, Sinhala


## 📋 Citation

```
TBA
```

## 🔗 Related Resources

- **X-Fact Paper**: https://aclanthology.org/2021.acl-short.86.pdf

## Contact

For any questions or collaboration:
- **Hanna Shcharbakova** - Saarland University, aniezka.sherbakova@gmail.com
